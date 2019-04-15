<template>
  <div>
    <h2>Results</h2>
    <p>Here are the top ten noisiest users you follow:</p>
    <table>
      <tbody>
        <tr>
          <th>total</th>
          <th>user</th>
          <th>tweets</th>
          <th>retweets</th>
          <th>quotes</th>
        </tr>
        <UserRow v-for="user in users" :key="user.id" :user="user" />
      </tbody>
    </table>
    <button>Load more</button>
  </div>
</template>

<script>
import UserRow from './UserRow.vue';

export default {
  name: 'Results',
  components: {
    UserRow,
  },
  data() {
    return {
      users: [
        {
          id: 1,
          username: 'jamestkirk',
          total: 999,
          tweets: 700,
          retweets: 99,
          quotes: 7,
        },
        {
          id: 2,
          username: 'spock',
          total: 275,
          tweets: 137,
          retweets: 72,
          quotes: 4,
        },
        {
          id: 3,
          username: 'bones',
          total: 150,
          tweets: 120,
          retweets: 50,
          quotes: 3,
        },
        {
          id: 4,
          username: 'scotty',
          total: 125,
          tweets: 80,
          retweets: 44,
          quotes: 1,
        },
        {
          id: 5,
          username: 'uhura',
          total: 50,
          tweets: 40,
          retweets: 12,
          quotes: 0,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
table {
  border-spacing: 1em 0.5em;
  margin: auto;
}

th {
  text-align: left;
}
</style>
