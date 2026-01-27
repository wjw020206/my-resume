<template>
  <div class="work-experience">
    <SectionTitle title="工作经历" />
    <div
      class="work-experience__company"
      v-for="item in workList"
      :key="item.company"
    >
      <div class="work-experience__row1">
        <div class="work-experience__name">{{ item.company }}</div>
        <div class="work-experience__info">
          <div class="work-experience__time">{{ item.time }}</div>
          <div class="work-experience__exit-reason" v-if="item.exitReason">
            ({{ item.exitReason }})
          </div>
        </div>
      </div>
      <div class="work-experience__row2">
        <div>{{ item.title }}</div>
        <div>{{ item.department }}</div>
      </div>
      <ul>
        <li>
          主要负责公司内部管理系统及内部工具的前端开发与维护，独立承担核心模块设计与实现
        </li>
        <li>
          次要负责根据客户业务需求进行功能设计和前端方案优化，确保项目按期交付
        </li>
      </ul>
    </div>
  </div>
</template>

<script setup lang="ts">
const workList = [
  {
    company: '宁波佳橙信息科技有限公司',
    time: '2024/07 - 2025/12',
    exitReason: '',
    title: '前端工程师',
    department: '',
    responsibilities: [
      '负责 WOOFi Pro 交易所 SDK 的开发、维护、优化，确保其高性能和稳定性，高效支撑前端业务的长期迭代',
      '实现了毫秒级延迟的订单簿（OrderBook）、下单（OrderEntry）、充值提现、行情面板等核心模块',
      '在前端实现了联合保证金（Multi-Collateral）、杠杆、LTV、滑点、最大可提现额度等金融公式计算',
      '主导前端性能优化，首屏加载时间从 4s 优化到 1.5s、re-renders 次数降低了 50% 以上',
    ],
  },
]
</script>

<style lang="scss" scoped>
.work-experience {
  width: 100%;
  max-width: 100%;
  margin: 0 auto;

  &__company {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
    width: 100%;
    max-width: 100%;
    margin: 10px 0;
    color: #000;

    ul {
      width: calc(100% - 20px);
      margin: 0;
      padding-inline-start: 20px;

      li {
        text-align: start;
        font-size: 15px;
        font-weight: 400;
        line-height: 24px;
      }
    }
  }

  &__row1 {
    display: flex;

    justify-content: space-between;
    align-items: center;
    width: 100%;
    max-width: 100%;
  }

  &__name {
    font-size: 18px;
    font-weight: 700;
    line-height: 32px;
  }

  &__info {
    display: flex;
    align-items: center;
    column-gap: 4px;
    font-weight: 400;
    font-size: 16px;
  }

  &__row2 {
    display: flex;
    justify-content: flex-start;
    align-items: center;
    column-gap: 20px;
    width: 100%;
    max-width: 100%;
    font-size: 16px;
    font-weight: 700;
    line-height: 32px;
    position: relative;
  }
}
</style>
