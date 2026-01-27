<template>
  <div class="skill-list">
    <SectionTitle title="相关技能" />
    <ul>
      <li>
        熟悉<span class="mx-1">Vue2/Vue3</span
        >及其原理，能够设计高可维护性、可扩展的业务组件，拥有丰富的<span
          class="mx-1"
          >Vue3 + TS</span
        >实践经验
      </li>
      <li>
        熟悉使用<span class="mx-1">TypeScript</span>开发，掌握最新版本<span
          class="mx-1"
          >TypeScript</span
        >特性，能在 strict 模式下无 any 类型流畅编写代码
      </li>
      <li>
        熟悉<span class="mx-1">uni-app</span>跨端开发，掌握<span class="mx-1"
          >小程序、H5、APP</span
        >
        等多端适配方案，<span class="mx-1">熟悉 APP 离线打包与云打包流程</span>
      </li>
      <li>
        熟悉前端性能优化，能够结合实际业务进行<span class="mx-1"
          >代码优化、打包优化与资源优化</span
        >
      </li>
      <li>
        熟练掌握<span class="mx-1">Webpack / Vite</span>
        等构建工具，能用以上工具搭建通用开发环境
      </li>
      <li>
        熟悉<span class="mx-1">Prettier / ESLint</span
        >配置，有良好编码习惯，强调实用主义与可维护性
      </li>
      <li>
        熟悉前端开发流程，包括<span class="mx-1"
          >协同开发、分支管理、项目配置</span
        >等，具备较强的工程实践能力
      </li>
      <li>
        熟悉代码开发到上线全流程，对<span class="ml-1">协同开发</span>、<span
          >分支管理</span
        >
        、<span class="mr-1">项目配置</span>等都有较深刻的最佳实践
      </li>
    </ul>
  </div>
</template>

<script setup lang="ts"></script>

<style lang="scss" scoped>
.skill-list {
  width: 100%;
  max-width: 100%;
  margin: 0 auto;

  ul {
    width: calc(100% - 20px);
    margin: 0;
    padding-inline-start: 20px;

    li {
      color: #000;
      text-align: start;
      font-size: 15px;
      font-weight: 400;
      line-height: 24px;

      span {
        font-weight: 600;
      }
    }
  }
}
</style>
