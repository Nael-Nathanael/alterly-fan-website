<script>
	import { fade } from 'svelte/transition';

	let showed = false;

	export let charname;

</script>


<main class='shadow' on:mouseup={() => {showed = !showed}}>
	{#if showed}
		<div class='gif' id='0' in:fade>
			<img alt='' src='/img/avatar/{charname}/0.gif' width='300'>
		</div>
	{:else}
		<img alt='' class='static' height='300'
				 src='/img/avatar/{charname}/0.jpg' width='300' in:fade>
	{/if}
</main>

<style>
    main.shadow {
        position: relative;
        cursor: pointer;
        width: 300px;
        z-index: 1000;
				height: 100%;
    }

    .gif {
        position: absolute;
        left: 50%;
        top: 50%;
        transform: translate(-50%, -50%);
        z-index: 1;
    }
</style>