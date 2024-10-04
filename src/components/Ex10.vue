<template>
  <div>
    <v-table density="compact">
      <thead>
        <tr>
          <th class="text-left">Name</th>
          <th class="text-left">Project Name</th>
          <th>Post</th>
          <th>Status</th>
          <th>Budget</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="item in projects" :key="item.name">
          <td>{{ item.name }}</td>
          <td>{{ item.project }}</td>
          <td>{{ item.post }}</td>
          <td>
            <v-chip
              color="green"
              size="small"
              variant="text"
            >
              {{ item.status }}
            </v-chip>
          </td>
          <td>{{ item.budget }}</td>
        </tr>
      </tbody>
      <div style="display: flex; gap: 20px; justify-content: flex-end; align-items: center;">
        <div>
          <div>Item per page</div>
          <v-select density="compact" style="width: 80px" :items="['5', '10']" label="5" />
        </div>
        <div>1-5 of 10</div>
        <v-pagination :length="4"></v-pagination>
      </div>
    </v-table>
  </div>
</template>

<script setup>
import { ref } from 'vue'

// Dữ liệu mới
const projects = ref([
  {
    name: 'Sunil Joshi',
    project: 'Elite Admin',
    post: 'Web Designer',
    status: 'Active',
    budget: '$3.9k',
  },
  {
    name: 'Andrew McDownland',
    project: 'Real Homes WP Theme',
    post: 'Project Manager',
    status: 'Pending',
    budget: '$24.5k',
  },
  {
    name: 'Christopher Jamil',
    project: 'MedicalPro WP Theme',
    post: 'Project Manager',
    status: 'Completed',
    budget: '$12.8k',
  },
  {
    name: 'Nirav Joshi',
    project: 'Hosting Press HTML',
    post: 'Frontend Engineer',
    status: 'Active',
    budget: '$2.4k',
  },
  {
    name: 'Micheal Doe',
    project: 'Helping Hands WP Theme',
    post: 'Content Writer',
    status: 'Cancel',
    budget: '$9.3k',
  }
])
</script>

<style scoped>
</style>
