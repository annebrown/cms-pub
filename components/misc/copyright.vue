<template>
	<div id="copyright">
		/Copyright &copy; Anne Brown <span>| {{ currentYear }}</span>
	</div>
</template>

<script>
export default {
    data() {
        return {
            currentYear: "",
        };
    },
    mounted() {
        if (process.client) {
            let getYear = new Date();
            this.currentYear = getYear.getUTCFullYear();
        }
    },
};
</script>

<style lang="scss" scoped>
#copyright {
    font-family: $font-accent;
    font-size: $font-size7;
    color: $white;
}
</style>