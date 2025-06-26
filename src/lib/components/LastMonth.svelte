<script>
  import Button from "./ui/button/button.svelte";
</script>

<div class="flex flex-col gap-12">
  <h3
    class="text-2xl sm:text-3xl font-cofo-bold-italic max-w-full sm:max-w-3xs"
  >
    Le Bandit du mois de Juin
  </h3>
  <div class="flex flex-col md:flex-row gap-8 max-w-full">
    <div class="flex flex-col basis-full md:basis-1/2 gap-8">
      <div class="flex flex-col sm:flex-row gap-4">
        <img
          src="/images/PRINT_1.png"
          alt="Quête - print 1"
          class="w-full sm:w-1/2 max-w-xs h-auto"
          style="aspect-ratio: auto;"
        />
        <img
          src="/images/PRINT_2.png"
          alt="Quête - print 2"
          class="w-full sm:w-1/2 max-w-xs h-auto"
          style="aspect-ratio: auto;"
        />
      </div>
      <p class="max-w-full sm:max-w-md">
        Collection d'affiches du Bandit du mois<br />Premier Prix décerné à
        Havas France pour la campagne Shein.
      </p>
      <div class="flex flex-col sm:flex-row mt-auto gap-4 sm:gap-16">
        <p class="font-cofo-italic max-w-full sm:max-w-md">
          Imprimé en France, en papier recyclé.<br />Le pack de 4 affiches coûte
          8€.<br />100% des bénéfices (4€/pack) sont reversés à la Coalition
          Stop Fast Fashion.
        </p>
        <Button class="mt-4 sm:mt-auto w-full sm:w-auto">Pré-commande</Button>
      </div>
    </div>
    <img
      src="/images/PRINT_3.png"
      alt="Quête - print 3"
      class="aspect-auto md:w-1/2 self-start"
    />
  </div>
</div>
