<template>
  <main>
    <section class="card">
      <figure class="card__image" role="img"></figure>
      <article class="card__text">
        <h1>Get <span>insights</span> that help your business grow.</h1>
        <p>
          Discover the benefits of data analytics and make better decisions
          regarding revenue, customer experience, and overall efficiency.
        </p>
        <section class="card__text__numbers">
          <p>
            <strong>10k+</strong>
            COMPANIES
          </p>
          <p><strong>314</strong>TEMPLATES</p>
          <p><strong>12M+</strong>QUERIES</p>
        </section>
      </article>
    </section>
  </main>
  <footer class="attribution">
    Challenge by
    <a href="https://www.frontendmentor.io?ref=challenge" target="_blank"
      >Frontend Mentor</a
    >. Coded by
    <a href="https://www.frontendmentor.io/profile/Gonzalo-Barra"
      >Gonzalo Barra</a
    >.
  </footer>
</template>
<script>
export default {};
</script>
<style>
main {
  align-items: center;
  border-radius: 0.652rem;
  display: flex;
  flex-flow: column;
  justify-content: center;
}

.card {
  align-items: center;
  align-self: center;
  background-color: hsl(244, 38%, 16%);
  border-radius: 0.652rem;
  display: flex;
  flex-flow: column;
  justify-content: center;
  width: 18.75rem;
}

.card__image {
  background-image: url("/images/header-mobile.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  border-radius: 0.625rem 0.625rem 0 0;
  height: 13rem;
  width: 18.7rem;
}

.card__image::after {
  background-color: #550081;
  border-radius: 0.625rem 0.625rem 0 0;
  content: "";
  height: 100%;
  object-fit: cover;
  opacity: 0.5;
  position: absolute;
  width: 100%;
}

.card__text {
  max-width: 90%;
}

h1 {
  color: white;
  font-family: Inter, sans-serif;
  font-size: 1.5625rem;
  font-weight: 700;
  line-height: 1.2;
  margin: 1.25rem;
  text-align: center;
}

h1 span {
  color: hsl(277, 64%, 61%);
  font-family: Inter, sans-serif;
  font-weight: 700;
}
p {
  font-size: 0.9375rem;
  text-align: center;
}

.card__text__numbers p {
  display: flex;
  flex-direction: column;
  font-family: "Lexend Deca", sans-serif;
  margin-bottom: 0.9375rem;
  margin-top: 1.875rem;
}

.card__text__numbers p strong {
  color: white;
  font-size: 1.5rem;
  font-weight: 700;
}
.attribution {
  font-size: 0.68753rem;
  text-align: center;
}
.attribution a {
  color: hsl(228, 45%, 44%);
}

@media only screen and (min-width: 90rem) {
  main {
    align-items: center;
    border-radius: 0.625rem;
    display: flex;
    flex-flow: row;
    justify-content: center;
  }

  .card {
    align-items: center;
    display: flex;
    flex-flow: row;
    justify-content: center;
    width: 63.75rem;
  }

  .card__image {
    background-image: url("/images/header-desktop.jpg");
    border-radius: 0 0.625rem 0.625rem 0;
    height: 30rem;
    order: 1;
    width: 50rem;
  }

  .card__image::after {
    border-radius: 0 0.625rem 0.625rem 0;
    height: 100%;
    object-fit: cover;
    width: 100%;
  }
  h1 {
    font-size: 2rem;
    margin: 0;
    padding-bottom: 2.5rem;
    text-align: left;
  }
  p {
    text-align: left;
    padding-top: 0;
  }

  .card__text {
    max-width: 50%;
    padding: 0 3.125rem;
  }
  p .card__text {
    align-items: center;
    display: flex;
    flex-flow: column;
    justify-content: center;
  }

  .card__text__numbers {
    align-items: left;
    align-self: start;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
  }
}
</style>
