<script>
	import CharacterCard from '../components/CharacterCard.svelte';
</script>


<main>
	<CharacterCard charname='rora' />
	<CharacterCard charname='milly' />
	<CharacterCard charname='leifa' />
	<CharacterCard charname='rhea' />
</main>

<style>
    main {
        background: rgb(89, 0, 119);
        background: linear-gradient(90deg, rgba(89, 0, 119, 1) 0%, rgba(238, 2, 120, 1) 100%);
        width: 100vw;
        min-height: 100vh;
        display: flex;
        justify-content: space-around;
        align-items: center;
    }
</style>