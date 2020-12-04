<template>
  <div class="container">
    <div class="regis">
      <div class="judul">
         <h1>Register</h1>
      </div>
      <div class="isian">
        <form>
        <label for="username">Username :</label>
        <input type="text" id="username" name="username" v-model="username">
        <label for="alamat">Alamat</label>
        <input type="text" id="alamat" name="alamat" v-model="alamat">
        <label for="email">Email :</label>
        <input type="text" id="email" name="email" v-model="email">
        <label for="pass">Password :</label>
        <input type="text" id="pass" name="pass" v-model="password">
        <label for="password">Ulangi Password :</label>
        <input type="text" id="password" name="password" v-model="ulangiPassword">
        <input type="submit" value="submit" @click="submit">
        </form>
      </div>
      <a href="/login">Sudah Punya Account ?</a>
    </div>
    <a href="/">Kembali Ke Beranda</a>
  </div>
</template>

<script>
export default {
  data() {
    return{
      username: "",
      alamat: "",
      email: "",
      password:"",
      ulangiPassword: ""
    }
  },
  methods: {
    submit(e) {
      e.preventDefault()
      if (this.username !== "" && this.password !== "" && this.alamat !=="" && this.email !=="" && this.ulangiPassword !=="") {
        console.log(this.username, this.password, this.alamat, this.email, this.ulangiPassword)
        if (this.password === this.ulangiPassword) {
          console.log(this.password, this.ulangiPassword, window.location = "/afterlogin") 
        } else {
          window.alert("password harus sama")
        }
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
  .regis {
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