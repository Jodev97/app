<template>
  <div id="cCard1" class="cards-wrapper">
    <div class="card-grid-space">
      <a
        class="card"
        href="#"
        :style="{
          'background-image':
            'linear-gradient(rgba(0, 0, 0, 0.1), rgba(0, 0, 0, 0.6)),url(' +
            require(`@/assets/${image}`) +
            ')',
        }"
      >
        <div>
          <h1>HTML Syntax</h1>
          <p>
            The syntax of a language is how it works. How to actually write it.
            Learn HTML syntax…
          </p>
          <div class="date">6 Oct 2017</div>
          <div class="tags">
            <div class="tag">READ MORE</div>
          </div>
        </div>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: String,
    image: String,
    tag: String,
  },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css?family=Heebo:400,700|Open+Sans:400,700");
:root {
  --color: #3c3163;
  --transition-time: 0.5s;
}
#cCard1 {
  a {
    color: inherit;
  }

  .cards-wrapper {
    display: grid;
    justify-content: center;
    align-items: center;
    grid-template-columns: 1fr 1fr 1fr;
    grid-gap: 4rem;
    padding: 4rem;
    margin: 0 auto;
    width: max-content;
  }

  .card {
    font-family: "Heebo";
    height: 15em;
    font-size: 1.5em;
    color: white;
    padding: 1em;
    display: flex;
    align-items: flex-end;
    background-size: cover;
    background-position: center;
    box-shadow: 0 3px 7px -1px #0000001a;
    transition: all, var(--transition-time);
    position: relative;
    overflow: hidden;
    text-decoration: none;
    border-radius: 0;
  }

  .card:hover {
    transform: rotate(0);
  }

  .card h1 {
    margin: 0;
    font-size: 1.5em;
    line-height: 1.2em;
  }

  .card p {
    font-size: 0.75em;
    font-family: "Open Sans";
    margin-top: 0.5em;
    line-height: 2em;
  }

  .card .tags {
    display: flex;
  }

  .card .tags .tag {
    font-size: 0.75em;
    background: rgba(255, 255, 255, 0.5);
    padding: 0 0.5em;
    margin-right: 0.5em;
    line-height: 1.5em;
    transition: all, var(--transition-time);
  }

  .card:hover .tags .tag {
    background: var(--color);
    color: white;
  }

  .card .date {
    position: absolute;
    top: 0;
    right: 0;
    font-size: 0.75em;
    padding: 1em;
    line-height: 1em;
    opacity: 0.8;
  }

  .card:before,
  .card:after {
    content: "";
    transform: scale(0);
    transform-origin: top left;
    position: absolute;
    left: -50%;
    top: -50%;
    z-index: -5;
    transition: all, var(--transition-time);
    transition-timing-function: ease-in-out;
  }

  .card:before {
    background: #ddd;
    width: 250%;
    height: 250%;
  }

  .card:after {
    background: white;
    width: 200%;
    height: 200%;
  }

  .card:hover {
    color: var(--color);
  }

  .card:hover:before,
  .card:hover:after {
    transform: scale(1);
  }

  .card-grid-space .num {
    font-size: 3em;
    margin-bottom: 1.2rem;
    margin-left: 1rem;
  }

  .info {
    font-size: 1.2em;
    display: flex;
    padding: 1em 3em;
    height: 3em;
  }

  .info img {
    height: 3em;
    margin-right: 0.5em;
  }

  .info h1 {
    font-size: 1em;
    font-weight: normal;
  }

  /* MEDIA QUERIES */
  @media screen and (max-width: 1285px) {
    .cards-wrapper {
      grid-template-columns: 1fr 1fr;
    }
  }

  @media screen and (max-width: 900px) {
    .cards-wrapper {
      grid-template-columns: 1fr;
    }
    .info {
      justify-content: center;
    }
    .card-grid-space .num {
      /*margin-left: 0;
    text-align: center;*/
    }
  }

  @media screen and (max-width: 500px) {
    .cards-wrapper {
      padding: 4rem 2rem;
    }
    .card {
      max-width: calc(100vw - 4rem);
    }
  }

  @media screen and (max-width: 450px) {
    .info {
      display: block;
      text-align: center;
    }
    .info h1 {
      margin: 0;
    }
  }
}
</style>
