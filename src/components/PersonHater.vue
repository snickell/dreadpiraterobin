<template>
  <div>
    Spew hate about {{ name }}
    <div>
      <button v-on:click="doHate" type="button">Hate on {{ name }}</button>
      (You have invoked {{ howManyHates }} hates on {{ name }})
    </div>
  </div>
</template>

<script>
export default {
  name: "PersonHater",
  props: {
    name: String,
  },
  data() {
    return {
      howManyHates: 0,
    };
  },
  methods: {
    doHate() {
      if (this.name === "Brownie") {
        alert("FUCK YOU: those who hate brownie hate themselves");
        this.howManyHates = -9000;
      } else {
        alert("FUCK " + this.name);
        this.howManyHates = this.howManyHates + 1;
      }
    },
  },
};
</script>

<style scoped>
div {
  padding: 20px;
  background: black;
  color: red;
}
</style>