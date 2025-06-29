<template>
  <section class="bg-white py-20 px-4">
    <h2 class="text-3xl font-bold text-center mb-10">이력 소개</h2>
    
    <div class="grid gap-6 sm:grid-cols-2 lg:grid-cols-3 max-w-5xl mx-auto">
      <div
        v-for="(item, index) in resumeItems"
        :key="index"
        class="bg-gray-100 rounded-xl p-6 shadow hover:shadow-lg transition"
      >
        <h3 class="text-xl font-semibold text-blue-700 mb-2">{{ item.title }}</h3>
        <p class="text-sm text-gray-500 mb-4">{{ item.period }}</p>
        <p class="text-gray-700 text-base">{{ item.desc }}</p>
      </div>
    </div>
  </section>
</template>

<script setup>
const resumeItems = [
  {
    title: "University of Sussex",
    period: "2022 - 현재",
    desc: "AI 전공 학부생으로 머신러닝과 딥러닝에 집중."
  },
  {
    title: "보드게임 동아리 운영",
    period: "2023 - 현재",
    desc: "전략 보드게임 기획 및 교내 보드게임 커뮤니티 운영."
  },
  {
    title: "음악 크리에이터",
    period: "2021 - 2022",
    desc: "로파이 및 인디음악을 직접 작곡하고 SNS에 공유."
  }
]
</script>

<style scoped>
/* 선택적으로 스타일 추가 가능 */
</style>
