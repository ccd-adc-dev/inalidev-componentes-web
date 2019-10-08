<script>
  //import { createEventDispatcher } from 'svelte'
  // your script goes here
  //export let lengua 

//   const dispatch = createEventDispatcher()

// 	const cerrar = (event) => {
//     dispatch('cerrar')
//   }
// 	const verMas = (event) => {
//     dispatch('vermas')
//   }

//   $: console.log(lengua)
</script>

<style>
  /* your styles go here */
  .card {
    position: absolute;
    top: 10rem;
    left: 50%;
    width: 18%;
    background-color: rgba(197, 190, 190, 0.9);
    /* height: calc( 100% - 2rem ); */
    /* max-height: 20rem; */
    border-radius: 2rem 2rem 2rem 0;
    height: 16rem;    
    padding: 2rem;
    display: flex;
    flex-direction: column;
  }

  footer {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    width: 120%;
    height: 3rem;
    background-color: #465D72;
    border-radius: 0 0 2rem 0;

  }

  
</style>

<!-- {#if lengua} -->
  <section class="card">
    <header>
      <h3 class="NombreVariante">
        Nahuatl (Del Istmo)
        <!-- {
          lengua.NOM_FAM ? lengua.NOM_FAM :
          lengua.NOM_AGRUP ? lengua.NOM_AGRUP : 
          lengua.NOM_VAR 
        } -->
      </h3>
      <p>
        Nahuatl (Del Istmo)
      </p>
    </header>
    <!-- <button on:click={cerrar}>X</button> -->
    <!-- <button on:click={verMas}>Ver más</button> -->
    
    <!-- content here -->
    <footer>
        <div class="SaberMas">
            Saber mas
        </div>
    </footer>
  </section>
<!-- {/if} -->


<!-- {#if lengua}
  <div class="card">
    <header>
      <h2>
        {
          lengua.NOM_FAM ? lengua.NOM_FAM :
          lengua.NOM_AGRUP ? lengua.NOM_AGRUP : 
          lengua.NOM_VAR 
        }
      </h2>
    </header>
    <button on:click={cerrar}>X</button>
    <button on:click={verMas}>Ver más</button>
    
    content here
  </div>
{/if} -->