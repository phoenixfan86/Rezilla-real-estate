<script>
export default {}
</script>

<template>
	<header>
		<div class="contact__item">
			<div class="img">
				<img src="/src/assets/img/ico/loc_ico.png" alt="" />
			</div>
			<a href="#" class="_white">Rezilla, 18 Grattan St, Brooklyn</a>
		</div>
		<div class="header__contact">
			<div class="contact__item">
				<div class="img">
					<img src="/src/assets/img/ico/phone_ico.png" alt="" />
				</div>
				<span class="_white">+1 206-214-2298</span>
			</div>
			<div class="contact__item">
				<div class="img">
					<img src="/src/assets/img/ico/mail_ico.png" alt="" />
				</div>
				<a href="mailto:support@rezilla.com" class="_white"
					>support@rezilla.com</a
				>
			</div>
		</div>
	</header>
</template>

<style scoped>
header {
	width: 100%;
	max-width: 1440px;
	height: 40px;
	display: flex;
	align-items: center;
	justify-content: space-between;
	background-color: var(--primary-colour);
}

.header__contact {
	display: flex;
	align-items: center;
	gap: 30px;
}

.contact__item {
	height: 100%;
	display: flex;
	align-items: center;
	justify-content: center;
	gap: 10px;
}
</style>
