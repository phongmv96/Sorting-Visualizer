<script setup lang="ts">
import { ICol } from "~/types/col";

defineProps<{
  col: ICol;
}>();
</script>

<template>
  <div class="col" :style="{ height: col?.height + 'px', backgroundColor: `${col.status}` }"></div>
</template>

<style scoped lang="scss">
.col {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 10px;
  background-color: rgba(245, 124, 0);
  margin-right: 3px;
}


</style>
