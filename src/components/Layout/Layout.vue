<template>
  <div class="layout">
    <test :data="menu"/>
  </div>
</template>

<script>
  import test from '../test';

  const menu = [
    {
      name: 'Feed',
      path: '/',
    }, {
      name: 'New Quote',
      path: '/new',
    }, {
      name: 'Profile',
      path: '/profile/me',
    }, {
      name: 'Settings',
      path: '/settings',
    }, {
      name: 'Search',
      path: '/search',
    }, {
      name: 'Notifications',
      path: '/notifications',
    }, {
      name: 'Messages',
      path: '/messages',
    },
  ];

  export default {
    name: 'Layout',
    data() {
      return {
        menu,
      };
    },
    components: { test },
  };
</script>

<style>

</style>
