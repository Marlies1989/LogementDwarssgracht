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
    <nav>
        <div class="mobile-open" @click="showMenu()">
            <p>Menu</p>
        </div>
            <div class="menu-wrapper" :class="this.showMobileMenu ? 'open-menu' : 'closed-menu'"> 
                <ul class="menu">
                    <li><a href="#over">Over</a></li>
                    <li><a href="">Tarieven</a></li>
                    <li><a href="">Foto's</a></li>
                    <li><a href="">Contact</a></li>
                 </ul>
        </div>
    </nav>
</header>

</template>

<style scoped>
header {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
}

nav {
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  align-items: center;
}

.mobile-open p {
    font-family: var(--title);
    padding: var(--space-md);
    font-size: var(--step-1);
    color: var(--color-primary);
    text-decoration-line: underline;
    -moz-text-decoration-line: underline;
}

.open-menu {
  display: flex !important;
}

.menu-wrapper {
  position: absolute;
  top: 4rem;
  width: 100%;
  z-index: 100;
  gap: var(--space-md);
  display: none;
  flex-direction: column;
}

.menu {
  gap: var(--space-md);
  display: flex;
  flex-direction: column;
  background-color: var(--color-primary);
  padding-inline: 0;
  padding-block: var(--space-md);
}

.menu > li {
  margin-inline: var(--space-md);
  font-family: var(--title);
  font-size: var(--step-1);
  color: var(--color-secondary);
  list-style: none;
}

.menu > li > a {
  color: var(--color-secondary);
  text-decoration: none;
  width: 100%;
  display: flex;
  align-items: end;
  justify-content: space-between;
  border-bottom: 1px solid var(--color-secondary);
}

.menu > li > a:hover {
  color: var(--color-secondary);
}


@media screen and (min-width: 800px) {
  .mobile-open {
    display: none;
  }

  .menu-wrapper {
    display: flex;
    flex-direction: column-reverse;
    top: 0;
    position: relative;
    align-items: center;
  }

  .menu {
    flex-direction: row;
    justify-content: flex-end;
    gap: 0;
    position: relative;
    padding: 0;
    background-color: transparent;
  }

  .menu > li {
    border-bottom: none;
    margin: 0;
    list-style: none;
    display: flex;
    flex: 1;
    padding-inline: var(--space-md);
  }

  .menu li:hover a {
    color: var(--color-primary);
    text-decoration: underline;
  }

  .menu > li > a {
    color: var(--color-primary);
    border-bottom: none;
    justify-content: center;
    align-items: center;
  }
}
</style>