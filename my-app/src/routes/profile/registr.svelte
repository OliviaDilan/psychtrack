<script>
    let showModal = false;
    import Modal from './modal.svelte'
</script>

<button class="modal-open bg-transparent border border-gray-500 hover:border-indigo-500 text-gray-500 hover:text-indigo-500 font-bold py-2 px-4 rounded-full" on:click="{() => showModal = true}">
	показать модальное окно
</button>

{#if showModal}
	<Modal on:close="{() => showModal = false}"></Modal>
{/if}