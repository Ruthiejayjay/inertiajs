<template>
  <Link
    class="text-black hover:underline"
    :class="{ 'font-bold underline': active }"
  >
    <slot />
  </Link>
</template>
<script setup>
import { Link } from "@inertiajs/inertia-vue3";
defineProps({
    active: Boolean
})
</script>
