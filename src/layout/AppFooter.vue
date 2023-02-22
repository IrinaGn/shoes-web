<template>
  <section class="footer">
    <div class="container">
      <iframe
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2719.780566939694!2d28.820627999999996!3d47.024912099999995!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x40c97d581230cee1%3A0x4d23504ec74fb6b1!2z0KDQtdC80L7QvdGCINC-0LHRg9Cy0Lgg0Lgg0YPRhdC-0LQg0LfQsCDQutC-0LbQsNC90YvQvNC4INC40LfQtNC10LvQuNGP0LzQuCBTaG9lc21ha2VybWQ!5e0!3m2!1sru!2s!4v1653604042198!5m2!1sru!2s"
        width="100%"
        height="400"
        style="border: 0"
        allowfullscreen=""
        loading="lazy"
        referrerpolicy="no-referrer-when-downgrade"
      >
      </iframe>
    </div>
    <div>
      <h5>2022 Shoesmaker</h5>
    </div>
  </section>
</template>

<script>
export default {
  name: "AppFooter",
  props: {
    //msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.footer {
  background-color: #7b5438;
  color: rgb(255, 255, 255);
  padding-bottom: 10px;
}
</style>
