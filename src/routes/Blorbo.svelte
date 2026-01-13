<script lang="ts">
	import { PLUSHIES } from '$lib';
	import { onMount } from 'svelte';

	let time: number = $state(0.0);
	let plushieIndex: number = $state(0);
	let timeSinceJump: number = $state(-10000.0);

	function update(currentTime: number) {
		time = currentTime / 500.0;
		requestAnimationFrame(update);
	}

	function jump() {
		timeSinceJump = time;
	}

	onMount(() => {
		plushieIndex = Math.floor(Math.random() * PLUSHIES.length);
		requestAnimationFrame(update);
	});

	export function updateBlorbo(index: number) {
		plushieIndex = index;
	}
</script>

<button
	class="absolute left-36 cursor-pointer"
	style={`top: ${36 + 5 * Math.sin(time) - Math.max(0, 200 * (time - timeSinceJump) * (1 - (time - timeSinceJump)))}px`}
	onclick={jump}
>
	<img src={`plushies/${PLUSHIES[plushieIndex]}`} alt="plushie" class="h-28" />
</button>
