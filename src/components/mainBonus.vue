<template>
  
    <section>
        <div class="container">

            <ul>
                <li v-for="(element, i) in bonusSection" :key="`element-${i}`">

                    <div class="container-image">
                        <img :src="element.link" :alt="element.text">
                    </div>
                    <a href="#">{{element.text}}</a>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
export default {
    name: 'mainBonus',
    data() {
        return {
            bonusSection: [
                {
                    text: 'digital comics',
                    link: require('@/assets/img/buy-comics-digital-comics.png'),
                },
                {
                    text: 'dc merchandise',
                    link: require('@/assets/img/buy-comics-merchandise.png'),
                },
                {
                    text: 'subscription',
                    link: require('@/assets/img/buy-comics-subscriptions.png'),
                },
                {
                    text: 'comic shop locator',
                    link: require('@/assets/img/buy-comics-shop-locator.png'),
                },
                {
                    text: 'dc power visa',
                    link: require('@/assets/img/buy-dc-power-visa.svg'),
                },
            ],
        }
    },
}
</script>

<style lang="scss" scoped>

    section{
        background-color: #0c7cec;

        div.container{

            padding: 20px 0;

            ul{
                display: flex;

                li{
                    width: calc(100% / 5);
                    display: flex;
                    align-items: center;

                    div.container-image{
                        width: 50px;

                        img{
    
                            width: 100%;
                        }
                    }
                    a{
                        margin-left: 10px;
                        color: white;
                        text-transform: uppercase;
                        font-weight: bold;
                        text-decoration: none;
                    }

                    transition: transform 0.3s;

                    &:hover{
                        transform: scale(1.1);
                    }
                }
            }
    
        }
    }
</style>