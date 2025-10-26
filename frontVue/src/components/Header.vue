<script>
export default {
    data() {
        return {};
    },
    methods: {
        onClick(page) {
            this.$emit("linkClicked", page);
        },
    },
};
</script>

<template>
    <header>
        <div className="header">
            <div class="headerElementFirst">
                <p>Rostelecom</p>
            </div>
            <div class="headerElement">
                <p class="link">
                    <a href="#" @click.prevent="onClick('Dashboard')">
                        Дашборд
                    </a>
                </p>
            </div>
            <div class="headerElement">
                <p class="link">
                    <a href="#" @click.prevent="onClick('Projects')">
                        Проекты
                    </a>
                </p>
            </div>
            <div class="headerElement">
                <p class="link">
                    <a href="#">Отчёты</a>
                </p>
            </div>
            <div class="headerElementLast">
                <p class="link">
                    <a href="#">Админ-панель</a>
                </p>
            </div>
        </div>
    </header>
</template>

<style scoped>
.header {
    display: grid;
    grid: 1fr / 1fr 1fr 1fr 1fr 1fr;
    border: 1px solid #503d80;
    background-color: #6750a4;
    justify-content: space-around;
    align-items: center;
    border-radius: 7px;
}
.headerElement {
    color: white;
    font-family: "Balsamiq Sans", sans-serif;
    font-size: large;
    border-right: 2px solid #503d80;
    padding: 1px 10px;
    display: flex;
    justify-content: center;
}
.headerElementFirst {
    color: white;
    font-family: "Balsamiq Sans", sans-serif;
    font-size: large;
    border-right: 2px solid #503d80;
    padding: 1px 10px;
    display: flex;
    justify-content: center;
}
.headerElementLast {
    color: white;
    font-family: "Balsamiq Sans", sans-serif;
    font-size: large;
    padding: 1px 10px;
    display: flex;
    justify-content: center;
}
.link a:link,
a:hover,
a:visited,
a:active {
    text-decoration: none;
    color: white;
    cursor: pointer;
}
</style>
