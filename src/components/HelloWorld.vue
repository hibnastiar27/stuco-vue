<script setup lang="ts">
import { ref } from "vue";

defineProps<{ msg: string }>();

const count = ref(0);
</script>

<template>
  <h1>{{ msg }}</h1>

  <div class="">
    <button
      class="px-4 py-2 bg-amber-500 rounded-full"
      type="button"
      @click="count++"
    >
      count is {{ count }}
    </button>
  </div>
</template>
