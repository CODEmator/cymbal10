<script setup>
import HeroItem from './HeroItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
</script>

<template>
  <div class="container">
    <HeroItem>
      <template #icon>
        <DocumentationIcon />
      </template>
      <template #heading>About</template>

      Meet Cymbal10
   </HeroItem>

    <HeroItem>
      <template #icon>
        <ToolingIcon />
      </template>
      <template #heading>Highlights</template>

      This is the highlights of cymbal's carier.
    </HeroItem>

    <HeroItem>
      <template #icon>
        <EcosystemIcon />
      </template>
      <template #heading>Origin</template>

      watch video highlights of Cymbal
    </HeroItem>

    <HeroItem>
      <template #icon>
        <CommunityIcon />
      </template>
      <template #heading>shartinga</template>

      Get the official fashion brand by cymbal
    </HeroItem>

    <HeroItem>
      <template #icon>
        <SupportIcon />
      </template>
      <template #heading>Partners</template>

    this are the official partners of cymbal
    </HeroItem>
  </div>
</template>

<style scoped>
  .container {
    display: flex;
    flex-direction: row;
    width: 100%;
    overflow-x: scroll;
  }
</style>
