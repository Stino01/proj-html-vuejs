<template>
    <header>
        <img src="../assets/img/logotype.png" alt="logo">
        <nav>
            <ul>
                <li class="active"><a href="#">Home</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Project</a></li>
                <li><a href="#">Service</a></li>
                <li><a href="#">Blog</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    name: "HeaderApp",
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

            li {
                padding: 1.5em 1em;

                a {
                    text-decoration: none;
                    color: $tx-grey;
                    text-transform: uppercase;
                }
            }
        }
    }

    .active {
        color: $tx-white;
        border-top: 2px solid $border-white;
    }
</style>