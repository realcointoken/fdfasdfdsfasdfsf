<template>
  <div v-if="connected">
    <UButton
      icon="i-heroicons-adjustments-vertical"
      size="xl"
      color="primary"
      variant="outline"
      label="Wallet"
      trailing
    />
  </div>
  <div v-else>
    <UButton size="xl" color="primary" variant="solid" label="Connect Wallet" />
  </div>
</template>

<script lang="ts" setup>
import { dappClient } from "~/utils/walletconnect";
// Here you can add logic for the Connect Wallet button
const connected = dappClient().instance ? true : false;
</script>
