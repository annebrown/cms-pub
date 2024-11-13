<template>
	<main id="main" class="home">
		<MiscParseMarkdown :markdownString="home.content" />
	</main>

</template>

<script setup>
useHead({
  script: [
    { src: "https://identity.netlify.com/v1/netlify-identity-widget.js" },
  ],
});

const { data: home } = reactive(await useAsyncData("home", () =>
	queryContent("/pages/home").findOne())
);

setSeoHead(home.SEOmetaData);

</script>

<style lang="scss" scoped>
main {
	display: grid;
	justify-items: center;
	align-items: center;
	:deep(div) {
		max-width: 50em;
	}
	// assets/scss/mixins
	@include fade-in;
}
</style>
