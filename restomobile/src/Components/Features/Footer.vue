<script setup lang="ts">


</script>

<template>
 
  <section>
    <div class="container-footer">
        <div class="content-footer">
            <div class="content-logo">
                <div class="logo-part">
                    <img src="@/assets/images/logo.svg" alt="">
                </div>
            </div>
            <div class="content-diner">
                <div class="name-diner">
                    <h3>MARTHWAITE, SEDBERGH CUMBRIA</h3>
                    <p>+00 44 123 4567</p>
                </div>
                <div class="open-times">
                    <h3>OPEN TIMES</h3>
                    <p>MON - FRI: 09:00 AM - 10:00 PM</p>
                    <p>SAT - SUN: 09:00 AM - 11:30 PM</p>
                </div>
            </div>
        </div>
    </div>
</section>

</template>

<style scoped lang="scss">
@use '@/assets/base.scss';
    .container-footer {
        height: 60vh;
        background-color: var(--primary-2);
        color: var(--white-1);
        display: flex;
        justify-content: center;
        align-items: center;
        .content-footer {
            height: 90%;
            width: 80%;
            display: flex;
            flex-direction: column;
            justify-content: space-around;
            align-items: center;
           
            .content-diner {
                height: 70%;
                width: 100%;
                display: flex;
                flex-direction: column;
                justify-content: space-around;
                .open-times, .name-diner {
                    display: flex;
                    flex-direction: column;
                    justify-content: center;
                    align-items: center;
                }
            }
         
        }
    }

@media (min-width: 768px) {

    .container-footer {
        height: 50vh;
       
        .content-footer {        
            flex-direction: row;  
            height: 80%;
            width: 90%;
            .content-logo {
                height: 100%;
            } 
            .content-diner {
                width: 50%;
                height: 100%;
                justify-content: space-between;
                .open-times, .name-diner {
                    align-items: start;
                   height: 40%;
                }
            }
         
        }
    }

}
@media (min-width: 1023px) {

    .container-footer {
        height: 30vh;
       
        .content-footer {        
            flex-direction: row;  
            height: 60%;
            width: 90%;
            .content-logo {
                height: 100%;
            } 
            .content-diner {
                width: 70%;
                height: 100%;
                flex-direction: row;
                justify-content: space-between;
                .open-times, .name-diner {
                    height: 100%;
                }
            }
         
        }
    }
}
</style>
