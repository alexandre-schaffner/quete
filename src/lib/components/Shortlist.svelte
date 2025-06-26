<script>
  import Project from "./Project.svelte";
</script>

<div id="shortlist">
  <h3
    class="text-3xl sm:text-5xl font-cofo-bold max-w-full sm:max-w-1/2 mb-8 sm:mb-12 text-center sm:text-left"
  >
    Shortlist - Le Bandit du mois de Juillet 2025
  </h3>
  <div class="flex flex-col gap-8 sm:gap-16">
    <Project
      index="1"
      author="KLM"
      title="Fly Responsibly"
      description={`La campagne "Fly Responsibly" de KLM encourageait à compenser les émissions de CO₂ et à envisager d'autres modes de transport. KLM se présentait comme un acteur engagé pour un avenir plus vert, malgré l'impact considérable du secteur aérien sur le climat. Cette initiative a été vivement critiquée pour greenwashing, car elle donnait l'impression qu'il était possible de « voler de manière responsable », ce que beaucoup d'ONG environnementales jugent trompeur.`}
      votes={20}
      images={["/images/FLY_RESPONSIBLY.png"]}
      learnMore="https://www.lemonde.fr/economie/article/2024/03/21/klm-perd-un-proces-pour-greenwashing-aux-pays-bas_6223250_3234.html"
      isTop1={true}
    />
    <Project
      index="2"
      author="Cannes Lions 2025"
      title="Les Safes Zones"
      description={`Les Cannes Lions mettent cette année en place des Safes Zones. Une Safe Zone est un espace sécurisé destiné à protéger et soutenir les personnes se sentant en danger ou mal à l'aise lors d'un événement.Le problème, c'est que ces zones isolent les victimes au lieu de prévenir ou punir les comportements abusifs, ce qui reporte la responsabilité sur elles plutôt que sur les agresseurs.`}
      votes={16}
      images={["/images/CANNES_LION.png"]}
      learnMore="https://lareclame.fr/cannes-lions-2025-safe-zone-metoo-316525"
      isTop1={false}
    />
    <Project
      index="3"
      author="SNCF"
      title="Augmentation des écrans publicitaires"
      description={`En 2025, le nombre d'écrans publicitaires dans les gares françaises va fortement augmenter. Le problème, c'est que cette prolifération transforme des lieux de passage en espaces de consommation forcée, saturant l'environnement visuel sans réel consentement. Ce développement est le fruit de choix d'acteurs du transport privé, dont la SNCF.`}
      votes={20}
      images={["/images/PUB_TRANSPORT.png"]}
      learnMore="https://reporterre.net/Les-ecrans-publicitaires-dans-les-gares-vont-proliferer-en-2025"
      isTop1={false}
    />
  </div>
</div>
