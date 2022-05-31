<template>
  <q-item clickable tag="a" target="_blank" v-ripple>
    <q-item-section v-if="icon" avatar>
      <q-icon :name="props.icon" />
    </q-item-section>

    <q-item-section>
      <q-item-label>{{ title }}</q-item-label>
      <q-item-label caption>{{ caption }}</q-item-label>
    </q-item-section>
  </q-item>
</template>

<script setup lang="ts">
const props = defineProps({
  title: String,
  caption: String,
  link: String,
  icon: String,
});
</script>
