<template>
	<div class="home flx-center">123</div>
</template>

<script setup lang="ts" name="home">
import { onMounted } from "vue";
import { getOutTime } from "@/api/modules/login";
onMounted(async () => {
	const res = await getOutTime();
	console.log(res, "εεΊη»ζ");
});
</script>

<style scoped lang="scss">
@import "./index.scss";
</style>
