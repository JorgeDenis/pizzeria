<template>
    <div class="footer">
        <div class="footer__container">
            <div class="footer__container__iconos">
                <div class="footer__container__iconos__pago">
                    <img src="../../assets/footer/metodo-de-pago.png" alt="" class="">
                    <div class="footer__container__iconos__pago__texto">
                        <h3 class="footer__container__iconos__pago__texto__titulo">Pago en línea</h3>
                        <p class="footer__container__iconos__pago__texto__desc">Pagos con tarjeta de crédito y QR</p>
                    </div>
                </div>
                <div class="footer__container__iconos__delivery">
                    <img src="../../assets/footer/moto.png" alt="">
                    <div class="footer__container__iconos__delivery__texto">
                        <h3 class="footer__container__iconos__delivery__texto__titulo">Entregas</h3>
                        <p class="footer__container__iconos__delivery__texto__desc">Pagos con tarjeta de crédito y QR</p>
                    </div>
                </div>
                <div class="footer__container__iconos__compra">
                    <img src="../../assets/footer/candado.png" alt="">
                    <div class="footer__container__iconos__compra__texto">
                        <h3 class="footer__container__iconos__compra__texto__titulo">Compra Segura</h3>
                        <p class="footer__container__iconos__compra__texto__desc">Pagos con tarjeta de crédito y QR</p>
                    </div>
                </div>
            </div>
            <div class="footer__container__info">
                <div class="footer__container__info__contacto">
                    <div class="footer__container__info__contacto__titulo">
                        <p><span>Contacto</span></p>
                    </div>
                    <div class="footer__container__info__contacto__email">
                        <p><span>Email: </span>colossuspizza@gmail.com</p>
                    </div>
                    <div class="footer__container__info__contacto__telefonos">
                        <p>
                            <span>Santa Cruz: </span><br>
                            <span>Roca y coronado: </span>+59177660088 <br>
                            <span>Virgen de Lujan: </span>+5916900275 <br>
                        </p>
                    </div>
    
                </div>
                <div class="footer__container__info__acerca">
                    <div class="footer__container__info__acerca__titulo">
                        <p><span>Acerca de Colossus Pizza</span></p>
                    </div>
                    <a href="#" class="footer__container__info__acerca__link">Nuestro menú</a> <br>
                    <a href="#" class="footer__container__info__acerca__link">Nuestra marca</a> <br>
                    <!-- <a href="#" class="footer__container__info__acerca__link">Nuestra salsa de Ajo</a> <br> -->
                    <!-- <a href="#" class="footer__container__info__acerca__link">Colosus Pizza internacional</a> <br> -->
                    <a href="#" class="footer__container__info__acerca__link">Sostenibilidad</a> <br>
                    <a href="#" class="footer__container__info__acerca__link">Comunicado gallinas libres</a> <br>
                    <a href="#" class="footer__container__info__acerca__link">Súmate a ECO</a> <br>
                </div>
    
    
                <div class="footer__container__info__servicio">
                    <div class="footer__container__info__servicio__titulo">
                        <p><span>Servicio al cliente</span></p>
                        <a href="#" class="footer__container__info__acerca__link">Preguntas frecuentes</a> <br>
                        <a href="#" class="footer__container__info__acerca__link">Soporte vía Whatsapp</a> <br>
                        <a href="#" class="footer__container__info__acerca__link">Trabaja con nosotros</a> <br>
                    </div>
                </div>
    
    
                <div class="Legal">
                    <div class="footer__container__info__legal__titulo">
                        <p><span>Legal</span></p>
                        <a href="#" class="footer__container__info__acerca__link">Términos y condiciones</a> <br>
                        <a href="#" class="footer__container__info__acerca__link">Política de Tratamiento de Datos</a> <br>
                        <a href="#" class="footer__container__info__acerca__link">T&C Promociones</a> <br>
                        <a href="#" class="footer__container__info__acerca__link">Cookies</a> <br>
                        <a href="#" class="footer__container__info__acerca__link">www.sic.gov.bo</a> <br>
                    </div>
                </div>
            </div>

            <div class="footer__container__copy">
                <div class="footer__container__copy__imagenes">
                    <img src="../../assets/footer/1.webp" alt="" class="footer__container__copy__imagenes__img1">
                    <img src="../../assets/footer/2.webp" alt="" class="footer__container__copy__imagenes__img2">
                </div>
                <div class="footer__container__copy__parrafo">
                    <p>
                        Promociones disponibles por tiempo limitado en los restaurantes de Colossus Pizza. Sujeto a disponibilidad y cobertura del punto de venta. No acumulable con otras promociones. Fotos de referencia publicitaria. No incluye el valor del domicilio.

                        Declaración de Alérgenos Querido invitado, lo invitamos a que tenga en cuenta que en nuestras cocinas se manejan ingredientes que contienen: harina de trigo (gluten), trazas de soya, lácteos, huevo, maní, nueces, entre otros, que pueden producir alergia.

                        ©2023 Colosus Pizza. Todos los derechos reservados

                    </p>
                </div>
            </div>
        </div>

    </div>

</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
    .footer{
        display: flex;
        width: 100%;
        background: $color5;
        justify-content: center;
        padding-top: 10px;

        
        
        &__container{
            border-radius: 10px;
            background: rgba( 255, 255, 255, 0.05 );
            box-shadow: 0 8px 32px 0 rgba(242, 86, 29, 0.20);
            backdrop-filter: blur( 3px );
            -webkit-backdrop-filter: blur( 3px );
            border: 1px solid rgba( 255, 255, 255, 0.18 );
            margin-bottom: 20px;
            @include hasta($small){
                width: 365px;
            }
            &__iconos{
                border-top-left-radius: 10px;
                border-top-right-radius: 10px;
                display: flex;
                justify-content: space-between;
                padding: 20px  150px 0px 150px;
                width: 1500px;
                background: $color1;

                @include hasta($small){
                    width: 365px;
                    padding: 10px;
                }

                img{
                    width: 50px;
                    height: 50px;
                    margin-right: 10px;
                 
                    @include hasta($small){
                        width: 30px;
                        height: 30px;   
                    }
                }
                &__pago{
                    display: flex;
                    align-items: center;
                    width: 250px;

                    @include hasta($small){
                        width: 100px;
                    }

                    &__texto{
                        &__titulo{
                            font-size: 20px;
                            margin: 0px;
                            font-weight: bold;
                            color: $color2;
                            font-family: $ff2;

                            @include hasta($small){
                                font-size: 15px;
                            }
                        }
                        &__desc{
                            font-size: 15px;
                            @include hasta($small){
                                font-size: 10px;
                            }
                        }
                    }
                }
                &__delivery{
                    display: flex;
                    align-items: center;
                    width: 250px;

                    @include hasta($small){
                        width: 100px;
                    }
                    &__texto{
                        &__titulo{
                            margin: 0px;
                            font-size: 20px;
                            font-weight: bold;
                            color: $color2;
                            font-family: $ff2;

                            @include hasta($small){
                                font-size: 15px;
                            }
                        }
                        &__desc{
                            font-size: 15px;

                            @include hasta($small){
                                font-size: 10px;
                            }

                        }
                    }
                }
                &__compra{
                    display: flex;
                    align-items: center;
                    width: 250px;

                    @include hasta($small){
                        width: 100px;
                    }
                    &__texto{
                        &__titulo{
                            font-size: 20px;
                            margin: 0px;
                            font-weight: bold;
                            color: $color2;
                            font-family: $ff2;

                            @include hasta($small){
                                font-size: 15px;
                            }

                        }
                        &__desc{
                            font-size: 15px;

                            @include hasta($small){
                                font-size: 10px;
                            }
                        }
                    }
                }
            }
            
            &__info{
                background: $color2;
                display: flex;
                color: $color1;
                justify-content: space-between;
                padding: 30px 30px;

                @include hasta($small){
                    flex-direction: column;
                    font-size: 12px;
                    padding: 10px 0px;
                    text-align: center;
                    width: 365px;
                }

                span{
                    font-weight: bold;
                }

                &__contacto{
                    @include hasta($small){
                        margin-bottom: 15px;
                    }
                }

                &__acerca{
                    @include hasta($small){
                        margin-bottom: 25px;
                    }
                    &__titulo{
                        
                        text-decoration: none;
                    }
                    &__link{
                        color: $color1;
                    }
                    :hover{
                        text-decoration: underline;
                        color: $color1;
                        font-weight: bold;
                    }
                    
                }
            }
            &__copy{
                border-bottom-left-radius: 10px;
                border-bottom-right-radius: 10px;
                width: 1500px;
                background: $color1;

                @include hasta($small){
                    width: 365px;
                }

                &__imagenes{
                    display: flex;
                    justify-content: space-between;
                    padding: 30px 200px;

                    @include hasta($small){
                        padding: 10px 50px;
                    }

                    &__img1{
                        width: 400px;
                        height: 50px;
                        @include hasta($small){
                            width: 100px;
                            height: 12px;
                        }   
                    }
                    &__img2{
                        width: 200px;
                        height: 50px;
                        @include hasta($small){
                            width: 50px;
                            height: 12px;
                        }
                    }
                }
                &__parrafo{
                    padding: 20px 50px;
                    @include hasta($small){
                        padding: 10px 30px;
                        font-size: 10px;
                    }   
                }
            }
        }
    }
</style>