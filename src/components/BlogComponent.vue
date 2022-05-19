<template>
    <div class="blog">
        <div class="line"></div>
        <h3>Blog</h3>
        <div class="tx">
            <h2>The recent news you must read it</h2>
            <span>View all</span>
        </div>
        <div class="info">
            <div class="holder uno">
                <img src="../assets\img\startup-business-people-and-strategy-board-PAJ3P9K-1390x1042.jpg" alt="">
                <div class="message">
                    <span>july 4, 2019</span>
                    <h2>Canadian Consulting Firm acquired by UK Giant</h2>
                    <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a ...</p>
                </div>
            </div>
            <div class="holder due">
                <img src="../assets\img\business-people-working-together-on-project-and-5FHSKBL-1390.jpg" alt="">
                <div class="message">
                    <span>july 4, 2019</span>
                    <h2>Canadian Consulting Firm acquired by UK Giant</h2>
                    <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a ...</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "BlogComponent"
}
</script>

<style lang="scss" scoped>
    @import "../style/vars.scss";

    .blog {
        padding: 15em 7.5em;
        color: $tx-white;

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
            text-transform: uppercase;
        }

        .tx {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1em 0;
            text-transform: uppercase;

            h2 {
                width: 60%;
                font-size: 2.5em;
            }

            span {
                padding: 1em 3em;
                color: $tx-black;
                background-color: $bg-green;
                transition: .5s;

                &:hover {
                    box-shadow: inset 0 0 0 2em $bg-red-ligth;
                }
            }
        }

        .info {
            display: flex;
            justify-content: center;
            gap: 2em;
            padding-top: 3em;

            .holder {
                width: 50%;
                position: relative;

                img {
                    width: 100%;
                }

                .message {
                    width: 80%;
                    background-color: $bg-white;
                    padding: 3em 8em 3em 5em;
                    position: absolute;
                    right: 0;
                    bottom: -6em;
                    transition: 0.5s;

                    span {
                        color: $tx-red;
                    }

                    h2 {
                        color: $tx-black;
                        font-weight: 600;
                        padding: 1em 0;
                    }

                    p {
                        color: $tx-grey;
                    }
                }
            }
        }    
        
        .uno {
            &:hover .message {
                background-color: $bg-green-ligth;
                bottom: -7em;
            }
        }

        .due {
            &:hover .message {
                background-color: $bg-green-ligth;
                bottom: -7em;
            }
        }
    }
</style>