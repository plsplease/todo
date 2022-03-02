<template>
  <v-container>
    <center>
    <h1>To-Do List</h1>
    </center>
    <v-card
      class="mx-auto"
      max-width="700"
      v-for="(item, index) in XM"
      :key="index"
      height="100"
      tile
    >
      <v-list-item-content>
        
          
          <v-list-item-subtitle>
           <p class="font-weight-black">
             {{ item.name }}
           </p>
            
            <br>
           <v-btn
                  rounded
                  color="red lighten-1 white--text"
                  @click="deleteTodo(index)"
                >
                  Delete
                </v-btn>
            
          </v-list-item-subtitle>
          
  
         
      </v-list-item-content>
      
    </v-card>
  </v-container>
</template>

<script>
export default {
  props: ["XM"],
  methods: {
    deleteTodo(index) {
      this.XM.splice(index, 1);
    },
  },
};
</script>

<style>
</style>
