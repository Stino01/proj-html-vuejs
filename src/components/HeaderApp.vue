<template>
    <header>
        <img src="../assets/img/logotype.png" alt="logo">
        <nav>
            <ul>
                <li class="active">Home</li>
                <li>About</li>
                <li>Projectli</li>
                <li>Service</li>
                <li>Blog</li>
                <li>Contact</li>
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

            .active {
                color: white;
                border-top: 2px solid white;
            }

            li {
                padding: 1.5em 0;
                margin: 0 1em;
                color: $tx-grey;
                text-transform: uppercase;
                cursor: pointer;
            }
        }
    }
</style>