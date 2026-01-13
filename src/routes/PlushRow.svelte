<script lang="ts">
	const PLUSHIES = [
		'acrid.png',
		'astrobot.png',
		'banjo.png',
		'claire.png',
		'ena.png',
		'gup.png',
		'kita.png',
		'knight.png',
		'madotsuki.png',
		'niko.png',
		'peppino.png',
		'quaber.png',
		'reibek.png',
		'sans.png',
		'shovelknight.png',
		'skelly.png',
		'slime.png',
		'spamtong.png'
	];
	let activePlushies: string[] = $state([]);
</script>

<div class="flex flex-row">
	{#each activePlushies as plushie}
		<img src={`plushies/${plushie}`} />
	{/each}
</div>
