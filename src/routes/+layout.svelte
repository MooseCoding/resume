<script lang="ts">
	import '../app.css';
	import NavBar from '$lib/main/NavBar.svelte'; 
	let { children } = $props();
</script> 

<NavBar />
{@render children()}
