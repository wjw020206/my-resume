<template>
  <div class="social-info">
    <SectionTitle title="社交信息" />
    <div
      class="social-info__item"
      v-for="item in socialInfo"
      :key="item.platform"
    >
      <component :is="item.icon" class="social-info__icon" />
      <span class="social-info__platform">{{ item.platform }}：</span>
      <a class="social-info__link" :href="item.href" target="_blank">{{
        item.href
      }}</a>
    </div>
  </div>
</template>

<script setup lang="ts">
const socialInfo = [
  {
    platform: 'GitHub',
    href: 'https://github.com/wjw020206',
    icon: IconCustomGithubOutlined,
  },
  {
    platform: '掘 金',
    href: 'https://juejin.cn/user/2665653959139032/posts',
    icon: IconCustomJuejinOutlined,
  },
]
</script>

<style lang="scss" scoped>
.social-info {
  width: 100%;
  max-width: 100%;
  margin: 0 auto;

  &__item {
    display: flex;
    color: #000;
    text-align: start;
    align-items: center;
    column-gap: 6px;
    font-size: 15px;
    font-weight: 400;
    line-height: 24px;
  }

  &__icon {
    font-size: 16px;
  }

  &__platform {
    display: inline-block;
    min-width: 76px;
  }

  &__link {
    white-space: nowrap;
    text-overflow: ellipsis;
    overflow: hidden;
    color: #166dff;
    font-weight: 700;
  }
}
</style>
