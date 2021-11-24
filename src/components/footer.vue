<template>
  <section>
      <div class="container">

        <nav class="nav-footer">

            <!-- col uno -->
            <div class="col">
                
                <ul class="dc-comics">

                    <h3>dc comics</h3>

                    <li tabindex="0" v-for="(element, i) in linkDcComics" :key="`element-${i}`">
                        <a href="">{{element.text}}</a>
                    </li>
                </ul>

                <ul class="dc">

                    <h3>shop</h3>

                    <li tabindex="0" v-for="(element, i) in linkShop" :key="`element-${i}`">
                        <a href="">{{element.text}}</a>
                    </li>
                </ul>
            </div>

            <!-- col due -->
            <div class="col">
                
                <ul class="dc-comics">

                    <h3>dc</h3>

                    <li tabindex="0" v-for="(element, i) in linkDc" :key="`element-${i}`">
                        <a href="">{{element.text}}</a>
                    </li>
                </ul>
            </div>

            <!-- col tre -->
            <div class="col">
                
                <ul class="dc-comics">

                    <h3>sites</h3>

                    <li tabindex="0" v-for="(element, i) in linkSites" :key="`element-${i}`">
                        <a href="">{{element.text}}</a>
                    </li>
                </ul>
            </div>

        </nav>

        <div class="image-dc-back">

        </div>
        <!-- <img src="@/assets/dc-logo-bg.png" alt=""> -->

      </div>
  </section>
</template>

<script>
export default {
    name: 'Footer',
    data() {
        return {
            linkDcComics: [
                {
                    text: 'characters',
                },
                {
                    text: 'comics',
                },
                {
                    text: 'movies',
                },
                {
                    text: 'tv',
                },
                {
                    text: 'games',
                },
                {
                    text: 'videos',
                },
                {
                    text: 'news',
                },
            ],
            linkShop: [
                {
                    text: 'Shop DC',
                },
                {
                    text: 'Shop DC Collectibles',
                },
            ],
            linkDc: [
                {
                    text: 'Terms Of Use',
                },
                {
                    text: 'Privacy policy (New)',
                },
                {
                    text: 'Ad Choices',
                },
                {
                    text: 'Advertising',
                },
                {
                    text: 'Jobs',
                },
                {
                    text: 'Subscription',
                },
                {
                    text: 'Talent',
                },
                {
                    text: 'CPSC Certificates',
                },
                {
                    text: 'Ratings',
                },
                {
                    text: 'Shop Help',
                },
                {
                    text: 'Contact Us',
                },
            ],
            linkSites: [
                {
                    text: 'DC',
                },
                {
                    text: 'MAD Magazine',
                },
                {
                    text: 'DC Kids',
                },
                {
                    text: 'DC Universe',
                },
                {
                    text: 'DC Power Visa',
                },
            ],
        }
    },
}
</script>

<style lang="scss" scoped>

    section{
        background-image: url('../assets/footer-bg.jpg');
        background-repeat: no-repeat;
        background-size: cover;
        /* height: 450px; */
        overflow: hidden;

        .container{
            height: 100%;
            display: flex;
            justify-content: space-between;

            div.image-dc-back{
                background-image: url('../assets/dc-logo-bg.png');
                background-repeat: no-repeat;
                background-position: center;
                z-index: 1;
                width: 50%;
            }

            nav{

                min-width: 50%;
                padding: 20px;
                display: flex;

                div.col:nth-child(2){
                    margin: 0px 30px;
                }

                div.col{

                    ul{
                        list-style: none;
                        margin-bottom: 30px;
    
                        h3{
                            color: white;
                            margin-bottom: 15px;
                            text-transform: uppercase;
                        }
                        li{
                            margin: 8px 0;

                            a{
                                text-decoration: none;
                                color: #959595;
                                border: 0;
                            }
                        }
                    }
                }
            }
        }
    }
</style>