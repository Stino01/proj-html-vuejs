<template>
    <footer>
        <div class="container">
            <div class="up">
                <img src="../assets\img\logotype-2-139x23.png" alt="logo">
                <ul>
                    <li>Home</li>
                    <li>About</li>
                    <li>Project</li>
                    <li>Service</li>
                    <li>Blog</li>
                    <li>Contact</li>
                </ul>
                <div>
                    <font-awesome-icon :icon="['fab', 'fa-instagram']" class="icon"/>
                    <font-awesome-icon :icon="['fab', 'fa-linkedin-in']" class="icon"/>
                    <font-awesome-icon :icon="['fab', 'fa-facebook']" class="icon"/>
                    <font-awesome-icon :icon="['fab', 'fa-twitter']" class="icon"/>
                </div>
            </div>
            <div class="down">
                <div>
                    <p>Term of use</p>
                    <p>Privacy Environmental Policy</p>
                </div>
                <p>Copyright @ 2020 Phlox Consulting. All Rights Reserved.</p>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: "FooterApp",
}
</script>

<style lang="scss" scoped>
    @import "../style/vars.scss";

    .container {
        width: 85vw;
        margin: 0 auto;

        .up {
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-bottom: 1px solid $tx-grey-1;
            padding: 5em 0;

            ul {
                display: flex;
                list-style-type: none;

                li {
                    text-transform: uppercase;
                    padding: 0 1em;
                    color: $tx-grey-1;

                    &:hover {
                        color: $tx-red;
                    }
                }
            }

            .icon {
                padding: 0 1em;
                color: $tx-white;

                &:hover {
                    color: $tx-red;
                }
            }
        }

        .down {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 2em 0;

            p {
                color: $tx-grey-1;
            }
        }
    }
</style>