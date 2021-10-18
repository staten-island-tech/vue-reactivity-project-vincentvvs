<template>
  <div class="home">
    <button @click="changeStudent">Change from Leyna to Eva</button>
    <h1 class="APTest">Hello {{ student }}</h1>
    <ul class="myList">
      <li v-for="animal in animals" :key="animal">{{ animal }}</li>
    </ul>
    <button v-if="isLoggedIn === false">Login</button>
    <button v-else>Logout</button>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "Home",
  components: {},
  data() {
    return {
      student: "Leyna",
      animals: ["Pig", "Cow", "Daniel", "Monkay", "Gibbon"],
      isLoggedIn: true,
    };
  },
  methods: {
    changeStudent: function () {
      this.student = "Eva";
    },
  },
};
</script>
<style>
.APTest {
  color: red;
}
</style>
