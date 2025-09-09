<template>
  <teleport v-if="teleport" :to="teleport">
    <slot />
  </teleport>
  <slot v-else />
</template>

<script setup>
/**
 * The Popper Teleport Wrapper component.
 */
defineProps({
    /**
     * Teleport popper element to selector
     */
    teleport: {
        type: String,
        default: null,
    },
});
</script>
