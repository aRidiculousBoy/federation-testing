<script setup lang="ts">
import { useRouter } from "vue-router";
import { defineAsyncComponent } from "vue";

defineOptions({
  name: "403"
});

const router = useRouter();
const remoteSuccess = defineAsyncComponent(() => import("naive-ui-admin/Success"));
</script>

<template>
  <div class="flex justify-center items-center h-[640px]">
    <remoteSuccess />
  </div>
</template>
