<template>
  <v-app>
    <v-content class="bg">   
        <v-card class="mx-3 my-12 pb-5" max-width="374">
          <v-card-title class="d-flex justify-center py-10">{{question}}</v-card-title>
          <div class="mx-auto my-2 d-flex justify-center d-flex align-start flex-column">
            <div class="mx-auto" v-for="(button,index) in btn" :key="index">
              <v-btn width="230" height="50" rounded class="cyan accent-2 mb-8">{{button}}</v-btn>
            </div>
          </div>
        </v-card>    
    </v-content>
  </v-app>
</template>


<script>

export default {
  data: function(){
    return {
    question: '好きな言語はなんですか？',
    btn: ["C", "Java","Java script","PHP","ruby"]
    }
  }
}

</script>

<style>

  .bg {
    width: 100%;
    height: 100%;
    position: absolute;
    top: 0;
    left: 0;
    background-size: cover;
    background-image: url("~@/assets/foo.jpg");
  }
  
</style>
