<script lang="ts">
    import '../app.css';
    import '$lib/theme.css';
    let { children } = $props();
</script>

<div class="wrap gradient-surface">
  <main class="container">
    {@render children()}
  </main>
  <footer class="footer">
    <p>Simple Notes Organizer</p>
  </footer>
</div>

<style>
  .wrap {
    min-height: 100vh;
    display: grid;
    grid-template-rows: auto 1fr auto;
  }
  .container {
    width: 100%;
    max-width: 920px;
    margin: 0 auto;
    padding: 1rem;
  }
  .footer {
    text-align: center;
    color: #64748b;
    font-size: 0.85rem;
    padding: 1rem 0 2rem;
  }
</style>
