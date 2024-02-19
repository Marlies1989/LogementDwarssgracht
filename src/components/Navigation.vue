<script>
export default {
  data() {
    return {
      showMobileMenu: false,
      };
  },
  methods: {
    showMenu() {
      this.showMobileMenu = !this.showMobileMenu;
      },
  },
};
</script>

<template>

  <header>
    <h1>Logement Dwarsgracht</h1>
    <nav class="mobile-open">
        <ul class="menu">
          <li  @click="showMenu()">Menu
            <ul :class="this.showMobileMenu ? 'open-menu' : 'closed-menu'">
              <li><a href="#over">Over</a></li>
              <li><a href="#tarieven">Tarieven</a></li>
              <li><a href="#fotos">Foto's</a></li>
              <li><a href="#contact">Contact</a></li>
            </ul>
          </li>
        </ul>
    </nav>
</header>

</template>

<style scoped>
header {
  display: flex;
  flex-direction: row;
  align-items: center;
  text-align: center;
  margin-inline-start: auto;
  margin-inline-end: auto;
}

h1 {
  flex: 2;
  text-wrap: nowrap;
  white-space: nowrap;
  margin-inline: 0.5rem;
}

nav {
  display: flex;
  flex-direction: column;
  flex: 1;
  align-items: center;
  width: 100%;
}

.menu {
  list-style: none;
  margin: 0;
  padding: 0;
  width: 100%;
}

.menu > li {
  position: relative;
  padding: 0.5rem;
}

.closed-menu {
  display: none;
}

.menu > li ul {
  position: absolute;
  top: 100%;
  right: 0;
  width: 100dvw;
  list-style: none;
  margin: 0;
  padding: 0;
  background-color: var(--color-primary);
}

.menu > li ul li {
  width: 100%; 
  padding: 0.5rem;
}

.menu > li ul li a {
  color: var(--color-secondary);
  text-decoration: none;
}

.menu > li ul li:hover a {
  background-color: var(--color-primary);
  color: var(--color-secondary);
  width: 100%;
  height: 100%;
}

@media screen and (min-width: 800px) {
  header {
      width: min(1280px, 100vw - 2rem);
  }

  h1 {
    flex: 1;
    margin: 0;
    font-size: var(--step-2);
    text-align: left;
  }

  nav {
    flex: 2;
  }

  .menu > li {
    visibility: hidden;
    display: flex;
    justify-content: flex-end;
  }

  .menu > li > ul {
    visibility: visible;
    display: flex;
    gap: 2rem;
    background: transparent;
    position: relative;
    width: auto;
  }

  .menu > li > ul > li > a {
    color: var(--color-primary);
  }

}

</style>