<template>
  <h1 class="home">
    Hacemos páginas increíbles con
    <vue-typer
      :text="['VueJs', 'Angular', 'Wordpress (PHP)']"
      :repeat="Infinity"
      :shuffle="false"
      initial-action="typing"
      :pre-type-delay="70"
      :type-delay="70"
      :pre-erase-delay="2000"
      :erase-delay="250"
      erase-style="select-all"
      :erase-on-complete="false"
      caret-animation="blink"
    ></vue-typer>
  </h1>
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
