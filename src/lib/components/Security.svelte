<script>
  // Security component
</script>

<section class="py-20 max-w-[1400px] mx-auto overflow-hidden">
  <div class="px-4 md:px-8 flex flex-col items-center text-center mb-20">
    <div class="flex items-center gap-2 mb-4">
      <div class="w-2 h-2 rounded-full bg-[#22C55E]"></div>
      <span class="font-medium text-sm">Secure and private</span>
    </div>
    <h2 class="text-6xl md:text-7xl font-bold tracking-tighter max-w-4xl leading-tight">
      The Secure way 
      <span class="inline-flex items-center justify-center bg-[#A4C8F5] text-white w-16 h-12 rounded-full text-4xl align-middle mx-2">
         <svg width="24" height="24" viewBox="0 0 24 24" fill="black" stroke="black" stroke-width="2">
             <path d="M12 2L3 7v6c0 5.55 3.84 10.74 9 12 5.16-1.26 9-6.45 9-12V7l-9-5z" fill="none"/>
             <path d="M12 22c4.97-1.21 8-6.15 8-11.5V7.3l-8-4.44V22z"/>
         </svg>
      </span>
      to Web3
    </h2>
  </div>

  <!-- Horizontal Scroll Container -->
  <div class="flex overflow-x-auto gap-6 px-4 md:px-8 pb-10 snap-x snap-mandatory">
    
    <!-- Card 1: Portfolio Overview -->
    <div class="min-w-[300px] md:min-w-[360px] bg-[#F2F2F2] rounded-[2rem] p-6 flex flex-col snap-center">
      <h3 class="text-lg font-bold mb-2">Portfolio overview</h3>
      <p class="text-sm text-gray-500 mb-6">Track your entire portfolio in one place.</p>
      <div class="flex-1 bg-white rounded-xl border-4 border-gray-100 overflow-hidden relative h-[300px]">
           <!-- Simple phone UI -->
           <div class="p-4">
               <div class="h-4 w-1/2 bg-gray-100 rounded mb-4"></div>
               <div class="h-8 w-3/4 bg-gray-200 rounded mb-2"></div>
               <div class="h-4 w-1/4 bg-green-100 rounded mb-6"></div>
               <div class="space-y-2">
                   <div class="flex items-center gap-2"><div class="w-8 h-8 rounded-full bg-orange-100"></div><div class="h-4 w-20 bg-gray-100 rounded"></div></div>
                   <div class="flex items-center gap-2"><div class="w-8 h-8 rounded-full bg-blue-100"></div><div class="h-4 w-20 bg-gray-100 rounded"></div></div>
               </div>
           </div>
      </div>
    </div>

    <!-- Card 2: Hardware wallet support -->
    <div class="min-w-[300px] md:min-w-[360px] bg-[#F2F2F2] rounded-[2rem] p-6 flex flex-col snap-center">
      <h3 class="text-lg font-bold mb-2">Hardware wallet support</h3>
      <p class="text-sm text-gray-500 mb-6">Keeps funds safe on your Ledger / Trezor.</p>
      <div class="flex-1 flex items-center justify-center gap-4">
           <div class="w-20 h-20 bg-black rounded-2xl flex items-center justify-center">
               <!-- Ledger icon approx -->
               <svg width="40" height="40" viewBox="0 0 24 24" fill="white"><rect x="4" y="4" width="16" height="16" rx="2"/></svg>
           </div>
           <div class="w-20 h-20 bg-[#22C55E] rounded-2xl flex items-center justify-center">
               <!-- Trezor icon approx -->
               <svg width="40" height="40" viewBox="0 0 24 24" fill="white"><path d="M6 6h12v4h-4v8h-4v-8H6V6z"/></svg>
           </div>
      </div>
    </div>

    <!-- Card 3: Malicious address alerts -->
    <div class="min-w-[300px] md:min-w-[360px] bg-[#F2F2F2] rounded-[2rem] p-6 flex flex-col snap-center">
      <h3 class="text-lg font-bold mb-2">Malicious address alerts</h3>
      <p class="text-sm text-gray-500 mb-6">We flag malicious and suspicious addresses for you.</p>
      <div class="flex-1 bg-white rounded-xl border-4 border-gray-100 overflow-hidden relative h-[300px] flex items-center justify-center">
           <div class="w-4/5 bg-white shadow-lg rounded-lg p-4 border border-gray-100">
               <div class="flex items-center gap-2 mb-2 text-red-500 font-bold text-xs uppercase">
                   <svg width="12" height="12" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2L2 22h20L12 2z"/></svg>
                   Warning
               </div>
               <div class="h-2 w-full bg-gray-100 rounded mb-1"></div>
               <div class="h-2 w-2/3 bg-gray-100 rounded"></div>
           </div>
      </div>
    </div>

    <!-- Card 4: No IP tracking -->
    <div class="min-w-[300px] md:min-w-[360px] bg-[#F2F2F2] rounded-[2rem] p-6 flex flex-col snap-center">
      <h3 class="text-lg font-bold mb-2">No IP tracking</h3>
      <p class="text-sm text-gray-500 mb-6">We do not record any user IP addresses.</p>
      <div class="flex-1 flex flex-col items-center justify-center gap-2">
           <div class="bg-black rounded-full px-4 py-2 flex gap-2">
               {#each Array(5) as _}
                  <div class="w-4 h-4 rounded-full bg-[#333] border border-gray-600"></div>
               {/each}
           </div>
           <div class="bg-black rounded-full px-4 py-2 flex gap-2 opacity-80">
               {#each Array(5) as _}
                  <div class="w-4 h-4 rounded-full bg-[#333] border border-gray-600"></div>
               {/each}
           </div>
           <div class="bg-black rounded-full px-4 py-2 flex gap-2 opacity-60">
               {#each Array(5) as _}
                  <div class="w-4 h-4 rounded-full bg-[#333] border border-gray-600"></div>
               {/each}
           </div>
      </div>
    </div>

  </div>
</section>
