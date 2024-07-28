<script>
    export let step;
</script>

<a href={step.href} target="_blank" class="p-4 sm:p-6 md:p-8 flex flex-col gap-4 rounded-lg border border-solid border-violet-700
text-center cursor-pointer group hover:border-violet-400 duration-200 md:max-w-[400px]">
    <div class="bg-slate-950 grid place-items-center px-4 text-4xl md:text-5xl -mt-10 sm:-mt-12 md:-mt-14 lg:-mt-16 mx-auto duration-200">
        <i class={step.icon}></i>
    </div>
    <h3 class="font-medium text-xl sm:text-2xl md:text-3xl">{step.name}</h3>
    <slot />
    <div class="flex flex-1 items-end justify-between gap-4">
        <div class="ml-auto cursor-pointer hover:text-violet-400 duration-200 relative after:absolute after:top-0 after:h-0 after:right-full after:bg-white after:w-full after:duration-200 hover:after:translate-x-full after:z-[-1] overflow-hidden">
            <a href={step.link} target="_blank" class="z-4">Go to &rarr;</a>
        </div>
    </div>
</a>    