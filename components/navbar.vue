<template>
  <div class="navbar container">
    <NuxtLink to="/" class="logo">
      <img src="@/assets/logo.png" alt="logo">
    </NuxtLink>
    <div class="navbar-right">

      <NuxtLink to="/tools">Инструменты</NuxtLink>
      <NuxtLink>Профиль</NuxtLink>
    </div>

  </div>
</template>
<style>
.navbar{
  display: flex;
  width: 100%;
  margin-top: 20px;
  justify-content: space-between;
  border: 2px solid #000;
  border-radius: 50px;
  padding: 10px 40px;
  align-items: center;
  box-sizing: border-box;
}
.logo{
  width: 111px;
  height: 22px;
  text-decoration: none;
}
.logo img{
  width: 100%;
  height: 100%;
}
.navbar-right{
  width: max-content;
  gap: 25px;
  display: flex;
  align-items: center;
  justify-content: end;
}
.navbar-right a{
  font-size: 20px;
  color: #000;
  line-height: 18px;
  text-decoration: none;

}
.navbar-right a:nth-of-type(2){
  border: 2px solid #000;
  padding: 10px;
  border-radius: 50px;
}
@media (max-width: 769px) {
  .navbar-right a{
    font-size: 18px;
  }
  .logo {
    width: 89px;
    height: 20px;
  }
  .navbar{
    width: 96%!important;
  }
}
</style>