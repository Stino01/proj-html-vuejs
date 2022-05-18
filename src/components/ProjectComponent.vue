<template>
    <div class="project">
        <div class="line"></div>
        <h3>Project</h3>
        <div class="arrow">
            <h2>Our expert trusted consultants help clients</h2>
            <div>
                <font-awesome-icon :icon="['fas', 'fa-arrow-left-long']" class="icon"/>
                <font-awesome-icon :icon="['fas', 'fa-arrow-right-long']" class="icon"/>
            </div>
        </div>
        <div class="row">
            <div class="data">
                <img src="../assets/img/DRY-1-790x592.jpg" alt="">
            </div>
            <div class="data">
                <img src="../assets/img/221bf0b7-8134-43bb-936a-5acbe42db64a-790x592.jpg" alt="">
            </div>
            <div class="data">
                <img src="../assets/img/z1el4c4p-790x592.jpg" alt="">
            </div>
        </div>
        <div class="testimonial">
            <h3>Testimonial</h3>
            <div class="line"></div>
            <h2>What's the customer say about our work</h2>
            <div class="started">

            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "ProjectContent",
}
</script>

<style lang="scss" scoped>
    @import "../style/vars.scss";

    .project {
        padding: 15em 7.5em 0 7.5em;
        color: $tx-white;
        text-transform: uppercase;

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
            font-weight: 300;
        }

        h2 {
            width: 60%;
            font-size: 2.5em;
            padding: 0.5em 0 1em 0;
        }

        .arrow {
            display: flex;
            justify-content: space-between;
            align-items: center;

            .icon {
                background-color: $bg-grey;
                padding: 1em;
                margin: 0 2px;
                transition: .5s;
    
                &:hover {
                    background-color: $bg-green-ligth;
                }
            }
        }

        .row {
            display: flex;
            flex-flow: row nowrap;
            justify-content: center;
            gap: 2em;

            .data {
                width: calc(100% / 3);

                img {
                    width: 100%;
                }
            }
        }

        .testimonial {
            display: flex;
            flex-flow: column;
            align-items: flex-end;
            padding-top: 10em;

            .line {
                display: inline-block;
                width: 50px;
                height: 3px;
                background-color: $bg-green-ligth;
                border-radius: 2px;
            }

            h3 {
                display: inline-block;
                align-self: center;
            }

            h2 {
                width: 41%;
                text-align: end;
            }
        }
    }  
</style>