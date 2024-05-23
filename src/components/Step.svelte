<script>
    export let step;
</script>

<a href={step.href} target="_blank" 
   class="relative p-4 sm:p-6 flex flex-col gap-4 rounded-lg border border-solid border-violet-700 text-center group cursor-pointer hover:border-violet-400 duration-200">
    <div class="bg-slate-950 grid place-items-center px-4 text-5xl md:text-6xl -mt-10 sm:-mt-12 md:-mt-14 lg:-mt-16 mx-auto duration-200 relative z-10 rounded-md p-2"> <!-- Added padding here -->
        <i class={step.icon} />
    </div>
    <h3 class="font-medium text-xl sm:text-2xl md:text-3xl relative z-10">{step.name}</h3>
    <slot class="relative z-10" />
    <div class="flex-1 flex justify-between gap-4 items-center relative z-10">
        <div class="ml-auto cursor-pointer hover:text-slate-950 duration-200 relative
         after:absolute after:top-0 after:h-0 after:right-full after:w-full after:h-full after:bg-white
         after:duration-200 hover:after:translate-x-full after:z-[-1] overflow-hidden">
            <p class="relative z-10">check it out &rarr;</p>
        </div>
    </div>

    <!-- Background image that fades in on hover -->
    <div class="absolute inset-0 bg-cover bg-center opacity-0 group-hover:opacity-50 transition-opacity duration-500" 
         style="background-image: url({step.image}); z-index: -1;"></div>
</a>