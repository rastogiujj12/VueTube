<template>
  <div class="description" v-if="render.descriptionBodyText">
    <yt-text-formatter :textRuns="render.descriptionBodyText.runs">
    </yt-text-formatter>
  </div>
</template>

<style scoped>
.description {
  white-space: pre-line;
}
</style>

<script>
import YtTextFormatter from "~/components/UtilRenderers/YtTextFormatter.vue";

export default {
  props: ["render"],

  components: {
    YtTextFormatter,
  },
};
</script>
