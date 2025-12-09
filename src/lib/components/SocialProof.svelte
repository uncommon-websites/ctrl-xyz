<script>
  // SocialProof component
</script>

<section class="py-20 px-4 md:px-8 max-w-[1400px] mx-auto">
  <div class="flex flex-col items-center text-center mb-20">
    <div class="flex items-center gap-2 mb-4">
      <div class="w-2 h-2 rounded-full bg-[#FF5F52]"></div>
      <span class="font-medium text-sm">Take Ctrl</span>
    </div>
    <h2 class="text-5xl md:text-6xl font-bold tracking-tighter max-w-4xl leading-tight">
      Join the 
      <span class="inline-flex items-center justify-center text-5xl align-middle mx-2">✌️</span>
      600,000+ people<br>who trust Ctrl.
    </h2>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    <!-- Card 1 -->
    <div class="bg-[#A4C8F5] rounded-[2.5rem] p-8 flex flex-col justify-between min-h-[320px] relative overflow-hidden">
      <p class="text-xl font-medium leading-snug max-w-xs">
        Founded in 2020, Ctrl (formerly XDEFI) was the world's first multichain wallet.
      </p>
      
      <div class="mt-8 relative">
        <div class="w-16 h-16 bg-black rounded-xl flex items-center justify-center transform rotate-3">
             <svg width="32" height="32" viewBox="0 0 24 24" fill="white">
                 <path d="M2 2h9v9h-9zM13 2h9v9h-9zM2 13h9v9h-9zM13 13h9v9h-9z"/>
             </svg>
        </div>
        <!-- Cursor -->
        <div class="absolute top-10 left-10">
             <svg width="24" height="24" viewBox="0 0 24 24" fill="#FFD93D" stroke="black" stroke-width="1.5">
                 <path d="M3 3l7.07 16.97 2.51-7.39 7.39-2.51L3 3z"/>
             </svg>
        </div>
      </div>
    </div>

    <!-- Card 2 -->
    <div class="bg-[#FFC8DD] rounded-[2.5rem] p-8 flex flex-col justify-between min-h-[320px]">
      <p class="text-xl font-medium leading-snug max-w-xs">
        4.8 star rating in the Google Chrome Store after 650+ reviews.
      </p>
      
      <div class="mt-8 space-y-3">
        <div class="bg-white rounded-full px-4 py-2 inline-flex gap-1 border border-black/5 shadow-sm">
             {#each Array(5) as _}
                <svg width="20" height="20" viewBox="0 0 24 24" fill="#FFD93D" stroke="#B8860B" stroke-width="1">
                    <polygon points="12 2 15.09 8.26 22 9.27 17 14.14 18.18 21.02 12 17.77 5.82 21.02 7 14.14 2 9.27 8.91 8.26 12 2"/>
                </svg>
             {/each}
        </div>
        <div class="bg-white rounded-full px-4 py-2 inline-flex gap-1 border border-black/5 shadow-sm opacity-80">
             {#each Array(5) as _}
                <svg width="20" height="20" viewBox="0 0 24 24" fill="#FFD93D" stroke="#B8860B" stroke-width="1">
                    <polygon points="12 2 15.09 8.26 22 9.27 17 14.14 18.18 21.02 12 17.77 5.82 21.02 7 14.14 2 9.27 8.91 8.26 12 2"/>
                </svg>
             {/each}
        </div>
        <div class="bg-white rounded-full px-4 py-2 inline-flex gap-1 border border-black/5 shadow-sm opacity-60">
             {#each Array(5) as _}
                <svg width="20" height="20" viewBox="0 0 24 24" fill="#FFD93D" stroke="#B8860B" stroke-width="1">
                    <polygon points="12 2 15.09 8.26 22 9.27 17 14.14 18.18 21.02 12 17.77 5.82 21.02 7 14.14 2 9.27 8.91 8.26 12 2"/>
                </svg>
             {/each}
        </div>
      </div>
    </div>

    <!-- Card 3 -->
    <div class="bg-[#FFE57F] rounded-[2.5rem] p-8 flex flex-col justify-between min-h-[320px]">
      <p class="text-xl font-medium leading-snug max-w-xs">
        24/7 live customer support. Our global team is here to help you.
      </p>
      
      <div class="mt-8 relative h-32">
        <div class="absolute bottom-10 left-0 bg-white rounded-full px-4 py-2 text-sm font-medium border border-black/5 shadow-sm">
            Job done ;)
        </div>
        <div class="absolute bottom-0 right-0 bg-white rounded-full px-4 py-2 text-sm font-medium border border-black/5 shadow-sm">
            Thx, you rock!
        </div>
        <div class="absolute bottom-0 right-[-10px] w-8 h-8 rounded-full bg-black/10 flex items-center justify-center">
            👋
        </div>
      </div>
    </div>
  </div>
</section>
