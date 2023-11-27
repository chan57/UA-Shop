<script setup>
import { reactive, ref, onUnmounted } from "vue";

defineProps({
  msg: String,
});

function countinio(str) {
  return str.split("") + " - " + this.color;
}

const count = ref(0);
const count_value = ref(0);
const styleObj = reactive({
  color: "blue",
  fontSize: 30,
});
let victoria = "victoria";
let sett = [...new Set(victoria.split(''))];

const prompromi = new Promise((res, rej) => {
  res('data');
})
prompromi.then((dat)=> console.log(dat));
console.log(countinio.call(styleObj, "stroka"));



// onUnmounted(()=>{

// })
</script>

<template>
  <div>
    <h2>
      {{ sett }}
    </h2>
    <h1
      :style="{ 'font-size': +styleObj.fontSize + 'px', color: styleObj.color }"
    >
      {{ msg }}
    </h1>
  </div>
</template>

<style scoped>
</style>
