<template>
    <section>
        <div class="container-left clearfix">
            <div class="text-container">
                <h1>every moment counts</h1>
                <div class="text-separator">

                </div>
                <p>Curabitur non mi et turpis pharetra vulputate. Cras consequat, risus nec commodo vehicula, nisi est laoreet leo, ac convallis nisi nibh id velit. Aliquam mattis metus a nisi pretium.</p>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent ac nibh vestibulum, laoreet ipsum quis, vestibulum nisi. Curabitur non mi et turpis pharetra vulputate. Ipsum dolor sit amet, consectetur adipiscing elit. Praesent ac nibh vestibulum, laoreet ipsum quis, vestibulum nisi.</p>
                <p>Curabitur non mi et turpis pharetra vulputate. Cras consequat, risus nec commodo vehicula, nisi est laoreet leo, ac convallis nisi nibh id velit.</p>
                <button>our mission</button>
            </div>
        </div>
        <div class="container-right clearfix">
            <div class="icon-container">
                <p><i class="far fa-heart"></i> 2032</p>
                <span>Volunteers worldwide</span>
            </div>
            <div class="icon-container">
                <p><i class="fas fa-globe-americas"></i>132</p>
                <span>Active projects</span>
            </div>
            <div class="icon-container">
                <p>$ 3.8M</p>
                <span>Donated</span>
            </div>
           
        </div>
    </section>
    
</template>

<script>
export default {
    name: 'FirstSection'
}
</script>

<style lang="scss" scoped>
    section{
        height: 90vh;
        
            .container-left{
                width: 65%;
                height: 100%;
                float: left;
                
                    .text-container{
                        width: 80%;
                        height: 80%;
                        margin: auto;
                        
                            h1{
                                text-transform: uppercase;
                                font-weight: 400;
                                letter-spacing: 2px;
                                margin: 70px 0 30px 0;
                            }
                           
                            p{
                                color: #78787b;
                                font-size: 18px;
                                margin: 50px 0;
                                font-weight: 300;
                            }
                            button{
                                padding: 10px 30px;
                                border: none;
                                background-color: #fcd66c;
                                color: white;
                                font-weight: 600;
                                text-transform: uppercase;
                                    &:hover{
                                        background-color: black;
                                        transition: 0.3s;
                                    }
                                
                            }
                    }
            }
            .container-right{
                width: 35%;
                height: 100%;
                float: right;
                background-image: url('../assets/img/home-content-bg-1.jpg');
                background-size: cover;
                    .icon-container{
                        text-align: center;
                        color: white;
                        margin-top: 70px;
                            p{
                                font-size: 50px;
                            }
                            span{
                                font-size: 24px;
                            }
                    }

            }
    }
</style>