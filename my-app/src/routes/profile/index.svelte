<script>
	let user = { loggedIn: false };

	function toggle() {
		user.loggedIn = !user.loggedIn;
    }
    
    import Auth from './auth.svelte'
    import Reg from './registr.svelte'
</script>

{#if user.loggedIn}
		<Auth />
{/if}

{#if !user.loggedIn}
<div class="w-full max-w-screen-xl mx-auto px-6">
<div class="max-w-screen-xl -mx-6">
  <Auth />
</div>
</div>

{/if}