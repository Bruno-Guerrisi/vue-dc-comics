<template>
  <header>

    <div class="container">
        <img src="@/assets/dc-logo.png" alt="dc logo">

        <ul>
            <li tabindex="0" v-for="(element, i) in linkNav" :key="`element-${i}`">
                <a href="">{{element.text}}</a>
                </li>
        </ul>
    </div>
  </header>
</template>

<script>
export default {
    name: 'Header',
    data() {
        return {
            linkNav: [
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
                    text: 'collectibles',
                },
                {
                    text: 'videos',
                },
                {
                    text: 'fans',
                },
                {
                    text: 'news',
                },
                {
                    text: 'shop',
                },
            ],
        }
    },
}
</script>

<style lang="scss" scoped>

    header{
        height: 120px;
        padding: 10px 20px;

        .container{


            display: flex;
            align-items: center;
            justify-content: space-between;
    
            ul{
                display: flex;
                align-items: center;
                list-style: none;
                height: 100%;
    
                li{
                    margin: 0 10px;
                    text-transform: uppercase;
                    height: 100%;
                    display: flex;
                    align-items: center;
                    border-bottom: 5px solid transparent;
    
                    &:focus,
                    &:hover{
                        border-bottom-color: #0c7cec;
                        color: #0c7cec;
                        cursor: pointer;
                    }
    
                    a{
                        text-decoration: none;
                        color: currentColor;
                        border: 0;
                    }
                }
    
            }
        }
    }
</style>
