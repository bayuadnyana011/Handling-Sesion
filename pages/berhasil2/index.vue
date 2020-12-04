<template>
  <div class="container">
    <div class="header">
      <nuxt-link class="link" to="/afterlogin">Beranda</nuxt-link>
      <nuxt-link class="link" to="/berhasil1">Page one</nuxt-link>
      <nuxt-link class="link" to="/berhasil2">Page two</nuxt-link>
      <nuxt-link class="link" to="/berhasil3">Page three</nuxt-link>
    </div>
    <div class="judul">
      <h1 class="title">SUDAH LOGIN AHH MANTAP</h1>
      <a href="/">LOG OUT</a>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.container {
  position: relative;
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: flex-end;
  align-items: center;
  flex-direction: column;
  background: #c23091;
  .header {
    position: relative;
    width: 100%;
    height: 5rem;
    display: flex;
    justify-content: flex-end;
    align-items: flex-end;
    flex-direction: row;
    padding-left: 2rem;
    background: rgb(39, 110, 138);
    .link {
      position: relative;
      width: 100%;
      height: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
      color: rgb(255, 255, 255);
      font-family: Arial, Helvetica, sans-serif;
      text-decoration: none;
      font-size: 3rem;
    }   
  }
  .judul {
    position: relative;
    width: 100vw;
    height:  calc(100vh - 5rem);
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
    h1.title {
     font-size: 5rem;
     font-family: Arial, Helvetica, sans-serif;
     color: #000;
    }
    a {
      position: relative;
      padding: 2rem;
      color: black;  
      font-size: 1.70rem;
    }
  }
}
</style>
