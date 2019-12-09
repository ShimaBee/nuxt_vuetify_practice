<template>
  <v-app>
    <v-container class="bg">
      <v-card class="mx-auto my-12 pb-5" max-width="374">
        <v-card-title class="d-flex justify-center">{{question}}</v-card-title>
        <div class="mx-auto my-2 d-flex justify-center d-flex align-start flex-column">
          <div class="my-4 mx-auto" v-for="(button,index) in btn" :key="index">
            <v-btn x-large color="success">{{button}}</v-btn>
          </div>
        </div>
      </v-card>
    </v-container>
  </v-app>
</template>
<script>

export default {
  data: function(){
    return {
    question: 'ボタンを押してね！',
    btn: ["foo", "boo", "hoge", "fuga"]
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
