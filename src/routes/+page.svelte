<script lang="ts">
	// @ts-ignore
	import Countdown from 'svelte-countdown/src/index.js';
</script>

<div class="h-screen bg-[#191A24]">
	<div class="flex h-full w-full flex-col items-center justify-center gap-8 sm:gap-16">
		<span class="px-2 text-center text-2xl font-semibold tracking-widest text-white sm:text-3xl">
      Brand new life!
		</span>
		<Countdown
			from="2024-05-17 18:00:00"
			dateFormat="YYYY-MM-DD H:m:s"
			zone="Asia/Shanghai"
			let:remaining
		>
			<div class="flex justify-center gap-3 sm:gap-8">
				<div class="relative flex flex-col gap-5">
					<div
						class="flex h-16 w-16 items-center justify-between rounded-lg bg-[#343650] sm:h-32 sm:w-32 lg:h-40 lg:w-40"
					>
						<div
							class="relative !-left-[6px] h-2.5 w-2.5 rounded-full bg-[#191A24] sm:h-3 sm:w-3"
						></div>
						<span class="text-3xl font-semibold text-[#a5b4fc] sm:text-6xl lg:text-7xl">
							{remaining.days}
						</span>
						<div
							class="relative -right-[6px] h-2.5 w-2.5 rounded-full bg-[#191A24] sm:h-3 sm:w-3"
						></div>
					</div>
					<span class="text-center text-xs capitalize text-[#8486A9] sm:text-2xl">
						{remaining?.days == 1 ? 'Day' : 'Days'}
					</span>
				</div>
				<div class="relative flex flex-col gap-5">
					<div
						class="flex h-16 w-16 items-center justify-between rounded-lg bg-[#343650] sm:h-32 sm:w-32 lg:h-40 lg:w-40"
					>
						<div
							class="relative !-left-[6px] h-2.5 w-2.5 rounded-full bg-[#191A24] sm:h-3 sm:w-3"
						></div>
						<span class="text-3xl font-semibold text-[#a5b4fc] sm:text-6xl lg:text-7xl">
							{remaining?.hours}
						</span>
						<div
							class="relative -right-[6px] h-2.5 w-2.5 rounded-full bg-[#191A24] sm:h-3 sm:w-3"
						></div>
					</div>
					<span class="text-center text-xs font-medium text-[#8486A9] sm:text-2xl">
						{remaining?.hours == 1 ? 'Hour' : 'Hours'}
					</span>
				</div>
				<div class="relative flex flex-col gap-5">
					<div
						class="flex h-16 w-16 items-center justify-between rounded-lg bg-[#343650] sm:h-32 sm:w-32 lg:h-40 lg:w-40"
					>
						<div
							class="relative !-left-[6px] h-2.5 w-2.5 rounded-full bg-[#191A24] sm:h-3 sm:w-3"
						></div>
						<span class="text-3xl font-semibold text-[#a5b4fc] sm:text-6xl lg:text-7xl">
							{remaining?.minutes}
						</span>
						<div
							class="relative -right-[6px] h-2.5 w-2.5 rounded-full bg-[#191A24] sm:h-3 sm:w-3"
						></div>
					</div>
					<span class="text-center text-xs capitalize text-[#8486A9] sm:text-2xl">
						{remaining?.minutes == 1 ? 'Minute' : 'Minutes'}
					</span>
				</div>
				<div class="relative flex flex-col gap-5">
					<div
						class="flex h-16 w-16 items-center justify-between rounded-lg bg-[#343650] sm:h-32 sm:w-32 lg:h-40 lg:w-40"
					>
						<div
							class="relative !-left-[6px] h-2.5 w-2.5 rounded-full bg-[#191A24] sm:h-3 sm:w-3"
						></div>
						<span class="text-3xl font-semibold text-[#a5b4fc] sm:text-6xl lg:text-7xl">
							{remaining?.seconds}
						</span>
						<div
							class="relative -right-[6px] h-2.5 w-2.5 rounded-full bg-[#191A24] sm:h-3 sm:w-3"
						></div>
					</div>
					<span class="text-center text-xs capitalize text-[#8486A9] sm:text-2xl">
						{remaining?.seconds == 1 ? 'Second' : 'Seconds'}
					</span>
				</div>
			</div>
		</Countdown>
	</div>
</div>
