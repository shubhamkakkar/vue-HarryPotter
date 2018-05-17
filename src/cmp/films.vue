<style scoped>
</style>

<template>

<div>
    <div class="container m-auto">
        <div class="display-1 text-center text-info" style="text-decoration: underline;">
            Movies
        </div>
        <br>
        <div class="row ">
            <div class="col-md-3 m-auto p-3" v-for="(cardItem, index) in cardData.cardsList">
                <div class="card mb-5 p-3 border-0">
                    <div class="card-title m-auto p-3 d-block text-center"  style=" background: linear-gradient(#00ddcc, #ece7e3; ">
                        <h4>  {{ cardItem }} </h4>
                    </div>
                    <div class="card-img d-lg-block d-none">
                        <img :src="cardData.imglink[index]" :alt="cardItem" class="img" style="max-width : 100%; max-height:100%;width : 100%; height :400px">
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>

</template>

<script>

export default {
    data() {
        return {
            cardData: {
                cardsList: [
                    "Harry Potter And The Sorcerer's Stone",
                    'Harry Potter And The Chamber Of Secrets',
                    'Harry Potter And The Prizoner Of Azkaban',
                    'Harry Potter And The Goblet Of Fire',
                    'Harry Potter And The Order Of Pheonix',
                    'Harry Potter And The Half Blood Price',
                    'Harry Potter And The Deathly Hollows Part-I',
                    'Harry Potter And The Deathly Hollows Part-II'
                ],

                imglink: [
                    "img/movie/sorcerers_stone_movie.jpg",
                    "img/movie/chambe_of_secrets.jpg",
                    "img/movie/prisoner_of_azkaban_movie.jpeg",
                    "img/movie/The-Goblet-Of-Fire-movie.jpg",
                    "img/movie/order-of-the-phoenix.jpg",
                    "img/movie/the-half-blood-prince-movie.jpg",
                    "img/movie/Deathly_Hallows_1_poster.jpg",
                    "img/movie/Deathly_Hallows_2_poster.jpg"
                ]
            } //cardData
        } //return
    }
}

</script>
