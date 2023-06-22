<script setup lang="ts">

</script>

<template>
 
    <section>
        <div class="container-localy">
            <div class="content-localy">
                <div class="picture">
                </div>
                <div class="text-localy">
                    <div class="text-content">
                        <img src="@/assets/images/patterns/pattern-divide.svg" alt="">
                        <h3>The most locally sourced food</h3>
                        <p>All our ingredients come directly from our farm or local fishery. So you can be sure that you’re eating the freshest, most sustainable food.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

</template>

<style scoped lang="scss">
@use '@/assets/base.scss';

.container-localy {
    height: 100vh;
    .content-localy {
        height: 100%;
        width: 90%;
        margin: auto;

        .picture {
            height: 50%;
            background-image: url(@/assets/images/homepage/locally-sourced-mobile.jpg);
            background-size: cover;
            background-position: center;
            box-shadow: rgba(0, 0, 0, 0.2) 0px 15px 45px;

        }
        .text-localy {
            height: 50%;
            display: flex;
            align-items: center;
            img {
                width: 20%;
            }
            .text-content {
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
    }
}

@media (min-width: 768px) {
    .container-localy {
        .content-localy {
            .picture {
                background-image: url(@/assets/images/homepage/locally-sourced-tablet.jpg);
                top: -10%;
                width: 90%;
                margin: auto;
            }
            .text-localy {
                height:50%;
                justify-content: center;
                .text-content {
                    height: 60%;
                    width: 60%;
                    justify-content: space-between;
                    p {
                        text-align: center;
                    }
                }
            } 
        }
    }   
}

@media (min-width: 1023px) {
    .container-localy {
        .content-localy {
            position: relative;
            top: 5%;
            display: flex;
            flex-direction: row-reverse;
            width: 80%;
            .picture {
                background-image: url(@/assets/images/homepage/locally-sourced-desktop.jpg);
                height: 100%;
                width: 60%;
                top: -7%;
            }
            .text-localy {
                height: 90%;
                .text-content {
                   height: 50%;
                }
            } 
        }
    }   
}
</style>
