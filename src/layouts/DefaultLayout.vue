<template>
  <main class="layout">
    <header>
      <slot name="header"></slot>
    </header>
    <section>
      <slot></slot>
    </section>
    <aside>
      <slot name="aside"></slot>
    </aside>
    <footer>
      <slot name="footer"></slot>
    </footer>
  </main>
</template>

<style lang="scss">
.layout {
  display: grid;
  grid-template:
    'header header header' auto
    'section section aside' auto
    'footer footer footer' auto / 1fr 1fr 1fr;

  > header {
    grid-area: header;
  }
  > aside {
    grid-area: aside;
  }
  > section {
    grid-area: section;
  }
  > footer {
    grid-area: footer;
  }
}
</style>
