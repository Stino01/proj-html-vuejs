<template>
    <main>
        <hero-component/>
        <consult-component/>
        <about-component/>
        <div class="started">
            <h2>We help to deliver the business case</h2>
            <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown</p>
            <span>Get started</span>
        </div>
        <project-component/>
        <div class="started rigth">
            <div class="data" v-for="(item, index) in dati" :key="index">
                <p>{{item.text}}</p>
                <h3>{{item.name}}</h3>
                <p>{{item.agency}}</p>
            </div>
        </div>
        <blog-component/>
        <started-component/>
        <div class="goup" @click="goUp">
            <font-awesome-icon :icon="['fas', 'fa-arrow-up']" class=""/>
        </div>
    </main>
</template>

<script>
import data from "../data.js"
import HeroComponent from "./HeroComponent.vue"
import ConsultComponent from "./ConsultComponent.vue"
import AboutComponent from "./AboutComponents.vue"
import ProjectComponent from './ProjectComponent.vue'
import BlogComponent from './BlogComponent.vue'
import StartedComponent from './StartedComponent.vue'

export default {
    name: "MainApp",
    components: {
        HeroComponent,
        ConsultComponent,
        AboutComponent,
        ProjectComponent,
        BlogComponent,
        StartedComponent,
    },
    data() {
        return {
            dati: data.datiTestimonial,
        }
    },
    methods: {
        goUp: function() {
            window.scrollTo({
                top: 0,
                behavior: "smooth",
            })
        }
    }
}
</script>

<style lang="scss" scoped>
    @import "../style/vars.scss";
    main {
        position: relative;

        .goup {
            position: fixed;
            bottom: 3em;
            right: 5em;
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background-color: $bg-white;
            display: flex;
            justify-content: center;
            align-items: center;
            cursor: pointer;
            border: 1px solid black;
        }
    }
    .started {
        display: flex;
        width: 90vw;
        background-color: $bg-green-ligth;
        justify-content: space-between;
        align-items: center;
        padding: 6em 18em;
        position: relative;

        h2 {
            width: 30%;
            font-size: 1.5em;
            text-transform: uppercase;
        }

        p {
            width: 45%;
        }

        span {
            position: absolute;
            bottom: 0;
            right: 0;
            color: $tx-white;
            background-color: $bg-red-ligth;
            text-transform: uppercase;
            padding: 1em 2.5em;
            transition: .5s;
    
            &:hover {
                box-shadow: inset 0 0 0 2em $bg-purple;
            }
        }
    }

    .rigth {
        background-color: $bg-white;
        justify-content: center;
        margin-left: 9.1vw;
        padding: 0 7.5em 0 0;

        .data {
            width: calc(100% / 3);
            padding: 3em 5em;

            p {
                color: $tx-grey;
                width: 100%;
            }

            h3 {
                padding-top: 3em;
            }
        }
    }
</style>