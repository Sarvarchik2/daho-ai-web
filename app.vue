<template>
<div class="dahoai">
  <Navbar/>
<NuxtPage/>
  <Footer/>
</div>
</template>

<script setup>
</script>

<style >
@import url('https://fonts.googleapis.com/css2?family=Inter:ital,opsz,wght@0,14..32,100..900;1,14..32,100..900&family=Montserrat:ital,wght@0,100..900;1,100..900&family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

*{
  font-family: 'Poppins', sans-serif;
  font-weight: 400;
  color: #000;


}

body {
  margin: 0;
  font-family: "Poppins", sans-serif;
  font-weight: 400;
  background: #fff;
  color: #000;
  box-sizing: border-box;
  padding: 0;
}

/* Основной класс .container */
.container {
  width: 100%;
  padding-right: var(--bs-gutter-x, 0.75rem);
  padding-left: var(--bs-gutter-x, 0.75rem);
  margin-right: auto;
  margin-left: auto;
}

/* Ширина .container на разных брейкпоинтах */
@media (min-width: 576px) {
  .container {
    max-width: 540px;
  }
}

@media (min-width: 768px) {
  .container {
    max-width: 720px;
  }
}

@media (min-width: 992px) {
  .container {
    max-width: 960px;
  }
}

@media (min-width: 1200px) {
  .container {
    max-width: 1140px;
  }
}

@media (min-width: 1400px) {
  .container {
    max-width: 1320px;
  }
}


</style>
