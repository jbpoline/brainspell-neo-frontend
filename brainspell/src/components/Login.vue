<template>
  <div class="container login mb-3 mt-3 pt-3">
    <h1> <i class="fa fa-exclamation-triangle"></i> Brainspell Login Information </h1>
    <p class="lead mt-3 pt-3">
      Brainspell requires read and write access to all your GitHub repositories.
    </p>

    <p class="lead">
      We promise to only create repositories for your brainspell collections
      and only write to those repositories.
    </p>

    <p class="lead">
      If you don't feel
      comfortable with this, you can create a new GitHub account just for brainspell
      collections.
    </p>

    <p class="lead pt-3 mt-3">
      <b-btn variant="info" @click="login">I understand! Let me login</b-btn>
    </p>
  </div>
</template>

<style>

</style>

<script>
export default {
  name: 'login',
  data() {
    return {

    };
  },
  methods: {
    login() {
      this.$emit('doLogin');
      this.$router.replace('/');
    },
  },
};
</script>
