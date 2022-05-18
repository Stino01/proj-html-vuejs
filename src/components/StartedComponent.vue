<template>
    <div class="getstarted">
        <img src="../assets\img\business-people-working-together-on-project-and-B3MZ4TX.jpg" alt="">
        <div class="text">
            <h1>Let's talk about work</h1>
            <p>A wonderful serenity has taken possession far far away, behind the word mountains.</p>
            <span>Get started</span>
        </div>
    </div>
</template>

<script>
export default {
    name: "StartedComponent",
}
</script>

<style lang="scss" scoped>
    @import "../style/vars.scss";

    .getstarted {
        position: relative;

        img {
            width: 100%;
        }

        .text {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            text-align: center;
            width: 30%;

            h1 {
                color: $tx-white;
                text-transform: uppercase;
                font-size: 2em;
            }

            p {
                color: $tx-grey;
                width: 80%;
                margin: 0 auto;
                padding: 1em 0 2em 0;
            }

            span {
                padding: 1em 3em;
                background-color: $bg-purple;
                color: $tx-white;
                text-transform: uppercase;
                transition: 0.5s;

                &:hover {
                    box-shadow: inset 0 0 0 2em $bg-green-ligth;
                }
            }
        }
    }
</style>