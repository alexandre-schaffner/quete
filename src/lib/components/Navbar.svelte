<script lang="ts">
  import { onMount } from "svelte";
  let {
    sections,
    shortlistEl,
  }: { sections: string[]; shortlistEl: HTMLElement | null } = $props();
  let currentSection = $state(0);

  function handleScroll() {
    if (!shortlistEl) return;
    const rect = shortlistEl.getBoundingClientRect();
    if (rect.top < window.innerHeight / 2) currentSection = 1;
    else currentSection = 0;
  }

  onMount(() => {
    window.addEventListener("scroll", handleScroll);
    handleScroll();
    return () => window.removeEventListener("scroll", handleScroll);
  });
</script>

<div
  class="hidden sm:flex flex-row sm:flex-col max-w-full sm:max-w-3xs gap-2 sm:gap-4 sm:mt-64 mr-0 sm:mr-12 w-full sm:sticky sm:top-1/2 sm:self-start"
>
  {#each sections as section, index}
    {#if index === currentSection}
      <div>
        <div class="flex">
          <h2 class="text-2xl sm:text-6xl font-black">0{index + 1}.</h2>
          <img
            src="/svg/FLECHE.svg"
            alt="Point d'exclamation"
            class="w-[64px] ml-2 sm:ml-4"
          />
        </div>
        <p class="text-base sm:text-lg">{section}</p>
      </div>
    {:else}
      <div class="text-gray-500">
        <h2 class="font-black text-2xl sm:text-6xl">0{index + 1}.</h2>
        <p class="text-base sm:text-lg">{section}</p>
      </div>
    {/if}
  {/each}
</div>
