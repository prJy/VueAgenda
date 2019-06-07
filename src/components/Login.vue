<template>
<b-container>
  <b-row align-v="center" align-h="center">
    <b-col cols="6">
      <h2>
        Login
      </h2>
      <b-jumbotron>
          <b-form v-on:submit="handleSubmit($event)">
            <b-form-group :label-cols="2" breakpoint="md" label="E-mail">
              <b-form-input id="Usuario"
              placeholder="email@email.com"
              type="email" v-model="user.email"
              required>
              </b-form-input>
            </b-form-group>
              <b-form-group :label-cols="2" breakpoint="md" label="Senha">
              <b-form-input id="password" type="password" v-model="user.password" required>
              </b-form-input>
          </b-form-group>
          <b-button align-h="end" type="submit" variant="primary">Acessar</b-button>
        </b-form>

      </b-jumbotron>
    </b-col>
  </b-row>
</b-container>
</template>

<script>
export default {
  name: 'Login',
  title: 'Login',
  data() {
    return {
      user: {
        email: null,
        password: null,
      },
    };
  },
  methods: {
    handleSubmit: (event) => {
      event.preventDefault();
    },
  },

};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
