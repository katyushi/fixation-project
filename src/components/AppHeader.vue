<template>
  <header class="header">
      <template class="inner-header">
      <img src="../assets/logo.png" alt="logo" width="50" height="50">
      <form>
        <input name="busca" id="busca" type="text" placeholder="Buscar...">
        <input type="submit" id="lupa" value="Buscar" >
      </form>
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

form {
  width: 450px;
  position: relative;
}

@media (max-width: 700px) {
  form {
    width: 28.571vw;
  }
}

#busca {
  width: 100%;
  padding: 10px;
  border: none;
}

#busca:focus,
#busca:hover {
  transform: scale(1.1);
}

#lupa {
  width: 35px;
  height: 35px;
  background: url("../assets/search.svg") no-repeat center center;
  text-indent: -150px;
  border: none;
  cursor: pointer;
  position: absolute;
  top: 0px;
  right: -20px;
  box-shadow: none;
}
</style>