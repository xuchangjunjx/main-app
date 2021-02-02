<template>
  <div class="sub-app-container">
    <Application
      id="my-sub-app1"
      class="test-class"
      :sandBox="{
        initialPath: '/sub-app1',
        disableFakeBody: true,
        disable: false
      }"
      manifest="http://localhost:9999/sub-app1/my-sub-app1.manifest.json"
    />
  </div>
</template>

<script>
// 引入@alicloud/console-os-vue-host-app依赖
import Application from "@alicloud/console-os-vue-host-app";

export default {
  name: "App",
  components: {
    Application
  }
};
</script>
