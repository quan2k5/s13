<script setup>
import LocalMallIcon from '@mui/icons-material/LocalMall';
import Ex1 from './components/Ex1.vue'
import Ex2 from './components/Ex2.vue'
import Ex3 from './components/Ex3.vue'
import Ex4 from './components/Ex4.vue'
import Ex5 from './components/Ex5.vue'
import Ex6 from './components/Ex6.vue'
import Ex7 from './components/Ex7.vue'
import Ex8 from'./components/Ex8.vue'
import Ex9 from './components/Ex9.vue'
import Ex10 from './components/Ex10.vue'
</script>
<template>
<div>
  <h1>vuetify</h1>
  <v-btn color="warning">click</v-btn>
  <button>click</button>
  <v-text-field label="email" width="200px"></v-text-field>
  <v-select label='moi chon phong ban' :items="['phong ke toan','phong bao ve','phong ky thuat']"></v-select>
  <!-- <v-carousel>
  <v-carousel-item
    src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
    cover
  ></v-carousel-item>

  <v-carousel-item
    src="https://cdn.vuetifyjs.com/images/cards/hotel.jpg"
    cover
  ></v-carousel-item>

  <v-carousel-item
    src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
    cover
  ></v-carousel-item>
</v-carousel> -->
  <v-container class="bg-surface-variant">
    <v-row no-gutters>
      <v-col cols="12" md="5">
        cot 1
      </v-col>
      <v-col md='7'>
       cot 2
      </v-col>
      <v-col cols='12'>
       cot 3
      </v-col>
      <v-col>
       cot 4
      </v-col>
      <v-col>
       cot 5
      </v-col>
      <v-col>
       cot 6
      </v-col>

      <v-col>
       cot 7
      </v-col>
      <v-col>
       cot 8
      </v-col>
      <v-col>
       cot 9
      </v-col>
      <v-col>
       cot 10
      </v-col>
      <v-col>
       cot 11
      </v-col>
      <v-col>
       cot 12
      </v-col>

    </v-row>

    <!-- <v-row no-gutters>
      <v-col>
       cot 3
      </v-col>
      <v-col>
       cot 4
      </v-col>
      <v-col>
       cot 5
      </v-col>
    </v-row>

    <v-row no-gutters>
      <v-col cols="2">
        cot 6
      </v-col>
      <v-col>
      vot 7
      </v-col>
    </v-row> -->
  </v-container>
  <v-container>
    <v-row>
      <v-col cols="12" md="7+" offsert="3">1</v-col>
      <v-col md="2">2</v-col>
      <v-col>3</v-col>
    </v-row>
  </v-container>
  <p>Bai 1</p>
  <ex-1></ex-1>
  <p>Bai 2</p>
  <ex-2></ex-2>
  <p>Bai 3</p>
  <ex-3></ex-3>
  <p>Bai 4</p>
  <ex-4></ex-4>
  <p>Bài 5</p>
  <ex-5></ex-5>
  <p>Bài 6</p>
  <ex-6></ex-6>
  <p>Bài 7</p>
  <ex-7></ex-7>
  <p>Bài 8</p>
  <ex-8></ex-8>
  <p>Bài 9</p>
  <ex-9></ex-9>
  <p>Bài 10</p>
  <ex-10></ex-10>
</div>
</template>

<style scoped>
</style>