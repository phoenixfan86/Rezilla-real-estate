<script>
import Header from "./components/Header.vue";
import Topnav from "./components/Topnav.vue";
import RealEstate from "./components/RealEstate.vue";
import Brands from "./components/Brands.vue";
import Whoarewe from "./components/Whoarewe.vue";


export default {
	components: { Header, Topnav, RealEstate, Brands, Whoarewe },
}
</script>

<template>
	<div>
		<Header />
		<Topnav />
		<RealEstate />
		<Brands />
		<Whoarewe />
	</div>
</template>

<style scoped></style>
