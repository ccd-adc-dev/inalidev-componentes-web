<script>
  import Lateral from "../Lateral/Lateral.svelte";
</script>

<style>

dl {
    display: grid;
    grid-template-columns: 1fr 1fr;
}

</style>
<svelte:head>
  <title>Glosario INALI</title>
</svelte:head>


<Lateral backgroundColor="rgba(70, 93, 114,0.85)">

  <h1>Glosario</h1>

  <dl>

    <dt>
        Familia lingüística..................................
    </dt>
    <dd>
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dolorem accusantium voluptatibus, dolore obcaecati ipsam ratione molestiae ab eius ullam, hic officia? Voluptatem, commodi nobis.</p>
        <p>Porro atque amet architecto odit, fugit magni cumque, id ad beatae delectus odio itaque doloribus, nihil nostrum tempora placeat neque dignissimos? Magni, voluptates repellendus.</p>
    </dd>

    <dt>
        Otro término de glosario
    </dt>
    <dd>
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dolorem accusantium voluptatibus, dolore obcaecati ipsam ratione molestiae ab eius ullam, hic officia? Voluptatem, commodi nobis.</p>
        <p>Porro atque amet architecto odit, fugit magni cumque, id ad beatae delectus odio itaque doloribus, nihil nostrum tempora placeat neque dignissimos? Magni, voluptates repellendus.</p>
    </dd>

    <dt>
        Término
    </dt>
    <dd>
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dolorem accusantium voluptatibus, dolore obcaecati ipsam ratione molestiae ab eius ullam, hic officia? Voluptatem, commodi nobis.</p>
        <p>Porro atque amet architecto odit, fugit magni cumque, id ad beatae delectus odio itaque doloribus, nihil nostrum tempora placeat neque dignissimos? Magni, voluptates repellendus.</p>
    </dd>

  </dl>

</Lateral>
