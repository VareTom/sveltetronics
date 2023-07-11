<script lang="ts">
  import { parallax, pinch } from "sveltronics";
</script>

<main>
  <div class="card" use:parallax={[500, 10]} use:pinch>
    <div class="card__content">
      VareToc
    </div>
  </div>
</main>

<style lang="scss">
  main {
    display: grid;
    align-items: center;
  }
  .card {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 10rem;
    width: 20rem;
    background: rgba( 255, 255, 255, 0.25 );
    box-shadow: 0 .8rem 3.2rem 0 rgba( 31, 38, 135, 0.37 );
    backdrop-filter: blur( .4rem );
    -webkit-backdrop-filter: blur( .4rem );
    border-radius: 1rem;
    border: .1rem solid rgba( 255, 255, 255, 0.18 );

    &__content {
      font-size: 2.4rem;
    }
  }
</style>
