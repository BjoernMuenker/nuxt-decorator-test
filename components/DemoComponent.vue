<template>
  <div>
    <div>{{ headline }}</div>
  </div>
</template>

<script lang="ts">
import { Component, Vue, Prop, PropSync, Ref } from "nuxt-property-decorator";

@Component
export default class DemoComponent extends Vue {
  mounted() {
    // this.$props.headline = "Test";
  }

  @Prop({ default: "Headline" })
  headline!: string;

  /*
  @PropSync("headline", { default: "Headline" })
  headline!: string;
  */
}
</script>
