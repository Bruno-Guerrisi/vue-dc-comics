<template>
  <footer>
      <div class="container">

        <nav class="nav-footer">

            <div class="col">
                
                <ul class="dc-comics">

                    <h3>DC COMICS</h3>

                    <li tabindex="0" v-for="(element, i) in linkDcComics" :key="`element-${i}`">
                        <a href="">{{element.text}}</a>
                    </li>
                </ul>

                <ul class="dc">

                    <h3>SHOP</h3>

                    <li tabindex="0" v-for="(element, i) in linkDc" :key="`element-${i}`">
                        <a href="">{{element.text}}</a>
                    </li>
                </ul>
            </div>

        </nav>

        <img src="@/assets/dc-logo-bg.png" alt="">

      </div>
  </footer>
</template>

<script>
export default {
    name: 'Header',
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
            linkDc: [
                {
                    text: 'Shop DC',
                },
                {
                    text: 'Shop DC Collectibles',
                },
            ],
        }
    },
}
</script>

<style lang="scss" scoped>

    footer{
        background-image: url('../assets/footer-bg.jpg');
        background-repeat: no-repeat;
        height: 450px;
        margin-bottom: 20px;
        overflow: hidden;

        .container{
            padding: 20px 0;
            display: flex;
            justify-content: space-between;

            img{
                position: relative;
                top: -50px;
            }

            nav{

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