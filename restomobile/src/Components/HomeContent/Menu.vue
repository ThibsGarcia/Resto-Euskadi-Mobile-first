<script setup lang="ts">

</script>

<template>
    <section>
        <div class="container-menu">
            <div class="content-menu">
                <div class="text-menu">
                    <div class="content-text">
                        <img src="@/assets/images/patterns/pattern-divide.svg" alt="">
                        <h3>A faw highlights from our menu</h3>
                        <p>We cater for all dietary requirements, but here’s a glimpse at some of our diner’s favourites. Our menu is revamped every season.</p>
                    </div>
                </div>
                <div class="menu-picture">
                    <div class="bloc">
                        <div>
                            <img src="@/assets/images/homepage/salmon-mobile.jpg" alt="">
                        </div>
                        <div class="bloc-text">
                            <h4>Seared Salmon Filet</h4>
                            <p>Our locally sourced salmon served with a refreshing buckwheat summer salad</p>
                        </div>
                    </div>
                    <div class="line"></div>
                    <div class="bloc">
                        <div>
                            <img src="@/assets/images/homepage/beef-mobile.jpg" alt="">
                        </div>
                        <div class="bloc-text">
                            <h4>Rosemary Filet Mignon</h4>
                            <p>Our prime beef served to your taste with a delicious choice of seasonal sides.</p>
                        </div>
                    </div>
                    <div class="line"></div>
                    <div class="bloc">
                        <div>
                            <img src="@/assets/images/homepage/chocolate-mobile.jpg" alt="">
                        </div>
                        <div class="bloc-text">
                            <h4>Summer Fruit Chocolate Mousse</h4>
                            <p>Creamy mousse combined with summer fruits and dark chocolate shavings.</p>
                        </div>
                    </div>
                </div>
            </div>

        </div>
    </section>
</template>

<style scoped lang="scss">
@use '@/assets/base.scss';
.container-menu {
    height: 250vh;
    background-color: var(--primary-2);
    color: var(--white-1);
    .content-menu {
        width: 90%;
        height: 100%;
        margin: auto;
        .text-menu {
            height: 20%;
            display: flex;
            justify-content: center;
            align-items: center;
            .content-text {
                height: 70%;
                display: flex;
                flex-direction: column;
                align-items: center;
                justify-content: space-around;
                p {
                    text-align: center;
                }
            }
        }
        .menu-picture {
            width: 100%;
            height: 80%;
            display: flex;
            flex-direction: column;
            justify-content: space-around;
            .bloc {
                display: flex;
                flex-direction: column;
                justify-content: space-between;
                align-items: center;
                height: 30%;
                img {
                    width: 100%;
                }
                p {
                    text-align: center;
                }
                .bloc-text {
                    display: flex;
                    flex-direction: column;
                    align-items: center;
                }
            }
            .line {
                height: 1px;
                width: 100%;
                background-color: var(--white-1);
            }
        }
    }
}


@media (min-width: 768px) {
        .container-menu {
            height: 160vh;
        .content-menu {
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            .text-menu {
                height: 30%;
                width: 80%;
                margin: auto;
                .content-text {
                    
                    h2 {
                        text-align: center;
                    }
                }
            }
            .menu-picture {
                
                height: 65%;
                width: 80%;
                margin: auto;
                justify-content: space-around;
                .bloc {
                    flex-direction: row;
                    height: 25%;
                    img {
                       height: 100%;
                       width: 75%;
                    }
                  
                }
            }
        }
    }
}

@media (min-width: 1023px) {
    .container-menu {
            height: 100vh;
            display: flex;
            align-items: center;
        .content-menu {
            display: flex;
            flex-direction: row;
            justify-content: flex-start;
            width: 80%;
            height: 80%;
            .text-menu {
                width: 40%;
                height: 70%;
                align-items: start;
                .content-text {
                    height: 75%;
                    width: 80%;
                    align-items: start;
                }
            }
            .menu-picture {
                width: 45%;
             
                .bloc {
                    
                    img {
                       
                    }
                  
                }
            }
        }
    }
}
</style>
