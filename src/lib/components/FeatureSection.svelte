<script lang="ts">
  export let title: string;
  export let description: string;
  export let linkText: string;
  export let href: string = '#';
  export let imagePosition: 'left' | 'right' = 'right';
</script>

<section class="py-24 px-6 max-w-[1400px] mx-auto">
  <div class="flex flex-col md:flex-row items-center gap-16 {imagePosition === 'left' ? 'md:flex-row-reverse' : ''}">
    <div class="flex-1 space-y-6">
      <h2 class="text-4xl md:text-5xl font-medium tracking-tight text-gray-900 leading-[1.1]">
        {title}
      </h2>
      <p class="text-xl text-gray-500 leading-relaxed max-w-lg">
        {description}
      </p>
      <a {href} class="inline-flex items-center text-[#FF4F00] font-medium hover:underline gap-1">
        {linkText}
        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14"/><path d="m12 5 7 7-7 7"/></svg>
      </a>
    </div>
    <div class="flex-1 w-full">
      <div class="bg-gray-100 rounded-xl aspect-[4/3] w-full shadow-lg border border-gray-200 overflow-hidden relative">
        <slot name="image">
            <div class="absolute inset-0 flex items-center justify-center text-gray-400">
                Feature Image Placeholder
            </div>
        </slot>
      </div>
    </div>
  </div>
</section>
