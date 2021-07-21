<template>
  <div class="container">
    <header>
      <div class="img-wrapper">
        <img src="../assets/imagens/bg.jpg" alt="Foto De Fundo">
      </div>
      <div class="banner">
        <h1>Web Developer & Front End Designer</h1>
        <p>Guilherme Lima de Oliveira</p>
        <button>Saiba mais</button>
      </div>
    </header>
  </div>

</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<style scoped>

  @import url("https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css");
  @import url('https://fonts.googleapis.com/css2?family=Josefin+Slab:wght@100&display=swap');
  @import url('https://fonts.googleapis.com/css2?family=Mulish:wght@200&display=swap');
  /*
    font-family: 'Mulish', sans-serif;
    font-family: 'Josefin Slab', serif;
  */

header {
  width: 100%;
  height: 100vh;
  overflow: hidden;
  position: relative;
}
.img-wrapper {
  width: 100%;
  height: 100%;
  overflow: hidden;
  background-color: rgba(0, 0, 0, 0.8);
}
.img-wrapper img {
  animation: zoom 10s;
  width: 100%;
  height: 100%;
  object-fit: cover;
  opacity: 0.5;
}
.banner {
  position: absolute;
  top: 30%;
  left: 15%;
}
.banner h1 {
  animation: moveBanner 1s forwards;
  color: white;
  font-family: 'Mulish', sans-serif;
  font-size: 3rem;
  opacity: 0;
  font-weight: 300;
  text-shadow: .2rem .3rem 2px rgba(0, 0, 0, .4);
}
.banner p {
  margin-top: 30px;
  animation: moveBanner 2s forwards;
  font-family: 'Josefin Slab', serif;
  font-size: 2rem;
  color: white;
  padding: 10px;
  text-shadow: .1rem .1rem rgba(0, 0, 0, .4);
  margin-bottom: 20px;
}
.banner button {
  animation: moveBanner 3s forwards;
  font-family: 'Mulish', sans-serif;
  letter-spacing: .1rem;
  text-transform: uppercase;
  color: #fff;
  background-image: linear-gradient(to right, #C84FE0, #9B3DAD);
  margin: 10px;
  padding: 1rem 2rem;
  border: none;
  border-radius: 8px;
  cursor: pointer;
  }
  .banner button:hover {
    opacity: 2;
    color: black;
  }  
  @keyframes zoom {
    0% {
      transform: scale(1.3);   
    }
    100% {
      transform: scale(1);   
      }  
    }
    @keyframes moveBanner {
      0%{
        transform: translateY(30rem) rotateY(-30deg);     
      }
      100% {
        transform: translateY(0rem) rotateY(0deg);
        opacity: 1;
      }
    }
    
    
    </style>
