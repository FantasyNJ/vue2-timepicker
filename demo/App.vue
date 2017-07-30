<script>
import vueTimepicker from 'src/vue-timepicker.vue'


export default {
  components: {
      'vue-timepicker': vueTimepicker,
  }
}
</script>

<template>
    <div>
        <vue-timepicker></vue-timepicker>
    </div>
</template>

<style lang="sass">
@import "./assets/demo.scss";
</style>
