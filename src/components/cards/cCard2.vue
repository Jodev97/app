<template>
  <div id="cCard2" class="container">
    <div class="blog-posts">
      <div>
        <a href="#" class="row">
          <div
            class="col-sm-12 col-lg-5 image-card"
            :style="{
              'background-image':
                'linear-gradient(rgba(0, 0, 0, 0.1), rgba(0, 0, 0, 0.6)),url(' +
                require(`@/assets/bg_5.jpg`) +
                ')',
            }"
          >
            <div class="time">
              <div class="date">04</div>
              <div class="month">APR</div>
            </div>
          </div>
          <div class="col-sm-12 col-lg-7">
            <h1>
              Multiply created make behold fourth yielding living male very god.
            </h1>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quas
              illo tempore at eveniet adipisci harum error deserunt in sint
              aspernatur magni asperiores explicabo corporis ratione praesentium
              illum magnam esse ipsa dignissimos quaerat perferendis dolor vero?
              Maiores hic modi optio eaque...
            </p>
            <div class="meta">
              <div class="icon-comment">22 Comments</div>
              <ul class="tags">
                <li></li>
                <li></li>
              </ul>
            </div>
          </div>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
$blog--height: 200px;

#cCard2 {
  a {
    color: #2125298f;
    text-decoration: none;
  }
  .time {
    background: rgba(255, 255, 255, 0.5);
    width: 50px;
    text-align: center;
    padding: 0.5em 0;
    color: #444;

    .date {
      font-weight: bolder;
    }

    .month {
      font-size: 0.7rem;
    }
  }
  .image-card {
    height: 250px;
    background-size: cover;
    background-position: center;
  }
  .blog-posts {
    .featured {
      width: 100% !important;
      height: 250px !important;
      margin: 0.5em 0 1em 0 !important;
      .image {
        height: 250px !important;
      }
      .content {
        height: 250px !important;
      }
    }

    .row {
      display: flex;
      .post {
        &:last-child {
          margin-right: 0 !important;
        }
      }
    }

    .post {
      //float: left;
      //width: calc(50% - 0.25em);
      flex: 1;
      overflow: hidden;
      background: white;
      height: $blog--height;
      //@include box-shadow(0 0 2px 0 rgba(0, 0, 0, 0.2));
      margin-right: 1em;
      margin-bottom: 1em;

      &:hover {
        //@include box-shadow(0 0 3px 2px rgba(0, 0, 0, 0.1));
        .image {
          opacity: 0.8;
        }
      }

      .image,
      .content {
        display: inline-block;
        position: relative;
        //@include transition(all 500ms ease);
      }

      .image {
        float: left;
        width: 50%;
        height: $blog--height;
        background-size: cover;
        background-position: center center;
      }

      .content {
        padding: 0.5em 1em;
        width: 50%;
        //@include box-shadow(-2px 0 2px -1px rgba(0, 0, 0, 0.1));
        height: $blog--height;

        &:before {
          content: "";
          position: absolute;
          background: white;
          width: 10px;
          height: 10px;
          top: 20%;
          left: -5px;
          // @include transform(rotate(45deg));
          // @include box-shadow(-1px 0 2px -1px rgba(0, 0, 0, 0.1));
        }

        h1 {
          font-weight: 600;
          line-height: 2;
          white-space: nowrap;
          overflow: hidden;
          text-overflow: ellipsis;
        }

        p {
          font-weight: 300;
          font-size: 0.7rem;
          line-height: 1.5;
          margin-bottom: 0.5em;
          font-family: "Merriweather", sans-serif;
        }

        .meta {
          .icon-comment {
            font-size: 0.7em;
            line-height: 2;
            margin-top: auto;
          }
        }
      }
    }
  }
}
</style>
