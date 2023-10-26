<template>
    <div class="presentacion">
        <div class="presentacion__video">
            <div class="presentacion__video__info">
                <p class="presentacion__video__info__slogan">
                    <span>Bienvenidos a Colossus Pizza</span> <br>
                    más sobre nosotros:
                </p>
                <p class="presentacion__video__info__texto">
                    Somos una pizzería artesanal que elabora sus productos <br>
                    con ingredientes frescos, orgánicos y de primera calidad, <br>
                    nuestra recetas tanto de masa y salsa cautivará tu <br>
                    paladar al primer bocado. <br>
                    Te invitamos a descubrir todos nuestros increíbles sabores! <br>
                </p>
            </div>

            <video controls muted>
                <source src="../../assets/principal/video.mp4" type="video/mp4">
                Tu navegador no es compatible con videos HTML5
            </video>
        </div>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
    .presentacion{
        display: flex;
        width: 100%;
        justify-content: center;

        

        video{
            height: 400px;
            @include hasta($small){
                height: 250px;
                margin-bottom: 10px;
            }
        }

        
        
        &__video{
            display: flex;
            justify-content: space-between;
            width: 1500px;
            padding: 30px 100px;            
            margin: 10px 0px;

            border-radius: 10px;
            background: rgba( 255, 255, 255, 0.05 );
            box-shadow: 0 8px 32px 0 rgba(242, 86, 29, 0.20);
            backdrop-filter: blur( 3px );
            -webkit-backdrop-filter: blur( 3px );
            border: 1px solid rgba( 255, 255, 255, 0.18 );

            @include hasta($small){
                flex-direction: column;
                width: 365px;
                padding: 0%;
                margin: 5px 0px;
            }

            &__info{
                margin: 50px;
                color: $color1;
                
                @include hasta($small){
                    margin: 15px;
                }


                &__slogan{
                    font-size: 40px;
                    font-family: $ff1;
                    @include hasta($small){
                        font-size: 15px;
                    }
                    span{
                        color: $color3;
                    }
                }

                &__texto{
                    font-size: 17px;
                    font-family: $ff3;
                    @include hasta($small){
                        font-size: 10px;
                    }
                }
            }
        }
    }
</style>