<script>
import vueTimepicker from 'src/vue-timepicker.vue'


export default {
    data(){
        return {
            yourTimeValue: {
                HH: "06",
                mm: "00",
            },
        }
    },
  components: {
      'vue-timepicker': vueTimepicker,
  }
}
</script>

<template>
    <div>
        <vue-timepicker
                format="HH:mm"
                v-model="yourTimeValue"
                :hide-clear-button="true"
                :minute-interval="5"
                :startHour="4"
        ></vue-timepicker>



        <vue-timepicker
                format="HH:mm"
                v-model="yourTimeValue"
                :hide-clear-button="true"
                :minute-interval="5"
                :startHour="4"
        ></vue-timepicker>
    </div>
</template>

<style lang="sass">
@import "./assets/demo.scss";
</style>
