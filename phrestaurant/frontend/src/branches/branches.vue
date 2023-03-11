<template>
    <select v-model="selectedBranch" class="branch-select">
      <option v-for="branch in branches" :key="branch.id" @click="redirectToBranch">{{ branch.name }}</option>
    </select>
  </template>
<script>
export default {
  data() {
    return {
      branches: [
        { id: 1, name: 'Inasal'    },
        { id: 2, name: 'karenderia' },
      ],
      selectedBranch: 1
    };
  }
};

</script>
  
<style>
 .branch-select {
    font-size: 16px;
    background-color: #fff;
    border: none;
    padding: 6px;
 }   
</style>