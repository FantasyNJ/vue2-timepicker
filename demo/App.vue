<script>
import vueTimepicker from 'src/vue-timepicker.vue'


export default {
    data(){
        return {
            yourTimeValue: {
                HH: "06",
                mm: "00",
            },
            value: {
                HH: "",
                mm: "",
            }
        }
    },
  components: {
      'vue-timepicker': vueTimepicker,
  }
}
</script>

<template>
    <div>
        <!--<vue-timepicker-->
                <!--format="HH:mm"-->
                <!--v-model="yourTimeValue"-->
                <!--:minute-interval="5"-->
                <!--:startHour="4"-->
        <!--&gt;</vue-timepicker>-->

        <vue-timepicker
                format="HH:mm"
                v-model="value"
                :hide-clear-button="false"
                :minute-interval="5"
                :startHour="4"
                error="haha"
        ></vue-timepicker>
    </div>
</template>

<style lang="sass">
@import "./assets/demo.scss";
</style>
