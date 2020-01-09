<template>
  <div class="groceries">
    <h1>Liste de courses</h1>
    <Grocery v-for= "grocery in groceries"  :key="grocery"  :msg="grocery"/>
  </div>
</template>

<script>
import Grocery from './Grocery.vue'
export default {
  name: 'Groceries',
  data : function() {
    return {
      groceries : ["biere", "rhum", "pastis", "saucisson"]
    }
  },
  components: {
    Grocery
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>