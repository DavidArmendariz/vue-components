<template>
  <div>
    <TheHeader />
    <BadgeList />
    <UserInfo
      :full-name="activeUser.name"
      :info-text="activeUser.description"
      :role="activeUser.role"
    />
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue';
import UserInfo from './components/UserInfo';
import BadgeList from './components/BadgeList.vue';

export default {
  components: {
    TheHeader,
    UserInfo,
    BadgeList,
  },
  data() {
    return {
      activeUser: {
        name: 'David Armendariz',
        description: 'Admin',
        role: 'admin',
      },
    };
  },
};
</script>

<style>
html {
  font-family: sans-serif;
}

body {
  margin: 0;
}
</style>
