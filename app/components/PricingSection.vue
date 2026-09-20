<script setup>
const plans = [
  {
    name: 'Free',
    price: '$0',
    period: '',
    description: 'Start tracking appointments right away.',
    features: ['Search appointment locations', 'Save locations'],
    cta: 'Start searching for free',
    highlighted: false,
  },
  {
    name: 'Pro',
    price: '$15',
    period: '/mo',
    description: 'Everything in Free, plus real-time alerts.',
    features: ['Everything in Free', 'Email notifications'],
    cta: 'Get Pro',
    highlighted: true,
  },
]
</script>

<template>
  <section class="pricing-section py-5">
    <div class="container">
      <h2 class="fw-bold mb-2">Pricing</h2>
      <p class="text-muted mb-5">Start free. Upgrade anytime for instant email alerts.</p>

      <div class="row g-4 justify-content-center">
        <div v-for="plan in plans" :key="plan.name" class="col-md-6 col-lg-4">
          <div class="pricing-card h-100 rounded-4 p-4" :class="{ 'pricing-card-highlighted': plan.highlighted }">
            <span v-if="plan.highlighted" class="pricing-badge fw-semibold mb-3">Most Popular</span>

            <p class="pricing-name fw-bold mb-1">{{ plan.name }}</p>
            <p class="pricing-description text-muted mb-4">{{ plan.description }}</p>

            <p class="mb-4">
              <span class="pricing-price fw-bold">{{ plan.price }}</span>
              <span v-if="plan.period" class="pricing-period">{{ plan.period }}</span>
            </p>

            <ul class="list-unstyled pricing-features mb-4">
              <li v-for="feature in plan.features" :key="feature" class="d-flex align-items-start mb-2">
                <span class="pricing-check me-2">✓</span>
                <span class="fw-semibold">{{ feature }}</span>
              </li>
            </ul>

            <a
              href="#"
              class="btn w-100 fw-semibold pricing-btn"
              :class="plan.highlighted ? 'pricing-btn-highlighted' : 'pricing-btn-default'"
            >
              {{ plan.cta }}
            </a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.pricing-card {
  background-color: #f7f7f6;
  color: #2b2420;
  border: 1px solid transparent;
}

.pricing-card-highlighted {
  background-color: #2b2420;
  color: #fff;
  border-color: #2b2420;
}

.pricing-badge {
  display: inline-block;
  background-color: #f1705a;
  color: #fff;
  font-size: 0.75rem;
  text-transform: uppercase;
  letter-spacing: 0.05em;
  padding: 0.25rem 0.75rem;
  border-radius: 999px;
}

.pricing-name {
  font-size: 1.25rem;
}

.pricing-card-highlighted .pricing-description {
  color: #c9c3be !important;
}

.pricing-price {
  font-size: 2.5rem;
}

.pricing-period {
  color: inherit;
  opacity: 0.7;
}

.pricing-check {
  color: #f1705a;
  font-weight: 700;
}

.pricing-btn {
  border-radius: 0.6rem;
  padding: 0.75rem 1.5rem;
}

.pricing-btn-default {
  background-color: #e7e7e5;
  color: #2b2420;
}

.pricing-btn-default:hover {
  background-color: #dadad8;
  color: #2b2420;
}

.pricing-btn-highlighted {
  background-color: #f1705a;
  color: #fff;
}

.pricing-btn-highlighted:hover {
  background-color: #dd5b45;
  color: #fff;
}
</style>
