<template>
  <div class="container">
    <div class="loged">
      <div class="judul">
        <h1>Login</h1>
      </div>
      <div class="isian">
        <form>
          <label for="username">Username</label>
          <input type="text" id="username" name="username" v-model="username">
          <label for="pass">Password</label>
          <input type="text" id="pass" name="pass" v-model="password">
          <input type="submit" value="submit" @click="submit" link="/afterlogin">
       </form>
      </div>
      <a href="/register">Belum memiliki account ?</a>
    </div>
    <a href="/">Kembali Ke Beranda</a>
  </div>
</template>

<script>
export default {
  data() {
    return { 
      username: "",
      password: ""
    }
  },
  methods: {
    submit(e) {
      e.preventDefault()
      if (this.username !== "" && this.password !== "") {
        console.log(this.username, this.password, window.location = "/afterlogin") 
      } else {
        window.alert("eror plese input right")
      }  
    }
  }
}
</script> 

<style lang="scss" scoped>
.container {
  position: relative;
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  .loged {
    position: relative;
    width: 100vw;
    height: calc(100vh - 20rem);
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    padding: 2rem;
    .judul {
      position: relative;
      display: flex;
      justify-content: center;
    }
    .isian {
      position: relative;
      width:100%;
      height:70%;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      padding: 2rem;
      form {
       position: relative;
       width:100%;
       height:70%;
       display: flex;
       justify-content: center;
       align-items: center;
       flex-direction: column;
       font-size: 1.60rem;
       input.submit{
         position: relative;
         width: 2rem;
        }
      }
    }
    a {
     position: relative;
     padding: 2rem;
     color: black;  
     font-size: 1.70rem;
    }
  }
  a {
   position: relative;
   padding: 2rem;
   color: black;  
   font-size: 1.70rem;
  }
}
</style>