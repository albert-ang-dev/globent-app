<script setup>
const problems = [
  "You check the CBP appointment system and every slot is booked for 6+ months",
  "You've refreshed the page a hundred times hoping something opens up",
  "You have a trip coming up and no interview scheduled",
  "You don't have time to babysit a government website all day",
]
</script>

<template>
  <section class="problem-section py-5">
    <div class="container">
      <h2 class="fw-bold mb-4">Sound Familiar?</h2>

      <ul class="problem-list list-unstyled mb-4">
        <li v-for="(problem, index) in problems" :key="index" class="d-flex align-items-start mb-3">
          <span class="bullet me-3"></span>
          <span class="fw-semibold problem-text">{{ problem }}</span>
        </li>
      </ul>

      <p class="transition-line fw-bold mb-0">There's a faster way.</p>
    </div>
  </section>
</template>

<style scoped>
.bullet {
  width: 10px;
  height: 10px;
  min-width: 10px;
  border-radius: 50%;
  background-color: #f1705a;
  margin-top: 8px;
}

.problem-text {
  color: #2b2420;
  font-size: 1.1rem;
}

.transition-line {
  color: #f1705a;
  font-size: 1.35rem;
}
</style>
