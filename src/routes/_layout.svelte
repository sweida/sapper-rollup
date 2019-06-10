<script>
	import '../style/main.css'
	import Nav from '../components/Nav.svelte';
	import Foot from '../components/Foot.svelte';
	import Head from '../components/Head.svelte';

	export let segment;
</script>

<style>
	/* main {
		position: relative;
		max-width: 56em;
		background-color: white;
		margin: 40px auto;
		box-sizing: border-box;
	} */
</style>

<Head />

<main>
	<slot></slot>
</main>

<Nav {segment}/>
<!-- <Foot></Foot> -->