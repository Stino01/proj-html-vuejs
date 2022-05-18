<template>
    <div class="type"> 
        <h2>Our consultants can help you</h2>
        <div class="line"></div>
        <div class="info">
            <div class="data" v-for="(item, index) in dati" :key="index">
                <font-awesome-icon :icon="['fas', item.fa]" class="circle"/>
                <div class="consult">
                    <h3>{{item.title}}</h3>
                    <p>{{item.text}}</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import data from "../data.js"

export default {
    name: "ConsultComponent",
    data() {
        return {
            dati: data.datiConsulting,
        }
    }
}
</script>

<style lang="scss" scoped>
    @import "../style/vars.scss";

    .type {
        background-color: $bg-white;

        .line {
                display: inline-block;
                width: 900px;
                height: 3px;
                background-color: $bg-green-ligth;
                border-radius: 2px;
        }

        h2 {
            display: inline-block;
            text-transform: uppercase;
            padding: 4em 2em 2em 12em;
        }

        .info {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            width: 65vw;
            padding: 2em 0;
            margin: 0 auto;

            .data {
                width: 40%;
                padding: 4em 0;
                display: flex;

                .circle {
                    border-radius: 50%;
                    padding: 1em 1em;
                    background-color: $bg-red-ligth;
                }

                .consult {
                    padding: 0 2em;

                    h3 {
                        text-transform: uppercase;
                        font-size: 1.3em;
                    }

                    p {
                        padding: 1em 0;
                        color: $tx-grey-1;
                        font-size: 0.9em;
                    }
                }
            }
        }
    }
</style>