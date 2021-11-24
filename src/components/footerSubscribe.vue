<template>
  <section>
      <div class="container">

        <button>sign-up now!</button>

        <div class="follow-us">
            <span>follow us</span>

            <ul>
                <li v-for="(element, i) in linkSocial" :key="`element-${i}`">
                    <a href="">
                        
                        <img :src="element.link" alt="element.text">
                    </a>
                </li>
            </ul>
        </div>

      </div>
  </section>
</template>

<script>
export default {
    name: 'FooterSubscribe',
    data() {
        return {
            linkSocial: [
                {
                    text: 'facebook',
                    link: require('@/assets/img/footer-facebook.png'),
                },
                {
                    text: 'twitter',
                    link: require('@/assets/img/footer-twitter.png'),
                },
                {
                    text: 'youtube',
                    link: require('@/assets/img/footer-youtube.png'),
                },
                {
                    text: 'pinterest',
                    link: require('@/assets/img/footer-pinterest.png'),
                },
                {
                    text: 'periscope',
                    link: require('@/assets/img/footer-periscope.png'),
                },
            ],
        }
    },
}
</script>

<style lang="scss" scoped>

    section{
        background-color: #303030;
        height: 100px;
        padding: 10px 20px;
        display: flex;
        align-items: center;

        .container{

            width: 100%;
            display: flex;
            align-items: center;
            justify-content: space-between;

            button{
                padding: 10px;
                text-transform: uppercase;
                color: white;
                border: 3px solid #0c7cec;
                background-color: unset;
                font-weight: bold;
                font-size: 16px;
                cursor: pointer;
                transition: transform 0.3s;

                &:hover{
                    transform: scale(1.1);
                }
            }

            div.follow-us{
                display: flex;
                align-items: center;

                span{
                    color: #0c7cec;
                    text-transform: uppercase;
                    font-weight: bold;
                    margin-right: 15px;
                }

                ul{
                    list-style: none;
                    display: flex;
                    
                    li{
                        margin-right: 8px;

                        transition: transform 0.3s;

                        &:hover{
                            transform: scale(1.1);
                        }
                    }
                    li:last-of-type{
                        margin-right: 0;
                    }
                }
            }
        }
    }
</style>