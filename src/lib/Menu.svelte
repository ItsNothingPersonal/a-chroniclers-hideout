<script lang="ts">
	let clazz = '';
	export { clazz as class };
</script>

<nav class={`bg-secondary rounded-lg p-4 text-white shadow-lg ${clazz}`}>
	<ul>
		<li class="mb-2"><a href="/" class="hover:bg-primary block rounded p-2">Home</a></li>
		<li class="mb-2"><a href="/about" class="hover:bg-primary block rounded p-2">About</a></li>
		<li class="mb-2"><a href="/contact" class="hover:bg-primary block rounded p-2">Contact</a></li>
		<li class="mb-2">
			<a href="/services" class="hover:bg-primary block rounded p-2">Services</a>
		</li>
	</ul>
</nav>
