<script>
import Header from "@/components/Header.vue";
import Dashboard from "@/pages/Dashboard.vue";
import Projects from "@/pages/Projects.vue";
export default {
    components: {
        Dashboard,
        Header,
        Projects,
    },
    data() {
        return {
            page: "Dashboard",
        };
    },
    methods: {
        updateMessage(value) {
            this.page = value;
        },
    },
};
</script>

<template>
    <Header @linkClicked="updateMessage" />
    <component :is="page" />
</template>

<style scoped></style>
