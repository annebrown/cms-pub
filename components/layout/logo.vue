<template>
	<div
		id="header__logo"
		class="company-logo"
	>
        <NuxtLink to="https://annebrown.ca" target="_blank">
			<img
				src="/images/logos/book.svg"
				alt="logo"
				width="200"
				height="200"
			/>
		</NuxtLink>	
        <NuxtLink to="https://misscommunication.ca" target="_blank">
			<img
				src="/images/logos/logo.svg"
				alt="logo"
				width="200"
				height="200"
			/>
	    </NuxtLink>
	</div>
</template>

<style lang="scss" scoped>
	.company-logo {
		position: relative;
		height: 2em; 
		margin: 1em;
		padding-bottom: 3em;
		padding-right: 1em;
		width: max-content;
		img {
			position: relative;
			height: 3em;
			width: auto;
		}

	}
</style>
