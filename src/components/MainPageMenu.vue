<template>
<div>
  <b-nav pills>
    <b-nav-item href="/#/">Home</b-nav-item>
    <b-nav-item href="/#/login">Acesso ao Sistema</b-nav-item>
    <b-nav-item-dropdown
      id="my-nav-dropdown"
      text="Informação"
      toggle-class="nav-link-custom"
      right
    >
      <b-dropdown-item>Mensagens</b-dropdown-item>
      <b-dropdown-item>Meu Perfil</b-dropdown-item>
      <b-dropdown-divider></b-dropdown-divider>
      <b-dropdown-item>Sair</b-dropdown-item>
    </b-nav-item-dropdown>
  </b-nav>
</div>
</template>

<script>
export default {
  name: 'MainPageMenu',
};
</script>
