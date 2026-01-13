<script lang="ts">
	import PlushRow from './PlushRow.svelte';
</script>

<div class="mb-8 w-full">
	<div class="relative mr-8 ml-8 h-128 rounded-b-2xl bg-[#F8F32B] inset-shadow-lg">
		<div class="m-auto flex h-full max-w-250 flex-row align-middle">
			<div class="flex flex-col justify-center p-8">
				<h1 class="text-left text-8xl">Shrine</h1>
				<h2 class="text-2xl">
					Make and code a project about your favorite fictional character, get a grant to buy merch
					of your character!
				</h2>
				<a
					class="mt-8 w-48 rounded-lg bg-[#2B2D42] p-4 text-center text-lg font-bold text-white underline"
					href="https://goog.fillout.com/shrine-ysws-rsvp">RSVP Here!</a
				>
			</div>
		</div>
		<img
			src="https://assets.hackclub.com/flag-orpheus-top.svg"
			class="absolute top-0 left-8"
			alt="hack club flag"
		/>
	</div>
</div>

<div class="h-32">
	<PlushRow />
	<!-- row of merch that scrolls by -->
</div>

<div class="w-full bg-[#2B2D42] p-8 text-white inset-shadow-lg/50">
	<div class="m-auto max-w-250">
		<h1 class="mb-4 text-4xl font-bold">What is Shrine?</h1>
		<p class="mb-8 text-lg">
			Shrine is a YSWS where you build a project (Must be tracked with Hackatime) about your
			favorite fictional character! It could be anything! Like, a website about your character, a
			Visual Novel with RenPy, anything related to that character! After you submit and we check
			your project, you'll receive a grant to go buy merch of your favorite character!
		</p>
		<h1 class="mb-4 text-4xl font-bold">How do I join?</h1>
		<p class="mb-8 text-lg">
			Join us at <a
				class="text-[#F8F32B] underline"
				href="https://hackclub.enterprise.slack.com/archives/C09A37XECJV"
			>
				#shrine
			</a>
			and make sure you RSVP on the form above!
		</p>
		<h1 class="mb-4 text-4xl font-bold">When will this launch?</h1>
		<p class="mb-8 text-lg">
			We dont have an ETA right now since this YSWS draft is freshly new and we haven't found a
			sponsor yet!
		</p>
		<h1 class="mb-4 text-4xl font-bold">What kind of merch can I buy?</h1>
		<p class="mb-8 text-lg">
			It could be a figurine, hoodies, shirts, stationary, stickers, anything as long it's related
			to your character!
		</p>
		<h1 class="mb-4 text-4xl font-bold">How many hours do I have to work?</h1>
		<p class="mb-8 text-lg">
			We haven't set how many hours. It might be 5 or 6 hours. Although, this might change, please
			take it with a grain of salt!
		</p>
		<h1 class="mb-4 text-4xl font-bold">Any policy about AI usage?</h1>
		<p class="mb-8 text-lg">
			Please do not vibe-code your project! You can use AI to get help on your project but please
			dont vibe code it!
		</p>
		<h1 class="mb-4 text-4xl font-bold">Is there anything I can contribute to this YSWS?</h1>
		<p class="mb-8 text-lg">
			Yes! You can spread the word about this. If you want to co-org this YSWS, free feel to <a
				class="text-[#F8F32B] underline"
				href="https://app.slack.com/client/E09V59WQY1E/D0A7TQRKCBH"
			>
				DM me on the Slack
			</a>
			or
			<a class="text-[#F8F32B] underline" href="mailto:me@ifeellikeharukananase.tech">email me</a>!
		</p>
	</div>
</div>

<div class="mt-8 w-full">
	<div
		class="relative mr-8 ml-8 flex flex-row justify-evenly rounded-t-2xl bg-[#8D99AE] p-8 text-black inset-shadow-lg"
	>
		<h1 class="text-3xl font-bold">Links</h1>
		<a href="https://hackclub.com/" class="underline">Hack Club</a>
		<a href="https://auth.hackclub.com/slack" class="underline">Hack Club Slack</a>
		<a href="https://hackclub.enterprise.slack.com/archives/C09A37XECJV" class="underline">
			#shrine Channel
		</a>
	</div>
</div>
