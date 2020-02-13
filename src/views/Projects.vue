<template>
  <div>
    <div id="nav">
      <router-link to="/">INICIO</router-link> |
      <router-link to="/about">QUIÉNES SOMOS</router-link>|
        <router-link to="/projects">NUESTROS PROYECTOS</router-link>
    </div>
    
    
          <div class="container center-container section__hero">
        <div class="section__form bg-white p-4  shadow-md rounded center-feriaza">
          <h1 class="mb-2 text-4xl font-bold text-grey-darkest title-center">FERIAZA</h1>
          <h2 class="mb-6 text-base text-grey-dark font-bold title-about" style="color:#38a89d">
            Encuentra espacios ideales para tu marca
          </h2>
              <form class="form__search">
                <Button type="success" 
                  class="px-2 py-4 bg-yellow-dark font-semibold w-full rounded text-yellow-darker"
                >
                  VER PROYECTO
                </Button>
              </form>
        </div>
      </div>
  </div>
</template>


<style>
@import url("https://fonts.googleapis.com/css?family=Permanent+Marker&display=swap");

.section__hero {
  min-height: 450px;
  background-image: url("../assets/4.png");
  display: -webkit-box;
  display: -moz-box;
  display: -ms-flexbox;
  display: -webkit-flex;
  display: flex;
  justify-content: center;
  align-items: center;
}

.title-center {
  font-size: 5em !important;
  font-family: "Permanent Marker", cursive;
}

.title-brand-modal {
  font-size: 2em !important;
  font-family: "Permanent Marker", cursive;
}

.title-about {
  font-size: 2em !important;
}

.form__field .input-icon {
  top: 7px;
  left: 9px;
}

.form__field > .input__search {
  @apply pl-10;
}

.center-feriaza {
  background-color: rgba(255, 255, 255, 0.85) !important;
  display: flex;
  justify-content: center !important;
  flex-direction: column;
  align-items: center;
}

/* .center-container {
  width: 50% !important;
} */

  .align-button {
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center !important;
    display: flex;
  }

@media (max-width: 576px) {
  .section__hero {
    min-height: 250px;
  }

  .title-center {
    font-size: 2em !important;
  }

  .title-about {
    font-size: 1.3em !important;
  }

  .center-container {
    width: 90% !important;
  }

  .section__form {
    @apply w-full;
  }
}

@media (min-width: 576px) {
  /* .center-feriaza{
    width: 350px !important;
  } */
}

@media (min-width: 768px) {
  .ivu-col-span-md-10 {
    display: block;
    width: 80% !important;
  }
}
</style>
