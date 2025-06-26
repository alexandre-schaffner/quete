<script lang="ts">
  const {
    title = "Quête",
    moto = "Garant du maintient de l'ordre public",
    no,
    edition,
  } = $props();
</script>

<div class="p-4 flex flex-col sm:flex-row items-center gap-4 sm:gap-0">
  <div
    class="flex gap-4 items-center w-full sm:w-auto justify-center sm:justify-start"
  >
    <img
      src="/logotype.svg"
      alt="Logo"
      class="w-32 min-w-0 max-w-full h-auto object-contain"
      style="aspect-ratio: auto;"
    />
    <!-- <h1 class="text-4xl">{title}</h1> -->
    <p
      class="w-full sm:w-5/12 font-cofo-italic text-center sm:text-left text-base sm:text-lg"
    >
      {moto}
    </p>
  </div>
  <div
    class="flex flex-col ml-0 sm:ml-auto items-center sm:items-end w-full sm:w-auto mt-4 sm:mt-0"
  >
    <p class="text-sm sm:text-base">Numéro {no}</p>
    <p class="text-xs sm:text-base">{edition}</p>
  </div>
</div>
