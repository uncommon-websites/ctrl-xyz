<script>
  import { onMount } from 'svelte';
</script>

<section class="pt-32 pb-20 px-4 md:px-8 max-w-[1400px] mx-auto flex flex-col items-center">
  <div class="text-center mb-16">
    <p class="text-gray-600 font-medium mb-4">One wallet<br>for all your crypto</p>
    <h1 class="text-7xl md:text-8xl font-bold tracking-tighter flex items-center justify-center gap-4">
      Take 
      <div class="bg-black text-white w-16 h-16 md:w-20 md:h-20 rounded-2xl flex items-center justify-center">
        <svg width="40" height="40" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
          <rect x="2" y="2" width="9" height="9" rx="2" stroke="currentColor" stroke-width="2.5"/>
          <rect x="13" y="2" width="9" height="9" rx="2" stroke="currentColor" stroke-width="2.5"/>
          <rect x="2" y="13" width="9" height="9" rx="2" stroke="currentColor" stroke-width="2.5"/>
          <rect x="13" y="13" width="9" height="9" rx="2" stroke="currentColor" stroke-width="2.5"/>
          <path d="M12 2V22" stroke="black" stroke-width="4"/>
          <path d="M2 12H22" stroke="black" stroke-width="4"/>
        </svg>
        <!-- Actually the icon is a square with 4 sub-squares, but let's look closer at the screenshot. 
             It looks like a black square with a white symbol inside. The symbol looks like a grid or a window.
             Let's try to approximate it better. It looks like a 4-pane window with rounded corners.
        -->
        <div class="absolute inset-0 flex items-center justify-center">
             <svg width="48" height="48" viewBox="0 0 24 24" fill="white" xmlns="http://www.w3.org/2000/svg">
                <path fill-rule="evenodd" clip-rule="evenodd" d="M4 4H10V10H4V4ZM14 4H20V10H14V4ZM4 14H10V20H4V14ZM14 14H20V20H14V14ZM2 6C2 3.79086 3.79086 2 6 2H18C20.2091 2 22 3.79086 22 6V18C22 20.2091 20.2091 22 18 22H6C3.79086 22 2 20.2091 2 18V6Z" opacity="0.0"/>
                <!-- Let's just draw 4 squares -->
                <rect x="5" y="5" width="6" height="6" rx="1" fill="white"/>
                <rect x="13" y="5" width="6" height="6" rx="1" fill="white"/>
                <rect x="5" y="13" width="6" height="6" rx="1" fill="white"/>
                <rect x="13" y="13" width="6" height="6" rx="1" fill="white"/>
             </svg>
        </div>
      </div>
      Ctrl.
    </h1>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-12 gap-6 w-full max-w-6xl">
    
    <!-- Left Card -->
    <div class="md:col-span-4 bg-[#DCEAF9] rounded-[2.5rem] p-8 flex flex-col justify-between h-[400px] md:h-auto relative overflow-hidden group">
        <!-- Gradient overlay/effect -->
        <div class="absolute top-0 right-0 w-64 h-64 bg-[#C4DDF7] rounded-full blur-3xl -translate-y-1/2 translate-x-1/2"></div>
        
        <h2 class="text-4xl font-medium leading-tight text-gray-800 relative z-10">
            Create your<br>wallet in<br>seconds.
        </h2>
        
        <div class="relative z-10">
            <button class="bg-white/60 backdrop-blur-sm px-6 py-2 rounded-full text-sm font-medium text-gray-600">
                Simple
            </button>
        </div>
        
        <!-- Decorative lightning bolt -->
        <div class="absolute top-8 right-8 text-gray-400/50">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                <path d="M13 2L3 14H12L11 22L21 10H12L13 2Z" stroke-linejoin="round" stroke-linecap="round"/>
            </svg>
        </div>
    </div>

    <!-- Center Phone -->
    <div class="md:col-span-4 flex justify-center items-end -mb-20 md:mb-0 z-10">
        <div class="bg-white rounded-[2.5rem] shadow-2xl border-[6px] border-gray-100 w-[320px] overflow-hidden relative">
            <!-- Status Bar -->
            <div class="h-6 w-full flex justify-between px-6 pt-3">
                <!-- <span class="text-[10px] font-bold">9:41</span> -->
            </div>

            <!-- App Header -->
            <div class="px-6 pt-4 pb-2">
                <div class="flex justify-between items-center mb-4">
                    <div class="flex items-center gap-2">
                        <div class="w-6 h-6 rounded-full bg-gray-200 flex items-center justify-center text-[10px]">P</div>
                        <span class="font-semibold text-sm">Portfolio</span>
                        <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M6 9l6 6 6-6"/></svg>
                    </div>
                    <div class="flex gap-3">
                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="11" cy="11" r="8"/><path d="M21 21l-4.35-4.35"/></svg>
                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 5v14M5 12h14"/></svg>
                    </div>
                </div>
                
                <div class="mb-6">
                    <h3 class="text-3xl font-bold tracking-tight">$48,708.09</h3>
                    <p class="text-[#22C55E] text-sm font-medium flex items-center gap-1">
                        +11% ($1427.35)
                    </p>
                </div>

                <div class="flex gap-6 border-b border-gray-100 pb-2 mb-4">
                    <button class="font-semibold text-black border-b-2 border-black pb-2 -mb-2.5">Tokens</button>
                    <button class="font-medium text-gray-400">NFTs</button>
                </div>
            </div>

            <!-- Token List -->
            <div class="px-4 pb-4 space-y-1">
                <!-- Bitcoin -->
                <div class="flex items-center justify-between p-2 hover:bg-gray-50 rounded-xl">
                    <div class="flex items-center gap-3">
                        <div class="w-10 h-10 rounded-full bg-[#F7931A] flex items-center justify-center text-white font-bold text-lg">₿</div>
                        <div>
                            <div class="font-semibold text-sm">Bitcoin</div>
                            <div class="text-xs text-gray-500">0.1512 BTC</div>
                        </div>
                    </div>
                    <div class="text-right">
                        <div class="font-semibold text-sm">$7,050</div>
                        <div class="text-xs text-[#22C55E]">+2% ($140)</div>
                    </div>
                </div>

                <!-- Solana -->
                <div class="flex items-center justify-between p-2 hover:bg-gray-50 rounded-xl">
                    <div class="flex items-center gap-3">
                        <div class="w-10 h-10 rounded-full bg-black flex items-center justify-center overflow-hidden">
                             <!-- Gradient for Solana -->
                             <div class="w-full h-full bg-gradient-to-br from-[#9945FF] to-[#14F195]"></div>
                        </div>
                        <div>
                            <div class="font-semibold text-sm">Solana</div>
                            <div class="text-xs text-gray-500">59.3279 SOL</div>
                        </div>
                    </div>
                    <div class="text-right">
                        <div class="font-semibold text-sm">$6,012.45</div>
                        <div class="text-xs text-[#22C55E]">+4% ($240)</div>
                    </div>
                </div>

                <!-- THORChain -->
                <div class="flex items-center justify-between p-2 hover:bg-gray-50 rounded-xl">
                    <div class="flex items-center gap-3">
                        <div class="w-10 h-10 rounded-full bg-[#33FF99] flex items-center justify-center relative overflow-hidden">
                            <div class="absolute inset-0 bg-[#00CCFF] opacity-50 rotate-45"></div>
                             <!-- Simple hammer shape -->
                             <svg width="20" height="20" viewBox="0 0 24 24" fill="white" stroke="white" stroke-width="2">
                                <path d="M12 2L2 12h20L12 2z"/>
                             </svg>
                        </div>
                        <div>
                            <div class="font-semibold text-sm">THORChain</div>
                            <div class="text-xs text-gray-500">1,505.421 RUNE</div>
                        </div>
                    </div>
                    <div class="text-right">
                        <div class="font-semibold text-sm">$5,887</div>
                        <div class="text-xs text-[#22C55E]">+2.18% ($130.14)</div>
                    </div>
                </div>

                <!-- ATOM -->
                <div class="flex items-center justify-between p-2 hover:bg-gray-50 rounded-xl">
                    <div class="flex items-center gap-3">
                        <div class="w-10 h-10 rounded-full bg-[#2E3148] flex items-center justify-center text-white text-xs">
                           ATOM
                        </div>
                        <div>
                            <div class="font-semibold text-sm">ATOM</div>
                            <div class="text-xs text-gray-500">642.0323 ATOM</div>
                        </div>
                    </div>
                    <div class="text-right">
                        <div class="font-semibold text-sm">$4,067.23</div>
                        <div class="text-xs text-[#22C55E]">+6.13% ($290.17)</div>
                    </div>
                </div>

                 <!-- Pepe -->
                <div class="flex items-center justify-between p-2 hover:bg-gray-50 rounded-xl">
                    <div class="flex items-center gap-3">
                        <div class="w-10 h-10 rounded-full bg-[#46A048] flex items-center justify-center text-white text-xs overflow-hidden">
                           <!-- Simple Pepe face approximation -->
                           <svg width="24" height="24" viewBox="0 0 24 24" fill="none">
                               <circle cx="12" cy="12" r="12" fill="#46A048"/>
                               <path d="M7 10C7 10 8 9 10 9C12 9 13 10 13 10" stroke="white" stroke-width="1.5" stroke-linecap="round"/>
                               <path d="M15 9C15 9 16 8 18 8C20 8 21 9 21 9" stroke="white" stroke-width="1.5" stroke-linecap="round"/>
                               <circle cx="10" cy="12" r="1.5" fill="white"/>
                               <circle cx="18" cy="11" r="1.5" fill="white"/>
                               <path d="M10 16C10 16 12 18 16 17" stroke="white" stroke-width="1.5" stroke-linecap="round"/>
                           </svg>
                        </div>
                        <div>
                            <div class="font-semibold text-sm">Pepe</div>
                            <div class="text-xs text-gray-500">345,911,949.685 PEPE</div>
                        </div>
                    </div>
                    <div class="text-right">
                        <div class="font-semibold text-sm">$3,300</div>
                        <div class="text-xs text-[#22C55E]">+1% ($33)</div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Right Card -->
    <div class="md:col-span-4 bg-[#F2F2F2] rounded-[2.5rem] p-8 flex flex-col justify-center h-[400px] md:h-auto relative">
        <h2 class="text-4xl font-medium leading-tight text-gray-800 mb-8">
            Using your social<br>account or<br>Google.
        </h2>
        
        <div class="flex gap-3">
            <div class="w-10 h-10 rounded-full bg-white flex items-center justify-center shadow-sm">
                <!-- Google G -->
                <svg width="20" height="20" viewBox="0 0 24 24">
                    <path d="M22.56 12.25c0-.78-.07-1.53-.2-2.25H12v4.26h5.92c-.26 1.37-1.04 2.53-2.21 3.31v2.77h3.57c2.08-1.92 3.28-4.74 3.28-8.09z" fill="#4285F4"/>
                    <path d="M12 23c2.97 0 5.46-.98 7.28-2.66l-3.57-2.77c-.98.66-2.23 1.06-3.71 1.06-2.86 0-5.29-1.93-6.16-4.53H2.18v2.84C3.99 20.53 7.7 23 12 23z" fill="#34A853"/>
                    <path d="M5.84 14.09c-.22-.66-.35-1.36-.35-2.09s.13-1.43.35-2.09V7.07H2.18C1.43 8.55 1 10.22 1 12s.43 3.45 1.18 4.93l2.85-2.22.81-.62z" fill="#FBBC05"/>
                    <path d="M12 5.38c1.62 0 3.06.56 4.21 1.64l3.15-3.15C17.45 2.09 14.97 1 12 1 7.7 1 3.99 3.47 2.18 7.07l3.66 2.84c.87-2.6 3.3-4.53 6.16-4.53z" fill="#EA4335"/>
                </svg>
            </div>
            <div class="w-10 h-10 rounded-full bg-white flex items-center justify-center shadow-sm text-[#1877F2]">
                <!-- Facebook F -->
                <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor">
                    <path d="M24 12.073c0-6.627-5.373-12-12-12s-12 5.373-12 12c0 5.99 4.388 10.954 10.125 11.854v-8.385H7.078v-3.47h3.047V9.43c0-3.007 1.792-4.669 4.533-4.669 1.312 0 2.686.235 2.686.235v2.953H15.83c-1.491 0-1.956.925-1.956 1.874v2.25h3.328l-.532 3.47h-2.796v8.385C19.612 23.027 24 18.062 24 12.073z"/>
                </svg>
            </div>
            <div class="w-10 h-10 rounded-full bg-white flex items-center justify-center shadow-sm text-[#1DA1F2]">
                <!-- Twitter/X -->
                <svg width="18" height="18" viewBox="0 0 24 24" fill="currentColor">
                    <path d="M23.953 4.57a10 10 0 01-2.825.775 4.958 4.958 0 002.163-2.723c-.951.555-2.005.959-3.127 1.184a4.92 4.92 0 00-8.384 4.482C7.69 8.095 4.067 6.13 1.64 3.162a4.822 4.822 0 00-.666 2.475c0 1.71.87 3.213 2.188 4.096a4.904 4.904 0 01-2.228-.616v.06a4.923 4.923 0 003.946 4.827 4.996 4.996 0 01-2.212.085 4.936 4.936 0 004.604 3.417 9.867 9.867 0 01-6.102 2.105c-.39 0-.779-.023-1.17-.067a13.995 13.995 0 007.557 2.209c9.053 0 13.998-7.496 13.998-13.985 0-.21 0-.42-.015-.63A9.935 9.935 0 0024 4.59z"/>
                </svg>
            </div>
            <div class="w-10 h-10 rounded-full bg-[#24C45E] flex items-center justify-center shadow-sm text-white">
                <!-- Phone/Whatsapp icon -->
                <svg width="18" height="18" viewBox="0 0 24 24" fill="currentColor">
                    <path d="M.057 24l1.687-6.163c-1.041-1.804-1.588-3.849-1.587-5.946.003-6.556 5.338-11.891 11.893-11.891 3.181.001 6.167 1.24 8.413 3.488 2.245 2.248 3.481 5.236 3.48 8.414-.003 6.557-5.338 11.892-11.893 11.892-1.99-.001-3.951-.5-5.688-1.448l-6.305 1.654zm6.597-3.807c1.676.995 3.276 1.591 5.392 1.592 5.448 0 9.886-4.434 9.889-9.885.002-5.462-4.415-9.89-9.881-9.892-5.452 0-9.887 4.434-9.889 9.884-.001 2.225.651 3.891 1.746 5.634l-.999 3.648 3.742-.981zm11.387-5.464c-.074-.124-.272-.198-.57-.347-.297-.149-1.758-.868-2.031-.967-.272-.099-.47-.149-.669.149-.198.297-.768.967-.941 1.165-.173.198-.347.223-.644.074-.297-.149-1.255-.462-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.297-.347.446-.521.151-.172.2-.296.3-.495.099-.198.05-.372-.025-.521-.075-.148-.669-1.611-.916-2.206-.242-.579-.487-.501-.669-.51l-.57-.01c-.198 0-.52.074-.792.372s-1.04 1.016-1.04 2.479 1.065 2.876 1.213 3.074c.149.198 2.095 3.2 5.076 4.487.709.306 1.263.489 1.694.626.712.226 1.36.194 1.872.118.571-.085 1.758-.719 2.006-1.413.248-.695.248-1.29.173-1.414z"/>
                </svg>
            </div>
        </div>
    </div>
  </div>
</section>
