<template>
  <div class="h-full flex items-center justify-center">
    <name-picker :names="['Bill', 'Bob', 'Alice']" />
  </div>
</template>

<script>
import NamePicker from './components/NamePicker'

export default {
  name: 'app',
  components: {
    NamePicker
  }
}
</script>

<style>
@tailwind preflight;
@tailwind components;
@tailwind utilities;
</style>
