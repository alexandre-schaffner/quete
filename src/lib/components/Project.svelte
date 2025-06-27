<script lang="ts">
  import Button from "./ui/button/button.svelte";

  let { index, author, title, description, images, learnMore, isTop1 } =
    $props();

  let votes: number = $state(
    Math.floor(
      Math.random() * (index === "1" ? 100 : index === "2" ? 50 : 25),
    ) + 1,
  );
</script>

<div class="flex flex-col gap-8">
  <h4
    class="text-lg sm:text-xl font-cofo-bold flex flex-col sm:flex-row gap-2 items-center"
  >
    {#if isTop1}
      <span
        class="flex flex-col items-center gap-2 font-cofo-bold text-2xl sm:text-3xl"
      >
        <img src="/svg/BONNET D-ANE.svg" alt="Bonnet d'âne" class="w-[32px]" />
        <span
          class="flex flex-col rounded-full bg-black text-white p-1 w-6 h-6 items-center justify-center"
          style="background: radial-gradient(circle, #000 100%, transparent 100%);"
        >
          {index}
        </span>
      </span>
    {:else}
      <span
        class="rounded-full bg-black text-white p-1 w-6 h-6 flex items-center justify-center"
        style="background: radial-gradient(circle, #000 100%, transparent 100%);"
      >
        {index}
      </span>
    {/if}
    <span class="font-cofo-italic text-right text-xs">0{votes}<br />Votes</span>

    <span class="text-center sm:text-left"
      >{author} - <span class="font-cofo-italic">{title}</span></span
    >
  </h4>
  <div class="flex flex-col md:flex-row gap-4 md:gap-8 h-full">
    <div class="flex gap-2 md:gap-4 justify-center md:justify-start">
      {#each images as image}
        <img
          src={image}
          alt={title}
          class="w-full h-auto object-contain"
          style="aspect-ratio: auto;"
        />
      {/each}
    </div>
    <div class="flex flex-col gap-4 min-h-full w-full md:w-auto">
      <p class="font-cofo-italic max-w-full sm:max-w-xs">{description}</p>
      <div class="flex flex-col sm:flex-row gap-2 mt-auto w-full">
        <Button class="w-full sm:w-auto" onclick={() => (votes += 1)}
          >Je vote pour ce projet</Button
        >
        <Button
          class="bg-gray-200 w-full sm:w-auto"
          variant="secondary"
          href={learnMore}>En savoir plus</Button
        >
      </div>
    </div>
  </div>
</div>
