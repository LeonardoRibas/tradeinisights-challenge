<template>
    <ul class="grid grid-cols-1 lg:grid-cols-2 gap-4 place-content-center p-16">
        <Item
            v-for="item in list"
            :key="item.id"
            :code="item.code"
            :name="item.name"
        />
    </ul>
</template>

<script>
import Item from "./components/Item.vue";
import axios from "axios";
export default {
    name: "App",

    components: {
        Item,
    },

    data() {
        return {
            list: [],
        };
    },

    async mounted() {
        let result = await axios.get("http://127.0.0.1:8000/api");
        this.list = result.data;
    },
};
</script>
