<template>
  <demo-component />
</template>

<script lang="ts">
import { Component, Vue, Prop, PropSync, Ref } from "nuxt-property-decorator";
import DemoComponent from "../components/DemoComponent.vue";

@Component({
  components: {
    DemoComponent,
  },
})
export default class SecondScreenMediaOverlay extends Vue {}
</script>
