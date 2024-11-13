<template>
	<footer>
		
	</footer>
</template>

<style lang="scss" scoped>
	footer {
		position: relative;
		height: max-content;
		display: grid;
		grid-template-columns: repeat(3, 1fr);
		gap: $spacing5;
		margin-inline: $spacing4;
		opacity: 0;
		animation: 5s ease 3s forwards appear;
		@keyframes appear {
			0% {
				opacity: 0;
			}
			100% {
				opacity: 1;
			}
		}
		@include media(xsm) {
			display: block;
			height: auto;
			margin-top: $spacing2;
			margin-inline: 0;
		}
	}

	#__by-sailsnake {
		grid-column: 2;
		padding: $spacing1;
		justify-self: center;
		border-top: 0.1em solid $light-grey;
		p {
			margin: 0;
			display: inline-block;
			font-family: $font-art;
		}
		a {
			margin-left: $spacing1;
			display: inline-block;
			font-style: normal;
			text-transform: uppercase;
			font-family: $font-accent;
			img {
				height: $font-size5;
				width: auto;
				aspect-ratio: 941 / 408;
			}
		}
	}
</style>
