<script setup>
const features = [
  {
    title: 'Real-Time Monitoring',
    description: 'Checks run around the clock, not just once a day.',
  },
  {
    title: 'Multi-Location Search',
    description: 'Track several enrollment centers at once to widen your odds.',
  },
  {
    title: 'Instant Alerts',
    description: 'Get notified within seconds of a new opening.',
  },
  {
    title: 'No More Manual Refreshing',
    description: 'Let automation do the tedious part.',
  },
  {
    title: 'Simple Setup',
    description: "Enter your info once and you're covered.",
  },
]
</script>

<template>
  <section class="features-section py-5">
    <div class="container">
      <h2 class="fw-bold mb-5">Built to Save You Time</h2>

      <div class="row row-cols-1 row-cols-sm-2 row-cols-lg-3 g-4">
        <div v-for="(feature, index) in features" :key="index" class="col">
          <div class="feature-card h-100 rounded-4 p-4">
            <p class="feature-title fw-bold mb-2">{{ feature.title }}</p>
            <p class="fw-semibold mb-0">{{ feature.description }}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.feature-card {
  background-color: #f4f4f4;
  color: #2b2420;
}

.feature-title {
  color: #f1705a;
}
</style>
