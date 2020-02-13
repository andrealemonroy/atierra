<template>
  <div class="home">
    <div id="nav">
      <router-link to="/">INICIO</router-link> |
      <div class="animated infinite heartBeat delay-2s slow">
        <router-link to="/about">QUIÉNES SOMOS</router-link>
      </div>
      |
      <router-link to="/projects">NUESTROS PROYECTOS</router-link>
    </div>
    <br />
    <br />
    <br />
    <br />
    <Row type="flex" justify="space-around">
      <Col class="top-80" :lg="14">
        <br />
        <br />
        <br />
        <br />
        <Row type="flex" justify="space-around">
          <Col :lg="18">
            <h1 class="align-left">
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
        <Row type="flex" justify="space-around">
          <Col :lg="18">
            <h1 class="align-left">UN MUNDO JUNTXS</h1>
          </Col>
        </Row>
      </Col>
      <Col :lg="6">
        <img class="maxw-100 top-20 height-240" src="../assets/world.png" />
      </Col>
    </Row>
  </div>
</template>

<script>
// @ is an alias to /src
import { VueTyper } from "vue-typer";

export default {
  name: "Home",
  components: {
    // ES6; property shorthand + Vue should automatically dasherize the key for us
    VueTyper
  }
};
</script>
