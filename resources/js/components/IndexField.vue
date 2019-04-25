<template>
  <span class="fontawesome-index-icon"><i :class="field.value"></i></span>
</template>

<script>
import { library } from "@fortawesome/fontawesome-svg-core";
import { fas } from "@fortawesome/pro-solid-svg-icons";
import { fal } from "@fortawesome/pro-light-svg-icons";
import { far } from "@fortawesome/pro-regular-svg-icons";
import { fab } from "@fortawesome/free-brands-svg-icons";

// Add all icons to the library so you can use it in your page
library.add(fal, fas, far, fab);

import "@fortawesome/fontawesome-pro/js/fontawesome.js";

export default {
  props: ["resourceName", "field"]
};
</script>

<style>
.fontawesome-index-icon {
  font-size: 1.5em;
}

.fontawesome-index-icon svg {
  width: 1em !important;
  height: 1.5em !important;
}
</style>
