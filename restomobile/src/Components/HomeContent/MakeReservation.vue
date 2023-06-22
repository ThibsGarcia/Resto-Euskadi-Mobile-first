<script setup lang="ts">


</script>

<template>
 
  <section>
    <div class="container-reservation">
        <div class="content-reservation">
            <div class="title-reservation">
                <h3>Ready to make a reservation?</h3>
            </div>
            <div class="btn-reservation">
                <button class="btn-4">BOOK A TABLE</button>
            </div>
        </div>
    </div>
 </section>

</template>

<style scoped lang="scss">
@use '@/assets/base.scss';
.container-reservation {
    height: 50vh;
    background-image: url(@/assets/images/homepage/ready-bg-mobile.jpg);
    background-size: cover;
    color: var(--white-1);
    display: flex;
    align-items: center;
    justify-content: center;
    .content-reservation {
        height: 60%;
        display: flex;
        flex-direction: column;
        justify-content: space-around;
        align-items: center;
    }
}
@media (min-width: 768px) {
    .container-reservation {
        height: 40vh;
        background-image: url(@/assets/images/homepage/ready-bg-tablet.jpg);
        .content-reservation {
            height: 70%;
        }
    }
}

@media (min-width: 1023px) {
    .container-reservation {
        height: 40vh;
        background-image: url(@/assets/images/homepage/ready-bg-desktop.jpg);
        .content-reservation {
            flex-direction: row;
            display: flex;
            justify-content: space-around;
            height: 70%;
            width: 80%;
        }
    }
}
</style>
