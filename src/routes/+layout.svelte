<script>
    import { SvelteUIProvider, Space, SimpleGrid, Group, Button } from '@svelteuidev/core';
    import { onMount } from 'svelte';
    import { typewriter } from '@svelteuidev/motion';
    import Page from './+page.svelte';

    let type = false;
    onMount(() => {
        type = true;
	});
    function handleAnchorClick (event) {
		event.preventDefault()
		const link = event.currentTarget
		const anchorId = new URL(link.href).hash.replace('#', '')
		const anchor = document.getElementById(anchorId)
		window.scrollTo({
			top: anchor.offsetTop,
			behavior: 'smooth'
		})
	}

</script>

<style>
    h1 {
    margin:0;
    color: #111; font-family: 'Helvetica Neue', sans-serif; font-size: 40px; font-weight: bold; letter-spacing: -1px; line-height: 1; 
    }


</style>

<div style="position: fixed; display:flex; flex-direction:row;">
    
    {#if type}
    <h1 in:typewriter={{  }}>Bronx Science Senate</h1>
    {/if}
    <Group>
        <!-- <Button on:click={handleAnchorClick} variant="subtle" href="#about"> <b>About Us</b></Button> -->
    </Group>


     
</div>

<SvelteUIProvider ssr>
    <slot/>
</SvelteUIProvider>