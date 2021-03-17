<template>
  <header class="header">
      <template class="inner-header">
      <img src="../assets/logo.png" alt="logo" width="50" height="50">
      <input type="search" name="" id="">
      <ul>
        <li>
          <a>a</a>
        </li>
        <li>
          <a>aa</a>
        </li>
        <li>
          <a>aaa</a>
        </li>
      </ul>
    </template>
  </header>
</template>

<script>
export default {
    name: "AppHeader"
}
</script>

<style scoped>
header {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    background-color: var(--primary);
    padding: 5px 15px;
}
ul {
  list-style: none;
  color: white;
  display: flex;
  flex-direction: row;
}
ul li {
  margin: 0 5px;
}
</style>