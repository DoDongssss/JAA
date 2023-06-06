<script lang="ts">
import { defineComponent } from 'vue'
import { RouterLink, RouterView } from 'vue-router'
import index from '../src/views/index.vue'
import about from '../src/views/about.vue'
import skills from '../src/views/skills.vue'
import experience from '../src/views/experience.vue'
import contact from '../src/views/contact.vue'

export default defineComponent({
    components: {
      index,
      about,
      skills,
      experience,
      contact
    },
    setup () {
        

        return {}
    }
})
</script>

<template>
  <index/>
  <about/>
  <skills/>
  <experience/>
  <contact/>
</template>

<style scoped>

</style>
