<template>
    <section>
        <div class="text-container">
            <h1>change a life today</h1>
            <div class="text-separator"></div>
            <p>As long as poverty, injustice & inequality persist, none of us can truly rest. It doesn’t take much to change a life, Get in touch today and start making the difference.</p>
        </div>
        <div class="button-container">
            <button>volunteer</button>
            <button>donate now</button>
        </div>
    </section>
</template>

<script>
export default {
    name: 'SecondJumbotron'    
}
</script>

<style lang="scss" scoped>
    section{
        height: 80vh;
        background-image: url('../assets/img/home-footer.jpg');
        background-size: cover;
        background-position: center center;
        margin-top: 15vh;
            .text-container{
                display: flex;
                flex-direction: column;
                align-items: center;
                padding-top: 100px;
                    h1{
                        text-transform: uppercase;
                        color: white;
                        font-weight: 300;
                    }
                    .text-separator{
                        margin-top: 20px;
                    }
                    p{
                        margin-top: 40px;
                        font-size: 24px;
                        max-width: 900px;
                        text-align: center;
                        color: #fff;
                    }
                    
            }
            .button-container{
                width: 80%;
                margin: auto;
                display: flex;
                justify-content: center;
                padding-top: 30px;  
                    button{
                         padding: 10px 30px;
                         border: 2px solid white;
                         background-color: transparent;
                         color: white;
                         font-weight: 600;
                         text-transform: uppercase;
                         margin: 20px;
                            &:hover{
                                border: 2px solid #fcd66c;
                                color: #fcd66c;
                                transition: 0.3s;
                            }
                    }
            }
    }
</style>