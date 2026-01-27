<template>
  <div class="resume-wapper">
    <div class="resume-container">
      <PersonInfo />
      <Introduction />
      <SocialInfo />
      <Educational />
      <SkillList />
      <ProjectExperience />
      <WorkExperience />
      <Thanks />
    </div>
  </div>
</template>

<script setup lang="ts"></script>

<style lang="scss" scoped>
.resume {
  &-wapper {
    min-height: 100%;
    background-color: #000;
    padding: 40px 0;
  }

  &-container {
    display: flex;
    flex-direction: column;
    row-gap: 12px;
    max-width: 860px;
    margin: 0 auto;
    background-color: #fff;
    padding: 30px;
  }
}
</style>
