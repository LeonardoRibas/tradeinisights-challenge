<script>
export default {
    props: ["code", "name"],
};
</script>

<template>
    <li class="p-8 rounded-md">
        <p class="font-sans font-bold text-lg mb-2">{{ code }}</p>
        <p class="font-sans text-base text-slate-500">{{ name }}</p>
    </li>
</template>
