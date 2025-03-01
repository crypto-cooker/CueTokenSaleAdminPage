<template>
    <section class="py-20 lg:bg-contain bg-top bg-no-repeat">
      <div class="container mx-auto px-4">
        <div class="max-w-sm mx-auto mb-12 text-center" >
          <h2 class="mb-4 text-3xl md:text-4xl font-bold font-heading">Frequently Asked&nbsp;Questions</h2>
          <p class="text-sm md:text-base leading-loose text-blueGray-500">
            <span>Can’t find the answer you’re looking for? Write out to our </span>
            <a class="text-blue-600 hover:text-blue-700" href="mailto:support@ethereumx.com">customer support team.</a>
          </p>
        </div>
        <div class="max-w-3xl mx-auto">
          <ul class="space-y-4">
            <li class="px-6 py-4 bg-white rounded shadow">
              <button
                  class="w-full flex justify-between items-center text-left font-bold font-heading hover:text-blueGray-700"
                  @click="selected !== 1 ? selected = 1 : selected = null"
              >
                <span>When does the token sale end?</span>
                <svg class="w-4 h-4 ml-2 text-blueGray-300" fill="none" stroke="currentColor"
                     viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                        d="M19 9l-7 7-7-7"></path>
                </svg>
              </button>
              <p class="mt-2 text-blueGray-400 text-left font-normal leading-loose relative overflow-hidden transition-all max-h-0 duration-700"
                ref="container1"
                v-bind:style="selected == 1 ? 'max-height: ' + $refs.container1.scrollHeight + 'px' : ''"
              >
                The EthereumX token sale will have 25 rounds. The first round starts at the lowest price per token. The price goes up every round. A round ends when all tokens in that round have been sold or when the timer runs out. After 25 rounds, the token sale ends and participants can claim the token.</p>
            </li>
            <li class="px-6 py-4 bg-white rounded shadow">
              <button class="w-full flex justify-between items-center text-left font-bold font-heading text-blue-600 hover:text-blue-700"
                @click="selected !== 2 ? selected = 2 : selected = null"
              >
                <span>How much can I contribute?</span>
                <svg class="w-4 h-4 ml-2 text-blueGray-500" fill="none" stroke="currentColor"
                     viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                        d="M19 9l-7 7-7-7"></path>
                </svg>
              </button>
              <p class="mt-2 text-left text-blueGray-400 font-normal leading-loose relative overflow-hidden transition-all max-h-0 duration-700"
                ref="container2"
                v-bind:style="selected == 2 ? 'max-height: ' + $refs.container2.scrollHeight + 'px' : ''"
              >
                You can send a maximum of 20 ETH and 100 BNB.
               </p>
            </li>
            <li class="px-6 py-4 bg-white rounded shadow">
              <button
                  class="w-full flex justify-between items-center text-left font-bold font-heading hover:text-blueGray-700"
                  @click="selected !== 3 ? selected = 3 : selected = null"
                >
                <span>Is there a minimum contribution?</span>
                <svg class="w-4 h-4 ml-2 text-blueGray-300" fill="none" stroke="currentColor"
                     viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                        d="M19 9l-7 7-7-7"></path>
                </svg>
              </button>
              <p class=" mt-2 text-blueGray-400 text-left font-normal leading-loose relative overflow-hidden transition-all max-h-0 duration-700"
                ref="container3"
                v-bind:style="selected == 3 ? 'max-height: ' + $refs.container3.scrollHeight + 'px' : ''"
              >
                Yes, 0.01 ETH or 0.01 BNB.</p>
            </li>
            <li class="px-6 py-4 bg-white rounded shadow">
              <button class="w-full flex justify-between items-center text-left font-bold font-heading hover:text-blueGray-700"
                @click="selected !== 4 ? selected = 4 : selected = null"
              >
                <span>What happens if I send more than the maximum amount?</span>
                <svg class="w-4 h-4 ml-2 text-blueGray-300" fill="none" stroke="currentColor"
                     viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                        d="M19 9l-7 7-7-7"></path>
                </svg>
              </button>
              <p class="mt-2  text-left text-blueGray-400 font-normal leading-loose relative overflow-hidden transition-all max-h-0 duration-700"
                ref="container4"
                v-bind:style="selected == 4 ? 'max-height: ' + $refs.container4.scrollHeight + 'px' : ''"
              >
                If you send more, the transaction will fail and the funds are returned to your wallet.</p>
            </li>
            <li class="px-6 py-4 bg-white rounded shadow">
              <button class="w-full flex justify-between items-center text-left font-bold font-heading hover:text-blueGray-700"
                @click="selected !== 5 ? selected = 5 : selected = null"
              >
                <span>Can I send money from an exchange wallet like Coinbase?</span>
                <svg class="w-4 h-4 ml-2 text-blueGray-300" fill="none" stroke="currentColor"
                     viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                        d="M19 9l-7 7-7-7"></path>
                </svg>
              </button>
              <p class="mt-2 text-left text-blueGray-400 font-normal leading-loose relative overflow-hidden transition-all max-h-0 duration-700"
                ref="container5"
                v-bind:style="selected == 5 ? 'max-height: ' + $refs.container5.scrollHeight + 'px' : ''"
              >
                No, do not send money from an exchange wallet. If for any reason we need to return funds back to your wallet, funds that
                were originally sent from an exchange wallet will be lost and you will not be able to receive the tokens you purchase.</p>
            </li>
            <li class="px-6 py-4 bg-white rounded shadow">
              <button class="w-full flex justify-between items-center text-left font-bold font-heading hover:text-blueGray-700"
                @click="selected !== 6 ? selected = 6 : selected = null"
              >
                <span>When will I receive my tokens?</span>
                <svg class="w-4 h-4 ml-2 text-blueGray-300" fill="none" stroke="currentColor"
                     viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                        d="M19 9l-7 7-7-7"></path>
                </svg>
              </button>
              <p class="mt-2 text-left text-blueGray-400 font-normal leading-loose relative overflow-hidden transition-all max-h-0 duration-700"
                ref="container6"
                v-bind:style="selected == 6 ? 'max-height: ' + $refs.container6.scrollHeight + 'px' : ''"
              >
                Immediately after the token sale ends.</p>
            </li>
            <li class="px-6 py-4 bg-white rounded shadow">
              <button class="w-full flex justify-between items-center text-left font-bold font-heading hover:text-blueGray-700"
                @click="selected !== 7 ? selected = 7 : selected = null"
              >
                <span>How do I know that my contribution was successfully accepted?</span>
                <svg class="w-4 h-4 ml-2 text-blueGray-300" fill="none" stroke="currentColor"
                     viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                        d="M19 9l-7 7-7-7"></path>
                </svg>
              </button>
              <p class="mt-2 text-left text-blueGray-400 font-normal leading-loose relative overflow-hidden transition-all max-h-0 duration-700"
                ref="container7"
                v-bind:style="selected == 7 ? 'max-height: ' + $refs.container7.scrollHeight + 'px' : ''"
              >
                Just check your transaction in metamask after purchase. If the transactions are successful, you have bought tokens.</p>
            </li>
            <li class="px-6 py-4 bg-white rounded shadow">
              <button class="w-full flex justify-between items-center text-left font-bold font-heading hover:text-blueGray-700"
                @click="selected !== 8 ? selected = 8 : selected = null"
              >
                <span>How can I trust I am sending to the official EthereumX address?</span>
                <svg class="w-4 h-4 ml-2 text-blueGray-300" fill="none" stroke="currentColor"
                     viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                        d="M19 9l-7 7-7-7"></path>
                </svg>
              </button>
              <p class="mt-2 text-left text-blueGray-400 font-normal leading-loose relative overflow-hidden transition-all max-h-0 duration-700"
                ref="container8"
                v-bind:style="selected == 8 ? 'max-height: ' + $refs.container8.scrollHeight + 'px' : ''"
              >
                Always double check that you are on the official tokensale.ethereumx.com URL.</p>
            </li>
          </ul>
        </div>
      </div>
    </section>
</template>

<script>
export default {
    data(){
        return {
            selected:null
        }
    }
}
</script>

<style>

</style>
