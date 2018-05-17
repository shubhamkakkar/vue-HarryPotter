<style>



</style>

<template lang="html">

<div id="trio">
    <div class="display-1 text-center text-info" style="text-decoration: underline;">
        TRIO
    </div>
    <br>
    
    <div class="container">
        <div class="row">
            <div class="col-md-4 m-auto p-4" v-for="(data, index) in castData.name">
                <div class="card border border-0">
                    <div class="card-img m-auto p-4">
                        <img :src="castData.img[index]" :alt="data" style="width : 250px; height: 359px; display : block ; margin : 10% auto">
                    </div>
                    <div class="card-body text-center m-auto p-4">
                        <div class="card-title m-auto p-4">
                            <h3>{{ data }}</h3>
                        </div>
                        <div class="card-text m-auto p-4">
                            <i>
                               <h6>{{ castData.abt[index] }}</h6>
                             </i>
                        </div>
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
                castData: {
                    name: [
                        'Daniel Redclif',
                        'Emma Watson',
                        'Rupert Grint'
                    ],
                    abt: [
                        'The Boy Who Lived, The Chosen One',
                        'The Finest Witch Of Her Age',
                        'The Friend Who Stood By His Side'
                    ],
                    img: [
                        'img/harry.jpg',
                        'img/emma.jpg',
                        'img/ron.jpg'
                    ]
                }
            };
        } //data
} //default

</script>
