<template>
  <button type="button" class="add-network" @click="addNetwork">
    <img width="18" src="/images/metamask_logo.svg" alt="Metamask">
    Add {{ chainName }}
  </button>
</template>

<script setup>
const props = defineProps(['network'])
const {network} = props
const chainName = props.network === 'mainnet' ? 'zkSync Era Mainnet' : 'zkSync Era Sepolia Testnet'
function addNetwork() {
  const config = {
    mainnet: {
      chainId: '0x144',
      rpcUrls: ['https://mainnet.era.zksync.io'],
      blockExplorerUrls: ['https://explorer.zksync.io/'],
    },
    testnet: {
      chainId: '0x12c',
      rpcUrls: ['https://sepolia.era.zksync.dev'],
      blockExplorerUrls: ['https://sepolia.explorer.zksync.dev/'],
    },
  }[network];
  window.ethereum.request({
    method: 'wallet_addEthereumChain',
    params: [
      {
        chainId: config.chainId,
        chainName: chainName,
        nativeCurrency: {name: 'Ethereum', symbol: 'ETH', decimals: 18},
        iconUrls: ['https://docs.zksync.io/favicon-32x32.png'],
        rpcUrls: config.rpcUrls,
        blockExplorerUrls: config.blockExplorerUrls,
      },
    ],
  });
}
</script>

<style scoped>
.add-network {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 4px 8px;
  gap: 4px;
  cursor: pointer;
}
img[src*="/images/metamask_logo.svg"] {
  content: url("/images/metamask_logo.svg");
}
</style>
