<template>
    <div>
        <div class="about">
            <div class="left">
                <img src="../assets/img/business-people-working-together-on-project-and-5FHSKBL.jpg" alt="about">
            </div>
            <div class="rigth">
                <div class="message">
                    <div class="line"></div>
                    <h3>About Us</h3>
                    <h1>We make your startegy work</h1>
                    <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed by when I hear the buzz of the little world among the stalks, and grow familiar indescribable forms of the insects and flies, then i fell the presence of the Almighty</p>
                </div>
            </div>
        </div>
    </div>

</template>

<script>
export default {
    name: "AboutComponent"
}
</script>

<style lang="scss" scoped>
    @import "../style/vars.scss";

    .about {
        display: flex;

        .left {
            width: 55vw;

            img {
                width: 100%;
            }
        }

        .rigth {
            width: 45vw;
            position: relative;

            .message {
                width: 60%;
                position: absolute;
                top: 50%;
                transform: translateY(-50%);
                left: 3em;

                .line {
                    display: inline-block;
                    width: 50px;
                    height: 3px;
                    background-color: $bg-green-ligth;
                    border-radius: 2px;
                    margin-right: 1em;
                }

                h3 {
                    display: inline-block;
                    color: $tx-white;
                    text-transform: uppercase;
                }

                h1 {
                    color: $tx-white;
                    text-transform: uppercase;
                    padding: 1em 0;
                    font-size: 3em;
                }

                p {
                    color: $tx-grey;
                }
            }
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
        }
    }
</style>