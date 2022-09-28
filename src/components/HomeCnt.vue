<script setup lang="ts">
import HomeItem from './HomeItem.vue'

import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'

import HeartIcon from './icons/IconHeart.vue'
</script>

<template>
  <HomeItem>
    <template #icon>
      <HeartIcon />
    </template>
    <template #heading>Intro</template>
      111
  </HomeItem>

  <HomeItem>
    <template #icon>
      <ToolingIcon />
    </template>
    <template #heading>Tooling</template>
      222
  </HomeItem>

  <HomeItem>
    <template #icon>
      <EcosystemIcon />
    </template>
    <template #heading>Ecosystem</template>
      333
  </HomeItem>
</template>
