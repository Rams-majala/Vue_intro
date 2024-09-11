<template>
    <div>
        <h1>{{heading}}</h1>
        <p>{{text}}</p>
        <h2 >{{list}}</h2>
        <ul>
            <li  v-for="fruit of fruits" :key="fruit">{{fruit}}</li>
        </ul>
        <ButtonComponent />
    </div>
</template>

<script>
import ButtonComponent from './home/ButtonComponent.vue'
    export default {
        name: 'AboutComponent',
        components: { ButtonComponent},
        data(){
            return{
                heading: 'This how components can be accesed to the main component',
                text: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Omnis qui dolorem dignissimos, nobis assumenda accusantium minima laudantium quam fuga dolore recusandae, inventore odit est, ipsa corporis aspernatur. Adipisci, nesciunt doloremque!',
                fruits: [
                    'Orange',
                    'Banana',
                    'Strawberry',
                    'Avocado',
                    'Apple'
                ],
                list: 'LIST OF FRUITS'

            }
        }

    }
</script>

<style  scoped>
*{
    text-align: start;
}
ul li{
    text-align: start;
    padding-top: 10px ;
    list-style: none;
}

</style>