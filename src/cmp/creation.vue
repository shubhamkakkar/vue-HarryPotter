<style scoped>



</style>

<template>

<div id="creations">

    <div class="container">
        <div class="row     ">
            <div class="col-md-4 text-center m-auto " v-for=" (creation, index) in creations ">
                <i class="fa fa-bolt fa-rotate-90" style="font-size:3em ; vertical-align : center"></i>
                <a href="#" @click="target(index)">
                    <strong class="display-4 font-weight-bold"> {{ creation }} </strong>
                </a>
                <i class="fa fa-bolt fa-rotate-90" style="font-size:3em; vertical-align : center"></i>
            </div>
        </div>
    </div>

    <app-Books></app-Books>
    <br>
    <app-Films></app-Films>


</div>

</template>

<script>

 import books from "./books.vue";
 import films from "./films.vue";

export default {
    data() {
            return {
                creations: {
                    0: 'Books',
                    1: 'Creation',
                    2: 'Films'
                }
            }
        },
        methods: {
            target(index) {
                // $('a').attr("href", index)
                if (index == 0) {
                    console.log(index);
                    $('a').attr('href', '#books');
                } else if (index == 2) {
                    console.log(index);
                    $('a').attr('href', '#films');
                }
            }
        },
        components:{
            appFilms : films,
            appBooks : books
        }

}

</script>
