<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header class="ds-header">
      <div class="container text-center">
          <div class="ds-logo">
            <a href="index.html">Holilur Rahman</a>
          </div>
      </div>
    </header>
    <!-- main -->
      <main class="ds-pge-wrap">
        <div class="container">
            <div class="row">
              <div class="col-12 col-sm-12  col-md-6  col-lg-5  col-xl-5  col-xxl-5 ds-left-section">
                  <div class="ds-sticky">
                    <figure>
                      <img src="src/assets/FotoProfile.jpg">
                    </figure>
                    <div class="ds-socail">
                      <span>Contact</span>
                      <ul>
                        <li><a href="mailto:test@test.com">Email</a></li>
                        <li><a href="https://www.instagram.com/holilurrahman._/" target="_blanck">Instagram</a></li>
                        <li><a href="https://github.com/holilurrr" target="_blanck">Github</a></li>
                      </ul>
                    </div>
                  </div>
              </div>
                
              <div class="col-12 col-sm-12  col-md-6  col-lg-7  col-xl-7  col-xxl-7 ds-right-section">
                <RouterView />
              </div>
            </div>
        </div>
      </main>

      <nav class="text-center">
        <RouterLink to="/"><i class="fa-solid fa-user"></i> Personal</RouterLink>
        <RouterLink to="/skill"><i class="fa-regular fa-bookmark"></i> Skill</RouterLink>
      </nav>
      <!-- main -->
      <!-- footer -->
      <footer class="ds-footer">
        <div class="container">
          <span class="ds-copyright">© 2021 All right reserved. <a href="https://wwww.designstub.com/" target="_blanck"></a>Free minimal bootstrap template by Designstub.</span>
        </div>
      </footer>
  
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
