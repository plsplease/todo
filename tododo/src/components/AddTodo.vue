<template>
  <center>
    <div class="container">
      <v-container>
        <h1>Homework</h1>
        <v-select
          v-model="select"
          :items="items"
          label="--Subject--"
          solo
        ></v-select>
        <v-text-field v-model="name" label="info" outlined></v-text-field>
        <center>
          <v-btn color="success" class="mr-4" @click="validate()">Add</v-btn>
        </center>
      </v-container>
    </div>
  </center>
</template>

<script>
export default {
  subject: "",
  work: "",
  data() {
    return {
      select: "",
      name: "",
      items: [
        "  คพ232 ",
        "  คพ252 ",
        "  คพ313 ",
        "  คพ343 ",
        "  ศท013 ",
        "  อื่นๆ",
      ],
      selectedItem: 1,
      additems: [],
    };
  },
  props: ["XM"],
  methods: {
    validate() {
      this.$emit("Input", this.select, this.name);
      (this.select = " "), (this.name = " ");
    },
  },
};
</script>

<style></style>
