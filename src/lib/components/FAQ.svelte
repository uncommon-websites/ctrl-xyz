<script lang="ts">
  import { slide } from 'svelte/transition';
  
  const faqs = [
    "How do I take part in the Midnight Scavenger Mine?",
    "How do I claim the Midnight Glacier Airdrop $NIGHT token?",
    "Do you have a mobile wallet application?",
    "Can I migrate my MetaMask, Phantom or Keplr wallet to Ctrl?",
    "How do I connect to a dapp if I don't see the Ctrl logo?",
    "What is a non-custodial wallet?",
    "XDEFI migrated to Ctrl. What does this mean for me as an XDEFI user?",
    "How do I migrate my $XDEFI to $CTRL?",
    "Are my funds safe?",
    "Does Ctrl have control of my coins?",
    "I have questions or concerns, where is the best place to ask?"
  ];

  let openIndex: number = -1;

  function toggle(index: number) {
    openIndex = openIndex === index ? -1 : index;
  }
</script>

<section class="py-20 px-4 md:px-8 max-w-[1000px] mx-auto">
  <div class="text-center mb-12">
    <p class="text-gray-600 font-medium mb-4">Any questions ?</p>
    <h2 class="text-5xl md:text-6xl font-bold tracking-tight">FAQ</h2>
  </div>

  <div class="space-y-4">
    {#each faqs as question, i}
      <div class="border border-gray-300 rounded-2xl overflow-hidden bg-[#F2F2F0]">
        <button 
          class="w-full flex items-center justify-between p-6 text-left hover:bg-gray-200 transition-colors"
          on:click={() => toggle(i)}
        >
          <span class="font-medium text-lg pr-8">{question}</span>
          <div class="flex-shrink-0 w-8 h-8 rounded-full border border-gray-400 flex items-center justify-center transition-transform duration-300 {openIndex === i ? 'rotate-45' : ''}">
            <svg width="12" height="12" viewBox="0 0 12 12" fill="none" stroke="currentColor" stroke-width="2">
              <path d="M6 1V11M1 6H11"/>
            </svg>
          </div>
        </button>
        {#if openIndex === i}
          <div class="p-6 pt-0 text-gray-600" transition:slide>
            <p>Answer to "{question}" goes here. This is a placeholder text.</p>
          </div>
        {/if}
      </div>
    {/each}
  </div>

  <div class="text-center mt-12">
    <button class="border border-black rounded-full px-8 py-3 text-sm font-medium hover:bg-black hover:text-white transition-colors">
      Show all questions
    </button>
  </div>
</section>
