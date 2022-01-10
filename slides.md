---
theme: seriph
background: /homepage.jpeg
class: text-center
highlighter: shiki
lineNumbers: false
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
drawings:
  persist: false
---

<h1 class="home">创新中心2021年度总结</h1>
<p> By Zach Zhao </p>

<!--
你们看不见的吧
-->

---

# 创新中心2021回顾

- 🛠 官网和各子官网的日常维护和迭代 <span class="hl">（上线150+次) </span>
- 📝 帮助中心的过渡性迁移 <span class="hl">（基于 Next.js 和 Nest.js) </span>
- 🎨 帮助中心的彻底的重构 <span class="hl">（基于 Next.js 和 Nest.js) </span>
- 🧑‍💻 ShopExpress 和 TeamPro 全新子官网 <span class="hl">（基于 Next.js 的多站点）</span>
- 💃 智慧商超和智慧生鲜的新官网
- 💪 盟羿，盟效，盟购的Facebook验证页
- 🐒 Take over 盟聚官网, Hand over 销氪官网
- 💅 官网后台案例库重整  <span class="hl"> (解绑案例预警) </span>
- 🤹 推广页面的低代码平台的完善 <span class="hl">(运营共创建线上页面 20+)</span>
- 🧔🏼‍♂️ 推广定制化页面 <span class="hl">(PC 和 Mobile 共计 20+)</span>
- 🎥 配合干禧的登录注册门户改造 <span class="hl">(AC迁移到Passport，已移交给奇文组)</span>
- 📤 官网整体重构 <span class="hl">（筹划中）</span>


---

# 帮助中心的架构迁移

<iframe style="border:none" width="800" height="450" src="https://whimsical.com/embed/3GvaXRZ7nFwRpk6dJAJsq8"></iframe>

---
layout: full
---

# 帮助中心迁移

- 数据库表从2张表扩展到10张表，共迁移文章2000+  <span class="hl"> --- 整体设计更加灵活 </span>

- 前端从Angular 1.x迁移到 Next.js <span class="hl"> --- 开发体验和性能提升一个Level </span>

- 后端从 Java 迁移到 Nest.js  <span class="hl"> --- 代码量减少了2/3  </span>

- 全端Typescript <span class="hl"> --- 编译期发现更多问题 </span>

- 全端Prettier进行代码格式化，Eslint进行风格检查  <span class="hl">  --- 保持团队代码风格一致 </span>

- 前后端部署在EP平台上的Node 14运行时里

- 选用一些Rust Based的Tooling(Swc和Prisma)增强开发体验和性能  <span class="hl"> --- 可以战未来 </span>

---

# 帮助中心后台文章编辑器增强

<div grid="~ cols-3 gap-4" class="mt-10">
<div>

- 提供文章大纲功能，锚点跟随

- 第三方图片链接自动批量转存

- 多图复制粘贴自动上传

- 粘贴时自动去除多余的样式

</div>
<div class="col-span-2">
  <img src="/editor.png" class="w-full">
</div>
</div>

---

# 帮助中心首页

<img src="/help-homepage.png" class="w-full">

---

# 帮助中心后台

<img src="/help-admin.png" class="w-full">

---

# 帮助中心搜索

<img src="/help-result.png" class="w-full">

---

# APIFox 进行API管理和协同

<div grid="~ cols-3 gap-4" class="mt-10">
  <div class="col-span-2">

  ![apifox](/apifox.png)
 
  </div>
  <div >

  - 完全遵从Restful规范设计API

  - 代码注解自动生成Swagger文档

  - Swagger文档自动导入到Apifox

  - Apifox保存并同步API调试用例

  - API Mock Server
      
  </div>
</div>

---
layout: two-cols
---
# ShopExpress 和 TeamPro

<div class="mt-10">

- 基于Nextjs的多站点，复用组件和配置

- 运用Tailwindcss，基于Design System和工具类编写css，开发效率++

- 混合使用SSR和SSG，性能和体验++

</div>

::right::
```jsx
<div className="flex items-center justify-end flex-none">
    <a
      data-wmdot="tap"
      data-wmdot-id="rgst_top"
      target="_blank"
      rel="noopener noreferrer"
      href={config && config.saasUrlList.register}
      className="whitespace-nowrap text-[14px] text-blue-primary"
    >
      免费试用
    </a>
    <a
      data-wmdot="tap"
      data-wmdot-id="login"
      href={config && config.saasUrlList.login}
      target="_blank"
      rel="noopener noreferrer"
      className="ml-[20px] w-[76px] h-[30px] whitespace-nowrap inline-flex items-center justify-center border border-blue-primary rounded-[4px] shadow-btns text-[14px] text-white bg-blue-primary"
    >
      登录
    </a>
</div>
```
---

# ShopExpress 的 lighthouse 跑分

<br>

![lighthouse](/lighthouse.png)

---
layout: full
---

# ShopExpress
<img src="/shopexpress.png" class="w-full" />

---
layout: full
---
# TeamPro
<img src="/teampro.png" class="w-full" />
---
layout: full
---
# 智慧商超

<img src="/zhsc.png" class="w-full" />
---

# 智慧生鲜

<img src="/zhsx.png" class="w-full" />


# 对于前端技术部的目标贡献

<br>

- 保证官网既有业务系统的稳定迭代，全年200+次发布

- 有序的进行技术栈的升级，减轻既有的技术债

- 新的子官网和帮助中心给用户体验带来良好的提升

---

# 团队目前面临的问题

<br>

- 常规的琐碎的维护性工作居多，团队缺少更有挑战性的项目去刺激和锻炼

- 产品端缺少长期的规划，严格来说更像是个项目经理而不是产品经理

- 主动和别的团队的交流偏少，往往只去了解和关注自己的这一摊事情


---

# 团队管理 - 能力提高部分
<br>

 > 我相信最好的管理是相互成就


<div grid="~ cols-2 gap-4" class="mt-10">
  <div>

  ### 管理动作

  - 不定期分享有价值的技术文章，激发讨论

  - 训练团队用英文检索技术问题的习惯

  - 落地新技术到实际项目中去

  - 合理分配任务，每个人尽量参与更多的项目

  - 有效示范解决棘手问题的步骤

  </div>
  <div>    

  ### 管理效果

  - 团队内讨论问题的气氛活跃

  - 更好的追根溯源

  - 保持对技术的热情和新鲜感，提高技术自信

  - 每个项目都可以尽量互相Backup

  - 提高独立解决问题的能力和自信心

  </div>
</div>


---

# 团队管理 - 梯度建设部分

<iframe style="border:none" width="850" height="400" src="https://whimsical.com/embed/2KwZ6xb53ixaHTTdXqN66D"></iframe>

<!--
韩鑫和程芸芸会进行重点培养，承担更多的团队责任，全栈的设计和思考的能力
-->

---

# 2022 目标和规划

<br>

- 官网和子官网的整体重构 （响应式）

- 帮助中心的后续完善和迭代

- 推广页面低代码化平台的2.0版 （响应式设计和实现）

- 前端Next.js的项目试点放到Serverless环境上去
