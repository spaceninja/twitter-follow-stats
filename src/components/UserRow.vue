<template>
  <tr>
    <td class="num">{{ user.total }}</td>
    <td><span class="at">@</span>{{ user.username }}</td>
    <td class="num">{{ user.tweets }}</td>
    <td class="num">{{ user.retweets }}</td>
    <td class="num">{{ user.quotes }}</td>
  </tr>
</template>

<script>
export default {
  name: 'UserRow',
  props: {
    user: { type: Object, required: true },
  },
};
</script>

<style lang="scss" scoped>
.at {
  opacity: 25%;
}
td {
  text-align: left;

  // stylelint-disable-next-line selector-no-qualifying-type
  &.num {
    font-variant-numeric: tabular-nums;
    text-align: right;
  }
}
</style>
