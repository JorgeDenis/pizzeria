<template>
    <div class="contenedor">
        <div class="menu">
            <div class="menu__logoNombre">
                <img src="../../assets/logo.png" class="menu__logoNombre__imagen" alt="">
                <h1 class="menu__logoNombre__nombre">
                    Colosus Pizza
                </h1>
            </div>
            <div class="menu__variantes">
                <div class="menu__variantes__clasicas">
                    <div class="menu__variantes__clasicas__tituloTam">
                        <h2 class="menu__variantes__clasicas__tituloTam__titulo">
                            CLÁSICAS
                        </h2>
                        <div class="menu__variantes__clasicas__tituloTam__tam">
                            <div class="menu__variantes__clasicas__tituloTam__tam__mediana">
                                <div class="menu__variantes__clasicas__tituloTam__tam__mediana__titulo">
                                    Mediana
                                </div>
                                <div class="menu__variantes__clasicas__tituloTam__tam__mediana__dibujo">
                                    <img src="../../assets/iconoMenuMediana.png" class="menu__variantes__clasicas__tituloTam__tam__mediana__dibujo__img" alt="">
                                </div>
                                <div class="menu__variantes__clasicas__tituloTam__tam__mediana__precio">
                                    30/40 Bs
                                </div>
                            </div>
                        </div>
    
                        <div class="menu__variantes__clasicas__tituloTam__tam">
                            <div class="menu__variantes__clasicas__tituloTam__tam__grande">
                                <div class="menu__variantes__clasicas__tituloTam__tam__grande__titulo">
                                    Grande
                                </div>
                                <div class="menu__variantes__clasicas__tituloTam__tam__grande__dibujo">
                                    <img src="../../assets/iconoMenuGrande.png" class="menu__variantes__clasicas__tituloTam__tam__grande__dibujo__img" alt="">
                                </div>
                                <div class="menu__variantes__clasicas__tituloTam__tam__grande__precio">
                                    40/50 Bs
                                </div>
                            </div>
                        </div>
    
                    </div>
    
                    <div class="menu__variantes__clasicas__opciones">
                        <div 
                            class="menu__variantes__clasicas__opciones__americana"
                            @mouseover="mostrarAmericana()"
                            @mouseout="ocultarFlotanteAmericana"
                        >
                            <img src="../../assets/menu/clasicas/Americana.jpg" alt="" 
                                class="menu__variantes__clasicas__opciones__americana__img slide-right"
                                :style="flotanteStylesAmericana"
                            >
                            <h2 class="menu__variantes__clasicas__opciones__americana__titulo">
                                1.- AMERICANA
                            </h2>
                            <h3 class="menu__variantes__clasicas__opciones__americana__descipcion">
                                mozzarella, jamón ahumado, choclo.
                            </h3>
                        </div>
    
                        <div 
                            class="menu__variantes__clasicas__opciones__calabresa"
    
                            @mouseover="mostrarCalabresa()"
                            @mouseout="ocultarFlotanteCalabresa"
                        >
                            <img src="../../assets/menu/clasicas/Calabresa.jpg" alt="" 
                                class="menu__variantes__clasicas__opciones__calabresa__img slide-right" 
                                :style="flotanteStylesCalabresa"
                            >
                            <h2 class="menu__variantes__clasicas__opciones__calabresa__titulo">
                                2.- CALABRESA
                            </h2>
                            <h3 class="menu__variantes__clasicas__opciones__calabresa__descipcion">
                                mozzarella, calabresa ahumada.
                            </h3>
                        </div>
    
                        <div 
                            class="menu__variantes__clasicas__opciones__margarita"
                            @mouseover="mostrarMargarita()"
                            @mouseout="ocultarFlotanteMargarita"    
                        >
                            <img src="../../assets/menu/clasicas/Margarita.jpg" alt="" 
                                class="menu__variantes__clasicas__opciones__Margarita__img slide-right"
                                :style="flotanteStylesMargarita"
                            >
                            <h2 class="menu__variantes__clasicas__opciones__margarita__titulo">
                                3.- MARGARITA
                            </h2>
                            <h3 class="menu__variantes__clasicas__opciones__margarita__descipcion">
                                mozzarella, tomate, albahaca.
                            </h3>
                        </div>
    
                        <div 
                            class="menu__variantes__clasicas__opciones__napolitana"
                            @mouseover="mostrarNapolitana()"
                            @mouseout="ocultarFlotanteNapolitana"    
                        >
                            <img src="../../assets/menu/clasicas/Napolitana.jpg" alt="" 
                                class="menu__variantes__clasicas__opciones__napolitana__img slide-right"
                                :style="flotanteStylesNapolitana"
                            >
                            <h2 class="menu__variantes__clasicas__opciones__napolitana__titulo">
                                4.- NAPOLITANA
                            </h2>
                            <h3 class="menu__variantes__clasicas__opciones__napolitana__descipcion">
                                mozzarella, parmesano, tomate.
                            </h3>
                        </div>
    
                        <div 
                            class="menu__variantes__clasicas__opciones__hawaiana"
                            @mouseover="mostrarHawaiana()"
                            @mouseout="ocultarFlotanteHawaiana"
                        >
                            <img src="../../assets/menu/clasicas/Hawaiana.jpg" alt="" 
                                class="menu__variantes__clasicas__opciones__hawaiana__img slide-right"
                                :style="flotanteStylesHawaiana"
                            >
                            <h2 class="menu__variantes__clasicas__opciones__hawaiana__titulo">
                                5.- HAWAIANA
                            </h2>
                            <h3 class="menu__variantes__clasicas__opciones__hawaiana__descipcion">
                                mozzarella, jamón ahumado, piña.
                            </h3>
                        </div>
    
                        <div 
                            class="menu__variantes__clasicas__opciones__fugazzeta"
                            @mouseover="mostrarFugazzeta()"
                            @mouseout="ocultarFlotanteFugazzeta"    
                        >
                            <img src="../../assets/menu/clasicas/Fugazzetta.jpg" alt="" 
                                class="menu__variantes__clasicas__opciones__fugazzeta__img slide-right"
                                :style="flotanteStylesFugazzeta"
                            >
                            <h2 class="menu__variantes__clasicas__opciones__fugazzeta__titulo">
                                6.- FUGAZZETA
                            </h2>
                            <h3 class="menu__variantes__clasicas__opciones__fugazzeta__descipcion">
                                mozzarella, cebolla blanca, champiñones.
                            </h3>
                        </div>
                    </div>
                </div>
    
    
                <div class="menu__variantes__premium">
                    <div class="menu__variantes__premium__tituloTam">
                        <h2 class="menu__variantes__premium__tituloTam__titulo">
                            PREMIUM
                        </h2>
                        <div class="menu__variantes__premium__tituloTam__tam">
                            <div class="menu__variantes__premium__tituloTam__tam__mediana">
                                <div class="menu__variantes__premium__tituloTam__tam__mediana__titulo">
                                    Mediana
                                </div>
                                <div class="menu__variantes__premium__tituloTam__tam__mediana__dibujo">
                                    <img src="../../assets/iconoMenuMediana.png" class="menu__variantes__premium__tituloTam__tam__mediana__dibujo__img" alt="">
                                </div>
                                <div class="menu__variantes__premium__tituloTam__tam__mediana__precio">
                                    35/45 Bs
                                </div>
                            </div>
                        </div>
    
                        <div class="menu__variantes__premium__tituloTam__tam">
                            <div class="menu__variantes__premium__tituloTam__tam__grande">
                                <div class="menu__variantes__premium__tituloTam__tam__grande__titulo">
                                    Grande
                                </div>
                                <div class="menu__variantes__premium__tituloTam__tam__grande__dibujo">
                                    <img src="../../assets/iconoMenuGrande.png" class="menu__variantes__premium__tituloTam__tam__grande__dibujo__img" alt="">
                                </div>
                                <div class="menu__variantes__premium__tituloTam__tam__grande__precio">
                                    45/55 Bs
                                </div>
                            </div>
                        </div>
    
                    </div>
    
                    <div class="menu__variantes__premium__opciones">
                        <div 
                            class="menu__variantes__premium__opciones__cheeseburger"
                            @mouseover="mostrarCheeseburger()"
                            @mouseout="ocultarFlotanteCheeseburger"
                        >
                            <img src="../../assets/menu/premium/Cheeseburger.jpg" alt="" 
                                class="menu__variantes__premium__opciones__cheeseburger__img slide-right"
                                :style="flotanteStylesCheeseburger"
                            >
                            <h2 class="menu__variantes__premium__opciones__cheeseburger__titulo">
                                7.- CHEESEBURGER
                            </h2>
                            <h3 class="menu__variantes__premium__opciones__cheeseburger__descipcion">
                                mozzarella, cheddar, cebolla blanca, carne, tocino.
                            </h3>
                        </div>
    
                        <div 
                            class="menu__variantes__premium__opciones__barbacoa"
    
                            @mouseover="mostrarBarbacoa()"
                            @mouseout="ocultarFlotanteBarbacoa"
                        >
                            <img src="../../assets/menu/premium/Barbacoa.jpg" alt="" 
                                class="menu__variantes__premium__opciones__barbacoa__img slide-right"
                                :style="flotanteStylesBarbacoa"
                            >
                            <h2 class="menu__variantes__premium__opciones__barbacoa__titulo">
                                8.- BARBACOA
                            </h2>
                            <h3 class="menu__variantes__premium__opciones__barbacoa__descipcion">
                                salsa barbacoa, mozzarella, cebolla, choclo, pollo o carne.
                            </h3>
                        </div>
    
                        <div 
                            class="menu__variantes__premium__opciones__carnivora"
                            @mouseover="mostrarCarnivora()"
                            @mouseout="ocultarFlotanteCarnivora"    
                        >
                            <img src="../../assets/menu/premium/Carnivora.jpg" alt="" 
                                class="menu__variantes__premium__opciones__carnivora__img slide-right"
                                :style="flotanteStylesCarnivora"
                            >
                            <h2 class="menu__variantes__premium__opciones__carnivora__titulo">
                                9.- CARNÍVORA
                            </h2>
                            <h3 class="menu__variantes__premium__opciones__carnivora__descipcion">
                                mozzarella, jamón, calabresa, tocino, carne.
                            </h3>
                        </div>
    
                        <!-- <div 
                            class="menu__variantes__premium__opciones__polloCrema"
                            @mouseover="mostrarPolloCrema()"
                            @mouseout="ocultarFlotantePolloCrema"    
                        >
                            <img src="../../assets/menu/premium/PolloCrema.jpg" alt="" 
                                class="menu__variantes__premium__opciones__polloCrema__img"
                                :style="flotanteStylesPolloCrema"
                            >
                            <h2 class="menu__variantes__premium__opciones__polloCrema__titulo">
                                10.- POLLO CREMA
                            </h2>
                            <h3 class="menu__variantes__premium__opciones__polloCrema__descipcion">
                                mozzarella, tomate, champiñones, cebolla, pimentón.
                            </h3>
                        </div> -->
    
                        <div 
                            class="menu__variantes__premium__opciones__veggie"
                            @mouseover="mostrarVeggie()"
                            @mouseout="ocultarFlotanteVeggie"
                        >
                            <img src="../../assets/menu/premium/Veggie.jpg" alt="" 
                                class="menu__variantes__premium__opciones__veggie__img slide-right"
                                :style="flotanteStylesVeggie"
                            >
                            <h2 class="menu__variantes__premium__opciones__veggie__titulo">
                                10.- VEGGIE
                            </h2>
                            <h3 class="menu__variantes__premium__opciones__veggie__descipcion">
                                mozzarella, tomate, champiñones, cebolla, pimentón.
                            </h3>
                        </div>
    
                        <!-- <div 
                            class="menu__variantes__premium__opciones__strogonoff"
                            @mouseover="mostrarStrogonoff()"
                            @mouseout="ocultarFlotanteStrogonoff"    
                        >
                            <img src="../../assets/menu/premium/Fugazzetta.jpg" alt="" 
                                class="menu__variantes__premium__opciones__strogonoff__img"
                                :style="flotanteStylesStrogonoff"
                            >
                            <h2 class="menu__variantes__premium__opciones__strogonoff__titulo">
                                12.- STROGONOFF
                            </h2>
                            <h3 class="menu__variantes__premium__opciones__strogonoff__descipcion">
                                mozzarella, salsa strogonoff, carne o pollo, papas fritas.
                            </h3>
                        </div> -->
    
                        <div 
                            class="menu__variantes__premium__opciones__carbonara"
                            @mouseover="mostrarCarbonara()"
                            @mouseout="ocultarFlotanteCarbonara"    
                        >
                            <img src="../../assets/menu/premium/Carbonara.jpg" alt="" 
                                class="menu__variantes__premium__opciones__carbonara__img slide-right"
                                :style="flotanteStylesCarbonara"
                            >
                            <h2 class="menu__variantes__premium__opciones__carbonara__titulo">
                                11.- CARBONARA
                            </h2>
                            <h3 class="menu__variantes__premium__opciones__carbonara__descipcion">
                                mozzarella, champiñones, cebolla blanca, tocino.
                            </h3>
                        </div>
    
                        <div 
                            class="menu__variantes__premium__opciones__quattroQuesos"
                            @mouseover="mostrarQuattroQuesos()"
                            @mouseout="ocultarFlotanteQuattroQuesos"    
                        >
                            <img src="../../assets/menu/premium/quattroQuesos.jpg" alt="" 
                                class="menu__variantes__premium__opciones__quattroQuesos__img slide-right"
                                :style="flotanteStylesQuattroQuesos"
                            >
                            <h2 class="menu__variantes__premium__opciones__quattroQuesos__titulo">
                                12.- QUATTRO QUESOS
                            </h2>
                            <h3 class="menu__variantes__premium__opciones__quattroQuesos__descipcion">
                                mozzarella, cheddar, parmesano, queso crema.
                            </h3>
                        </div>
    
                    </div>
                </div>

            </div>

        </div>
    </div>
    
</template>

<script>
    
    export default {
        name: 'MenuPrincipal',
        data() {
            return {
                flotanteVisibleAmericana: false,
                flotanteVisibleCalabresa: false,
                flotanteVisibleMargarita: false,
                flotanteVisibleNapolitana: false,
                flotanteVisibleHawaiana: false,
                flotanteVisibleFugazzeta: false,
                flotanteVisibleCheeseBurger: false,
                flotanteVisibleBarbacoa: false,
                flotanteVisibleCarnivora: false,
                flotanteVisiblePolloCrema: false,
                flotanteVisibleVeggie: false,
                flotanteVisibleStrogonoff: false,
                flotanteVisibleCarbonara: false,
                flotanteVisibleQuattroQuesos: false,

                flotantePosicion: { top: 0, left: 0 },

                
            }
        },
        computed: {
            flotanteStylesAmericana() {
                if (window.innerWidth > 600) { // Ancho de ventana menor a 600px
                    return {
                        display: this.flotanteVisibleAmericana ? 'block' : 'none',
                        top: `${this.flotantePosicion.top}px`,
                        left: `${this.flotantePosicion.left}px`,
                    };
                } else {
                    // Estilos para ancho de ventana mayor o igual a 600px
                    return {
                        display: this.flotanteVisibleAmericana ? 'none' : 'none',
                    };
                }

            },
            flotanteStylesCalabresa() {
                if (window.innerWidth > 600) {
                    return {
                        display: this.flotanteVisibleCalabresa ? 'block' : 'none',
                        top: `${this.flotantePosicion.top}px`,
                        left: `${this.flotantePosicion.left}px`,
                    };
                } else {
                    return {
                        display: this.flotanteVisibleCalabresa ? 'none' : 'none',
                    };
                }
            },
            flotanteStylesMargarita() {
                if (window.innerWidth > 600) {
                    return {
                        display: this.flotanteVisibleMargarita ? 'block' : 'none',
                        top: `${this.flotantePosicion.top}px`,
                        left: `${this.flotantePosicion.left}px`,
                    };
                } else {
                    return {
                        display: this.flotanteVisibleMargarita ? 'none' : 'none',
                    };
                }
            },
            flotanteStylesNapolitana() {
                if (window.innerWidth > 600) {
                    return {
                        display: this.flotanteVisibleNapolitana ? 'block' : 'none',
                        top: `${this.flotantePosicion.top}px`,
                        left: `${this.flotantePosicion.left}px`,
                    };
                } else {
                    return {
                        display: this.flotanteVisibleNapolitana ? 'none' : 'none',
                    };
                }

                
            },
            flotanteStylesHawaiana() {
                if (window.innerWidth > 600) {
                    return {
                        display: this.flotanteVisibleHawaiana ? 'block' : 'none',
                        top: `${this.flotantePosicion.top}px`,
                        left: `${this.flotantePosicion.left}px`,
                    };
                } else {
                    return {
                        display: this.flotanteVisibleHawaiana ? 'none' : 'none',
                    };
                }

                
            },
            flotanteStylesFugazzeta() {
                if (window.innerWidth > 600) {
                    return {
                        display: this.flotanteVisibleFugazzeta ? 'block' : 'none',
                        top: `${this.flotantePosicion.top}px`,
                        left: `${this.flotantePosicion.left}px`,
                    };
                } else {
                    return {
                        display: this.flotanteVisibleFugazzeta ? 'none' : 'none',
                    };
                }
            },



            flotanteStylesCheeseburger() {
                if (window.innerWidth > 600) {
                    return {
                        display: this.flotanteVisibleCheeseBurger ? 'block' : 'none',
                        top: `${this.flotantePosicion.top}px`,
                        left: `${this.flotantePosicion.left}px`,
                    };
                } else {
                    return {
                        display: this.flotanteVisibleCheeseBurger ? 'none' : 'none',
                    };
                }
            },
            flotanteStylesBarbacoa() {
                if (window.innerWidth > 600) {
                    return {
                        display: this.flotanteVisibleBarbacoa ? 'block' : 'none',
                        top: `${this.flotantePosicion.top}px`,
                        left: `${this.flotantePosicion.left}px`,
                    };
                } else {
                    return {
                        display: this.flotanteVisibleBarbacoa ? 'none' : 'none',
                    };
                }
            },
            flotanteStylesCarnivora() {
                if (window.innerWidth > 600) {
                    return {
                        display: this.flotanteVisibleCarnivora ? 'block' : 'none',
                        top: `${this.flotantePosicion.top}px`,
                        left: `${this.flotantePosicion.left}px`,
                    };
                } else {
                    return {
                        display: this.flotanteVisibleCarnivora ? 'none' : 'none',
                    };
                }
            },
            flotanteStylesPolloCrema() {
                return {
                    display: this.flotanteVisiblePolloCrema ? 'block' : 'none',
                    top: `${this.flotantePosicion.top}px`,
                    left: `${this.flotantePosicion.left}px`,
                };
            },
            flotanteStylesVeggie() {
                if (window.innerWidth > 600) {
                    return {
                        display: this.flotanteVisibleVeggie ? 'block' : 'none',
                        top: `${this.flotantePosicion.top}px`,
                        left: `${this.flotantePosicion.left}px`,
                    };
                } else {
                    return {
                        display: this.flotanteVisibleVeggie ? 'none' : 'none',
                    };
                }
            },
            flotanteStylesStrogonoff() {
                return {
                    display: this.flotanteVisibleStrogonoff ? 'block' : 'none',
                    top: `${this.flotantePosicion.top}px`,
                    left: `${this.flotantePosicion.left}px`,
                };
            },
            flotanteStylesCarbonara() {
                if (window.innerWidth > 600) {
                    return {
                        display: this.flotanteVisibleCarbonara ? 'block' : 'none',
                        top: `${this.flotantePosicion.top}px`,
                        left: `${this.flotantePosicion.left}px`,
                    };
                } else {
                    return {
                        display: this.flotanteVisibleCarbonara ? 'none' : 'none',
                    };
                }
            },
            flotanteStylesQuattroQuesos() {
                if (window.innerWidth > 600) {
                    return {
                        display: this.flotanteVisibleQuattroQuesos ? 'block' : 'none',
                        top: `${this.flotantePosicion.top}px`,
                        left: `${this.flotantePosicion.left}px`,
                    };
                } else {
                    return {
                        display: this.flotanteVisibleQuattroQuesos ? 'none' : 'none',
                    };
                }
            },

        },
        methods: {
            

            mostrarAmericana(){
                this.flotantePosicion = { top: 120, left: 400 };
                this.flotanteVisibleAmericana = true;
            },
            mostrarCalabresa(){
                this.flotantePosicion = { top: 200, left: 400 };
                this.flotanteVisibleCalabresa = true;
            },
            mostrarMargarita(){
                this.flotantePosicion = { top: 290, left: 400 };
                this.flotanteVisibleMargarita = true;
            },
            mostrarNapolitana(){
                this.flotantePosicion = { top: 375, left: 400 };
                this.flotanteVisibleNapolitana = true;
            },
            mostrarHawaiana(){
                this.flotantePosicion = { top: 460, left: 400 };
                this.flotanteVisibleHawaiana = true;
            },
            mostrarFugazzeta(){
                this.flotantePosicion = { top: 545, left: 400 };
                this.flotanteVisibleFugazzeta = true;
            },


            mostrarCheeseburger(){
                this.flotantePosicion = { top: 120, left: 1195 };
                this.flotanteVisibleCheeseBurger = true;
            },
            mostrarBarbacoa(){
                this.flotantePosicion = { top: 200, left: 1195 };
                this.flotanteVisibleBarbacoa = true;
            },
            mostrarCarnivora(){
                this.flotantePosicion = { top: 290, left: 1195 };
                this.flotanteVisibleCarnivora = true;
            },
            // mostrarPolloCrema(){
            //     this.flotantePosicion = { top: 1020, left: 400 };
            //     this.flotanteVisiblePollomostrarPolloCrema = true;
            // },
            mostrarVeggie(){
                this.flotantePosicion = { top: 375, left: 1195 };
                this.flotanteVisibleVeggie = true;
            },
            // mostrarStrogonoff(){
            //     this.flotantePosicion = { top: 520, left: 500 };
            //     this.flotanteVisibleStrogonoff = true;
            // },
            mostrarCarbonara(){
                this.flotantePosicion = { top: 460, left: 1195 };
                this.flotanteVisibleCarbonara = true;
            },
            mostrarQuattroQuesos(){
                this.flotantePosicion = { top: 545, left: 1195 };
                this.flotanteVisibleQuattroQuesos = true;
            },










            ocultarFlotanteAmericana() {
                this.flotanteVisibleAmericana = false;
            },
            ocultarFlotanteCalabresa() {
                this.flotanteVisibleCalabresa = false;
            },
            ocultarFlotanteMargarita() {
                this.flotanteVisibleMargarita = false;
            },
            ocultarFlotanteNapolitana() {
                this.flotanteVisibleNapolitana = false;
            },
            ocultarFlotanteHawaiana() {
                this.flotanteVisibleHawaiana = false;
            },
            ocultarFlotanteFugazzeta() {
                this.flotanteVisibleFugazzeta = false;
            },


            ocultarFlotanteCheeseburger() {
                this.flotanteVisibleCheeseBurger = false;
            },
            ocultarFlotanteBarbacoa() {
                this.flotanteVisibleBarbacoa = false;
            },
            ocultarFlotanteCarnivora() {
                this.flotanteVisibleCarnivora = false;
            },
            ocultarFlotantePolloCrema() {
                this.flotanteVisiblePolloCrema = false;
            },
            ocultarFlotanteVeggie() {
                this.flotanteVisibleVeggie = false;
            },
            ocultarFlotanteStrogonoff() {
                this.flotanteVisibleStrogonoff = false;
            },
            ocultarFlotanteCarbonara() {
                this.flotanteVisibleCarbonara = false;
            },
            ocultarFlotanteQuattroQuesos() {
                this.flotanteVisibleQuattroQuesos = false;
            },
        },
    }
</script>

<style lang="scss" scoped>
    .contenedor{
        display: flex;
        justify-content: center;
        align-items: center;
        background: $color5;
    }
    .menu{
        background: rgba( 255, 255, 255, 0.05 );
        box-shadow: 0 8px 32px 0 rgba(242, 86, 29, 0.37);
        backdrop-filter: blur( 3px );
        -webkit-backdrop-filter: blur( 3px );
        border-radius: 10px;
        border: 1px solid rgba( 255, 255, 255, 0.18 );


        padding: 0px 50px;        
        margin-top: 139px;
        display: block;
        color: $color1;
        width: 1500px;



        @include hasta($small){
            width: 365px;
            margin-top: 15px;
        }

        &__contenedor{
            background: $color3;
            position: relative;
            width: 400px;
            height: 400px;
        }

        &__logoNombre{
            display: flex;
            align-items: center;
            justify-content: center;

            &__imagen{
                width: 100px;
                @include hasta($small){
                    width: 50px;
                }
            }
            &__nombre{
                margin-top: 20px;
                font-family: $ff1;
                font-weight: 500;
                @include hasta($small){
                    margin-top: 10;
                }
            }
        }
        &__variantes{
            display: flex;
            justify-content: space-between;
            padding: 0px 150px;

            @include hasta($small){
                display: block;
                padding: 0px;
            }

            &__clasicas{
                margin-top: 10px;
                margin-bottom: 70px;
                &__tituloTam{
                    margin-bottom: 10px;
                    justify-content: center;
                    align-items: center;
                    display: flex;


                    &__titulo{
                        margin-right: 15px;
                        text-decoration: underline;
                        font-family: $ff2;
                        @include hasta($small){
                            font-size: 17px;
                        }
                    }
                    &__tam{
                        margin: 0px 5px;
                        width: 80px;
                        height: 100px;
                        border-radius: 15%;
                        background: rgba(255, 255, 255, 0.5);
                        text-align: center;
                        align-items: center;
                        &__mediana{
                            justify-content: center;
                            align-items: center;
                            display: block;
                            &__dibujo{
                                &__img{
                                    width: 50px;
                                    height: 50px;
                                }
                            }
                        }
                        &__grande{
                            justify-content: center;
                            align-items: center;
                            display: block;
                            &__dibujo{
                                &__img{
                                    width: 50px;
                                    height: 50px;
                                }
                            }
                        }
                    }
                }
                &__opciones{
                    :hover{
                        background: $color3;
                    }
                    h2{
                        font-size: 30px;
                        font-family: $ff2;
                        @include hasta($small){
                            font-size: 17px;
                        }
                    }
                    h3{
                        margin-left: 10px;
                        margin-bottom: 15px;
                        font-size: 15px;
                        font-family: $ff3;
                        @include hasta($small){
                            font-size: 13px;
                        }
                    }
                    img{
                        position: absolute; /* Cambia a "fixed" si quieres que el elemento se mantenga en la misma posición incluso al hacer scroll */
                        top: 235px; /* Ajusta la posición vertical según tus necesidades */
                        left: 500px; /* Ajusta la posición horizontal según tus necesidades */
                        width: 300px;
                        height: 300px;
                        border: 2px solid;
                        border-radius: 5%;
                        border-color: $color3;
                        z-index: 4; /* Controla la profundidad en la que se encuentra el elemento */
                    }
                    
                }
            }
    
            &__premium{
                margin-top: 10px;
                margin-bottom: 130px;
                &__tituloTam{
                    margin-bottom: 10px;
                    justify-content: center;
                    align-items: center;
                    display: flex;
                    
                    &__titulo{
                        margin-right: 15px;
                        text-decoration: underline;

                        @include hasta($small){
                            font-size: 17px;
                        }
                    }
                    &__tam{
                        margin: 0px 5px;
                        width: 80px;
                        height: 100px;
                        border-radius: 15%;
                        background: rgba(255, 255, 255, 0.5);
                        text-align: center;
                        align-items: center;
                        &__mediana{
                            justify-content: center;
                            align-items: center;
                            display: block;
                            &__dibujo{
                                &__img{
                                    width: 50px;
                                    height: 50px;
                                }
                            }
                        }
                        &__grande{
                            justify-content: center;
                            align-items: center;
                            display: block;
                            &__dibujo{
                                &__img{
                                    width: 50px;
                                    height: 50px;
                                }
                            }
                        }
                    }
                }
                &__opciones{
                    :hover{
                        background: $color3 0.5%;
                    }
                    h2{
                        font-size: 30px;
                        font-family: $ff1;

                        @include hasta($small){
                            font-size: 17px;
                        }
                    }
                    h3{
                        margin-left: 10px;
                        margin-bottom: 15px;
                        font-size: 15px;
                        font-family: $ff3;

                        @include hasta($small){
                            font-size: 13px;
                        }
                    }
                    img{
                        position: absolute; /* Cambia a "fixed" si quieres que el elemento se mantenga en la misma posición incluso al hacer scroll */
                        top: 235px; /* Ajusta la posición vertical según tus necesidades */
                        left: 500px; /* Ajusta la posición horizontal según tus necesidades */
                        width: 300px;
                        height: 300px;
                        border: 5px solid;
                        border: 2px solid;
                        border-radius: 5%;
                        border-color: $color3;
                        z-index: 4; /* Controla la profundidad en la que se encuentra el elemento */
                    }
                    
                }
            }
        }
    }
    .slide-right {
        animation: slide-right 0.5s cubic-bezier(0.250, 0.460, 0.450, 0.940) both;
        @keyframes slide-right {
            0% {
                transform: translateX(0);
                opacity: 0;
            }
            100% {
                transform: translateX(100px);
                opacity: 1;
            }
        }
    }

    .slide-left {
        animation: slide-left 0.5s cubic-bezier(0.250, 0.460, 0.450, 0.940) both;
        @keyframes slide-left {
            0% {
                transform: translateX(0);
                opacity: 0;
            }
            100% {
                transform: translateX(-100px);
                opacity: 1;
            }
        }
    }

    
    
</style>