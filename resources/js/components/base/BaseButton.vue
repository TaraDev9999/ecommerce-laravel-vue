<template>
    <button
        :type="type"
        class="px-6 py-2 font-semibold text-white rounded-md hover:opacity-90 transition-all duration-500 ease-in-out focus:outline-none"
        :class="props.backgroundColor"
    >
        <slot></slot>
    </button>
</template>

<script setup>
const props = defineProps({
    type: String,
    backgroundColor: String,
});
</script>
