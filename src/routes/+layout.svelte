<script>
    import{fly}from'svelte/transition';
    import{page}from'$app/stores';
    import Header from '$lib/components/Header.svelte';

    const{children} = $props();

    const startTransition = () => {
        document.body.classList.remove('page-transitioning')
    }
    const endTransition = () => {
        document.body.classList.remove('page-transitioning')
    }
</script>

<Header />

{#key $page.url}
<main
in:fly={{ x: -200, duration: 300, delay: 300 }}
		out:fly={{ x: 200, duration: 300 }}
		onintrostart={startTransition}
		onintroend={endTransition}
		onoutrostart={startTransition}
		onoutroend={endTransition}>
{@render children()}
    
</main>
{/key}

<style>

	/* :global ve svelte pro tyto globální html tagy, které nejsou v kodu tady v documentu musíme volat pomocí svelte funkce :global(nazev_elementu) */
	:global(body) {
		width: 100%; /* Nastaví šířku těla stránky na 100% dostupné šířky okna. */
		min-height: 100vh; /* Zaručuje, že tělo stránky bude mít minimální výšku rovnající se 100 % výšky okna (viewportu). */
		margin: 0; /* Odstraní veškeré výchozí odsazení kolem těla stránky. */
		padding: 0; /* Odstraní veškeré výchozí vnitřní odsazení těla stránky. */
		overflow: visible; /* Povolení viditelného přetečení, pokud obsah překročí výšku těla. */
		font-family: Arial, sans-serif; /* Nastaví výchozí font stránky na Arial, pokud není k dispozici, použije se jakýkoliv dostupný bezpatkový (sans-serif) font. */
	}

	main {
		min-height: 100vh; /* Zaručuje, že hlavní obsah zabere minimálně 100 % výšky okna. */
		width: 100%; /* Nastaví šířku hlavního obsahu na 100 % rodičovského kontejneru (těla stránky). */
		max-width: 1200px; /* Omezí maximální šířku hlavního obsahu na 1200 pixelů, takže se nebude rozšiřovat přes tuto hodnotu. */
		margin: auto; /* Vycentruje hlavní obsah horizontálně na stránce. */
		box-sizing: border-box; /* Zajistí, že při změně velikosti se do šířky a výšky prvku započítává také padding a ohraničení. */
	}


</style>
