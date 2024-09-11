<template>
<div>
    <h2>{{ heading }}</h2>
    <p>{{ text }}</p>
    <button>{{ btnText }}</button>
    <div v-show="true">
        <ul>
            <li v-for="car in cars" :key="car"  >{{ car }}</li>
        </ul>
    </div>
    <div v-for="(country, id) in countries" :key="id">
        <h3>{{ country.continent }}</h3>
        <p>{{ country.name }}</p>
        <span>{{ country.capital }}</span>
    </div>
    


   
   </div>
</template>

<script>
    export default {
      name: 'ReviewComponent',
      data(){
        return{
            heading: "Movie review's for different people",
            text: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Rem pariatur cupiditate officia, esse nostrum dolorem, beatae sint dolores et amet excepturi consequatur fuga eligendi illum debitis, doloribus nesciunt? Reprehenderit, enim.",
            btnText: 'Learn More',
            cars: ['tesla', 'BMW' , 'IST', 'Mazda', 'Hammer', 'Ford' ],
            countries: [
                {
                    id: 1,
                    continent: 'Africa',
                    name: 'Tanzania',
                    capital: 'Dodoma'
                },
                {
                    id: 2,
                    continent: 'Africa',
                    name: 'Congo',
                    capital: 'Kinshasa'
                },
                {
                    id: 3,
                    continent: 'S America',
                    name: 'Brazil',
                    capital: 'Lio de Jeneilo'
                },

            ],
            object: {
      title: 'How to do lists in Vue',
      author: 'Jane Doe',
      publishedAt: '2016-04-10'
    }
        
        }
      },
     



       
        
    }
</script>

<style scoped>
button{
    padding: 10px;
    background: magenta;
    color: #000;
    border-radius: 10px;


}

</style>