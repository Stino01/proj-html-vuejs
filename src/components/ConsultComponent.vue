<template>
    <div class="type">
        <h2>Our consultants can help you</h2>
        <div class="info">
            <div class="data">
                <div class="circle"></div>
                <div class="consult">
                    <h3>Statistical Consulting</h3>
                    <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a</p>
                </div>
            </div>
            <div class="data">
                <div class="circle"></div>
                <div class="consult">
                    <h3>Digital Consulting</h3>
                    <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a</p>
                </div>
            </div>
            <div class="data">
                <div class="circle"></div>
                <div class="consult">
                    <h3>Banking Consulting</h3>
                    <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a</p>
                </div>
            </div>
            <div class="data">
                <div class="circle"></div>
                <div class="consult">
                    <h3>Enterprice Consulting</h3>
                    <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>

export default {
    name: "ConsultComponent",
}
</script>

<style lang="scss" scoped>
    @import "../style/vars.scss";

    .type {
        background-color: $bg-white;

        h2 {
            text-transform: uppercase;
            padding-left: 12em;
            padding-top: 4em;
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
                    width: 150px;
                    height: 50px;
                    border-radius: 50%;
                    background-color: red;
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