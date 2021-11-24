<template>
  <section>
      <div class="container">

        <div class="title">
          <span>current series</span>
        </div>

        <ul>
          <li v-for="(element, i) in comicsSeries" :key="`element-${i}`">
            <Card :url="element.thumb" :title="element.series" />
          </li>
        </ul>

        <div class="load-other">
          <button>load more</button>
        </div>
      </div>
  </section>
</template>

<script>
import series from "@/data/dc-comics.js"
import Card from "@/components/Card.vue"

export default {
  name: 'main',
  components:{
    Card,
  },
  data(){
    return{
      comicsSeries: series,
    };
  },
}
</script>

<style lang="scss" scoped>

    section{
        background-color: #1c1c1c;
        color: white;
        padding: 10px 20px;
        
        .container{

          div.title{
              position: relative;
              top: -30px;
              margin-bottom: 20px;

            span{
              font-size: 18px;
              padding: 20px;
              text-transform: uppercase;
              background-color: #0c7cec;
              font-weight: bold;
            }
          }

          ul{
            display: flex;
            flex-wrap: wrap;

            li{
              cursor: pointer;
              list-style: none;
              padding: .5rem;
              width: calc(100% / 6);
              margin-bottom: 20px;
              transition: transform .3s;

              &:hover{
                transform: scale(1.1);
              }
            }
          }

          div.load-other{
            text-align: center;

            button{
              color: white;
              border: 0;
              font-size: 14px;
              padding: 10px 50px;
              text-transform: uppercase;
              background-color: #0c7cec;
              font-weight: bold;
              cursor: pointer;
              transition: transform .3s;
              margin-bottom: 20px;

              &:hover{
                transform: scale(1.1);
              }
            }
          }
        }
    }

</style>