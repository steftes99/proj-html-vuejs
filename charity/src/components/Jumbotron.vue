<template>
    <section>
        <div class="title-container">
            <h1>our values</h1>
            <div class="text-separator"></div>
        </div>

        <ul>
            <li v-for="item in listItems" :key="item.message">
                <span v-html="item.icon"></span>
                <h3>{{item.message}}</h3>
                <p>Nullam convallis, orci in congue aliquet, diam mauris cursus urna, Id maximus lectus magna maximus.</p>
                <button>learn more</button>

            </li>
        </ul>
       
    </section>
</template>

<script>
export default {
    name: 'Jumbotron',
    props: {
        listItems: Array
    }
    
}
</script>

<style lang="scss" scoped>
    section{
        height: 130vh;
        background-image: url('../assets/img/home-content-bg-2.jpg');
        background-size: cover;
            .title-container{
                padding-top: 150px;
                display: flex;
                flex-direction: column;
                align-items: center;
                    h1{
                        color: white;
                        text-transform: uppercase;
                        font-weight: 300;
                        letter-spacing: 2px;
                        padding-bottom: 10px;
                    }
        }
        ul{
            text-align: center;
            margin-top: 40px;
                li{
                    display: inline-block;
                    color: white;
                    margin: 10px;
                    text-align: center;
                    margin-top: 180px;
                        span{
                            font-size: 60px;
                            color: #fcd66c;
                        }
                        h3{
                            font-weight: 300;
                            margin-top: 10px;
                        }
                        p{
                            margin: 30px;
                            max-width: 250px;
                            line-height: 40px;
                            color: #ccd0d1;
                            
                        }
                        button{
                                padding: 10px 30px;
                                border: none;
                                background-color: #fcd66c;
                                color: white;
                                font-weight: 600;
                                text-transform: uppercase;
                                margin-top: 20px;
                        }
                }
        }
       
    }
</style>