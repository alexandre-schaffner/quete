<script>
  import Header from "$lib/components/Header.svelte";
  import Hero from "$lib/components/Hero.svelte";
  import Navbar from "$lib/components/Navbar.svelte";
</script>

<Header
  title="Quête!"
  moto="Garant du maintient de l'ordre public"
  no="01"
  edition="Juillet 2025"
/>
<div class="flex font-cofo">
  <Navbar
    sections={["Quête - La revue", "Shortlist - Le Bandit du mois de Juillet"]}
  />
  <div class="flex flex-col">
    <div class="flex flex-col">
      <h1 class="text-6xl mb-8 max-w-1/2">La Revue du mois de Juillet 2025</h1>
    </div>
    <Hero />
  </div>
</div>
