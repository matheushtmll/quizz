<template>
    <div id="root">

  <input v-model="newCat">
  <button v-on:click="addKitty">
    + ADD
  </button>
  <ul>
    <li v-for="cat in cats" :key="cat">{{ cat.name }}</li>
      
    
  </ul>
</div>
</template>

<script>

import { defineComponent } from '@vue/composition-api'

export default ({
        new: Vue ({
        el: '#root',
        data: {
        cats: [
            {name: 'kitkat'},
            {name: 'fish'},
            {name: 'henry'}
            
        ],
        newCat: ''
    },
    methods: {
        addKitty: function() {
        return this.cats.push({name: this.newCat})
        }
    }
    })
});
</script>
