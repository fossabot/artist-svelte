<script lang="ts">
	import { browser } from '$app/env';
	import { rtlHook } from '$lib/utilities/hook';
	import Switch from '$lib/components/switch';
	let darkMode = false;
	const { isEnabled, toggle } = rtlHook;
	$: if (browser) document.documentElement.classList.toggle('dark', darkMode);
</script>

<div style="display: flex;justify-content: center;align-items: center;direction: rtl;">
	<Switch color="default" bind:checked={darkMode}>
		<svelte:fragment slot="on">dark</svelte:fragment>
		<svelte:fragment slot="off">light</svelte:fragment>
	</Switch>

	<Switch color="secondary" on:change={toggle} checked={$isEnabled}>
		<svelte:fragment slot="on">Right-To-Left</svelte:fragment>
		<svelte:fragment slot="off">Left-To-Right</svelte:fragment>
	</Switch>
</div>
<nav>
	<a href="/">Home</a>
	<a href="/button">button</a>
	<a href="/alert">alert</a>
	<a href="/card">card</a>
	<a href="/paper">paper</a>
	<a href="/checkbox">checkbox</a>
	<a href="/switch">switch</a>
	<a href="/avatar">avatar</a>
	<a href="/radio">radio</a>
	<a href="/input">input</a>
	<a href="/modal">modal</a>
	<a href="/accordion">accordion</a>
	<a href="/drawer">drawer</a>
	<a href="/navbar">navbar</a>
	<a href="/link">link</a>
	<a href="/dropdown">dropdown</a>
</nav>
<slot />

<style lang="scss" global>
	@import './../lib/scss/GlobalStyles';
	@import './../lib/scss/modules/normalize';
	@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@100;200;300;400;500;600&display=swap');

	html,
	body {
		margin: 0;
		padding: 0;
		font-family: 'Poppins', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue',
			Arial, 'Noto Sans', 'Liberation Sans', sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji',
			'Segoe UI Symbol', 'Noto Color Emoji', Vazir;
	}
	html {
		background-color: hsl(var(--bg-color));
		color: hsl(var(--fg-color));
		transition: color 0.3s, background-color 0.3s;
	}
	::-webkit-scrollbar {
		width: 5px;
		height: 5px;
		display: block;
		background: hsl(var(--bg-color));
	}
	::-webkit-scrollbar-thumb {
		background: hsl(var(--fg-color));
		border-radius: 5px;
	}
</style>
