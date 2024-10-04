<template>
  <v-container>
    <v-tabs v-model="activeTab" background-color="blue" dark>
      <v-tab v-for="(tab, index) in tabs" :key="index">{{ tab.label }}</v-tab>
    </v-tabs>

    <v-tabs-items v-model="activeTab">
      <v-tab-item v-for="(tab, index) in tabs" :key="index">
        <v-container>{{ tab.content }}</v-container>
      </v-tab-item>
    </v-tabs-items>
  </v-container>
</template>

<script setup>
import { ref } from 'vue'

const activeTab = ref(0)

const tabs = [
  { label: 'Trang chủ', content: 'Nội dung trang chủ' },
  { label: 'Giới thiệu', content: 'Nội dung giới thiệu' },
  { label: 'Liên hệ', content: 'Nội dung liên hệ' }
]
</script>
<style scoped>
</style>
