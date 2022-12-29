<script>
	import Component2 from "./Component2.svelte";
	let text = `The FitnessGram Pacer Test is a multistage aerobic capacity test that progressively gets more difficult as it continues. 
	The 20 meter pacer test will begin in 30 seconds. Line up at the start. 
	The running speed starts slowly, but gets faster each minute after you hear this signal. [beep]
	A single lap should be completed each time you hear this sound. [ding]
	Remember to run in a straight line, and run as long as possible.
	The second time you fail to complete a lap before the sound, your test is over. The test will begin on the word start. On your mark, get ready, start.`.toUpperCase();
	let wide = "";
	for (let i = 0; i < text.length; i++) {
		wide = wide + text[i] + " ";
	}
</script>
<div class="card-content">
	<div class="card">
		<h1>
		 The fitnessgram pacer test	
		</h1>
		<p class="meme">
			{wide}
		</p>
		<hr>
		<a href="https://www.youtube.com /watch?v=FK_ZQeYN7uw">
			START
		</a>
	</div>

	<div class="card-2">
		<Component2 />
	</div>
</div>

<style>
	.meme {
		color: steelblue;
		font-size: 50px;
	}
	:global(*) {
		font-family: 'Helvetica';
		color: steelblue;
	}
	.card {
		border: solid 1px black;
		border-radius: 3px;
		box-shadow: 5px 1px 1px gray;
	}
	.card-2 {
		border: solid 1px gray;
		border-radius: 3px;
		box-shadow: 5px 1px 1px black;
	}
	
	.card-content > * {
		margin-top: 5px;
	}
</style>
