<script>
import Header from "./components/Header.vue";
import Topnav from "./components/Topnav.vue";
import RealEstate from "./components/RealEstate.vue";
import Brands from "./components/Brands.vue";

export default {
	components: { Header, Topnav, RealEstate, Brands },
}
</script>

<template>
	<div>
		<Header />
		<Topnav />
		<RealEstate />
		<Brands />
	</div>
</template>

<style scoped></style>
