<style scoped>
</style>

<template>

<div>
    <div class="container m-auto">
        <div class="display-1 text-center text-info" style="text-decoration: underline;">
            Books
        </div>
        <br>
        <div class="row ">
            <div class="col-md-3 m-auto p-auto" v-for="(cardItem, index) in cardData.cardsList" style="cursor : pointer">
                <div class="card border-0 mb-5 p-auto" >
                    <div class="card-title m-auto p-auto d-block text-center border border-0" style=" background: linear-gradient(#00ddcc, #ece7e3; ">
                        <h4>  {{ cardItem }} </h4>
                    </div>
                    <div class="card-img d-lg-block d-none m-auto p-auto">
                        <img :src="cardData.imgLink[index]" :alt="cardItem" class="img" style="max-width : 100%; max-height:100% ;width : 100%; height :400px">
                        <!--only to the one-->
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
                        'Harry Potter And The Deathly Hollows',
                        'Harry Potter And The Cursed Child'
                    ], //cardsList
                    imgLink: [
                        "img/books/sorcerers_stone.jpg",
                        "img/books/chamber_of_secrets_book.jpg ",
                        "img/books/the-goblet-of-fire.jpg ",
                        "img/books/prisoner_of_azkaban.jpeg ",
                        "img/books/order-of-the-phoenix-book.jpg ",
                        "img/books/half-blood0prince-book.jpg ",
                        "img/books/deathly-hollows.jpg ",
                        "img/books/cursed-child.jpg "
                    ]
                }
            }; //return
        }
} //default

</script>
