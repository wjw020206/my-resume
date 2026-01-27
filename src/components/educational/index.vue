<template>
  <div class="educational">
    <SectionTitle title="教育经历" />
    <div
      class="educational__universitys"
      v-for="item in universitys"
      :key="item.name"
    >
      <div class="educational__info">
        {{ item.name }}
        <span class="educational__time">{{ item.time }}</span>
      </div>
      <div class="educational__major">{{ item.major }}</div>
    </div>
  </div>
</template>

<script setup lang="ts">
const universitys = [
  {
    name: '浙江广厦建设职业技术大学',
    major: '软件工程',
    time: '2020/10 - 2024/06',
  },
]
</script>

<style lang="scss" scoped>
.educational {
  width: 100%;
  max-width: 100%;
  margin: 0 auto;

  &__universitys {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
    width: 100%;
    max-width: 100%;
  }

  &__info {
    display: flex;
    color: #000;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    max-width: 100%;
    font-size: 16px;
    font-weight: 700;
    line-height: 28px;
  }

  &__time {
    font-size: 16px;
    font-weight: 400;
    line-height: 24px;
  }

  &__major {
    color: #000;
    font-size: 14px;
    font-weight: 400;
    line-height: 24px;
  }
}
</style>
