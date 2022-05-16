<template>
    <div class="hero">
        <div class="left"></div>
        <div class="rigth">
            <img src="../assets/img/portrait-of-young-architect-woman-on-meeting-KFZCE3A.jpg" alt="hero">
        </div>
        <div class="message">
            <p>Alwats the best way you need it</p>
            <h1>The best business consulting</h1>
            <span class="button">Read more</span>
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
            background-color: $bg-purple;
        }

        .rigth {
            width: 65vw;

            img {
                width: 100%;
                height: 100%;
            }
        }

        .message {
            width: 40vw;
            position: absolute;
            top: 50%;
            left: 7.5em;
            transform: translateY(-50%);
            text-transform: uppercase;

            p {
                color: $tx-white;
                padding: 1em;
            }

            h1 {
                color: $tx-white;
                font-size: 5em;
                margin-bottom: 2vw;
            }

            .button {
                padding: 1em 3em;
                background-color: $bg-green-ligth;
            }
        }
    }
</style>