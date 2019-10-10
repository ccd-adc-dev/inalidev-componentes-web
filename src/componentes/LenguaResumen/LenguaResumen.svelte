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
   let IconoRiesgo = 'iconoRiesgo.svg';
   let IconoFamilia = 'iconoFamilia.svg';
   let IconoVariantes = 'iconoVariante.svg';
      
</script>

<style>
  /* your styles go here */
  .card {
    position: absolute;
    top: 10rem;
    left: 25%;
    width: 18rem;
    height: 21rem; 
    background-color: rgba(236, 236, 236, 0.9);
    border-radius: 2rem 2rem 2rem 0;   
    display: flex;
    flex-direction: column;
    box-shadow: 2px 4px 4px rgba(0, 0, 0, 0.15);
  }

  .Informacion{
    overflow: auto;
    padding: 0rem 2rem 2rem 2rem;
    height: 10rem;
    font-size: 0.8rem;
  }
  
   .NombreFamilia{
    padding: 0rem 0rem 0rem 2rem;
    color:rgba(61, 61, 61, 1);
    text-transform: uppercase;
    letter-spacing: 4px;
    font-weight: 200;
    font-size: 1rem;
    margin: 0px 0px -16px 0px;
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
    margin: 5px 0px 0px 0px;
  }

  .RiesgoDesaparicion{
    padding: 0rem 0rem 0rem 2rem;
    color:rgb(219, 4, 4);
    font-weight: 600;
    font-size: 0.9rem;
    margin: 5px 0px 0px 0px;

  }

  .FamiliaPertenece{
     padding: 0rem 0rem 0rem 2rem;
    color:rgba(61, 61, 61, 1);
    font-weight: 600;
    font-size: 0.9rem;
    margin: 5px 0px 0px 0px;
  }

  .Cerrar {
    display: flex;
    justify-content: flex-end;
    padding: 1rem 1rem 0 0;
  }
  
   .Cerrar a{
    color: rgba(135, 135, 135, 1);
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
     <span class="Cerrar">
      <a href="/">       
          <i class="fa fa-close"></i>
      </a>
     </span>
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
       <!--<p class="NumeroAgrupaciones">
        <span><img src="{IconoAgrupacion}"  alt="agrupacion"></span> Agrupaciones linguísticas      
      </p> -->
       <p class="RiesgoDesaparicion">
        <span><img src="{IconoRiesgo}"  alt="riesgo"></span> Alto riesgo de desaparición      
      </p>
      <p class="FamiliaPertenece">
        <span><img src="{IconoFamilia}"  alt="familia"></span> Familia Yuto-nahua      
      </p>
       <p class="FamiliaPertenece">
        <span><img src="{IconoVariantes}"  alt="variantes"></span> 30 variantes linguísticas      
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