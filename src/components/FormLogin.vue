<template>
<div class="titulo">
  <!-- <div class="imagens"> -->
      
      <img class="logoGama" src="../assets/logoGama.png" alt="logopss">
      
      <h1>Pessoas e Culturas Treinamentos</h1>
      
      <img class="logoPessoas" src="../assets/pessoacult.png" alt="logopss">
      
  <!-- </div> -->

  
</div>

  <form action="" method="post">
  
    <div class="container">
      <label for="uname"><b>Matricula</b></label>
      <input type="text" placeholder="Enter Username" name="uname" required>

      <label for="psw"><b>Senha</b></label>
      <input type="password" placeholder="Enter Password" name="psw" required>
    </div>
      <button type="submit">Login</button>
      <label>
        <input type="checkbox" checked="checked" name="remember"> Remember me
      </label>
    

    <div class="container" style="background-color:#f1f1f1">
      <button type="button" class="cancelbtn">Cancel</button>
      <span class="psw">Forgot <a href="#">password?</a></span>
    </div>
    
  </form>

  
</template>

<script>

export default {
  name: 'FormLogin',
  data: ()=>( {

  })
}

</script>


<style scoped lang="scss">

body {font-family: Arial, Helvetica, sans-serif;}

form {border: 3px solid #ebd1d1;margin-bottom:24vh;}
@media screen and (max-width: 600px) {
  form {
    width: 92%;
    }
}
div.imagens{
  width: 20%;
  // display: flex;
  // align-items: center;
  // justify-content: space-around;
}
.titulo {
  display: flex;
  align-items: center;
  justify-content: space-between;
  background-color: #bd3934;
  width: 100%;
  text-align: center;
  margin: 0 0 10%;
}
h1 {
  font-size: 26px;
  color: rgb(54, 54, 54);
}

div .container {
  text-align: left;
}

input[type=text], input[type=password] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  display: inline-block;
  border: 1px solid #ccc;
  box-sizing: border-box;
}

button {
  background-color: #bd3934;
  color: white;
  padding: 14px 20px;
  margin: 8px 0;
  border: none;
  cursor: pointer;
  width: 100%;
}

button:hover {
  opacity: 0.8;
}

.cancelbtn {
  width: auto;
  padding: 10px 18px;
  background-color: #bd3934;
}

div .imgcontainer {
  display: flex;
  justify-content: space-around;
  align-items: center;
  width: 50%;
  text-align: center;
  margin-bottom: 60px;
}
@media screen and (max-width: 600px) {
  .logoGama, .logoPessoas {
    opacity: 0;
    width: 0;
    margin: 0;
  }

}

@media screen and (min-width: 600px) {
  .logoGama {
    width: 4%;
    margin:2px 0 4px 10%;
  }
  .logoPessoas {
    margin:2px 10% 4px 0;
    width: 2%;
  }
}


// img.logo {
//   width: 20%;
//   margin-right: 45px;
// }

.container {
  padding: 16px;
}

span.psw {
  float: right;
  padding-top: 16px;
}

/* Change styles for span and cancel button on extra small screens */
@media screen and (max-width: 300px) {
  span.psw {
     display: block;
     float: none;
  }
  .cancelbtn {
     width: 100%;
  }
}

</style>
