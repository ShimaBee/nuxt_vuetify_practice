<template>
  <v-app>
    <v-content class="bg">      
    </v-content>
  </v-app>
</template>


<script>

export default {
  data: function(){
    return {
    question: ['好きな言語は？','好きな動物は？','好きな果物は？'],
    choices:[["C", "Java","Java script","PHP","ruby"],["ゾウ","キリン","カバ","ライオン"],["リンゴ","バナナ","ブドウ","モモ"]]
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
    background-image: url("~@/assets/images/foo.jpg");
  }
  
</style>
