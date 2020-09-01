<template>
  <section class="sectionTwo-warrper">
    <div class="container">
      <div class="row">
        <div class="col-md-10 mx-auto text-center">
          <h2 class="text-primary text-title">{{ $t("sectionTwo.title") }}</h2>
          <p class="text-muted lead">{{ $t("sectionTwo.textp1") }}</p>
          <p class="text-muted lead">{{ $t("sectionTwo.textp2") }}</p>
          <p class="text-muted lead">{{ $t("sectionTwo.textp3") }}</p>
          <p class="text-muted lead">{{ $t("sectionTwo.textp4") }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "sectionTwo"
};
</script>

<style lang="scss">
.sectionTwo-warrper {
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
}
</style>
