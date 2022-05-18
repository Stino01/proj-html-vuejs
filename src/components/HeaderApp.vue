<template>
    <header>
        <img src="../assets/img/logotype.png" alt="logo">
        <nav>
            <ul>
                <li v-for="(item, index) in info" :key="index" :class="{'active': index === currentIndex}" @click="item.active ? dropdown(index) : null">
                    <a href="#">{{item.text}}</a>
                    <font-awesome-icon :icon="['fas', 'fa-chevron-down']" v-if="item.active" class="icon"/>
                    <div class="dropdown-menu" v-if="toggle && item.active">
                        <p v-for="el in item.dropdown" :key="el.id">{{el.title}}</p>
                    </div>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
import data from "../data.js"

export default {
    name: "HeaderApp",
    data() {
        return {
            info: data.datiHeader,
            currentIndex: 0,
            toggle: false,
            active: false,
        }
    },
    methods: {
        dropdown: function(i){
            this.currentIndex = i
            this.toggle = !this.toggle

            return this.currentIndex            
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/vars.scss";

    header {
        display: flex;
        justify-content: space-between;
        width: 85vw;
        margin: 0 auto;
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        z-index: 1000;

        img {
            width: 7em;
            padding: 1.5em 0;
        }

        ul {
            display: flex;
            list-style-type: none;

            .active {
                color: white;
                border-top: 2px solid white;
                padding: 23px 0;

            }

            li {
                padding: 25px 0;
                margin: 0 1em;
                text-transform: uppercase;
                cursor: pointer;
                transition: .2s;
                position: relative;

                &:hover {
                    border-top: 2px solid white;
                    padding: 23px 0;
                }

                a {
                    text-decoration: none;
                    color: $tx-grey;
                }

                .icon {
                    color: $tx-grey;
                    padding-left: 5px;
                }

                .dropdown-menu {
                    position: absolute;
                    top: 3em;
                    right: 50%;
                    transform: translateX(+50%);
                    background-color: white;
                    border-radius: 10px;
                    width: 10em;

                    p {
                        z-index: 1100;
                        text-transform: none;
                        text-align: center;
                        font-size: 1em;
                        border-bottom: 1px solid $tx-grey;
                        padding: 1em 0;
                        margin: 0 1em;
                    }
                }
            }
        }
    }
</style>