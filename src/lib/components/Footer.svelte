<script>
  // Footer component
</script>

<footer class="pt-20 pb-10 px-4 md:px-8 max-w-[1400px] mx-auto">
  <!-- Newsletter -->
  <div class="flex flex-col items-center text-center mb-20">
    <h3 class="font-bold text-lg mb-2">Newsletter</h3>
    <p class="text-gray-500 text-sm mb-8">Subscribe to our amazing newsletter to receive all the latest news & updates.</p>
    
    <div class="relative w-full max-w-xl">
      <input 
        type="email" 
        placeholder="Your email address" 
        class="w-full border border-black rounded-full py-4 px-6 pr-32 focus:outline-none focus:ring-1 focus:ring-black"
      />
      <button class="absolute right-2 top-2 bottom-2 bg-black text-white rounded-full px-6 text-sm font-medium hover:bg-gray-800 transition-colors">
        Subscribe
      </button>
    </div>
  </div>

  <!-- Big Text -->
  <div class="text-center mb-20">
    <h2 class="text-[15vw] leading-none font-bold tracking-tighter">Level up.</h2>
  </div>

  <!-- Links Grid -->
  <div class="grid grid-cols-2 md:grid-cols-4 gap-10 mb-20 border-t border-gray-200 pt-10">
    <!-- Social Icons (Desktop: Left, Mobile: Bottom) -->
    <div class="col-span-2 md:col-span-1 flex gap-4 items-start">
      <a href="#" class="w-10 h-10 rounded-full border border-black flex items-center justify-center hover:bg-black hover:text-white transition-colors">
        <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M21 11.5a8.38 8.38 0 0 1-.9 3.8 8.5 8.5 0 0 1-7.6 4.7 8.38 8.38 0 0 1-3.8-.9L3 21l1.9-5.7a8.38 8.38 0 0 1-.9-3.8 8.5 8.5 0 0 1 4.7-7.6 8.38 8.38 0 0 1 3.8-.9h.5a8.48 8.48 0 0 1 8 8v.5z"/></svg>
      </a>
      <a href="#" class="w-10 h-10 rounded-full border border-black flex items-center justify-center hover:bg-black hover:text-white transition-colors">
        <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M23 3a10.9 10.9 0 0 1-3.14 1.53 4.48 4.48 0 0 0-7.86 3v1A10.66 10.66 0 0 1 3 4s-4 9 5 13a11.64 11.64 0 0 1-7 2c9 5 20 0 20-11.5a4.5 4.5 0 0 0-.08-.83A7.72 7.72 0 0 0 23 3z"/></svg>
      </a>
      <a href="#" class="w-10 h-10 rounded-full border border-black flex items-center justify-center hover:bg-black hover:text-white transition-colors">
        <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"/></svg>
      </a>
      <a href="#" class="w-10 h-10 rounded-full border border-black flex items-center justify-center hover:bg-black hover:text-white transition-colors">
        <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M19.615 3.184c-3.604-.246-11.631-.245-15.23 0-3.897.266-4.356 2.62-4.385 8.816.029 6.185.484 8.549 4.385 8.816 3.6.245 11.626.246 15.23 0 3.897-.266 4.356-2.62 4.385-8.816-.029-6.185-.484-8.549-4.385-8.816zm-10.615 12.816v-8l8 3.993-8 4.007z"/></svg>
      </a>
    </div>

    <!-- Product -->
    <div>
      <h4 class="font-bold mb-4">Product</h4>
      <ul class="space-y-2 text-sm text-gray-500">
        <li><a href="#" class="hover:text-black">Security</a></li>
        <li><a href="#" class="hover:text-black">Support</a></li>
      </ul>
    </div>

    <!-- Company -->
    <div>
      <h4 class="font-bold mb-4">Company</h4>
      <ul class="space-y-2 text-sm text-gray-500">
        <li><a href="#" class="hover:text-black">Introducing Ctrl</a></li>
        <li><a href="#" class="hover:text-black">About</a></li>
      </ul>
    </div>

    <!-- Resources -->
    <div>
      <h4 class="font-bold mb-4">Resources</h4>
      <ul class="space-y-2 text-sm text-gray-500">
        <li><a href="#" class="hover:text-black">News</a></li>
        <li><a href="#" class="hover:text-black">Docs</a></li>
        <li><a href="#" class="hover:text-black">Media Kit</a></li>
        <li><a href="#" class="hover:text-black">Shortcuts</a></li>
      </ul>
    </div>
  </div>

  <!-- Bottom Bar -->
  <div class="flex flex-col md:flex-row justify-between items-center text-[10px] text-gray-400 border-t border-gray-100 pt-8">
    <div class="flex gap-4 mb-4 md:mb-0">
      <a href="#" class="hover:text-black">Terms of use</a>
      <a href="#" class="hover:text-black">Privacy policy</a>
      <a href="#" class="hover:text-black">Cookie Preferences</a>
    </div>
    
    <div class="flex items-center gap-1">
      <span>English</span>
      <svg width="10" height="10" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M6 9l6 6 6-6"/></svg>
    </div>
  </div>
</footer>
