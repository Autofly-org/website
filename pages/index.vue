<template>
  <div class="container">
    <main>
      <home class="section home" />
      <mission class="section" />
      <features class="section" />
      <useCases class="section" />
      <design class="section" />
      <safety class="section" />
    </main>
    <footer>

    </footer>
  </div>
</template>

<script lang="ts">
import { Vue, Component } from 'nuxt-property-decorator'
import { Meta } from '@/decorators/meta'

import home from '@/components/home.vue'
import mission from '@/components/mission.vue'
import features from '@/components/features.vue'
import useCases from '@/components/useCases.vue'
import design from '@/components/design.vue'
import safety from '@/components/safety.vue'

@Component({
  components: {
    home,
    mission,
    features,
    useCases,
    design,
    safety
  }
})
export default class Home extends Vue {
  @Meta
  head() {
    return {
      title: "Autofly",
      meta: [
        {
          hid: "description",
          name: "description",
          content: "We are in the Prozess of creating a autonomous drone that can fullfill missions ranging from agricultural Tasks, like crop yield analysis, Forest Health analysis using machine learning to transportation tasks like transporting medicine to unaccessible areas."
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
main {
  padding: 50px;
  text-align: center;

  .section {
    margin: 33px 0;
  }

  .home {
    margin: 0 0 33px 0;
  }
}
</style>
