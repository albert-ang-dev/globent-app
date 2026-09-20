<script setup>
const year = new Date().getFullYear()

const columns = [
  {
    heading: 'Product',
    links: ['How It Works', 'Pricing', 'FAQ'],
  },
  {
    heading: 'Company',
    links: ['About', 'Contact', 'Blog'],
  },
  {
    heading: 'Legal',
    links: ['Terms of Service', 'Privacy Policy', 'Disclaimer (not affiliated with CBP/DHS)'],
  },
]
</script>

<template>
  <footer class="site-footer py-5">
    <div class="container">
      <div class="row g-4">
        <div v-for="column in columns" :key="column.heading" class="col-md-4">
          <p class="footer-heading fw-bold mb-3">{{ column.heading }}</p>
          <ul class="list-unstyled mb-0">
            <li v-for="link in column.links" :key="link" class="mb-2">
              <a href="#" class="footer-link">{{ link }}</a>
            </li>
          </ul>
        </div>
      </div>

      <hr class="footer-divider my-4">

      <p class="footer-copyright mb-0">
        © {{ year }} Globent. Not affiliated with U.S. Customs and Border Protection.
      </p>
    </div>
  </footer>
</template>

<style scoped>
.site-footer {
  background-color: #2b2420;
  color: #cfc9c4;
}

.footer-heading {
  color: #fff;
}

.footer-link {
  color: #cfc9c4;
  text-decoration: none;
}

.footer-link:hover {
  color: #f1705a;
}

.footer-divider {
  border-color: #4a423d;
  opacity: 1;
}

.footer-copyright {
  color: #a49e99;
  font-size: 0.9rem;
}
</style>
