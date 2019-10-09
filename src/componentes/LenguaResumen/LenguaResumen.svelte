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
    left: 25%;
    width: 18rem;
    background-color: rgba(223, 222, 222, 0.9);
    /* height: calc( 100% - 2rem ); */
    /* max-height: 20rem; */
    border-radius: 2rem 2rem 2rem 0;
    height: 21rem;    
    display: flex;
    flex-direction: column;
    box-shadow: 2px 4px 4px rgba(0, 0, 0, 0.15);
  }

  .Informacion{
    overflow: auto;
    font-size: 1rem;
    padding: 0rem 2rem 2rem 2rem;
    height: 9rem;
    font-size: 0.9rem;
  }

  .NombreVariante{
    padding: 0rem 0rem 0rem 2rem;
    font-weight: 600;
    font-size: 1rem;
  }

   .NombreFamilia{
    padding: 0rem 0rem 0rem 2rem;
    color:rgba(61, 61, 61, 1);
    text-transform: uppercase;
    letter-spacing: 3px;
    font-weight: 200;
    font-size: 0.8rem;
  }

  footer {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 3rem;
    background-color: #465D72;
    border-radius: 0 0 2rem 0;
    position: absolute;
    bottom: 0;

  }

  
</style>

<!-- {#if lengua} -->
  <main class="card">
    <header>
      <p class="NombreFamilia">
        Familia
        <!-- {
          lengua.NOM_FAM ? lengua.NOM_FAM :
          lengua.NOM_AGRUP ? lengua.NOM_AGRUP : 
          lengua.NOM_VAR 
        } -->
      </p>   
      <p class="NombreVariante">
        Nahuatl (Del Istmo)
        <!-- {
          lengua.NOM_FAM ? lengua.NOM_FAM :
          lengua.NOM_AGRUP ? lengua.NOM_AGRUP : 
          lengua.NOM_VAR 
        } -->
      </p>
    </header>
    <!-- <button on:click={cerrar}>X</button> -->
    <!-- <button on:click={verMas}>Ver más</button> -->
    <!-- content here -->
    <section>
      <p class="Informacion">
        La familia lingüística yuto-nahua recibe este nombre a partir de que el yute (Ute) es, por un lado, uno de los idiomas que se hablan en el extremo norte del área ocupada por esta familia –el estado de Idaho, en los Estados Unidos de América–, y de que el náhuatl es, por otro lado, el idioma que se habla en el extremo sur de la misma área.
      </p>
    </section>
    <footer>
        <div class="SaberMas">
            Saber mas
        </div>
    </footer>
  </main>
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