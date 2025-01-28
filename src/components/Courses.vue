<script setup>
import CourseCard from "./CourseCard.vue";
</script>

<template>
  <section class="courses">
    <span>Our Courses</span>
    <h2>Browse Our Best Courses</h2>
    <div class="container">
      <div class="wrapper">
        <CourseCard />
        <CourseCard />
        <CourseCard />
        <CourseCard />
      </div>
      <div class="wrapper">
        <CourseCard />
        <CourseCard />
        <CourseCard />
        <CourseCard />
      </div>
    </div>
  </section>
</template>
<style scoped>
.courses {
  text-align: center;
  margin: 10rem auto;
  
}
.container {
    position: relative;
    max-width: 1000px;
    margin: 2rem auto;
}
.container::before {
  content: "";
  width: 110%;
  height: 200px;
  background: var(--blue-dark);
  position: absolute;
  z-index: -1;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  border-radius: 20px;
}
.wrapper {
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 20px 0 ;
}
h2{
    color:#222;
    font-size: 2rem;
    margin-top: 0;
}
</style>