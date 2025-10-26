<script>
export default {
    data() {
        return {
            countProj: 4,
            countMoney: 16000000,
        };
    },
};
</script>

<template>
    <article>
        <br />
        <div class="gridConteiner">
            <div class="gridConteiner-first">
                <div class="aboutStat">
                    <p>
                        Общее количество проектов:<br />
                        <span class="orangeText">{{ countProj }}</span> <br />
                        Выручка проектов: <br />
                        <span class="orangeText">{{ countMoney }}</span>
                    </p>
                </div>
                <div class="stadyProj">
                    <p>Стадии проектов:</p>
                </div>
                <div class="averageTime">
                    <p>Среднее время нахождения на этапе:</p>
                </div>
            </div>
            <div class="gridConteiner-second">
                <div class="statManager">
                    <p>Статистика по менеджерам:</p>
                </div>
                <div class="statTime">
                    <p>Статистика по нахождению на этапе:</p>
                </div>
                <div class="moneyFuture">
                    <p>Выручка с учётом вероятности:</p>
                </div>
            </div>
        </div>
    </article>
</template>

<style scoped>
.backColor {
    background-color: #e3e3e3;
}
.gridConteiner {
    display: grid;
    grid: 1fr / 1fr 1fr;
    grid-column-gap: 10px;
    grid-row-gap: 10px;
    font-family: "Balsamiq Sans", sans-serif;
    color: #6750a4;
}
.gridConteiner-first {
    display: grid;
    grid: 1fr 1fr / 1fr 1fr 1fr;
    grid-column-gap: 10px;
    grid-row-gap: 10px;
}
.gridConteiner-second {
    display: grid;
    grid: 1fr 1fr / 1fr 1fr;
    grid-column-gap: 10px;
    grid-row-gap: 10px;
}
.aboutStat {
    grid-row: 1;
    grid-column: 1;
    border: 2px solid #c7c7c7;
    border-radius: 15px;
    padding: 1px 10px;
}
.stadyProj {
    grid-row: 1;
    grid-column: 2/4;
    border: 2px solid #c7c7c7;
    border-radius: 15px;
    padding: 1px 10px;
}
.averageTime {
    grid-row: 2;
    grid-column: 1/4;
    border: 2px solid #c7c7c7;
    border-radius: 15px;
    padding: 1px 10px;
}
.statManager {
    grid-row: 1;
    grid-column: 1;
    border: 2px solid #c7c7c7;
    border-radius: 15px;
    padding: 1px 10px;
}
.statTime {
    grid-row: 1;
    grid-column: 2;
    border: 2px solid #c7c7c7;
    border-radius: 15px;
    padding: 1px 10px;
}
.moneyFuture {
    grid-row: 2;
    grid-column: 1/3;
    border: 2px solid #c7c7c7;
    border-radius: 15px;
    padding: 1px 10px;
}
.orangeText {
    color: #d7751f;
}
</style>
