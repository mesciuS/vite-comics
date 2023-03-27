<script>
import AppProps from "./AppProps.vue";
export default {
    data() {
        return {
            comics: [
                {
                    thumb: "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    price: "$19.99",
                    series: "Action Comics",
                    type: "comic book"
                },
                {
                    thumb: "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    price: "$3.99",
                    series: "American Vampire 1976",
                    type: "comic book"
                },
                {
                    thumb: "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    price: "$16.99",
                    series: "Aquaman",
                    type: "graphic novel"
                },
                {
                    thumb: "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    price: "$2.99",
                    series: "Batgirl",
                    type: "comic book"
                },
                {
                    thumb: "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    price: "$3.99",
                    series: "Batman",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    price: "$2.99",
                    series: "Batman Beyond",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    price: "$3.99",
                    series: "Batman/Superman",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    price: "$4.99",
                    series: "Batman/Superman Annual",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    price: "$5.99",
                    series: "Batman: The Joker War Zone",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    price: "$6.99",
                    series: "Batman: Three Jokers",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    price: "$4.99",
                    series: "Batman: White Knight Presents: Harley Quinn",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    price: "$16.99",
                    series: "Catwoman",
                    type: "graphic novel"
                }
            ]
        };
    },

    components: {
        AppProps,
    }
};
</script>

<template>
    <div id="main">
        <div id="jumbotron">
            <img src="/img/jumbotron.jpg" alt="">
            <div class="current-series">current series</div>
        </div>
        <div id="card-container">
            <AppProps v-for="comic in comics" :img="comic.thumb" :serie="comic.series"></AppProps>
        </div>
        <div id="btn-container">
            <button>LOAD MORE</button>
        </div>
    </div>
</template>

<style lang="scss" scoped>
#main {
    height: 1000px;
    padding-bottom: 20px;
    
    #jumbotron {
        position: relative;
        height: 300px;
        img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            text-align: center;
        }
        .current-series {
            position: absolute;
            left: 330px;
            top: 280px;
            width: 220px;
            height: 40px;
            text-align: center;
            line-height: 40px;
            text-transform: uppercase;
            font-size: 1.3em;
            font-weight: bold;
            background-color: #0282f9;
        }
    }
    
    #card-container {
        display: flex;
        flex-flow: row wrap;
        justify-content: center;
        padding-top: 30px;
        padding-bottom: 30px;
        padding-left: 300px;
        padding-right: 300px;
        
        gap: 30px;
    }

    #btn-container {
        display: flex;
        justify-content: center;
        padding-bottom: 10px;

        button {
            width: 150px;
            height: 30px;
            border: none;
            background-color: #0282f9;

        }
    }

}
</style>