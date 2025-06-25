<script lang="ts">
  const {
    title = "Quête",
    moto = "Garant du maintient de l'ordre public",
    no,
    edition,
  } = $props();
</script>

<div class="p-4 flex items-center">
  <div class="flex gap-4 items-center">
    <img src="/logotype.svg" alt="Logo" class="w-32" />
    <!-- <h1 class="text-4xl">{title}</h1> -->
    <p class="w-5/12 font-cofo-italic">{moto}</p>
  </div>
  <div class="flex flex-col ml-auto">
    <p>Numéro {no}</p>
    <p>{edition}</p>
  </div>
</div>
