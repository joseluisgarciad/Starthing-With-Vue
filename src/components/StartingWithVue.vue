<template>
    <div class="hello">
        <div>
            <h1>{{ msg }}</h1>
            <p>
             Hello World from Your Starter Component
            </p>
            <br/>
            <p>
                {{ count }} <br/>
                <button @click="increment">-</button>
                <button @click="decrement">+</button>
            </p>
        </div>
        <br/>
        <div>
            <p>Mensaje original: "{{ msg }}"</p>
            <p>Mensaje invertido computado: "{{ reverseMessage }}"</p>
        </div>
        <br/>
        <div v-if="Math.random() > 0.5">
            Ahora me ves
        </div>
        <div v-else>
            Ahora no
        </div>
    </div>
</template>

<script>
//import { ref } from "vue";

export default {
    name: 'StartingWithVue',
    props: {
        msg: {required: true, type: String},
        type: {default: 'A', type: String}
    },
    data: () => ({
        /*This data is private and only for the component itself to use.
        other components do not have access to it*/
        count: 0
    }),
    computed:{
        reverseMessage:function() {
            return this.msg.split('').reverse().join('')
        }
    }
}
</script>
