<template>
  <div class="testimonial">
    <div class="testimonial-content">
      <p class="testimonial_text">
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dolores ipsa nesciunt
        necessitatibus nostrum quo debitis dolorum laborum autem. Soluta incidunt voluptas id
        nisi sapiente. Exercitationem consequatur officiis quae quo voluptates!
      </p>
      <div class="user_photo">
        <img src="../assets/guy.png" alt>
      </div>
      <div class="user_details">
        <p class="user_name">Jon Doe</p>
        <p class="title">UI/UX Designer</p>
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
.testimonial {
  border: 1px solid #cecece;
  padding: 15px;
  height: auto;
  border-radius: 5px;
  display: flex;
  .testimonial_text {
    color: grey;
    font-size: 14px;
    line-height: 18px;
    margin-top: 0;
  }
  .user_photo {
    width: 40px;
    height: 40px;
    margin: 0 20px 0 0;
    float: left;
    border-radius: 100%;
    overflow: hidden;
    img {
      width: 100%;
    }
  }
  .user_details {
    width: 70%;
    float: left;
    .user_name {
      font-size: 14px;
      font-weight: 600;
      margin: 0;
    }
    .title {
      font-size: 10px;
      margin: 0;
    }
  }
}
</style>
