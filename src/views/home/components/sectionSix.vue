<template>
  <section class="sectionSix-warrper">
    <div class="container">
      <div class="row">
        <div class="col-md-6 mx-auto text-center">
          <h2 class="text-primary text-title">{{ $t("sectionSix.title") }}</h2>
        </div>
      </div>
      <div class="row d-md-flex mt-4 text-center">
        <div class="col-md-3 mt-2 list" v-for="item in 8" :key="item">
          <img />
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: "sectionSix"
};
</script>
<style lang="scss">
.sectionSix-warrper {
  padding: 5rem 0 5rem 0;
  .text-title {
    font-size: 2rem;
    font-weight: bold;
    color: #fb203b !important;
    padding-bottom: 2rem;
  }
  .text-muted {
    text-align: left;
    padding-bottom: 1rem;
  }
  .list {
    img {
      display: block;
      height: 5rem;
      width: 100%;
      background-color: #959595;
    }
  }
}
</style>
