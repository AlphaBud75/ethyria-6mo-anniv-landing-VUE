<template>
  <div class="container">
    <h1>{{ msg }}</h1>
    <div class="subcontainer">
      <a
        href="https://6months.ennaalouette.com/#/"
        target="_blank"
        rel="noopener noreferrer"
      >
        <img id="enna" src="@/assets/SectionPortals/enna.jpg" alt="enna.jpg" />
      </a>
    </div>

    <div class="subcontainer">
      <a href="" target="_blank" rel="noopener noreferrer">
        <img id="nina" src="@/assets/SectionPortals/nina.jpg" alt="nina.jpg" />
      </a>
    </div>

    <div class="subcontainer">
      <a href="" target="_blank" rel="noopener noreferrer">
        <img
          id="reimu"
          src="@/assets/SectionPortals/reimu.jpg"
          alt="reimu.jpg"
        />
      </a>
    </div>

    <div class="subcontainer">
      <a
        href="https://6months.millieparfait.com/#/"
        target="_blank"
        rel="noopener noreferrer"
      >
        <img
          id="millie"
          src="@/assets/SectionPortals/millie.jpg"
          alt="millie.jpg"
        />
      </a>
    </div>
    <div class="subcontainer_bottom_text">
      <a href="" target="_blank" rel="noopener noreferrer">
        <img
          id="ethyria_text"
          src="@/assets/SectionPortals/ethyria_text.jpg"
          alt="ethyria_text.jpg"
        />
      </a>
    </div>
  </div>

  <div class="container" style="background-color: black; color: yellow">
    <h1>TO DO</h1>
    <ol>
      <li>5 PFPs and bot text pic</li>
      <li>background (tile) pic</li>
      <li>Nina and Reimu's links ??</li>
      <li>Test media query</li>
      <li>header footer.....</li>
      <li>delete green border</li>
      <li>art and words(learning vue3)</li>
    </ol>
  </div>
</template>

<script>
export default {
  name: 'SectionPortals',
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
// body {
//   background-image: url("background_pic.png");
//   background-repeat: repeat;
// }

div.container {
  margin: auto;
  border: 10px solid green;
  display: table;
}

div.subcontainer {
  display: inline-flex;
  margin: 0px;
}

div.subcontainer_bottom_text {
  margin-top: -5px;
}

.subcontainer img {
  -webkit-transition: transform 0.8s ease-in-out;
  -moz-transition: transform 0.8s ease-in-out;
  transition: transform 0.8s ease-in-out;
}

.subcontainer:hover img {
  -moz-transform: scale(1.2);
  -webkit-transform: scale(1.2);
  -o-transform: scale(1.2);
  -ms-transform: scale(1.2);
  -webkit-transform: scale(1.2);
  transform: scale(1.2);
  z-index: 99;
}

@media only screen and (max-width: 1400px) {
  div.container {
    zoom: 0.7;
  }
}

@media only screen and (max-width: 1000px) {
  div.container {
    zoom: 0.6;
  }
}

@media only screen and (max-width: 850px) {
  div.container {
    zoom: 0.5;
  }
}

/* phones */

@media only screen and (max-width: 700px) {
  div.container {
    zoom: 0.25;
  }
}
</style>
