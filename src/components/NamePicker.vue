<template>
  <div class="text-center">
    <p class="text-semibold text-xl uppercase tracking-wide text-grey-darker mb-3">
      Whose <del>line</del> lunch is it anyway?
    </p>
    
    <p class="text-bold text-6xl">
      {{ name }}’s
    </p>
  </div>
</template>

<script>
import _ from 'lodash'

export default {
  props: {
    names: {
      type: Array,
      required: true
    }
  },

  computed: {
    name: function () {
      let names = this.names

      return _.shuffle(names)[0]
    }
  }
}
</script>
