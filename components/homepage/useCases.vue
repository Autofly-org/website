<template>
  <div class="use-cases">
    <h2>Use Cases</h2>

    <imgElememt
      msg='We are using machine learning to analyze forsest and fields'
      title='Agriculture &amp; Forest analysis'
      img="/images/agriculture.jpg"
    />

    <imgElememt
      msg='Transporting Medical supplys or searching for drowning people'
      title='Rescue &amp; Transport'
      img="/images/rescue.jpg"
      right
    />
  </div>
</template>

<script lang="ts">
import { Vue, Component } from 'nuxt-property-decorator'
import imgElememt from '@/components/imgElememt.vue'

@Component({
  components: {
    imgElememt
  }
})
export default class useCases extends Vue {

}
</script>

<style lang="scss" scoped>
.use-cases {
  display: grid;
  gap: 20px;
  margin-top: 40px;
}
</style>
