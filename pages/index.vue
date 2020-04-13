<template>
  <div class="container">
    <main>
      <home class="section home" />
      <mission class="section" />
      <features class="section" />
      <useCases class="section" />
      <design class="section" />
      <safety class="section" />
      <about class="section" />
      <sponsor class="section" />
    </main>
    <footer>
      <nuxt-link to="/imprint">Imprint</nuxt-link>
      <p>© Autofly 2020</p>
    </footer>
  </div>
</template>

<script lang="ts">
import { Vue, Component } from 'nuxt-property-decorator'
import { Meta } from '@/decorators/meta'

import home from '@/components/homepage/home.vue'
import mission from '@/components/homepage/mission.vue'
import features from '@/components/homepage/features.vue'
import useCases from '@/components/homepage/useCases.vue'
import design from '@/components/homepage/design.vue'
import safety from '@/components/homepage/safety.vue'
import about from '@/components/homepage/about.vue'
import sponsor from '@/components/homepage/sponsor.vue'

@Component({
  components: {
    home,
    mission,
    features,
    useCases,
    design,
    safety,
    about,
    sponsor
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
@import '@/assets/colors';

main {
  padding: 50px;
}

footer {
  // position: fixed;
  bottom: 0;
  left: 0;
  padding: 10px 20px;
  width: 100vw;
  background: $footer;
  text-align: center;

  p {
    margin: 10px 0 0 0;
  }
}

</style>
