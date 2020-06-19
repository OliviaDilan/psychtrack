<script>
	import Nav from '../components/Nav.svelte';
	import Tailwind from '../components/Tailwind.svelte';
	import '../style/layout.css';

	export let segment;
</script>



<Tailwind />
<Nav {segment}/>

<div class="w-full max-w-screen-xl mx-auto px-6">
<div class="max-w-screen-xl -mx-6">
<main>
	<slot></slot>
</main>
</div>
</div>