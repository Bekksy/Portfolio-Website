<template>
  <div class="seite">
    <header>
      <section class= Page1>
      <div class="hero-layout" >
          <div class="hero-stack">
            <p class="hero-left-top">I AM</p>
            <h1 class="hero-center" id="seitentitel">BEKKS</h1>
            <p class="hero-right-bottom"> developer • designer • dreamer</p>
          </div>
        </div>
        <div class="social-row">
           <svg id="menu-icon" width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M4 6H20M4 12H20M4 18H20"
                    stroke="#000000"
                    stroke-width="2"
                    stroke-linecap="round"
                    stroke-linejoin="round" />
            </svg>
          <div class="social-icons">
            <a href="https://github.com/Bekksy" target="_blank" aria-label="GitHub">
              <svg xmlns="http://www.w3.org/2000/svg" width="15" height="15" class="social-icon" viewBox="0 0 24 24">
              <path d="M12 0.297c-6.63 0-12 5.373-12 12 0 5.302 3.438 9.8 8.205 
              11.385 0.6 0.113 0.82-0.258 0.82-0.577 
              0-0.285-0.01-1.04-0.015-2.04-3.338 
              0.724-4.042-1.61-4.042-1.61-0.546-1.385-1.333-1.754-1.333-1.754-1.089-0.745 
              0.084-0.729 0.084-0.729 1.205 0.084 
              1.838 1.236 1.838 1.236 1.07 1.835 
              2.809 1.305 3.495 0.998 0.108-0.776 
              0.418-1.305 0.76-1.605-2.665-0.3-5.467-1.335-5.467-5.93 
              0-1.31 0.469-2.381 1.236-3.221-0.124-0.303-0.536-1.523 
              0.117-3.176 0 0 1.008-0.322 3.301 
              1.23a11.52 11.52 0 013.003-0.404c1.018 
              0.005 2.042 0.138 3.003 0.404 2.291-1.552 
              3.297-1.23 3.297-1.23 0.655 1.653 
              0.243 2.873 0.119 3.176 0.77 0.84 
              1.234 1.911 1.234 3.221 0 4.61-2.807 
              5.625-5.479 5.921 0.43 0.372 0.823 
              1.102 0.823 2.222 0 1.606-0.015 
              2.896-0.015 3.293 0 0.319 0.216 
              0.694 0.825 0.576 4.765-1.587 
              8.2-6.084 8.2-11.385 0-6.627-5.373-12-12-12z"/>
              </svg>
            </a>
            <a href="https://www.linkedin.com/in/rebekka-rieseberg-6ba079363" target="_blank" aria-label="LinkedIn">
              <svg xmlns="http://www.w3.org/2000/svg" width="15" height="15" class="social-icon" viewBox="0 0 24 24">
                <path d="M4.98 3.5C4.98 4.88 3.87 6 2.5 6S0 4.88 0 3.5 1.12 1 2.5 1s2.48 1.12 2.48 2.5zM.5 8h4V24h-4V8zm7.5 0h3.7v2.1h.1c.5-.9 1.7-2.1 3.5-2.1 3.8 0 4.5 2.5 4.5 5.7V24h-4v-8.3c0-2-.03-4.5-2.7-4.5s-3.1 2.1-3.1 4.3V24h-4V8z"/>
              </svg>
            </a>
            <a href="https://www.xing.com/profile/Rebekka_Rieseberg" target="_blank" aria-label="Xing">
              <svg xmlns="http://www.w3.org/2000/svg" width="15" height="15" class="social-icon" viewBox="0 0 24 24">
                <path d="M16.66 3h3.63L14.9 13.19 21.99 24H18.3l-7.09-10.81L16.66 3zM7.86 7.33 10.14 11 5.72 18H2.05L6.47 11 4.19 7.33h3.67z"/>
              </svg>
            </a>
          </div>
      </div>
      </section>
    </header>

    <main>
      <section id="projekte">
        <h2 id="projekt-titel">Projekte</h2>
        <div class="projekt-grid">
          <ProjektCard
            v-for="projekt in projekte"
            :key="projekt.titel"
            :projekt="projekt"
          />
        </div>
      </section>
    </main>
     
    <footer>
      <p>&copy; 2025 Bekks</p>
    </footer>
  </div>
</template>

<script>
import ProjektCard from './components/ProjektCard.vue'

export default {
  components: {
    ProjektCard
  },
  data() {
    return {
      projekte: [
        {
          titel: 'Kartenspiel',
          beschreibung: 'Ein kleines Spiel, das ich in Java entwickelt habe.',
          link: '..'
        },
        {
          titel: 'LineAO and PointAO',
          beschreibung: 'Ein Tool zur grafischen Darstellung von Daten.',
          link: '..'
        },
        {
          titel: 'JavaScript',
          beschreibung: 'Ein Tool zur grafischen Darstellung von Daten.',
          link: '..'
        },
        {
          titel: 'CG-Projekte',
          beschreibung: 'Ein Tool zur grafischen Darstellung von Daten.',
          link: '..'
        }
      ]
    }
  }
}
</script>

