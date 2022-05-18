<template>
    <div class="hero">
        <div class="left"></div>
        <div class="rigth">
            <img src="../assets/img/portrait-of-young-architect-woman-on-meeting-KFZCE3A.jpg" alt="hero">
        </div>
        <div class="message">
            <div class="line"></div>
            <p>Alwats the best way you need it</p>
            <h1>The best business consulting</h1>
            <span class="button">Read more</span>
            <font-awesome-icon :icon="['far', 'fa-circle-play']" class="play"/>
        </div>
    </div>
</template>

<script>
export default {
    name: "HeroComponent",
}
</script>

<style lang="scss" scoped>
    @import "../style/vars.scss";

    .hero {
        width: 100%;
        height: 100vh;
        display: flex;
        position: relative;

        .left {
            width: 35vw;
        }

        .rigth {
            width: 65vw;

            img {
                width: 100%;
                height: 100vh;
            }
        }

        .message {
            width: 40vw;
            position: absolute;
            top: 50%;
            left: 7.5em;
            transform: translateY(-50%);
            text-transform: uppercase;

            .line {
                display: inline-block;
                width: 40px;
                height: 3px;
                background-color: $bg-green-ligth;
                border-radius: 2px;
            }

            p {
                display: inline-block;
                color: $tx-white;
                padding: 1em;
            }

            h1 {
                color: $tx-white;
                font-size: 6em;
                margin-bottom: 2vw;
            }

            .button {
                padding: 1em 3em;
                background-color: $bg-green-ligth;
                transition: .5s;
                
                &:hover {
                    box-shadow: inset 0 0 0 2em $bg-red-ligth;
                }
            }

            .play {
                width: 50px;
                height: 50px;
                position: relative;
                left: 2em;
                top: 20px;
                color: white;
            }
        }
    }
</style>