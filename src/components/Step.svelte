<script>
    export let step;
</script>
<!--This whole class is to create the effect of blocking the blue line -->
<a href={step.href} target="_blank" class="p-4 sm:p-6 md:p-8 flex flex-col gap-4 rounded-lg border boder-solid border-sky-600 text-center group cursor-pointer hover:border-sky-300 duration-200">
    <div class="bg-slate-950 grid place-items-center px-4 text-5xl md:text-6xl -mt-10 sm:-sm-12 md:-sm-14 lg:-mt-16 mx-auto duration-200">
        <i class={step.icon}/>
    </div>
    <h3 class="font-medium text-xl sm:text-2xl md:text-3xl">{step.name}</h3>
    <slot/>
    <div class="flex-1 flex justify-between gap-4 items-center">
        <div class="ml-auto cursor-pointer hover:text-slate-950 duration-200 relative after:absolute after:top-0 after:right-full after:w-full after:h-full after:duration-200 hover:after:translate-x-full after:z-[-1] after:bg-white after:rounded-md overflow-hidden">
            <p class="relative z-4">Go to &rarr;</p>
        </div>
    </div>
</a>