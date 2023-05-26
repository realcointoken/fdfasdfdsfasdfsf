<template>
  <nav class="flex items-center justify-between p-6">
    <!-- Left side -->
    <div class="flex space-x-8">
      <NuxtLink to="/swap" class="text-white font-bold text-xl">Swap</NuxtLink>
      <NuxtLink to="/pools" class="text-white font-bold text-xl"
        >Pools</NuxtLink
      >
    </div>

    <!-- Middle -->
    <div>
      <img src="/symm-logo.svg" alt="logo" class="h-16 w-auto" />
    </div>

    <!-- Right side -->
    <ConnectWallet />
  </nav>
</template>

<script lang="ts" setup>
// Here you can add logic for the Connect Wallet button
</script>
