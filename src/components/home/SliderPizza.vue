<template>    
    <div class="contenedorSlider d-flex justify-content-center align-items-center">
        <div id="carouselExampleIndicators" class="carousel slide" data-bs-ride="carousel">
            <div class="carousel-indicators">
                <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
                <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1" aria-label="Slide 2"></button>
                <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2" aria-label="Slide 3"></button>
        </div>
        <div class="carousel-inner">
            <div class="carousel-item active">
            <img src="../../assets/banner1.png" class="d-block w-100" alt="...">
            </div>
            <div class="carousel-item">
            <img src="../../assets/banner2.png" class="d-block w-100" alt="...">
            </div>
            <div class="carousel-item">
            <img src="../../assets/banner3.png" class="d-block w-100" alt="...">
        </div>
        </div>
            <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="prev">
                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                <span class="visually-hidden">Previous</span>
            </button>
            <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next">
                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                <span class="visually-hidden">Next</span>
            </button>
        </div>
    </div>
</template>

<script>
    import 'bootstrap/dist/css/bootstrap.css';
    import 'bootstrap/dist/js/bootstrap.js';
    export default {
        name: 'SliderPizza'
    }
</script>

<style lang="scss">
    .contenedorSlider{
        background: $color5;
    }
    .carousel{
        width: 365px;
        margin-top: 10px;
        margin-bottom: 5px;


        
        background: rgba( 255, 255, 255, 0.05 );
        box-shadow: 0 8px 32px 0 rgba(242, 86, 29, 0.20);
        backdrop-filter: blur( 3px );
        -webkit-backdrop-filter: blur( 3px );
        border-radius: 10px;
        border: 1px solid rgba( 255, 255, 255, 0.18 );

        @include desde($small){
            width: 1500px;
            margin-top: 165px;
            margin-bottom: 10px;
        }

        @include desde($medium){
            width: 1500px;
            margin-top: 165px;
            margin-bottom: 10px;
        }
        

        
        
    }
    .carousel-indicators{
        @include hasta($small){
            display: none;
        }
    }
    .carousel-inner{
        border-radius: 10px;
    }
 
</style>