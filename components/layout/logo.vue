<template>
	<div
		id="header__logo"
		class="company-logo"
	>
    <NuxtLink to="https://annebrown.ca" target="_blank">
			<img
				src="/images/logos/book.svg"
				alt="logo"
				width="300"
				height="300"
			/>
		</NuxtLink>	
    <NuxtLink to="https://misscommunication.ca" target="_blank">
			<img
				src="/images/logos/logo.svg"
				alt="logo"
				width="300"
				height="300"
			/>
		</NuxtLink>
       
		<span>cms.misscommunication.ca</span>
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
		border-right: 1px solid $light-grey;
		img {
			position: relative;
			height: 2em;
			width: auto;
		}
		span {
			position: absolute;
			font-size: 0.8em;
			right: 1em;
			bottom: 0;
            width: max-content;
			transform: translateX(5%);
			font-style: italic;
			font-family: $font-art;
			color: $dark-grey;
		}
	}
</style>
