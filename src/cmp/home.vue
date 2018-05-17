<style scoped>
    img {
        margin: 0;
        width: 100%;
        max-height: 500px;
        background-size: cover;
        opacity: 0.9;
    }
    
    .card-title {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
    }
</style>

<template>
    <div id="home" class="w-100 mb-auto ">
        <div class="card" style="width : 100%; margin : 0; padding : 0">
            <div class="card-body  d-lg-block d-none">
                <div id="slider2" class="carousel slide" data-ride="carousel">
                    <div class="carousel-inner" role="listbox">
                        <div class="carousel-item" id="gal" v-for="(img, index) in imglink">
                            <img class="d-block img-fluid" :src="imglink[index]" alt="Slide">
                        </div>
                    </div>
                    <a href="#slider2" class="carousel-control-prev" data-slide="prev">
                        <span class="carousel-control-prev-icon"></span>
                    </a>
    
                    <a href="#slider2" class="carousel-control-next" data-slide="next">
                        <span class="carousel-control-next-icon"></span>
                    </a>
                </div>
                <div class="card-title text-muted display-4 font-weight-bold">
                    Help is always given at <span>Hogwarts</span> to those who seek it
                </div>
            </div>
            <div class="card-header text-muted display-4 font-weight-bold  d-lg-none ">
                    Help is always given at <span>Hogwarts</span> to those who seek it
                </div>
        </div>
    </div>
    <!-- wrapping  -->
</template>

<script>
    export default {
        data() {
            return {
                home_overlay: {
                    text: 'Help is always given a hogwarts to those who need it'
                },
                imglink: [
                    'img/slider/1.jpg',
                    'img/slider/2.jpg',
                    'img/slider/3.jpg',
                    'img/slider/4.jpg',
                    'img/slider/5.jpg',
                    'img/slider/6.jpg',
                    'img/slider/7.jpg'
                ]
            };
        }, //data
        filters: {
            upperCase(value) {
                return value.toUpperCase();
            }
        }, // filters
        mounted: function() {
            console.log('mounted');
            let counter = 0;
            if (!counter) {
                $("#gal").addClass('active');
    
            }
        }
    } //export
</script>
