<script lang="ts">
  import NoteForm from "$lib/components/NoteForm.svelte";
  import NotesList from "$lib/components/NotesList.svelte";
</script>

<svelte:head>
  <title>Simple Notes Organizer</title>
  <meta name="description" content="Create, view, and organize your notes with a modern, ocean-inspired Svelte app." />
</svelte:head>

<header class="header card">
  <div class="brand">
    <div class="logo">📝</div>
    <div>
      <h1>Simple Notes Organizer</h1>
      <p class="subtitle">Capture ideas quickly. Find them faster.</p>
    </div>
  </div>
</header>

<section class="column">
  <NoteForm />
  <NotesList />
</section>

<style>
  .header {
    margin-top: 1rem;
    padding: 1rem;
  }
  .brand {
    display: flex;
    gap: 0.75rem;
    align-items: center;
  }
  .logo {
    width: 42px;
    height: 42px;
    display: grid;
    place-items: center;
    font-size: 1.35rem;
    border-radius: 12px;
    background: radial-gradient(120px 60px at 20% 10%, rgba(37,99,235,.25), rgba(255,255,255,0.9));
    box-shadow: 0 6px 18px rgba(37,99,235,.25);
  }
  h1 {
    margin: 0;
    font-size: 1.35rem;
  }
  .subtitle {
    margin: 0.2rem 0 0;
    color: #64748b;
  }
  .column {
    display: grid;
    gap: 1rem;
    margin-top: 1rem;
  }
</style>
