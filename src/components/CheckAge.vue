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
                    @click="checkResultAge"
                >Comprobar</button>    
            </div>
    
  </div>
  <div>
      <p>{{ result }}</p>
    </div>
</template>

<script>
export default {
  name: 'CheckAge',
  data(){
    return{
      result:"",
      inputAge:"",
    };
  },
  methods: {
    checkResultAge(){
    let inputAge = this.inputAge;
    if (inputAge == "") {
      this.result = "introduce tu edad"
    }
    else {
      if(inputAge >= 18) {
            this.result = "Puedes conducir";
        }
        else  {
           
          this.result = "No puedes conducir";
        }
    }    
    },
  }, 
}

/* methods: {
    checkCanDrive() {
      let age = this.ageInput;
      if (age == "" || age.match("[a-zA-Z]+")) {
        this.message = "Input inválido, escribe tu edad";
        this.placeholder = "";
      } else {
        if (age >= 18) {
          this.message = "Puede conducir";
        } else {
          this.message = "No Puede conducir";
        }
      }
    },
  },
};
 */
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.form-age {
  width: 50%;
  margin: 0 auto;
}
</style>