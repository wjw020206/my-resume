<template>
  <div class="person-info">
    <div class="person-info__name">王佳伟</div>
    <div class="person-info__subTitle">前端开发 / 1.5 年经验</div>
    <div class="person-info__contact">
      <div
        class="person-info__contact-item"
        v-for="item in contact"
        :key="item.name"
      >
        <component :is="item.icon" class="person-info__contact-icon" />
        <span>{{ item.value }}</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
const contact = [
  {
    name: 'Phone',
    icon: IconCustomPhoneOutlined,
    value: '+86 13567919504',
  },
  {
    name: 'WeChat',
    icon: IconCustomWechatOutlined,
    value: 'M63HhkCx',
  },
  {
    name: 'Email',
    icon: IconCustomMailOutlined,
    value: 'jiawei.wang2021@gmail.com',
  },
]
</script>

<style lang="scss" scoped>
.person-info {
  display: flex;
  flex-direction: column;
  row-gap: 8px;

  &__name {
    color: #000;
    text-align: center;
    letter-spacing: 4px;
    font-size: 24px;
    font-weight: 600;
  }

  &__subTitle {
    color: #333;
    text-align: center;
    width: 100%;
    max-width: 100%;
    font-size: 14px;
    font-weight: 400;
  }

  &__contact {
    display: flex;
    justify-content: center;
    align-items: center;
    color: #333;
    font-size: 14px;
    font-weight: 400;
    flex-wrap: wrap;
    column-gap: 20px;

    &-item {
      display: flex;
      align-items: center;
      column-gap: 8px;
    }

    &-icon {
      font-size: 16px;
    }
  }
}
</style>
