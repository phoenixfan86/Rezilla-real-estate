<script>
import Header from "./components/Header.vue";
import Topnav from "./components/Topnav.vue";
import RealEstate from "./components/RealEstate.vue";
import Brands from "./components/Brands.vue";
import Whoarewe from "./components/Whoarewe.vue";
import OurNew from "./components/OurNew.vue";


export default {
	components: { Header, Topnav, RealEstate, Brands, Whoarewe, OurNew },
}
</script>

<template>
	<Header />
	<Topnav />
	<RealEstate />
	<Brands />
	<Whoarewe />
	<OurNew />
</template>

<style scoped></style>
