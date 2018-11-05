<template>
  <b-container class="bv-example-row">
    <b-row>
      <b-col>
        <TabsPanel />
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
import TabsPanel from '@/components/TabsPanel.vue'

export default {
  name: 'HomePage',
  components: {
    TabsPanel
  }
}
</script>

<style scoped>

</style>
