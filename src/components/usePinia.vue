<template>
  <div></div>
</template>

<script lang="ts" setup>
import { useUserStore } from '@/store/user'
const useStore = useUserStore()
useStore.updateName('updatedName')
</script>
