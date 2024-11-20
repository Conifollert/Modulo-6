<script>
export default {
  name: "App", 
  data() {
    return {
      RUN: "22.222.222-2",
      apellidos: "MUSK",
      nombres: "ELON REVVE",
      nacionalidad: "SUDAFRICANO",
      sexo: "M",
      fechaDeNacimiento: "20 JUN 1972",
      numeroDeDocumento: "222.222.222",
      fechaDeEmision: "01 ENE 2025",
      fechaDeVencimiento: "01 ENE 2030",
    };
  },
};
</script>

<template>

 <div>
  <div class="carnet">
    <aside>
      <div>
        <span>CEDULA DE INDENTIDAD</span>
        <img width="40" src="./assets/img/chile_bandera.png" alt="">
      </div>

      <img src="./assets/img/foto_elon.jpg" alt="">
      <p>RUN {{ RUN }}</p>
    </aside>

    <main>
      <header>
        <p>REPUBLICA DE CHILE</p>
        <span>SERVICIO DE REGISTRO CIVIL E IDENTIFICACION</span>
      </header>

      <section>
        <article>
          <header>APELLIDOS</header>
          <span>{{ apellidos }}</span>
        </article>

        <article>
          <header>NOMBRES</header>
          <span>{{  nombres }}</span>
        </article>

        <div class="grid-2-column">
          <article>
            <header>NACIONALIDAD</header>
            <span>{{ nacionalidad }}</span>
          </article>

          <article>
            <header>SEXO</header>
            <span>{{  sexo }}</span>
          </article>
        </div>

        <div class="grid-2-column">
          <article>
            <header>FECHA DE NACIMIENTO</header>
            <span>{{ fechaDeNacimiento }}</span>
          </article>

          <article>
            <header>NUMERO DE DOCUMENTO</header>
            <span>{{ numeroDeDocumento }}</span>
          </article>
        </div>

          <div class="grid-2-column">
            <article>
              <header>FECHA DE EMISION</header>
              <span>{{ fechaDeEmision }}</span>
            </article>

            <article>
              <header>FECHA DE VENCIMENTO</header>
              <span>{{ fechaDeVencimiento }}</span>
            </article>
          </div>

          <div class="grid-1-column">
          <article>
            <header>FIRMA DE TITULAR</header>
            <span>x A A-12</span>
          </article>
        </div>
      </section>
    </main>
  </div>
 </div>
  
</template>

<style >

body {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 60vh;
  font-size: 10px;
  font-family: sans-serif;
}

.carnet {
  width: 400px;
  height: 230px;
  background: #c8deed;
  border-radius: 20px;
  display: grid;
  grid-template-columns: 30% 1fr;
  padding: 15px;
  box-shadow: 0px 0px 10px 2px black;
}

aside div {
  display: flex;
}

aside > img {
  margin-top: 15px;
  width: 100%;
}

aside p {
  text-align: center;
  font-size: 12px;
  font-weight: bold;
}

main {
  padding: 0px 14px;
}

main article {
  margin: 0px 0px;
}

main article header {
  font-weight: bold;
  color: #0235a4;
  font-size: 8px;
}

main header p {
  font-size: 20px;
  margin: 0;
  font-weight: bold;
  color: #0235a4;
}

main header span {
  font-size: 8px;
  color: #399be1;
}

main section {
  margin-top: 10px;
  text-align: start;
}

main section article span {
  font-size: 13px;
  font-weight: 600;
}

main section .grid-2-column {
  display: grid;
  grid-template-columns: 50% 50%;
  text-align: start;
  width: 100%;
}

main section .grid-1-column {
  display:block;
  grid-template-columns: 100% 0%;
  text-align: start;
}
</style>
