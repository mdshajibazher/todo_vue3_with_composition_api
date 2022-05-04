<template>
  <h1>{{fullName}}</h1>
  <slot name="slot_1"></slot>
  <slot name="slot_2"></slot>
</template>

<script>
export default {
  data() {
    return {
      f_name: "Shajib",
      l_name: "Azher",
    }
  },
  computed: {
    fullName(){
      return this.f_name + ' '+ this.l_name;
    }
  }
}
</script>

