<template>
	<div id="content">
		<template>
			<h2>Material Design</h2>
			<a v-bind:href="link1" target="_blank">Material Design 소개</a>
			<a v-bind:href="link2" target="_blank">Material Design 살펴보기</a>
			<br>
			<h2>Material UI</h2>
			<a v-bind:href="link3" target="_blank">https://material.io</a>
			<a v-bind:href="link4" target="_blank">https://vuematerial.io/</a>
		</template>

	</div>
</template>


<script>
	export default {
		name: 'content',
		data: () => ({
			link1:'https://developers-kr.googleblog.com/2014/07/this-is-material-design.html',
			link2:'https://www.slideshare.net/watchncompass/3-material-design',
			link3:'https://material.io',
			link4:'https://vuematerial.io/',
		})
	}
</script>

<style>
a{display:block;padding:5px;color:#000 !important;}
a:hover{}
</style>
