<template>
  
  <div>
      <div class="container-img">
        <img :src="url" :alt="title">
      </div>
      <h3>{{ title }}</h3>
  </div>
</template>

<script>
export default {
    name: 'Card',
        props:{
            url: String,
            title: String,
        }
    }
</script>

<style lang="scss" scoped>

    div{
        div.container-img{
            height: 160px;

            img{
                object-fit: cover;
                object-position: top;
                width: 100%;
                height: 100%;
            }
        }

        h3{
            margin-top: 10px;
        }
    }

</style>