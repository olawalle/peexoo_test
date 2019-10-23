<template>
  <div class="home">
    <div class="hero">
      <img
        src="https://images.unsplash.com/photo-1495542779398-9fec7dc7986c?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60"
        alt
        class="hero-img"
      >
      <div class="overlay"></div>
      <div class="hero-content">
        <h1>Join the community</h1>
        <h3>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Recusandae
          nostrum at quisquam quia natus molestiae debitis ab eius incidunt
          corrupti sint exercitationem aliquid quaerat reprehenderit tempore,
          earum qui numquam quae!
        </h3>
        <button class="yellow-btn">Join the community</button>
      </div>
    </div>
    <div class="grid">
      <div class="grid__item">
        <img src="https://source.unsplash.com/category/nature/" alt="title">
      </div>
      <div class="grid__item">
        <div class="grid_inner">
          <img src="https://source.unsplash.com/random" alt="title">
        </div>
        <div class="grid_inner">
          <img src="https://source.unsplash.com/category/nature/" alt="title">
        </div>
      </div>
      <div class="grid__item">
        <div class="grid_inner_bigger">
          <img src="https://source.unsplash.com/random" alt="title">
        </div>
        <div class="grid_inner_smaller">
          <img src="https://source.unsplash.com/category/nature/" alt="title">
        </div>
      </div>
    </div>
    <div class="community">
      <h1 class="heading">Why join the community?</h1>
      <div class="left">
        <p class="left_heading">
          <span>Meet</span>
          <span>great</span>
          <span>minds</span>
        </p>
        <p class="left_heading_text">
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ab esse,
          maiores voluptatem.
        </p>
      </div>
      <div class="right">
        <img src="../assets/guy.png" alt>
      </div>
      <div class="btn-wrapp">
        <button class="yellow-btn mt20">Join now</button>
      </div>
    </div>
    <div class="legends">
      <p class="heading yellow_heading">These legends are community members</p>
      <div class="legend">
        <div class="legend-img">
          <img src="../assets/guy.png" alt>
        </div>
        <h3 class="name">User name</h3>
      </div>
      <div class="legend">
        <div class="legend-img">
          <img src="../assets/guy.png" alt>
        </div>
        <h3 class="name">User name</h3>
      </div>
      <div class="legend">
        <div class="legend-img">
          <img src="../assets/guy.png" alt>
        </div>
        <h3 class="name">User name</h3>
      </div>
      <div class="legend">
        <div class="legend-img">
          <img src="../assets/guy.png" alt>
        </div>
        <h3 class="name">User name</h3>
      </div>
      <div class="legend">
        <div class="legend-img">
          <img src="../assets/guy.png" alt>
        </div>
        <h3 class="name">User name</h3>
      </div>
      <div class="legend">
        <div class="legend-img">
          <img src="../assets/guy.png" alt>
        </div>
        <h3 class="name">User name</h3>
      </div>
    </div>
    <div class="howitWorks">
      <p class="heading yellow_heading">How it works</p>
      <div class="col">
        <img src="../assets/one.png" alt>
        <span>Sign up</span>
      </div>
      <div class="col">
        <img src="../assets/two.png" alt>
        <span>Get vetted</span>
      </div>
      <div class="col">
        <img src="../assets/three.png" alt>
        <span>Attend meetups</span>
      </div>
      <br>
      <button class="yellow-btn">Join now</button>
    </div>
    <div class="testimonials">
      <p class="heading yellow_heading">What other photographers are saying</p>
      <div class="single_testimonial">
        <testimonial/>
      </div>
      <div class="single_testimonial">
        <testimonial/>
      </div>
      <div class="single_testimonial">
        <testimonial/>
      </div>
    </div>
  </div>
</template>
<script>
import Testimonial from "../components/Testimonial.vue";
export default {
  components: {
    Testimonial
  }
};
</script>
<style lang="scss" scoped>
$base-color: #e5a81d;
.home {
  .hero {
    color: #fff;
    position: relative;
    top: 0;
    height: 300px;
    overflow: hidden;
    text-align: center;
    .hero-img {
      position: absolute;
      top: -100px;
      left: 0;
      width: 100%;
      z-index: 3;
    }
    .overlay {
      background-color: #000;
      opacity: 0.7;
      position: absolute;
      top: -20px;
      height: 500px;
      width: 100%;
      z-index: 4;
    }
    .hero-content {
      position: absolute;
      top: 30px;
      height: 300px;
      z-index: 5;
    }
    h1 {
      font-size: 30px;
    }
    h3 {
      font-size: 14px;
      width: 40%;
      line-height: 20px;
      margin: 20px 30%;
    }
  }

  .grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(200px, 1fr));
    grid-auto-rows: minmax(30px, auto);
    grid-gap: 10px;
    grid-auto-flow: dense;
    padding: 10px;
    img {
      display: block;
      height: 100%;
      width: 100%;
      object-fit: cover;
    }

    .grid__item {
      height: 200px;
      overflow: hidden;
      display: grid;
      grid-gap: 10px;
      grid-auto-flow: dense;
      .grid_inner {
        display: block;
        width: 100%;
        height: 250px;
      }

      .grid_inner_bigger {
        display: block;
        width: 100%;
        height: 300px;
      }
      .grid_inner_smaller {
        display: block;
        width: 100%;
        height: 200px;
      }
    }

    .grid__item:nth-child(1) {
      grid-row: 1;
      height: 500px;
      grid-column-end: span 2;
    }

    .grid__item:nth-child(2) {
      grid-row: 1;
      height: 500px;
      grid-column-end: span 15;
    }

    .grid__item:nth-child(3) {
      grid-row: 1;
      height: 500px;
      grid-column-end: span 3;
    }
  }

  .community {
    padding: 30px 100px;
    background-color: #fefaf3;
    h1 {
      font-size: 40px;
      width: 100%;
      margin-bottom: 60px;
      text-align: center;
      color: #4d4d4d;
    }
    .left {
      width: 40%;
      float: left;
      .left_heading {
        text-align: left;
        font-weight: 600;
        font-size: 80px;
        color: #4d4d4d;
        span {
          display: block;
        }

        .left_heading_text {
          color: #4d4d4d;
          font-size: 30px;
          margin-right: 100px;
          text-align: left;
        }
      }
    }
    .right {
      width: 60%;
      float: right;
      img {
        width: 100%;
      }
    }
    .btn-wrapp {
      width: 100%;
      display: inline-block;
      text-align: center;
    }
  }

  .legends {
    padding: 20px 100px;
    background-color: #fefaf3;
    .legend {
      display: inline-block;
      max-width: 16.3%;
      height: 200px;
      overflow: hidden;
      padding: 0 10px;
    }
    .legend-img {
      width: 100%;
      height: 150px;
      overflow: hidden;
      border-radius: 10px;
      img {
        height: 120%;
        width: 120%;
        object-fit: cover;
      }
    }
    .name {
      font-size: 12px;
      text-align: center;
      color: #4d4d4d;
    }
  }
  .howitWorks {
    padding: 20px 150px 100px 150px;
    background-color: #fefaf3;
    text-align: center;
    .col {
      display: inline-block;
      max-width: 30%;
      min-width: 30%;
      img {
        height: 100px;
      }
      span {
        display: block;
        color: #4d4d4d;
      }
    }
    .yellow-btn {
      margin-top: 30px;
    }
  }
  .testimonials {
    padding: 40px 100px;
    .single_testimonial {
      display: inline-block;
      max-width: 33%;
      max-width: 33%;
      padding: 10px;
    }
  }
  .yellow_heading {
    color: $base-color;
    font-size: 30px;
    font-weight: 600;
    width: 100%;
    margin-top: 60px;
    text-align: center;
  }
}
</style>
