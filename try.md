  <section class="border-section">
    <div class="container">
      <h1 data-text="Namaste !">Namaste !</h1>
      <h1 data-text="I am Goutam Kumar Nayak">I am Goutam Kumar Nayak</h1>
    </div>
  </section>
  <style>
  @import url("https://fonts.googleapis.com/css2?family=Nunito:wght@300;400;600&display=swap");
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
html {
  font-family: "Nunito";
  background-color: #09111b;
}
:root {
  --var-color: rgb(0, 238, 255);
}
section {
  height: 100vh;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #09111b;
  border: 10px solid var(--var-color);
  border-radius: 20px;
  box-shadow: 0 0 20px var(--var-color);
  animation: flicker2 2s infinite linear forwards;
  animation-delay: 1s;
}

.container h1 {
  font-size: 6vw;
  color: var(--var-color);
  position: relative;
  display:flex;
    justify-content: center;
  align-items: center;  
    flex-direction: column;
 gap:15px;
}
.container h1::before {
  position: absolute;
  content: attr(data-text);
  text-shadow: 0px 0px 20px var(--var-color);
  filter: blur(10px) brightness(0);
  animation: flicker 2s infinite linear forwards;
  animation-delay: 1s;
}
@keyframes flicker {
  0% {
    filter: blur(5px) brightness(1);
  }
  3% {
    filter: blur(5px) brightness(0);
  }
  6% {
    filter: blur(5px) brightness(0);
  }
  7% {
    filter: blur(5px) brightness(1);
  }
  8% {
    filter: blur(5px) brightness(0);
  }
  9% {
    filter: blur(5px) brightness(1);
  }
  10% {
    filter: blur(5px) brightness(0);
  }
  20% {
    filter: blur(5px) brightness(1);
  }
  50% {
    filter: blur(5px) brightness(1);
  }
  99% {
    filter: blur(5px) brightness(0);
  }
  100% {
    filter: blur(5px) brightness(1);
  }
}


@keyframes flicker2 {
  0% {
    filter: brightness(1);
  }
  3% {
    filter: brightness(0);
  }
  6% {
    filter: brightness(0);
  }
  7% {
    filter: brightness(1);
  }
  8% {
    filter: brightness(0);
  }
  9% {
    filter: brightness(1);
  }
  10% {
    filter: brightness(0);
  }
  20% {
    filter: brightness(1);
  }
  50% {
    filter: brightness(1);
  }
  99% {
    filter: brightness(0);
  }
  100% {
    filter: brightness(1);
  }
}
</style>