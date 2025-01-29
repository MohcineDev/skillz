<script setup>
import CourseCard from "./CourseCard.vue";


</script>

<template>
  <section class="courses">
    <span>Our Courses</span>
    <h2>Browse Our Best Courses</h2>
    <div class="container">
      <div class="wrapper">
        <CourseCard title="Learn coding the fun way possible" tag="Business"/>
        <CourseCard title="Track your progress effortlessly" tag="Technology"/>
        <CourseCard  title="Master productivity with ease" tag="Health"/>
        <CourseCard  title="Stay organized and on top of tasks" tag="Education"/>
      </div>
      <div class="wrapper">
        <CourseCard  title="Collaborate seamlessly with your team" tag="Sports"/>
        <CourseCard  title="Unlock your creativity through design" tag="Politics"/>
        <CourseCard  title="Analyze data with just a few clicks" tag="Entertainment"/>
        <CourseCard  title="Get personalized health tips every day" tag="Literature"/>
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
  max-width: var(--max-width);
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
  justify-content: center;
  margin: 20px 0;
}

h2 {
  color: #222;
  font-size: 2rem;
  margin-top: 0;
}
</style>