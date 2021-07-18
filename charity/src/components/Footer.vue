<template>
    <footer>
       <div class="footer-top">
           <img src="../assets/img/avada-charity-mobile-logo.png" alt="">
       </div>
       <div class="footer-bottom">
           <p>© Copyright 2012 - 2021 | Avada Theme by <span>ThemeFusion</span> | All Rights Reserved | Powered by <span>WordPress</span></p>
            <ul>
                <li v-for="icon in socialIcons" :key="icon">
                    <span v-html="icon"></span>
                </li>
            </ul>
       </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer',
    props: {
        socialIcons: Array
    }
}
</script>

<style lang="scss" scoped>
    footer{
        height: 50vh;
            .footer-top{
                height: 50%;
                display: flex;
                justify-content: center;
                align-items: center;
                    img{
                        width: 20%;
                    }
            }
            .footer-bottom{
                height: 50%;
                background-color: #F5F5F5;
                    p{
                        text-align: center;
                        padding-top: 50px;
                        font-size: 14px;
                            span{
                                color: #fcd66c;
                            }
                    }
                    ul{
                        list-style: none;
                        display: flex;
                        justify-content: center;
                            li{
                                margin: 20px;
                                font-size: 20px;
                                color: #fcd66c;
                                background-color: white;
                                border-radius: 50%;
                                padding: 5px;
                                    &:hover{
                                        cursor: pointer;
                                    }
                            }
                    }
            }
        
    }
</style>