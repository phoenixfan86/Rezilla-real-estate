<script>
import Header from "./components/Header.vue";
import Topnav from "./components/Topnav.vue";
import RealEstate from "./components/RealEstate.vue";

export default {
	components: { Header, Topnav, RealEstate },
}
</script>

<template>
	<div>
		<Header />
		<Topnav />
		<RealEstate />
	</div>
</template>

<style scoped></style>
