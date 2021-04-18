<template>
  <div>
    <img
      src="../../assets/r960-1df4b252f48f766e0f3218b87ee44aff.jpg"
      class="position-fixed"
      :style="'top: -' + Math.floor(parallaxPosition) + 'px'"
      style="z-index: -1; width: 100%; left: 0"
      ref="parallaxImg"
    />
    <div
      class="h1 m-auto fw-bold"
      style="
        color: white;
        padding-bottom: 320px;
        padding-top: 200px;
        font-family: 'Roboto Slab';
        max-width: 1098px;
      "
    >
      Welcome to the Tulsa Geological Society Foundation
    </div>
    <div
      class="row p-4"
      style="background-color: white;"
      v-for="n in 4"
      :key="n"
    >
    <div class="col-sm-4">
        <img
          src="../../assets/r960-1df4b252f48f766e0f3218b87ee44aff.jpg"
          style="width: 100%"
        />
        <div class="fs-10">
        Photo courtesy of D.W. Smith
        </div>
      </div>
      <div class="col-sm-8 text-start">
        <div class="row">
          <div class="h2">Our Mission</div>
        </div>
        <div class="row">
          <p>
            “The Tulsa Geological Society Foundation has been formed to support
            the furtherance of the science of geology and related earth
            sciences, the practice of earth sciences as a profession, and to
            promote the advancement of earth science in all phases through
            educational, scientific, and charitable activities”.
          </p>
        </div>
      </div>
      
    </div>
  </div>
</template>

<script>
import { onMounted, ref } from "vue";
export default {
  name: "Body",
  setup() {
    const parallaxPosition = ref(0);
    const parallaxImg = ref(null);
    const scrollY = ref(window.scrollY);
    function handleScroll() {
      if (scrollY.value > window.scrollY) {
        parallaxPosition.value = 0 + Math.floor(window.scrollY) * 0.2;
      } else {
        parallaxPosition.value = 0 - Math.floor(window.scrollY) * 0.2;
      }
      parallaxImg.value.style.top = parallaxPosition.value + "px";
    }
    onMounted(() => {
      window.addEventListener("scroll", handleScroll);
    })

    return { 
        parallaxPosition, 
        parallaxImg,
        handleScroll
    }
  },
};
</script>

<style scoped>
.fs-10 {
    font-size: 12px
}
</style>