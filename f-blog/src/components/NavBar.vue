<template>
  <div>
    <b-navbar toggleable="lg" type="dark" variant="success" class="navbar">
      <b-container>
        <b-navbar-brand href="#">{{ logoText }}</b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <!-- Right aligned nav items -->
          <b-navbar-nav class="ml-auto align__right">
            <b-button variant="success" v-on:click="loginFunc">Login</b-button>
          </b-navbar-nav>
        </b-collapse>
      </b-container>
    </b-navbar>
  </div>
</template>

<script>
export default {
  data() {
    return {
      logoText: "Board",
    };
  },
  methods:{
      loginFunc() {
          alert()
      }
  }
};
</script>
<style scoped>
.align__right {
  width: 100%;
  justify-content: right;
}
.navbar {
  height: 70px;
}
</style>
