<template>
  <q-item clickable>
    <q-item-section>{{ id }} - {{ title }}</q-item-section>
  </q-item>
</template>

<script setup>
defineProps({
  id: {
    type: String,
  },
  title: {
    type: String,
  },
});
</script>

<style lang="scss" scoped></style>
