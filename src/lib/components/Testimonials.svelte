<script lang="ts">
  const testimonials = [
    {
      quote: "It was night and day from one batch to another, adoption went from single digits to over 60%. It just spread like wildfire, all the best builders were using Cursor.",
      name: "Diana Wu",
      role: "General Partner, Y Combinator",
      image: "https://randomuser.me/api/portraits/women/1.jpg" // Placeholder
    },
    {
      quote: "The most useful AI tool that I currently pay for, hands down, is Cursor. It's fast, autocompletes when and where you need it to, handles brackets properly, sensible keyboard shortcuts, bring-your-own-model... everything is well put together.",
      name: "shadcn",
      role: "Creator of shadcn/ui",
      image: "https://github.com/shadcn.png" // Placeholder
    },
    {
      quote: "The best LLM applications have an autonomy slider: you control how much independence to give the AI. In Cursor, you can do Tab completion, Cmd+K for targeted edits, or you can let it rip with the full autonomy agentic version.",
      name: "Andrej Karpathy",
      role: "CEO, Eureka Labs",
      image: "https://pbs.twimg.com/profile_images/1626268886361309185/19219219_400x400.jpg" // Placeholder
    },
    {
      quote: "Cursor quickly grew from hundreds to thousands of extremely enthusiastic Stripe employees. We spend more on R&D and software creation than any other undertaking, and there's significant economic outcomes when making that process more efficient and productive.",
      name: "Patrick Collison",
      role: "Co-Founder & CEO, Stripe",
      image: "https://pbs.twimg.com/profile_images/1626268886361309185/19219219_400x400.jpg" // Placeholder
    },
    {
      quote: "It's efficient.\n\nI hate vibe coding.\nI love Cursor tab coding.\n\nIt's wild.",
      name: "ThePrimeagen",
      role: "@ThePrimeagen",
      image: "https://pbs.twimg.com/profile_images/1626268886361309185/19219219_400x400.jpg" // Placeholder
    },
    {
      quote: "It's definitely becoming more fun to be a programmer. It's less about digging through pages and more about what you want to happen. We are at the 1% of what's possible, and it's in interactive experiences like Cursor where models like GPT-3 shine brightest.",
      name: "Greg Brockman",
      role: "President, OpenAI",
      image: "https://pbs.twimg.com/profile_images/1626268886361309185/19219219_400x400.jpg" // Placeholder
    }
  ];
</script>

<section class="py-24 px-6 max-w-[1400px] mx-auto">
  <h2 class="text-4xl md:text-5xl font-medium tracking-tight text-gray-900 mb-16 text-center md:text-left">
    The new way to build software.
  </h2>
  
  <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
    {#each testimonials as t}
      <div class="flex flex-col justify-between h-full space-y-6">
        <p class="text-lg text-gray-600 leading-relaxed whitespace-pre-line">
          {t.quote}
        </p>
        <div class="flex items-center gap-3">
          <div class="w-10 h-10 rounded-full bg-gray-300 overflow-hidden">
             <!-- <img src={t.image} alt={t.name} class="w-full h-full object-cover" /> -->
             <div class="w-full h-full bg-gray-400"></div>
          </div>
          <div>
            <div class="font-medium text-gray-900 text-sm">{t.name}</div>
            <div class="text-gray-500 text-sm">{t.role}</div>
          </div>
        </div>
      </div>
    {/each}
  </div>
</section>
