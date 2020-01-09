<template>
  <div class="grocery">
  <input type="checkbox" v-model="checked"/>
    <p @click="onclick(msg)" :class="groceryClass">{{msg}}</p>
  </div>
</template>

<script>
export default {
  name: 'Grocery',
  props: {
    msg: String
  },
  methods: {
      onclick(message) {
          alert(message)
      }  
  },
  data : function() {
    return {
      checked : false
    }
  },
  computed: {
      groceryClass() {
          return {
              strikethrough: this.checked
          }
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.strikethrough {
    text-decoration: line-through;
}
</style>