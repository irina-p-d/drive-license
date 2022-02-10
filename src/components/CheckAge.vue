<template>
  <div class="form-age">
   
    <div class="d-flex">
                <input
                    v-bind:type="passwordType" 
                    class="form-control" 
                    placeholder="Introduce tu edad"
                >
                <button 
                    class="btn btn-primary"
                    @click="showPassword"
                >{{showPasswordText}}</button>    
            </div>
    
  </div>
</template>

<script>
export default {
  name: 'CheckAge',
  props: {
    
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.form-age {
  width: 50%;
  margin: 0 auto;
}
</style>
