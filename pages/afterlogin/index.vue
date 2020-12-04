<template>
  <div class="container">
    <div class="header">
      <nuxt-link class="link" to="/afterlogin">Beranda</nuxt-link>
      <nuxt-link class="link" to="/berhasil1">Page one</nuxt-link>
      <nuxt-link class="link" to="/berhasil2">Page two</nuxt-link>
      <nuxt-link class="link" to="/berhasil3">Page three</nuxt-link>
    </div>
    <div class="section">
      <div class="icon">
        <img class="gambar" src="/Profil (3).jpg" alt="404 NOT FOUND!PLEASE RELOAD" > 
        <h2>I Wayan Bayu Adnyana</h2>
        <p>Young entrepreneur - Mahasiswa</p>
      </div>
      <div class="me" id= me>
        <div class="textMe">
          <h1 font-size = 34;>About Me</h1>
          <p  font-size = 0.85rem;>Hello, I am I Wayan Bayu Adnyana, from Demulih village. 
          I was born on 20 June 2001 in Bangli. My religion is Hindu. 
          My hobbies are traveling, Automotive, Bonsai.
          On this homepage you will see my profile, 
          you can find out more about me here.
          Because I have included some information about myself.
          Klik untuk
          <a href="/">LOG OUT</a>
          </p>
        </div>   
      </div>         
    </div>
  </div>
</template>

<style lang="scss" scoped>
.container {
  position: relative;
  width: 100vw;
  display: flex;
  justify-content: flex-start;
  align-items: center;
  flex-direction: column;
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
  .section {
    position: relative;
    width: 100vw;
    height:  calc(100vh - 5rem);
    display: flex;
    justify-content:flex-start;
    flex-direction:column;
    align-items: center;
    .icon{
      position: relative;
      width: 50%;
      height: 100%;
      display: flex;
      justify-content: center;
      flex-direction: column;
      align-items: center;
      .gambar {
        position: relative;
        height: 18rem;
        width: 9rem;
        object-fit: contain;
        background-color: #eaeaea;
        background-size: cover;
        border-radius: 100px;
        margin: 0 auto;
        border: 1px solid #eaeaea;
        object-fit: cover;
      }            
    }
    .me {
      position: relative;
      width: 100%;
      height: 100%;
      background-image: linear-gradient(-20deg, #9c1728 0%, #6944ff 100%);
      display: flex;
      align-items: center;
      padding: 2rem;
      box-sizing: border-box;
      flex-direction: column;
      justify-content: flex-start;  
      .textMe {
        position: relative;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: flex-start;
        color: whitesmoke; 
        .p {
         font-size: 18;
        }
         a {
          position: relative;
          padding: 2rem;
          color: rgb(255, 255, 255);  
         font-size: 1.70rem;
        }
      }                  
    }         
  }
}
</style>