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

   let IconoAgrupacion = 'iconoAgrupaciones.svg';
      
</script>

<style>
  /* your styles go here */
  .card {
    position: absolute;
    top: 10rem;
    left: 25%;
    width: 18rem;
    background-color: rgba(236, 236, 236, 0.9);
    border-radius: 2rem 2rem 2rem 0;
    height: 21rem;    
    display: flex;
    flex-direction: column;
    box-shadow: 2px 4px 4px rgba(0, 0, 0, 0.15);
  }

  .Informacion{
    overflow: auto;
    padding: 0rem 2rem 2rem 2rem;
    height: 10rem;
    font-size: 0.9rem;
  }
  
   .NombreFamilia{
    padding: 0rem 0rem 0rem 2rem;
    color:rgba(61, 61, 61, 1);
    text-transform: uppercase;
    letter-spacing: 4px;
    font-weight: 200;
    font-size: 1rem;
    margin: 18px 0px -16px 0px;
  }

  .NombreVariante{
    padding: 0rem 0rem 0rem 2rem;
    font-weight: 600;
    font-size: 1.1rem;
  }

  .SaberMas{
    font-size: 1rem;
    color:rgba(255, 255, 255, 1);

  }

   .SaberMas a{
    font-size: 1rem;
    color:rgba(255, 255, 255, 1);
  }

  .NumeroAgrupaciones{
    padding: 0rem 0rem 0rem 2rem;
    color:rgba(61, 61, 61, 1);
    font-weight: 600;
    font-size: 0.9rem;
    margin: 18px 0px 0px 0px;
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
    <i class="fa fa-arrow-close"></i>
      <p class="NombreFamilia">
        Familia      
      </p>   
      <p class="NombreVariante">
        Nahuatl (Del Istmo)
        <!-- {
          lengua.NOM_FAM ? lengua.NOM_FAM :
          lengua.NOM_AGRUP ? lengua.NOM_AGRUP : 
          lengua.NOM_VAR 
        } -->
      </p>
       <p class="NumeroAgrupaciones">
        <span><img src="{IconoAgrupacion}"  alt=" cultura"></span> Agrupaciones linguísticas      
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
           <a href="/">
                <span>
                  Saber mas
                </span>
                <i class="fa fa-arrow-right"></i>
            </a>
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