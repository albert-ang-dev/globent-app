<script setup>
</script>

<template>
  <section class="hero-section">
    <div class="container py-5">
      <div class="row align-items-center g-5 py-5">
        <div class="col-lg-6">
          <h1 class="hero-title fw-bold mb-4">Your Next Global Entry Slot, Found</h1>
          <p class="hero-subtitle fw-semibold mb-4">
            Real-time Global Entry appointment alerts, delivered the second a slot frees up.
          </p>
          <a href="#" class="btn hero-btn fw-semibold">Start searching for free</a>
        </div>

        <div class="col-lg-6 text-center text-lg-end">
          <img
            src="https://images.unsplash.com/photo-1522083165195-3424ed129620?q=80&w=1200&auto=format&fit=crop"
            alt="Brooklyn Bridge"
            class="img-fluid rounded-4 hero-image"
          >
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.hero-section {
  padding-top: 5px;
}

.hero-title {
  color: #2b2420;
  font-size: 3rem;
  line-height: 1.15;
}

.hero-subtitle {
  color: #2b2420;
  max-width: 460px;
  font-size: 1.1rem;
}

.hero-btn {
  background-color: #e7e7e5;
  border: none;
  border-radius: 0.6rem;
  padding: 0.85rem 1.75rem;
  color: #2b2420;
}

.hero-btn:hover {
  background-color: #dadad8;
  color: #2b2420;
}

.hero-image {
  max-width: 100%;
  box-shadow: 24px 24px 0 rgba(0, 0, 0, 0.08);
}

@media (max-width: 991.98px) {
  .hero-title {
    font-size: 2.25rem;
  }

  .hero-subtitle {
    max-width: 100%;
  }

  .hero-image {
    box-shadow: 14px 14px 0 rgba(0, 0, 0, 0.08);
  }
}
</style>
