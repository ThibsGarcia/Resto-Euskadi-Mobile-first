<script setup lang="ts">

</script>

<template>
 
    <section>
        <div class="container-enjoyable">
            <div class="content-enjoyable">
                <div class="picture">

                </div>
                <div class="text-enjoyable">
                    <div class="text-content">
                        <img src="@/assets/images/patterns/pattern-divide.svg" alt="">
                        <h3>Enjoyable place for all the family</h3>
                        <p>Our relaxed surroundings make dining with us a great experience for everyone. We can even arrange a tour of the farm before your meal.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

</template>

<style scoped lang="scss">
@use '@/assets/base.scss';

.container-enjoyable {
    height: 100vh;

    .content-enjoyable {

        height: 100%;
        width: 90%;
        margin: auto;

        .picture {
            position: relative;
            top: -5%;
            height: 60%;
            background-image: url(@/assets/images/homepage/enjoyable-place-mobile.jpg);
            background-size: cover;
            background-position: center;
            box-shadow: rgba(0, 0, 0, 0.2) 0px 15px 45px;

        }
        .text-enjoyable {
            height: 40%;
            display: flex;
            align-items: center;
            img {
                width: 20%;
            }
            .text-content {
                height: 80%;
                display: flex;
                flex-direction: column;
                align-items: center;
                justify-content: space-around;
            }
        }
    }
}

@media (min-width: 768px) {
    .container-enjoyable {
        .content-enjoyable {
            .picture {
                background-image: url(@/assets/images/homepage/enjoyable-place-tablet.jpg);
                top: -10%;
                width: 90%;
                margin: auto;
            }
            .text-enjoyable {
                height:35%;
                justify-content: center;
                .text-content {
                    height: 100%;
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
    .container-enjoyable {
        .content-enjoyable {
            display: flex;
            width: 80%;
            .picture {
                background-image: url(@/assets/images/homepage/enjoyable-place-desktop.jpg);
                height: 100%;
                width: 60%;
                top: -7%;
            }
            .text-enjoyable {
                height: 90%;
                .text-content {
                   height: 50%;
                }
            } 
        }
    }   
}
</style>
