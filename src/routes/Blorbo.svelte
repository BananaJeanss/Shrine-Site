<script lang="ts">
	import { PLUSHIES } from '$lib';
	import { onMount } from 'svelte';

	let time: number = $state(0.0);
	let plushieIndex: number = $state(0);

	function update(currentTime: number) {
		time = currentTime / 500.0;
		requestAnimationFrame(update);
	}

	onMount(() => {
		plushieIndex = Math.floor(Math.random() * PLUSHIES.length);
		requestAnimationFrame(update);
	});

	export function updateBlorbo(index: number) {
		plushieIndex = index;
	}
</script>

<img
	class="absolute left-36 h-28"
	src={`plushies/${PLUSHIES[plushieIndex]}`}
	style={`top: ${36 + 5 * Math.sin(time)}px`}
	alt="plushie"
/>
