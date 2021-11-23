<template>
  <footer>
      <div class="container">

        <button>sign-up now!</button>

        <div class="follow-us">
            <span>follow us</span>

            <ul>
                <li>
                    <a href="">
                        <img src="../assets/footer-facebook.png" alt="facebook">
                    </a>
                </li>
                
                <li>
                    <a href="">
                        <img src="../assets/footer-twitter.png" alt="twitter">
                    </a>
                </li>
                
                <li>
                    <a href="">
                        <img src="../assets/footer-youtube.png" alt="youtube">
                    </a>
                </li>
                
                <li>
                    <a href="">
                        <img src="../assets/footer-pinterest.png" alt="pinterest">
                    </a>
                </li>
                
                <li>
                    <a href="">
                        <img src="../assets/footer-periscope.png" alt="periscope">
                    </a>
                </li>
            </ul>
        </div>

      </div>
  </footer>
</template>

<script>
export default {
    name: 'FooterSubscribe',
    /* data() {
        return {
            linkSocial: [
                {
                    text: 'facebook',
                    link: '/footer-facebook.png',
                },
                {
                    text: 'twitter',
                    link: '/footer-twitter.png',
                },
                {
                    text: 'youtube',
                    link: '/footer-youtube.png',
                },
                {
                    text: 'pinterest',
                    link: '/footer-pinterest.png',
                },
                {
                    text: 'periscope',
                    link: '/footer-periscope.png',
                },
            ],
        }
    }, */
}
</script>

<style lang="scss" scoped>

    footer{
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