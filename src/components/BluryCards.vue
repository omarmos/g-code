<template>
    <v-main>
   <link href="https://fonts.googleapis.com/css?family=Montserrat:400,700" rel="stylesheet">

<section class="hero-section">
   
  <div class="card-grid">
      <router-link class="card" :to="item.to" v-for="item in items" :key="item.id">
      <div class="card__background" :style="item.src"></div>
      <div class="card__content">
        <p class="card__category">{{ item.category}}</p>
        <h3 class="card__heading">{{item.heading}}</h3>
      </div>
      </router-link>
 </div>
      
</section>
    </v-main>
</template>

<script>
export default {
    name: 'BlurryCards',
    data() {
      return {
        items:[
          {
            id:1,
            to: '/menasave',
            src: 'background-image: url(https://images.unsplash.com/photo-1557177324-56c542165309?ixlib=rb-1.2.1&auto=format&fit=crop&w=1950&q=80)',
            category: 'Category',
            heading: 'Example Card Heading'
          },
           {
            id:2,
            to: '/menasave',
            src: 'background-image: url(https://images.unsplash.com/photo-1557004396-66e4174d7bf6?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=800&q=60)',
            category: 'Category',
            heading: 'Example Card Heading'
          },
           {
            id:3,
            to: '/menasave',
            src: 'background-image: url(https://images.unsplash.com/photo-1556680262-9990363a3e6d?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=800&q=60)',
            category: 'Category',
            heading: 'Example Card Heading'
          },
           {
            id:4,
            to: '/menasave',
            src: 'background-image: url(https://images.unsplash.com/photo-1557187666-4fd70cf76254?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=800&q=60)',
            category: 'Category',
            heading: 'Example Card Heading'
          },
           {
            id:5,
            to: '/menasave',
            src: 'background-image: url(https://images.unsplash.com/photo-1557187666-4fd70cf76254?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=800&q=60)',
            category: 'Category',
            heading: 'Example Card Heading'
          },
           {
            id:6,
            to: '/menasave',
            src: 'background-image: url(https://images.unsplash.com/photo-1556680262-9990363a3e6d?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=800&q=60)',
            category: 'Category',
            heading: 'Example Card Heading'
          }
        ]
      }
    },
}
</script>

<style lang="scss">
@import '../sass/blurycards.css'
    
</style>