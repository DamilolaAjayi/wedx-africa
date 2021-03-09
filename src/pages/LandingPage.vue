<template>
  <div class="container">
    <div class="landing-page">
      <header>
          <h1 class="landing-page__title">Wedx.Africa</h1>
      </header>
      <hr>
      <div class="landing-page__description">
          <p>Redefining 'Fun' Wedding Experiences</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
 name: 'landing-page',   
};
</script>

<style scoped>
.container {
  margin: 0 auto;
  height: 100vh;
  display: flex;
  max-width: 1440px;
  justify-content: center;
  align-items: center;
  text-align: center;
  border: 5px solid var(--white);
}
.landing-page {
  max-width: 51rem;
  padding: 4rem 1.2rem;
  overflow-y: auto;
}
.landing-page__description {
  font-size: 1.2rem;
  margin: 1.2rem 0;
  font-weight: 500;
  line-height: 1.4;
  animation: 4s appearLater;
}
hr {
  width: 100%;
  border: 0.5px solid rgba(255, 255, 255, 0.12);
  margin: 3rem 0;
}
.landing-page__title {
  animation: 2.5s appear;
  margin: auto;
  font-weight: 600;
  letter-spacing: 1px;
}
@keyframes appear {
  0% {
    opacity: 0;
  }
}
@keyframes appearLater {
  0% {
    opacity: 0;
  }
  50% {
    opacity: 0;
  }
}
@media (min-width: 48rem) {
  .container {
    justify-content: center;
    border: 10px solid var(--white);
    padding: 4rem 0 0;
  }
  /* header {
    text-align: center;
  } */
  .landing-page__description {
    font-size: 1.8rem;
    margin: 1.2rem;
    line-height: 1.4;
  }
}
</style>
