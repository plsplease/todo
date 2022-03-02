<template>

  <div>
    
    <AddTodo @Input="validate"></AddTodo>
    <ShowTodo :XM="XM"></ShowTodo>
    </div>
    
</template>

<script>
import AddTodo from "../components/AddTodo.vue"
import ShowTodo from "../components/ShowTodo.vue"
export default {
  data: () => ({
    XM: [],
  }),
components :{AddTodo,ShowTodo},
XM: "Input",
  methods: {
    validate(select, name) {
      this.XM.push({
        name: select + " : " + name,
      });
    },
  },
};
</script>

<style>

</style>