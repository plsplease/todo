
  <template>
  <div><hello-world></hello-world>
    <h1 >lab6-todoWork</h1>
  </div>
</template>


<script>

import HelloWorld from "../components/HelloWorld.vue";


export default {
  data: () => ({
      show: false,
    }),
  name: "Home",

  components: {
    HelloWorld,

  },
};
</script>
