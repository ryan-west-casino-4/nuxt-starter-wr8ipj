<template>
  <div v-if="errors.length">
    <div class="font-medium text-red-600">Whoops! Something went wrong.</div>

    <ul class="mt-3 list-disc list-inside text-sm text-red-600">
      <li v-for="error in errors" :key="error">{{ error }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  props: ['errors'],
};
</script>
