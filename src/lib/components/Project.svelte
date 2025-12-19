<script lang="ts">
	export let src: string;
	export let title: string;
	export let alt: string = "";
	
	// Optional: loading state or intersection observer for fade-in
</script>

<div class="relative w-full group">
	<img {src} {alt} class="w-full h-auto block object-cover" loading="lazy" />
	
	<div class="absolute bottom-6 left-6 md:bottom-8 md:left-8 text-[10px] md:text-xs tracking-[0.15em] uppercase font-normal text-gray-900">
		{title}
	</div>
</div>
