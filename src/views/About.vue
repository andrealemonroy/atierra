<template>
  <div class="about">
    <div id="nav">
      <router-link to="/">INICIO</router-link> |
      <router-link to="/about">QUIÉNES SOMOS</router-link>|
      <div class="animated infinite heartBeat delay-5s slower">
        <router-link to="/projects">NUESTROS PROYECTOS</router-link>
      </div>
    </div>
    <Row type="flex" justify="space-around">
      <Col :lg="20">
        <h1>
          <vue-typer
            :text="[
              'CREEMOS',
              'DESARROLLEMOS',
              'DISEÑEMOS',
              'IDEEMOS',
              'TRABAJEMOS POR'
            ]"
            :repeat="Infinity"
            :shuffle="false"
            initial-action="typing"
            :pre-type-delay="70"
            :type-delay="70"
            :pre-erase-delay="200"
            :erase-delay="500"
            erase-style="select-all"
            :erase-on-complete="false"
            caret-animation="blink"
          ></vue-typer>
        </h1>
      </Col>
    </Row>
    <br />
    <br />
    <Row class="align-center" type="flex" justify="space-around">
      <Col :lg="8">
        <h2>IMPACTO SOCIAL</h2>
        <br />
        <img class="maxw-100" src="../assets/social.png" />
        <br />
        <br />
        <p class="font-22">
          Diseño inclusivo y accesible. Diseñar el mundo digital para tod@s
        </p>
      </Col>
      <Col :lg="8">
        <h2>SOLUCIONES DIGITALES</h2>
        <br />
        <img class="maxw-100" src="../assets/solution.jpg" />
        <br />
        <p class="font-22">
          Mejorar servicios tradicionales implementando soluciones digitales
          innovadoras.
        </p>
      </Col>
    </Row>
    <br />
    <br />
    <Row type="flex" justify="center">
      <Col :lg="10">
        <p class="align-center font-20">
          Queremos aportar en la comunidad LGTB. <br />Buscamos personas
          interesadas en crear proyectos interesantes y ayudar en crearlas y
          generar impacto haciéndolas INCLUSIVAS. Les mostramos un poco de
          nuestro proyecto ATIERRA.
        </p>
      </Col>
    </Row>
    <br />
    <br />
    <Row type="flex" justify="center">
      <Col class="m-auto align-center" :lg="4">
        <img class="br-50 maxw-100" src="../assets/image.jpeg" />
        <br />
        <br />
        <Button><a href="../assets/AndreaMonroy.png">DESCARGAR CV</a></Button>
      </Col>
      <Col class="m-auto align-center" :lg="4">
        <img class="br-50 maxw-100" src="../assets/image-fio.jpeg" />
        <br />
        <br />
        <Button><a>DESCARGAR CV</a></Button>
      </Col>
    </Row>
  </div>
</template>
<script>
import { VueTyper } from "vue-typer";
export default {
  components: {
    // ES6; property shorthand + Vue should automatically dasherize the key for us
    VueTyper
  }
};
</script>
