<template>
    
    <SliderPizza/>
    
    <div class="principal">
        <div class="principal__informacion">
            <h1 class="principal__informacion__titulo">
                COLOSSUS
            </h1>
            <h1 class="principal__informacion__titulo">
                PIZZA
            </h1>
            <p class="principal__informacion__descripcion">                
                Deléitate con nuestras exquisitas pizzas artesanales, donde la tradición italiana se fusiona con sabores únicos. 
            </p>
            <p class="principal__informacion__descripcion">                
                ¡Ven y descubre un festín de sabor en cada rebanada!
            </p>
            <div class="principal__informacion__formulario">
                <input type="text" class="principal__informacion__formulario__input" placeholder="email@ejemplo.com" />
                <a href="#" class="principal__informacion__formulario__boton">Confirmar</a>
            </div>
            <img src="../../assets/pizza.png" class="principal__informacion__imagen">
        </div>
    </div>
</template>
<script>
    export default {
    name: 'BannerComponent',    
}
</script>
<style lang="scss" scoped>
    
    .principal{
        background: $color5;
        display: flex;
        padding: 10px 0px;
        justify-content: center;
        
        
        &__informacion{
            display: flex;
            flex-direction: column;
            color: $color1;
            font-family: $ff1;
            width: 1500px;
            
            

            background: rgba( 255, 255, 255, 0.05 );
            box-shadow: 0 8px 32px 0 rgba(242, 86, 29, 0.20);
            backdrop-filter: blur( 3px );
            -webkit-backdrop-filter: blur( 3px );
            border-radius: 10px;
            border: 1px solid rgba( 255, 255, 255, 0.18 );

            @include hasta($small){
                width: 365px;
            }

            &__titulo{
                font-weight: bold;
                font-size: 150px;
                font-family: $ff1;
                margin-left: 50px;
                z-index: 1;
                @include hasta($small){
                    font-size: 50px;
                    margin-left: 15px;
                }
            }
            &__descripcion{
                font-family: $ff3;
                width: 650px;
                margin-left: 50px;
                z-index: 3;
                @include hasta($small){
                    font-size: 17px;
                    margin-left: 15px;
                    width: 300px;
                }
            }
            &__formulario{
                margin: 50px;
                display: flex;
                align-items: center;

                @include hasta($small){
                    margin: 15px;
                    font-size: 50px;
                    margin-left: 15px;
                    flex-direction: column;
                }

                &__input{
                    padding: 21px;
                    font-size: 19px;
                    border-width: 1px;
                    font-family: $ff2;
                    background-color: $color1;
                    color: $color5;
                    border-style: solid;
                    border-radius: 50px;
                    width: 250px;
                    margin-top: 19px;
                    &:focus{
                        outline:none; 
                    }
                }
                &__boton{
                    background-color:$color3;
                    font-family: $ff2;
                    border-radius:50px;
                    display:inline-block;
                    cursor:pointer;
                    color:$color1;
                    font-size:19px;
                    padding:10px 31px;
                    text-decoration:none;
                    margin-left: 15px;
                    &:hover{
                        background:$color4;
                        color: $color1;
                        font-weight: bold;
                        box-shadow: #f2561d;
                    }
                    &:active{
                        position: relative;
                        top: 1px;
                    }
                }
            }
            &__imagen{
                width: 1150px;
                height: 550px;
                margin-top: 195px;
                position: absolute;  
                margin-left: 500px;
                z-index: 2;
                transform: rotate(25deg);
                @include hasta($small){
                    width: 210px;
                    height: 110px;
                    margin-top: 60px;
                    margin-left: 150px;    
    
                }
            }
        }
        
    }

    

</style>