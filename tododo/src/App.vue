<template>
  <v-app>
    <v-app-bar app color="primary" white>
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://scontent.fcnx3-1.fna.fbcdn.net/v/t39.30808-6/232828080_3020754348209070_7092805187801869522_n.jpg?_nc_cat=107&ccb=1-5&_nc_sid=09cbfe&_nc_eui2=AeEzodfs8H3qWY8JWuyZ47hM87_SVN3lbz_zv9JU3eVvP2IUwXZ8zK6pw_1fImtsp76OF9LvjDB5dENsLNWYPi6n&_nc_ohc=e1uhAVczwGYAX9PVkFC&_nc_ht=scontent.fcnx3-1.fna&oh=00_AT_pk1kimm611tMUCxuoP126Ff2o6N_WTLcHPP9AP7jxDw&oe=62060E07"
          transition="scale-transition"
          width="95"
        />


      </div>

      <v-spacer></v-spacer>

      <v-btn to="/"  text>
        <span class="mr-2">Home</span>
      </v-btn>
       <v-btn to="/about"  text>
        <span class="mr-2">About</span>
      </v-btn>
       <v-btn to="/Todo"  text>
        <span class="mr-2">Todo</span>
      </v-btn>
    </v-app-bar>
    

    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: "App",

  data: () => ({
    //
  }),
};
</script>
