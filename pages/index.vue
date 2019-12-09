<template>
  <v-app>
    <v-container>
    <div class="d-flex justify-center title" color="red lighten-3">{{question}}</div>
    </v-container>
  </v-app>
</template>

<script>

export default {
  data: function(){
    return {
    question: 'ボタンを押してね！'
    }
  }
}
</script>
