<script></script>

<template>
    <div id="navbar-container">
        <div>
            <img src="/img/dc-logo.png" alt="">
        </div>
        <div>
            <ul>
                <li>Characters</li>
                <li>Comics</li>
                <li>Movies</li>
                <li>tv</li>
                <li>games</li>
                <li>collectibles</li>
                <li>videos</li>
                <li>fans</li>
                <li>news</li>
                <li>shop</li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    #navbar-container {
        display: flex;
        justify-content: space-around;
        align-content: center;
        align-items: center;
        height: 120px;
        background-color: white;
        color: black;

        ul {
            list-style-type: none;
            display: flex;
            gap: 20px;
            text-transform: uppercase;
            font-weight: bold;
        }
    }
</style>