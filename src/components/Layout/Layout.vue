<template>
  <div class="layout">
    <header>
      <div class="container">
        <test :data="menu"/>
      </div>
    </header>
    <main>
      <div class="container">
        <div class="content">
          <basic/>
        </div>
      </div>
    </main>
    <footer>
      <div class="container">
      <test :data="filters"/>
      </div>
    </footer>
  </div>
</template>

<script>
  import test from '../test';
  import basic from '../Slides/Basic';

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

  const filters = [
    {
      name: 'filter',
    }, {
      name: 'filter',
    }, {
      name: 'filter',
    }, {
      name: 'filter',
    }, {
      name: 'filter',
    }, {
      name: 'filter',
    }, {
      name: 'filter',
    }, {
      name: 'filter',
    }, {
      name: 'filter',
    }, {
      name: 'filter',
    }, {
      name: 'filter',
    }, {
      name: 'filter',
    }, {
      name: 'filter',
    }, {
      name: 'filter',
    }, {
      name: 'filter',
    }, {
      name: 'filter',
    },
  ];

  export default {
    name: 'Layout',
    data() {
      return {
        menu,
        filters,
      };
    },
    components: { test, basic },
  };
</script>

<style>
.layout {
  width: 100%;
  height: 100%;
  background-color: azure;
}

  header,
  footer {
    width: 100%;
    height: 70px;
    background-color: aquamarine;
  }

  main {
    width: 100%;
    height: calc(100% - 200px);
    margin: 30px 0;
  }

  .content {
    width: 100%;
    height: 100%;
    background-color: aquamarine;
  }

  .container {
    max-width: 1200px;
    margin: 0 auto;
    height: 100%;
  }
</style>
