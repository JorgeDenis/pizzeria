<template>
    <div class="header">
        <img src="../../assets/logosolo.png" alt="Logo" class="header__logo">
        <label class="buttons__burger" for="burger" >
            <input type="checkbox" id="burger" @click="toggleMenu">
            <span></span>
            <span></span>
            <span></span>
        </label>

        <ul class="header__menu scale-in-tr" :style="menuStyles">
            <li class="header__menu__item">
                <router-link :to="{ name: 'home'}" class="header__menu__item__link">
                    Inicio
                </router-link>
            </li>

            <li class="header__menu__item">
                <router-link :to="{ name: 'menu'}" class="header__menu__item__link">
                    Menu
                </router-link>
            </li>

            <li class="header__menu__item">
                <a class="header__menu__item__link">
                    Conócenos
                </a>
            </li>

            <li class="header__menu__item">
                <a class="header__menu__item__link">
                    Ingresar
                </a>
            </li>
            
            <li class="header__menu__item">
                <a class="header__menu__item__link">
                    Registrarse
                </a>
            </li>

        </ul>

    </div>
    
</template>

<script>

    export default {
        data() {
            return {
                menuVisible: false
            }
        },
        computed: {
            menuStyles() {
                if (window.innerWidth < 600) { // Ancho de ventana menor a 600px
                    return {
                        display: this.menuVisible ? 'block' : 'none',
                        position: 'absolute',
                        listStyle: 'none',
                        top: '65px',
                        right: '0px',
                        zIndex: '1',
                        background: '$color6', // Puedes usar tus variables SCSS aquí
                        fontWeight: 'bold',
                        height: '162px'
                    };
                } else {
                    // Estilos para ancho de ventana mayor o igual a 600px
                    return {
                        display: 'flex' // Puedes ajustar los estilos según sea necesario
                    };
                }
            }
        },

        methods:{
            toggleMenu(){
                this.menuVisible = !this.menuVisible;
            },
            
        }
    }
</script>

<style lang = "scss" scope>
 .header{
    background: $color6;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 10px 150px;
    position: fixed;
    top: 0;
    width: 100%;
    box-shadow: 0 8px 32px 0 rgba(242, 86, 29, 0.20);
    @include hasta($small){
        justify-content: space-between;
        padding: 8px 15px;
        position: relative;
    }
    @include desde($small){
        justify-content: space-between;
        padding: 8px 15px;
    }

    @include desde($medium){
        justify-content: space-between;

    }
    @include desde($large){
        justify-content: space-between;
        font-size: 30px;
    }
    &__logo{
        color: $color1;
        font-family: $ff-1;
        font-size: 24px;
        text-decoration: none;
        height: 70px;
        
        @include hasta($small){
            height: 50px;
        }

        @include desde($small){
            height: 70px;            
        }
    }
    &__menu{
        display: none;
        bottom: 0%;
        user-select: none;
        @include hasta($small){
            display: block;
            position: absolute;
            list-style: none;
            top: 65px;
            right: 0px;
            z-index: 1;
            background: $color6;
            font-weight: bold;
            height: 162px;
        }

        @include desde($small){
            display: none;
            list-style: none;
        }

        &__item{
            @include hasta($small){
                margin: 0px;
                :hover{
                    text-decoration: none;
                    color: $color1;
                    background: $color2;
                }
            }
            &__link{
                display: block;
                padding: 5px 30px;
                text-decoration: none;
                color: $color1;
                font-family: $ff2;
                font-size: 13px;

                @include hasta($small){
                    border: 1px solid $color5;
                }
            }
        }

        @include desde($medium){
            display: flex;
            list-style: none;
            padding: 0px;
            margin: 0px;
            &__item{
                margin: 5px;
                &__link{
                    display: block;
                    padding: 5px 30px;
                    text-decoration: none;
                    color: $color1;
                    font-family: $ff2;
                    font-size: 13px;
                    &:hover{
                        font-weight: 1000;
                        color: $color2;
                    }
                }
            }
        }
    }
 }

 .buttons__burger {
  --size: 30px;
  --clr: #d8d8d8;
  width: var(--size);
  height: calc(0.9 * var(--size));
  cursor: pointer;
  position: relative;
  display: none;

  @include hasta($small){
    display: block;
    justify-content: right;
  }
}

.buttons__burger #burger {
  display: none;
  width: 100%;
  height: 100%;
}

.buttons__burger span {
  display: block;
  position: absolute;
  width: 100%;
  border-radius: 0.5rem;
  border: 3px solid var(--clr);
  background-color: var(--clr);
  transition: 0.15s ease-in-out;
}

.buttons__burger span:nth-of-type(1) {
  top: 0;
  right: 0;
  transform-origin: right center;
}

.buttons__burger span:nth-of-type(2) {
  top: 50%;
  transform: translateY(-50%);
}

.buttons__burger span:nth-of-type(3) {
  top: 100%;
  right: 0;
  transform-origin: right center;
  transform: translateY(-100%);
}

.buttons__burger #burger:checked ~ span:nth-of-type(1) {
  transform: translateY(-30%) rotate(40deg);
  width: 50%;
  top: 50%;
}

.buttons__burger #burger:checked ~ span:nth-of-type(3) {
  transform: translateY(-70%) rotate(-40deg);
  width: 50%;
  top: 50%;
}


.scale-in-tr {
    animation: scale-in-tr 0.5s cubic-bezier(0.250, 0.460, 0.450, 0.940) both;
}
@keyframes scale-in-tr {
    0% {
        transform: scale(0);
        transform-origin: 100% 0%;
        opacity: 1;
    }
    100% {
        transform: scale(1);
        transform-origin: 100% 0%;
        opacity: 1;
    }
}

.scale-out-tr {
	animation: scale-out-tr 0.5s cubic-bezier(0.550, 0.085, 0.680, 0.530) both;
}

@keyframes scale-out-tr {
  0% {
    transform: scale(1);
    transform-origin: 100% 0%;
    opacity: 1;
  }
  100% {
    transform: scale(0);
    transform-origin: 100% 0%;
    opacity: 1;
  }
}
</style>