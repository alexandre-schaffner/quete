<script lang="ts">
  let { sections } = $props();
  let currentSection = $state(0);
</script>

<div class="p-4 max-w-3xs flex flex-col gap-4 mt-64 mr-8">
  {#each sections as section, index}
    {#if index === currentSection}
      <div>
        <h2 class="text-6xl font-black">0{index + 1}.</h2>
        <p>{section}</p>
      </div>
    {:else}
      <div class="text-gray-500">
        <h2 class="font-black text-6xl">0{index + 1}.</h2>
        <p>{section}</p>
      </div>
    {/if}
  {/each}
</div>
