<template>
  <div>
    <!-- eslint-disable-next-line vue/no-v-html -->
    <div v-html="test"></div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

// @ts-ignore
import test from '~/assets/test.md'

export default Vue.extend({
  name: 'IndexPage',
  computed: {
    test() {
      return test
    },
  },
})
</script>
