<template>
    <header class="header">
        <div class="container header__container">
            <router-link class="logo" to="/"><img src="../assets/Frame.png" alt="" class="logo__img"></router-link>
            <nav class="nav" :class="showing ? 'nav-rwd' : ''">
                <button class="close-btn" @click="show()">+</button>
                <router-link class="nav__item" to="/">About</router-link>
                <router-link class="nav__item" to="/features">Features</router-link>
                <router-link class="nav__item" to="/about-us">About Us</router-link>
            </nav>
            <div class="signing">
                <button class="signing__btn sign-in">Sign In</button>
                <button class="signing__btn superpeer">
                    <svg width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <g clip-path="url(#clip0)">
                            <path
                                d="M13.82 13.24L12.28 12.91L11.53 12.74L11.62 11.98V11.86C11.62 11.7 11.6 11.54 11.54 11.39L11.36 10.99L11.6 10.59C11.74 10.37 11.8 10.11 11.8 9.82C11.8 9.52 11.72 9.24 11.55 9.02L11.25 8.62L11.45 8.16C11.53 7.98 11.56 7.79 11.56 7.6C11.56 7.33 11.56 6.52 10.3 6.04C9.91163 5.91627 9.50751 5.84892 9.1 5.84L7.73 5.74L8.38 4.56C8.91 3.61 9.2 2.76 9.2 2.16C9.2 1.61 9.02 1.12 8.61 0.960003C7.2 0.340003 6.2 1.3 5.47 2.48C4.9 3.43 4.18 4.66 3.75 5.57C2.82 7.53 1.44 8.95 1.44 10.92C1.44 12.71 2.64 14.11 4.84 14.85C7.53 15.75 11.55 16 13.3 16C14.55 16 15.24 15.51 15.24 14.62C15.24 13.69 14.36 13.36 13.82 13.24Z"
                                fill="#FFD338" />
                            <path
                                d="M13.26 12.45L10.56 11.86C10.77 11.71 11 11.39 11 10.99C11 10.53 10.76 10.27 10.57 10.13C10.82 9.93001 11.17 9.59 11.17 8.96C11.17 8.29 10.71 7.94 10.47 7.78C10.66 7.6 10.93 7.24 10.93 6.74C10.93 5.86 10.25 5.46 9.70001 5.24C9.03774 5.06784 8.3538 4.99372 7.67001 5.02C6.46001 5.02 5.36001 5.11 4.83001 5.11C4.21001 5.11 4.29001 4.79 4.51001 4.49C4.66001 4.33 6.43001 1.99 6.76001 1.57C6.99001 1.27 7.26001 0.970004 7.46001 1.08C7.68001 1.2 7.59001 1.74 7.36001 2.32C7.02001 3.24 6.53001 3.83 6.42001 4.03L7.24001 4.53C7.55001 4.13 8.59001 2.41 8.59001 1.3C8.59001 0.800004 8.39001 0.380004 8.03001 0.150004C7.66001 -0.0599956 7.18001 -0.0499956 6.76001 0.200004C6.48001 0.370004 6.20001 0.610004 5.96001 0.920004L3.46001 4.09C2.76001 5.02 3.08001 6.17 4.60001 6.17C5.14001 6.17 6.89001 6.04 7.57001 6.04C8.35001 6.04 8.73001 6.08 9.00001 6.12C9.50001 6.19 9.80001 6.42 9.80001 6.72C9.80001 6.95 9.70001 7.1 9.52001 7.22C9.34001 7.35 9.18001 7.55 9.18001 7.82C9.18001 8.13 9.47001 8.26 9.66001 8.39001C9.92001 8.56001 10.07 8.67 10.07 8.94C10.07 9.18 9.89001 9.32001 9.69001 9.47001C9.52001 9.60001 9.30001 9.74 9.30001 10.04C9.30001 10.3 9.50001 10.44 9.62001 10.54C9.75001 10.64 9.89001 10.75 9.89001 10.97C9.89001 11.19 9.79001 11.29 9.53001 11.44C9.33001 11.56 9.03001 11.77 9.03001 12.08C9.03001 12.42 9.28001 12.58 9.57001 12.65C10.27 12.82 12.37 13.27 13.08 13.43C13.31 13.48 13.54 13.56 13.54 13.75C13.54 13.95 13.24 14.03 12.8 14.03C11.3 14.03 7.10001 13.73 4.64001 12.87C2.97001 12.31 2.05001 11.27 2.05001 10.04C2.05001 8.96 2.77001 8.01 3.55001 7.46L2.85001 6.74C2.29138 7.10164 1.82741 7.59172 1.49687 8.16929C1.16633 8.74687 0.978823 9.39516 0.950012 10.06C0.950012 11.56 1.85001 13.1 4.31001 13.93C6.93001 14.81 10.9 15.08 12.75 15.08C14.02 15.08 14.63 14.56 14.63 13.77C14.62 13.01 14 12.6 13.26 12.45Z"
                                fill="#222222" />
                        </g>
                        <defs>
                            <clipPath id="clip0">
                                <rect width="16" height="16" fill="white" />
                            </clipPath>
                        </defs>
                    </svg>
                    Become a Superpeer                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                
                </button>
            </div>
            <div class="burger" @click="show()">
                <div class="burger__wrapper">
                    <div class="burger__item"></div>
                    <div class="burger__item"></div>
                    <div class="burger__item"></div>
                </div>
            </div>
        </div>
    </header>
</template>

<script>
    export default {
        name: "Header",
        data () {
            return {
                showing: false
            }
        },
        methods: {
            show () {
                this.showing = !this.showing
            }
        },
        watch: {
            show () {
                if (this.show) {
                    document.body.style.overflow = "hidden"
                } else {
                    document.body.style.overflow = "scroll"
                }
            }
        }
    }
</script>

<style lang="scss">
    .header {
        padding: 16px 0;
        position: fixed;
        top: 0;
        right: 0;
        left: 0;
        display: block;
        background: white;
        z-index: 5;
        box-shadow: 0 4px 20px rgba(237, 208, 130, 0.5);


        .logo {
            &__img {
                max-width: 126px;
                width: 100%;
            }
        }
        &__container {
            display: flex;
            justify-content: space-between;
            align-items: center;

            .nav {
                display: flex;
                align-items: center;
                gap: 48px;

                .close-btn {
                    display: none;
                    font-size: 56px;
                    font-weight: 700;
                    border: none;
                    background: transparent;
                    outline: none;
                    transform: rotate(45deg);
                }

                &__item {
                    font-size: 16px;
                    line-height: 22px;
                    text-transform: uppercase;
                    color: #555555;

                    .router-link-exact-active {
                        color: #222222;
                    }
                }
            }

            .signing {
                display: flex;
                align-items: center;
                gap: 40px;

                &__btn {
                    font-size: 16px;
                    line-height: 22px;
                    text-transform: uppercase;
                    color: #222222;
                    cursor: pointer;
                }

                .sign-in {
                    border: none;
                    background: white;
                    outline: none;
                }

                
            }

            .burger {
                display: none;
                width: 38px;
                height: 38px;
                background: #FFD338;
                border-radius: 50%;

                &__wrapper {
                    width: 100%;
                    height: 100%;
                    display: flex;
                    flex-direction: column;
                    justify-content: center;
                    align-items: center;
                    gap: 4px;
                }

                &__item {
                    width: 18px;
                    background: white;
                    height: 2px;
                }

            }
        }
    }
    .superpeer {
        display: block;
        margin: auto;
        padding: 12px 16px;
        background: #FFD338;
        border-radius: 8px;
        border: none;
        outline: none;
        font-size: 16px;
        line-height: 22px;
        text-transform: uppercase;
        color: #222222;
        cursor: pointer;
        transition: 0.3s;
        
        &:hover {
            background: black;
            color: #FFD338;
        }
    }

    @media only screen and (max-width: 750px) {
        .header {
            width: 100%;

            
            .nav {
                position: absolute;
                top: 0;
                left: -100%;
                flex-direction: column;
                gap: 12px;
                background: #FFD338;
                width: 100%;
                height: 100vh;
                padding-top: 100px;
                transition: 0.3s;

                .close-btn {
                    display: block;
                    position: absolute;
                    top: 10px;
                    right: 40px;
                }
            }
            .nav-rwd {
                left: 0;
                transition: 0.3s;
            }
            .signing {
                display: none;
            }
            .burger {
                display: block;
            }
        }
    }
</style>