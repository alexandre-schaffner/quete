<script>
  import Button from "./ui/button/button.svelte";
</script>

<div class="flex flex-col gap-12 w-full">
  <h2
    class="text-4xl sm:text-6xl mb-8 max-w-full sm:max-w-1/3 text-center sm:text-left"
  >
    La Revue du mois de Juillet 2025
  </h2>
  <div class="flex flex-col lg:flex-row gap-8 lg:gap-16 w-full">
    <div class="w-full lg:flex-1/4 mb-8 lg:mb-0">
      <div class="flex flex-col gap-8 max-w-full sm:max-w-3xs">
        <h3 class="text-2xl sm:text-3xl font-cofo-bold-italic">
          Les Chasseurs De Primes
        </h3>
        <p>
          Publicité Libre<br />Les enjeux d'une agence de publicité indépendante
        </p>
        <p>
          Déborder Bolloré<br />Découverte du projet mené de front par 128
          maisons d'édition indépendantes.
        </p>
        <p>
          Publicité Libre<br />Les enjeux d'une agence de publicité indépendante
        </p>
      </div>
    </div>

    <div class="w-full lg:basis-1/2 min-w-0 mb-8 lg:mb-0">
      <div class="flex flex-col gap-8 w-full">
        <div class="flex flex-col sm:flex-row gap-4 w-full">
          <div class="flex-1">
            <img
              src="/images/COUV_1.jpg"
              alt="Revue Quête"
              class="w-full h-auto object-contain"
              style="aspect-ratio: auto;"
            />
          </div>
          <div class="flex-1 mt-4 sm:mt-0">
            <img
              src="/images/COUV_2.jpg"
              alt="Revue Quête"
              class="w-full h-auto object-cover rounded"
            />
          </div>
        </div>
        <div class="flex flex-col sm:flex-row gap-4 items-center">
          <div class="font-cofo-bold flex">
            <p>
              La revue coûte 13€.<br />
              <span class="font-cofo-italic">Précommande jusqu'au 27 juin.</span
              >
            </p>
          </div>
          <Button class="ml-0 sm:ml-auto w-full sm:w-auto" href="/not-ready"
            >Pré-commande</Button
          >
        </div>
      </div>
    </div>

    <div class="w-full lg:flex-1/4 flex justify-end">
      <div class="flex flex-col gap-8 max-w-full sm:max-w-3xs text-right">
        <h3 class="font-cofo-bold-italic text-2xl sm:text-3xl">Les Bandits</h3>
        <p>
          Etude de cas<br />Le Bandit du mois:<br /><span
            class="font-cofo-italic">Shein par Havas</span
          >
        </p>
        <p>
          <span class="font-cofo-italic">Impact</span><br />La coalition Stop
          Fast Fashion nous raconte son combat
        </p>
        <p>
          <span class="font-cofo-italic">Tout se paie</span><br />Le monde de la
          publicité en 2025
        </p>
      </div>
    </div>
  </div>
</div>
