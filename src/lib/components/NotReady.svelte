<script>
  import Button from "./ui/button/button.svelte";
</script>

<div
  class="absolute w-screen h-screen flex flex-col gap-8 items-center justify-center text-center"
>
  <img
    src="/logotype.svg"
    alt="Under Construction"
    class="w-96 h-auto mx-auto stroke-3"
  />
  <p class="text-xl font-cofo-italic max-w-sm">
    Malheureusement cette fonctionnalité n'est pas encore disponible.<br
    />Désolé.
  </p>
  <Button href="/">Retour à l'accueil</Button>
</div>
