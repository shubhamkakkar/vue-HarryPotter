

<template>

<div>
    <nav class="navbar navbar-expand-md navbar-dark fixed-top" style="opacity:0.9; background-color :#334aa9">
        <div class="container">
            <div class="row">
                <div class="col-md-6">
                    <a href="index.html" class="navbar-brand">Harry Potter</a>
                    <img src="img/prophecy.jpg" alt="logo" style="width: 12vw;border-radius: 25px;">
                    <button class="navbar-toggler" data-toggle="collapse" data-target="#navbarNav">
                        <span class="navbar-toggler-icon"></span>
                    </button>
                </div>
                <div class="col-md-6 ml-auto px-5">
                    <div class="collapse navbar-collapse" id="navbarNav">
                        <ul class="navbar-nav" v-for="(tabLink, index) in tablinks">
                            <li class="nav-item mx-3 px-1">
                                <a href="#" class="nav-link hrefSet text-white" @click="hrefSet(index)">
                                    {{ tabLink }}
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </nav>
</div>

</template>

<script>

export default {
    data() {
            return {
                tablinks: ['Home', 'Author', 'Creations', 'The Golden Trio', 'Contact']
            };
        },//data
        methods: {
            hrefSet(index) {
                // useing index paramter of the tablink to pass in the value from href attr
                // console.log("should somehow return the index as per tablinks");
                var attr;
                if (index == 0) {
                    attr = "#home";
                } else if (index == 1) {
                    attr = "#author";
                } else if (index == 2) {
                    attr = "#creations";
                } else if (index == 3) {
                    attr = "#trio";
                } else {
                    attr = "#contact";
                }
                $(".hrefSet").attr("href", attr);
                console.log(index, attr);
            }//hrefSet
        }//methods
}//default

</script>
