<template>
	<div class="home flx-center">123</div>
</template>

<script setup lang="ts" name="home">
import { onMounted } from "vue";
import { getOutTime } from "@/api/modules/login";
onMounted(async () => {
	const res = await getOutTime();
	console.log(res, "响应结果");
});
</script>

<style scoped lang="scss">
@import "./index.scss";
</style>
