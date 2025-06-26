<script>
  import Header from "$lib/components/Header.svelte";
  import Hero from "$lib/components/Hero.svelte";
  import LastMonth from "$lib/components/LastMonth.svelte";
  import Navbar from "$lib/components/Navbar.svelte";
  import Shortlist from "$lib/components/Shortlist.svelte";
</script>

<Header
  title="Quête!"
  moto="Garant du maintient de l'ordre public"
  no="01"
  edition="Juillet 2025"
/>
<div class="flex flex-col sm:flex-row font-cofo p-2 sm:p-4 gap-4 sm:gap-0">
  <Navbar
    sections={["Quête - La revue", "Shortlist - Le Bandit du mois de Juillet"]}
  />
  <div class="flex flex-col w-full gap-16 sm:gap-32">
    <Hero />
    <LastMonth />
    <Shortlist />
  </div>
</div>
