<template>
    <header>
        <div class="navbar-container">
            <div class="container-left">
                <img src="../assets/img/avada-charity-logo.png" alt="charity logo">
            </div>

            <div class="container-right">
                <ul>
                    <li v-for="item in items" :key="item.message">
                        {{ item.message }}
                    </li>
                </ul>
                <button>
                    donate
                </button>
            </div>
        </div>

        <div class="title-container">
            <h1>make a difference</h1>
            <p>As long as poverty, injustice & inequality persist, none of us can truly rest</p>
        </div>

        <div class="button-container">
            <button class="white">our mission</button>
            <button class="yellow">donate now</button>
        </div>


        
    </header>
</template>

<script>
export default {
    name: 'Header',
    props: {
        items: Array
    }
}

</script>

<style lang="scss" scoped>
     header{
        background-image: url('../assets/img/home-page-slider.jpg');
        background-size: cover;
        height: 100vh;
        margin: 0;
        padding: 0;
            .navbar-container{
                display: flex;
                justify-content: space-between;
                align-items: center;
                width: 90%;
                margin: auto;
                padding: 20px;
                    .container-left{
                        img{
                            width: 70%;
                        }
                    }
                    
                    .container-right{
                        display: flex;
                        justify-content: flex-start;
                        align-items: center;
                            ul{
                                list-style: none;
                                display: flex;
                                align-items: center;
                                    
                                    
                                    li{
                                        display: inline;
                                        color: white;
                                        text-transform: uppercase;
                                        margin: 35px;
                                            &:first-of-type{
                                            color: #fcd66c;
                                            }
                                            &:hover{
                                                color: #fcd66c;
                                                transition: 0.3s;
                                                cursor: pointer;
                                            }
                                           
                                    }
                            }
                            button{
                                padding: 10px 30px;
                                border: none;
                                background-color: #fcd66c;
                                color: white;
                                font-weight: 600;
                                text-transform: uppercase;
                                margin-bottom: 15px;    
                                    &:hover{
                                        background-color: black;
                                        transition: 0.3s;
                                    }
                            }
                    }
                   
            }
             .title-container{
                        width: 70%;
                        margin: auto;
                        margin-top: 130px;
                            h1{
                                color: white;
                                text-align: center;
                                text-transform: uppercase;
                                font-size: 86px;
                                font-weight: 400;
                            }
                            p{
                                color: white;
                                text-align: center;
                                font-size: 24px;
                            }
            }
            .button-container{
                width: 40%;
                margin: auto;
                display: flex;
                justify-content: center;
                    button{
                        padding: 10px 30px;
                        text-transform: uppercase;
                        background-color: transparent;
                        margin: 10px;
                        letter-spacing: 2px;
                           
                    }
                     .white{
                        border: 2px solid #fff;
                        color: #fff;
                            &:hover{
                               border: 2px solid #fcd66c;
                               color: #fcd66c; 
                               transition: 0.3s;
                            }
                    }
                    .yellow{
                        border: 2px solid #fcd66c;
                        color: #fcd66c;
                            &:hover{
                                border: 2px solid white;
                                color: white;
                                background-color: black;
                                transition: 0.3s;
                            }
                    }
            }
    }
</style>