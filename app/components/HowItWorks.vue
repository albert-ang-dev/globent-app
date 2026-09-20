<script setup>
const steps = [
  {
    title: 'Tell us your locations',
    description: "Pick one or several enrollment centers near you (or anywhere you're willing to travel).",
  },
  {
    title: 'We watch 24/7',
    description: 'Our system continuously checks for cancellations and newly released slots.',
  },
  {
    title: 'Get notified instantly',
    description: "The moment something opens, you'll know — by email, text, or push notification.",
  },
]
</script>

<template>
  <section class="how-it-works py-5">
    <div class="container">
      <div class="row g-5">
        <div class="col-lg-4">
          <div class="position-relative d-inline-block mb-3">
            <h2 class="fw-bold display-5 mb-0 lh-sm">How It<br>Works</h2>
            <span class="corner-asterisk">*</span>
          </div>
          <p class="text-muted mb-4">
            Three simple steps stand between you and your next available appointment slot.
          </p>
          <a href="#" class="process-link fw-semibold text-decoration-none">↳ Get started</a>
        </div>

        <div class="col-lg-8">
          <div v-for="(step, index) in steps" :key="index" class="process-card position-relative rounded-4 p-4 mb-4">
            <span class="corner-bracket"></span>
            <div class="d-flex">
              <span class="process-index fw-semibold me-4">{{ String(index + 1).padStart(2, '0') }}</span>
              <div>
                <p class="fw-bold fs-5 mb-2">{{ step.title }}</p>
                <p class="text-muted mb-0">{{ step.description }}</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.corner-asterisk {
  position: absolute;
  top: -0.25rem;
  right: -1.75rem;
  color: #f1705a;
  font-size: 1.5rem;
}

.process-link {
  color: #2b2420;
  border-bottom: 1px solid #2b2420;
  padding-bottom: 2px;
}

.process-link:hover {
  color: #f1705a;
  border-color: #f1705a;
}

.process-card {
  background-color: #f7f7f6;
}

.process-index {
  color: #b7b3af;
  font-size: 0.95rem;
}

.corner-bracket {
  position: absolute;
  top: 0;
  right: 0;
  width: 16px;
  height: 16px;
  border-top: 2px solid #f1705a;
  border-right: 2px solid #f1705a;
}
</style>
