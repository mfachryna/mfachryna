<script lang="ts">
	const skeletonLogos = Array(8).fill(null);
</script>

<section class="bg-background">
	<div class="relative overflow-hidden px-0 py-4">
		<div class="flex justify-center whitespace-nowrap">
			{#each skeletonLogos as _, i}
				<div
					class="bg-foreground/10 mx-5 h-10 w-10 animate-pulse cursor-pointer rounded-full md:mx-10"
					style="animation-delay: {i * 0.1}s"
				>
					<div class="flex h-full w-full items-center justify-center">
						<svg class="text-foreground/20 h-5 w-5 animate-spin" fill="none" viewBox="0 0 24 24">
							<circle
								class="opacity-25"
								cx="12"
								cy="12"
								r="10"
								stroke="currentColor"
								stroke-width="4"
							></circle>
							<path
								class="opacity-75"
								fill="currentColor"
								d="m4 12a8 8 0 018-8V0C5.373 0 0 5.373 0 12h4zm2 5.291A7.962 7.962 0 014 12H0c0 3.042 1.135 5.824 3 7.938l3-2.647z"
							></path>
						</svg>
					</div>
				</div>
			{/each}
		</div>
	</div>
</section>
