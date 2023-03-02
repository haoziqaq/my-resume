<template>
  <resume-app-bar />

  <div class="resume-layout">
    <resume-profile />

    <resume-blank :size="350"></resume-blank>

    <var-row :gutter="20">
      <var-col :span="12" :xs="24">
        <resume-timeline />
      </var-col>
      <var-col :span="12" :xs="24">
        <resume-skills />
      </var-col>
    </var-row>

    <resume-block title="项目经历" subtitle="**只列举部分典型项目**">
      <resume-block-item
        title="星芒低代码SaaS平台"
        description="一个为了提高应用落地效率的低代码平台，对标宜搭、用友。主要技术栈是 Typescript、Vue3、React、React Native。在项目中主要负责低代码设计器、可视化编程设计器的迭代，实现通过拖拉拽设计应用，通过卡片编排完成事件处理函数的编写。另外负责设计和迭代低代码物料和模板等资产。"
      />
      <resume-block-item
        title="机动车考试监管系统"
        description="该项目是为了满足成都车管所业务需求而研发的管理系统，可以做到考试的时实巡查。主要技术栈是 Vue2 全家桶 + Element UI。在项目中除了常规的增删查改、数字大屏、权限管理的业务之外，还有一些硬件的对接。如高拍仪、签字板，读卡器、监控摄像头、人脸识别摄像头等。该项⽬已应⽤在⽢孜、阿坝、雅安、⼴元等地考场，反馈都相当不错。"
      />
      <resume-block-item
        title="炼铠⼯⼚⼩程序/微信网页"
        description=" 该项⽬是一个铠甲销售租赁的平台小程序。基于 uniapp 开发，一套代码打包为小程序和微信网页。主要负责的工作是电商相关的功能，如商品列表，下单，⽀付，订单中⼼，分享，返利，海报，购物⻋，客服系统，搜索，个⼈中⼼，退货，秒杀，抢购，优惠券等等。"
      />
      <resume-block-item
        title="⼴汽菲克党员党⽀部学习双积分考核系统"
        description="该项⽬是微信企业号项⽬，主要处理党建学习业务。主要技术栈是 Vue2 全家桶 + Vant + Echarts。主要负责的工作是会议发布、会议签到、⽀部党员⼤会、党⼩组会、⽀部党课、主题党⽇....等 40 余个活动项⽬开展，包含大量图表。"
      />
      <resume-block-item
        title="闲友App"
        description="该项⽬是⼀个混合开发项⽬。主要的技术栈是 ionic + Angularjs。主要负责的工作是⽤户模块，拼团，代跑腿，商家直销，即时通讯，实时定位，路径导航，接⼊移动⽀付，App 的打包。"
      />
    </resume-block>

    <resume-block title="开源项目" subtitle="**只列举目前仍活跃项目**">
      <resume-block-item title="varletjs/varlet (仓库所有者)">
        <template #description>
          <div class="resume-layout-stars">stars: 3771</div>
          <div class="resume-layout-description">
            一个基于 Vue3 的 Material Design 风格移动端组件库，尤雨溪 Vue
            官方团队 2021 年 Vue Conf 推荐、Gitee GVP
            年度最有价值开源项目、阮一峰周刊推荐。提供 60+
            个高质量通用组件，支持按需引入，国际化、SSR、暗黑模式、90%
            以上的单元测试覆盖率，并提供了 VSCode 插件。
          </div>
          <div class="resume-layout-link-item">
            仓库地址:
            <var-link type="primary" href="https://github.com/varletjs/varlet">
              https://github.com/varletjs/varlet
            </var-link>
          </div>
          <div class="resume-layout-link-item">
            官方文档:
            <var-link type="primary" href="https://varlet.gitee.io/varlet-ui">
              https://varlet.gitee.io/varlet-ui
            </var-link>
          </div>
        </template>
      </resume-block-item>
      <resume-block-item title="antfu/unplugin-vue-components (仓库贡献者)">
        <template #description>
          <div class="resume-layout-stars">stars: 2605</div>
          <div class="resume-layout-description">
            一个 Vite 插件，可以实现自动按需引入在 Vue 中使用过的组件。
          </div>
          <div class="resume-layout-link-item">
            仓库地址:
            <var-link type="primary" href="https://github.com/antfu/unplugin-vue-components">
              https://github.com/antfu/unplugin-vue-components
            </var-link>
          </div>
        </template>
      </resume-block-item>
      <resume-block-item title="antfu/unplugin-vue-components (仓库贡献者)">
        <template #description>
          <div class="resume-layout-stars">stars: 10600</div>
          <div class="resume-layout-description">
            一套面向扩展设计的企业级低代码技术体系。
          </div>
          <div class="resume-layout-link-item">
            仓库地址:
            <var-link type="primary" link="https://github.com/alibaba/lowcode-engine">
              https://github.com/alibaba/lowcode-engine
            </var-link>
          </div>
          <div class="resume-layout-link-item">
            官方网站:
            <var-link type="primary" link="https://lowcode-engine.cn/index">
              https://lowcode-engine.cn/index
            </var-link>
          </div>
        </template>
      </resume-block-item>
    </resume-block>

    <resume-block title="技能清单">
      <resume-block-compact-item description="熟练使⽤ html5、css3、JavaScript、Typescript 构建 web 应⽤" />
      <resume-block-compact-item description="熟练使用 Vue、React 及其生态系统，并阅读过大部分的 Vue3 源码" />
      <resume-block-compact-item description="熟练使用 Varlet、Vant、AntDesign、AntDesignVue、element" />
      <resume-block-compact-item description="熟练使用 echarts、白鹭引擎、高德/腾讯/百度地图等图形化相关生态系统" />
      <resume-block-compact-item description="熟练使用 Vite、Webpack，能完成定制化插件的编写，并阅读过大部分 Vite 源码" />
      <resume-block-compact-item description="熟练使用 Jest、Vitest 等单元测试工具" />
      <resume-block-compact-item description="熟练使用 eslint、stylelint、prettier、husky、lint-staged、commitlint 等工具进行代码规范约束" />
      <resume-block-compact-item description="熟练使用 git、svn 版本控制软件" />
      <resume-block-compact-item description="熟练使用 react-native、electron 跨端开发" />
      <resume-block-compact-item description="熟悉微信平台开发，移动端混合开发、服务端 SSR、SSG" />
      <resume-block-compact-item description="了解一些 mysql、redis、mongodb 等后端存储软件" />
      <resume-block-compact-item description="学习过 JAVA、GOLANG 并有一定的理解和实际编码经验" />
    </resume-block>
  </div>
</template>

<style>
* {
  box-sizing: border-box;
}

@media print {
  * {
    box-shadow: none !important;
  }

  .print-disabled {
    display: none !important;
  }
}

body {
  margin: 0;
  font-family: 'Roboto', sans-serif;
  transition: background-color 0.25s, color 0.25s;
  color: var(--color-text);
  background-color: var(--color-body);
}

::-webkit-scrollbar {
  display: none;
}
</style>

<style lang="less" scoped>
.resume-layout {
  padding: 0 20px 30px;

  &-description {
    color: #888;
    font-size: 15px;
    margin-top: 10px;
    margin-bottom: 10px;
  }

  &-link-item {
    color: #888;
    font-size: 14px;
    margin-top: 6px;
  }

  &-stars {
    color: #555;
    margin-top: 10px;
    font-size: 15px;
  }
}
</style>
