<template>
  <h1>Resume</h1>
  <div class="timeline">
  <div class="container left">
    <div class="content">
      <h3>Sep 2022- present</h3>
      <h5>Life Choices Academy</h5>
      <p>Coding bootcamp</p>
    </div>
  </div>
  <div class="container right">
    <div class="content">
      <h3>2021 - 2022</h3>
      <h5>Digital Tribe</h5>
      <p>Customer Service Advisor</p>
    </div>
  </div>
  <div class="container left">
    <div class="content">
      <h3>2019-2020</h3>
      <h5>KFC</h5>
      <p>Team member</p>
    </div>
  </div>
  <div class="container right">
    <div class="content">
      <h3>2014 - 2018</h3>
      <h5>Salt River Secondary</h5>
      <p>Matric</p>
    </div>
  </div>
</div>
</template>

<script>
export default {

}
</script>

<style scoped>
/* The actual timeline (the vertical ruler) */
.timeline {
  position: relative;
  max-width: 1200px;
  margin: 0 auto;
  box-sizing: border-box;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

/* The actual timeline (the vertical ruler) */
.timeline::after {
  content: '';
  position: absolute;
  width: 6px;
  background-color: #23432a;
  top: 0;
  bottom: 0;
  left: 50%;
  margin-left: -3px;
}

/* Container around content */
.container {
  padding: 10px 40px;
  position: relative;
  background-color: inherit;
  width: 50%;
  margin-left: -3px;
}

/* The circles on the timeline */
.container::after {
  content: '';
  position: absolute;
  width: 25px;
  height: 25px;
  right: -17px;
  background-color: beige;
  border: 4px solid #23432a;
  top: 15px;
  border-radius: 50%;
  z-index: 1;
}

/* Place the container to the left */
.left {
  left: 0;
}

/* Place the container to the right */
.right {
  left: 50%;
}

/* Add arrows to the left container (pointing right) */
.left::before {
  content: " ";
  height: 0;
  position: absolute;
  top: 22px;
  width: 0;
  z-index: 1;
  right: 30px;
  border: medium solid #5b9466;
  border-width: 10px 0 10px 10px;
  border-color: transparent transparent transparent #5b9466;
}

/* Add arrows to the right container (pointing left) */
.right::before {
  content: " ";
  height: 0;
  position: absolute;
  top: 22px;
  width: 0;
  z-index: 1;
  left: 30px;
  border: medium solid #5b9466;
  border-width: 10px 10px 10px 0;
  border-color: transparent #5b9466 transparent transparent;
}

/* Fix the circle for containers on the right side */
.right::after {
  left: -10px;
}

/* The actual content */
.content {
  padding: 20px 30px;
  background-color: #5b9466;
  position: relative;
  border-radius: 6px;
}

/* Media queries - Responsive timeline on screens less than 600px wide */
@media screen and (max-width: 600px) {
/* Place the timelime to the left */
  .timeline::after {
    left: 31px;
  }

/* Full-width containers */
  .container {
    width: 100%;
    padding-left: 70px;
    padding-right: 25px;
  }

/* Make sure that all arrows are pointing leftwards */
  .container::before {
    left: 60px;
    border: medium solid #5b9466;
    border-width: 10px 10px 10px 0;
    border-color: transparent #5b9466 transparent transparent;
  }

/* Make sure all circles are at the same spot */
  .left::after, .right::after {
    left: 15px;
  }

/* Make all right containers behave like the left ones */
  .right {
    left: 0%;
  }
}

</style>