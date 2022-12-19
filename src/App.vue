<template>
  <div id="app">
    <dashboard :uppy="uppy" :plugins="['Webcam']" :props="{ theme: 'dark' }" />
  </div>
</template>

<script>
import { Dashboard } from "@uppy/vue";

import "@uppy/core/dist/style.css";
import "@uppy/dashboard/dist/style.css";
import "@uppy/webcam/dist/style.css";
import "@uppy/drag-drop/dist/style.css";
import "@uppy/progress-bar/dist/style.css";

import Uppy from "@uppy/core";
import Webcam from "@uppy/webcam";
import DragDrop from "@uppy/drag-drop";
import ProgressBar from "@uppy/progress-bar";

export default {
  name: "App",
  components: {
    Dashboard,
  },
  computed: {
    uppy: () => new Uppy().use(Webcam),
  },
  beforeUnmount() {
    this.uppy.close({ reason: "unmount" });
  },
};
</script>
