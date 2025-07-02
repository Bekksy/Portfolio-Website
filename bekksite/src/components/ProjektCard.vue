<template>
  <div class="karte">
    <h3>{{ projekt.titel }}</h3>
    <p>{{ projekt.beschreibung }}</p>
    <a :href="projekt.link" target="_blank">Zum Projekt</a>
  </div>
</template>

<script>
export default {
  props: ['projekt']
}
</script>

<style scoped>
.karte {
  background: var(--bg);
  padding: 1rem;
  margin-bottom: 1rem;
  border-radius: 8px;
  box-shadow: 0 0 5px rgba(0,0,0,0.1);
}
.karte h3 {
  margin: 0;
}
.karte a {
  display: inline-block;
  margin-top: 0.5rem;
  color: var(--accent-5);
  text-decoration: none;
}
</style>
