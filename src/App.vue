<template>
  <div id="app">
    <mu-appbar title="Archy">
      <mu-icon-button icon="menu" slot="left" />
      <mu-icon-button icon="expand_more" slot="right" />
    </mu-appbar>

    <router-view/>
  </div>
</template>

<style>
.mu-appbar {
  background: #f8462e;
}
</style>
