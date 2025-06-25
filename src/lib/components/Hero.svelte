<script>
  import Button from "./ui/button/button.svelte";
</script>

<div class="flex flex-col gap-12">
  <h2 class="text-2xl font-cofo-bold-italic w-3xs text-wrap">
    Les Chasseurs De Primes
  </h2>
  <div class="flex gap-16">
    <div class="flex flex-col gap-4 max-w-3xs">
      <p>
        Publicité Libre<br />Les enjeux d'une agence de publicité indépendante
      </p>
      <p>
        Déborder Bolloré<br />Découverte du projet mené de front<br />par 128
        maisons d'édition indépendantes.
      </p>
      <p>
        Publicité Libre<br />Les enjeux d'une agence<br />de publicité
        indépendante
      </p>
    </div>
    <div class="flex flex-col">
      <div class="flex gap-4 w-fit">
        <img
          src="/images/hero.png"
          alt="Image de la revue Quête"
          class="bg-gray-200 h-full aspect-[2/3] w-auto max-h-96"
        />
        <img
          src="/images/hero.png"
          alt="Image de la revue Quête"
          class="bg-gray-200 h-full aspect-[2/3] w-auto max-h-96"
        />
      </div>

      <div class="flex gap-4 w-min">
        <div class="font-cofo-bold flex mx-auto w-md">
          <p class="mr-auto">
            La revue coûte 13€.<br />
            <span class="font-cofo-italic">Précommande jusqu'au 27 juin.</span>
          </p>
        </div>
        <Button class="ml-auto">Pré-commande</Button>
      </div>
    </div>

    <div class="flex flex-col gap-4 text-right pr-4">
      <h3 class="font-cofo-bold-italic text-3xl">Les Bandits</h3>
      <p>
        Etude de cas<br />Le Bandit du mois:<br /><span class="font-cofo-italic"
          >Shein par Havas</span
        >
      </p>
      <p>
        <span class="font-cofo-italic">Impact</span><br />La coalition Stop Fast
        Fashion<br />
      </p>
      <p>
        <span class="font-cofo-italic">Publicité Libre</span><br />Les enjeux
        d'une agence de publicité indépendante
      </p>
    </div>
  </div>
</div>
