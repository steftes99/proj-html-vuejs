<template>
    <section>
        <div class="text-container">
            <h1>latest articles</h1>
            <div class="text-separator"></div>
        </div>
        <p>Together we make all the difference</p>
        <div class="articles-container">
            <div class="card">
                <img src="../assets/img/photo-1444213007800-cff19e1677ac.jpg" alt="">
                <h3>Understanding community complexities</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Prasent ac nibh vestibulum, laoreet ipsum.</p>
            </div>
            <div class="articles">
                <div class="article">
                    <img src="../assets/img/photo-1444664597500-035db93e2323-177x142.jpg" alt="">
                    <div class="text-wrapper">
                        <span class="yellow">Sustainable trade tactics</span> <br>
                        <span>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Prasent ac nibh vestibulum, laoreet ipsum.</span>
                    </div>
                   
                </div>
                <div class="article">
                    <img src="../assets/img/photo-1447430617419-95715602278e-177x142.jpg" alt="">
                   <div class="text-wrapper">
                        <span class="yellow">The human story of uniqueness</span> <br>
                        <span>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Prasent ac nibh vestibulum, laoreet ipsum.</span>
                    </div>
                </div>
                <div class="article">
                    <img src="../assets/img/photo-1460230525622-630fe3294cd7-177x142.jpg" alt="">
                   <div class="text-wrapper">
                        <span class="yellow">Farmers making a difference</span> <br>
                        <span>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Prasent ac nibh vestibulum, laoreet ipsum.</span>
                    </div>
                </div>
                <div class="article">
                    <img src="../assets/img/photo-1460600421604-5e138c208b9c-177x142.jpg" alt="">
                    <div class="text-wrapper">
                        <span class="yellow">Meeting remote tribes in Peru</span> <br>
                        <span>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Prasent ac nibh vestibulum, laoreet ipsum.</span>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Articles'
}
</script>

<style lang="scss" scoped>
    .text-container{
        display: flex;
        flex-direction: column;
        align-items: center;
        margin-top: 100px;
            h1{
                text-transform: uppercase;
                font-weight: 300;
                margin-bottom: 20px;
            }
    }
    p{
         margin-top: 50px;
         margin-left: 150px;
         color: #78787b;
    }
    .articles-container{
        width: 80%;
        margin: auto;
        margin-top: 80px;
        display: flex;
        justify-content: center;
        
            .card{
                width: 50%;
                border: 1px solid lightgray;
              
                    h3{
                        color: #fcd66c;
                        font-weight: 300;
                        margin-top: 30px;
                        margin-left: 20px;
                    }
                    p{
                        margin-top: 0;
                        margin-left: 20px;
                        line-height: 30px;
                    }
            }
            .articles{
                width: 45%;
                margin-left: 5%;
                    .article{
                        margin: 0 0 6% 0;
                        display: flex;
                            img{
                                width: 30%;
                                display: inline-block;
                                &:hover{
                                    transform: scale(1.05);
                                    transition: 0.3s;
                                    cursor: pointer;
                                }
                            }
                            .text-wrapper{
                                display: inline-block;
                                margin-top: 10px;
                                margin-left: 10px;
                                    span{
                                        line-height: 30px;
                                        color: #78787b;
                                    }
                                    .yellow{
                                        color: #fcd66c;
                                        font-size: 18px;
                                        letter-spacing: 3px;
                                    }
                            }
                    }
            }
    }
</style>