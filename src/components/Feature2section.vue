<script setup>
    import { Icon } from '@iconify/vue';
    const sliderImage = 'https://preview.colorlib.com/theme/launch/images/dashboard.jpg.webp'
    const bgColor = 'background-color: #F8F9FA'
    const margin = 'margin: 150px 0px'

    const features = [

        {
            id:1, 
            icon:'bi:app-indicator', 
            title:'Grow Your Business', 
            content:'Far far away, behind the word mountains, far from the countries Vokalia and Consonantia.',
            bgColor: 'background-color:#6FE7DD'
        },

        {
            id:2, 
            icon:'bi:arrow-repeat', 
            title:'Build Products', 
            content:'Far far away, behind the word mountains, far from the countries Vokalia and Consonantia.',
            bgColor:'background-color:#FFC93C'
        },

        {
            id:3, 
            icon:'ph:briefcase', 
            title:'Success Every Day', 
            content:'Far far away, behind the word mountains, far from the countries Vokalia and Consonantia.',
            bgColor:'background-color:#F73859'
        },

        {
            id:4, 
            icon:'bi:collection', 
            title:'Bring Ideas to Life', 
            content:'Far far away, behind the word mountains, far from the countries Vokalia and Consonantia.',
            bgColor:'background-color:#407BFF'
        }

    ]

</script>
<template>
    <div :style="[bgColor, margin]">
        <div class="container">
            <div class="row d-flex align-items-center">
                <div class="col-lg-5 col-md-7 col-sm-5">
                    <div class="row mt-5" style="cursor: pointer;">
                        <template v-for="feature in features" :key="id">
                            <div class="col-lg-2 col-md-2 col-sm-2">
                                <span :style="feature.bgColor" class="p-3 rounded-4 my-5"><Icon :icon="feature.icon" width="30" height="30" color="white" /></span>
                            </div>
                            <div class="col-lg-10 col-md-10 col-sm-10 list_style">
                                <h3 style="font-weight: 500; font-size: 18px;">{{ feature.title }}</h3>
                                <p style="color: #777;">{{ feature.content }}</p>
                            </div>
                        </template>
                    </div>
                </div>
                <div class="col-lg-7 col-md-5 col-sm-7 my-5">
                    <div class="border border-5">
                        <div id="carouselExampleControls" class="carousel slide" data-bs-ride="carousel">
                            <div class="carousel-inner">
                                <div class="carousel-item active">
                                <img :src="sliderImage" class="d-block w-100" alt="...">
                                </div>
                                <div class="carousel-item">
                                <img :src="sliderImage" class="d-block w-100" alt="...">
                                </div>
                                <div class="carousel-item">
                                <img :src="sliderImage" class="d-block w-100" alt="...">
                                </div>
                            </div>
                            <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="prev">
                                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                                <span class="visually-hidden">Previous</span>
                            </button>
                            <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="next">
                                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                                <span class="visually-hidden">Next</span>
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
    @media (min-width: 299px) and (max-width: 750px) {
        .list_style {
            cursor: pointer; 
            margin-top: 1.5rem; 
            margin-bottom: 3rem;
        } 
    }

    @media (min-width: 800px) and (max-width: 1600px) {
        .list_style {
            cursor: pointer; 
            margin-top: -1rem; 
            margin-bottom: 3rem;
        } 
    }
</style>