<template>
	<div class="row profile">
		<div class="col-sm-6 col-primary">
			<div class="profile__image" style="background-image:url(/images/me.jpg)"></div>
		</div>
		<div class="col-sm-6 profile__content" v-mousemove>
			<div class="title">Mark<div class="text-primary point-to-left">Mngoma</div></div>
			<h1 class="text-default">Back-end developer</h1>
			<p class="text-muted">I'm Ntsika Mark Mngoma and I love to develop<br/>efficient software.<br/>21 year old developer from <router-link to="/contact" class="link--styled">Durban, KZN</router-link></p>
		</div>
	</div>
</template>
<script>

export default {

}
</script>
