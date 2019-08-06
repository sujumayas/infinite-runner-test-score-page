<template>
  <Layout>
    <h1>Highscores</h1>
    <p>Just a simple description...</p>
    <ul v-if="loaded">
      <template v-for="user in users">
        <li>
          <p>
            <span>{{user.userName}}</span>:
            <span>{{user.userScore}}</span>
          </p>
        </li>
      </template>
    </ul>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: "About us"
  },
  data: function() {
    return {
      users: [],
      loaded: false
    };
  },
  mounted() {
    this.getUsers();
  },
  methods: {
    getUsers: async function() {
      const response = await fetch(
        "https://corre-manuela.firebaseio.com/userScores.json"
      );
      const json = await response.json();
      console.log(json);
      this.users = json;
      this.loaded = true;
    }
  }
};
</script>
