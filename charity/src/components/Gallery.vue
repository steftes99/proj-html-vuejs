<template>
    <section>
        <div class="text-container">
            <h1>recent causes</h1>
            <div class="text-separator"></div>
        </div>
        <p>We run projects in over 30 countries in 5 contintents</p>
        <div class="gallery">
            <div class="img-container">
                <img src="../assets/img/avada-charity-fair-trade-featured.jpg" alt="">
                <div class="img-hover">
                    <h3>fair trade</h3>
                </div>
            </div>

            <div class="img-container">
                <img src="../assets/img/avada-charity-shelter-featured.jpg" alt="">
                <div class="img-hover">
                    <h3>shelter</h3>
                </div>
            </div>

            <div class="img-container">
                <img src="../assets/img/avada-charity-farming-featured.jpg" alt="">
                <div class="img-hover">
                    <h3>farming</h3>
                </div>
            </div>

            <div class="img-container">
                <img src="../assets/img/avada-charity-vaccines-featured.jpg" alt="">
                <div class="img-hover">
                    <h3>vaccines</h3>
                </div>
            </div>
            

            
            
            
        </div>

        <button>view all our causes</button>
        
    </section>
</template>

<script>
export default {
    name: 'Gallery'
}
</script>

<style lang="scss" scoped>
    section{
        
            .text-container{
                display: flex;
                flex-direction: column;
                align-items: center;
                margin-top: 100px;
                    h1{
                        text-transform: uppercase;
                        font-weight: 300;
                        margin-bottom: 30px;
                    }
            }
            p{
                margin-top: 50px;
                margin-left: 350px;
                color: #78787b;
            }
            .gallery{
                width: 80%;
                margin: auto;
                display: flex;
                justify-content: center;
                margin-top: 100px;
                    .img-container{
                        width: 25%;
                        margin: 10px;
                        position: relative;
                            &:hover .img-hover, h3{
                                display: block;
                                transition: 1s;
                            }
                    }
                    img{
                        width: 100%;
                    }
            }
            button{
                margin-top: 100px;
                width: 100%;
                height: 150px;
                border: none;
                background-color: #ed6864;
                color: white;
                text-transform: uppercase;
                letter-spacing: 3px;
                font-weight: 500;
                &:hover{
                    background-color: #408292;
                    transition: 0.5s;
                }
            }
    }
</style>