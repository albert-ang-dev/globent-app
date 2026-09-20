<script setup>
</script>

<template>
  <header class="navbar-wrap">
    <nav class="navbar navbar-expand-lg globent-navbar">
      <div class="container-fluid px-3 px-md-4">
        <a class="navbar-brand fw-bold text-dark" href="#">Globent</a>

        <button
          class="navbar-toggler border-0 shadow-none"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#globentNavCollapse"
          aria-controls="globentNavCollapse"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>

        <div class="collapse navbar-collapse" id="globentNavCollapse">
          <ul class="navbar-nav mx-lg-auto gap-lg-4 py-2 py-lg-0">
            <li class="nav-item"><a class="nav-link fw-semibold" href="#">How It Works</a></li>
            <li class="nav-item"><a class="nav-link fw-semibold" href="#">Problems We Fix</a></li>
            <li class="nav-item"><a class="nav-link fw-semibold" href="#">Pricing</a></li>
            <li class="nav-item"><a class="nav-link fw-semibold" href="#">FAQ</a></li>
          </ul>
          <a href="#" class="globent-cta fw-bold text-uppercase">Start Now</a>
        </div>
      </div>
    </nav>
  </header>
</template>

<style scoped>
.navbar-wrap {
  padding: 24px 32px 0;
}

.globent-navbar {
  background-color: #f1f1ef;
  max-width: 1280px;
  margin: 0 auto;
  padding: 0.6rem 0.5rem;
  border-radius: 20px;
}

.nav-link {
  color: #f1705a;
}

.nav-link:hover,
.nav-link:focus {
  color: #dd5b45;
}

.globent-cta {
  color: #f1705a;
  text-decoration: none;
  letter-spacing: 0.3px;
}

.globent-cta:hover {
  color: #dd5b45;
}
</style>
