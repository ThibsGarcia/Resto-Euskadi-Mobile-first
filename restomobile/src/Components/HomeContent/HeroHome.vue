<script setup >

</script>

<template>
 
    <section>
        <div class="hero-container">
            <div class="hero-content">
                <div class="logo-hero">
                    <img src="@/assets/images/logo.svg" alt="">
                </div>
                <div class="text-hero">
                    <div class="title">
                        <h2>Exquisite dining since 1989</h2>
                    </div>
                    <div class="paragraphe">
                        Experience our seasonal menu in beautiful country surroundings. Eat the freshest produce from the comfort of our farmhouse.
                    </div>
                </div>
                <div class="btn-book">
                    <button class="btn-1">BOOK A TABLE</button>
                </div>
            </div>
        </div>
    </section>

</template>

<style scoped lang="scss">
@use '@/assets/base.scss';
.hero-container {
    height: 100vh;
    background-image: url(@/assets/images/homepage/hero-bg-mobile.jpg);
    background-size: cover;
    background-position: center;
    color: white;
    display: flex;
    align-items: center;
}
.hero-content {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
    height: 60%;
}
.logo-hero {
    height: 15%;
    display: flex;
    align-items: end;
}
.text-hero {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 80%;
}
@media (min-width: 768px) {
    .hero-container {
        background-image: url(@/assets/images/homepage/hero-bg-tablet.jpg);
    }
}
@media (min-width: 1024px) {
    .hero-container {
        background-image: url(@/assets/images/homepage/hero-bg-desktop.jpg);
        align-items: center;
        justify-content: center;
    }
    .hero-content {
        width: 80%;
        height: 80%;
        align-items: start;
    }
    .logo-hero {
        height: 0%;
    }
    .text-hero {
        justify-content: space-around;
        width: 60%;
        height: 40%;
        align-items: start; 
    }
    .paragraphe {
        width: 60%;
    }
}
</style>
