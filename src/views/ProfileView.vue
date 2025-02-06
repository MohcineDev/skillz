<script setup>
import FooterCmp from "@/components/footerCmp.vue";
import NavBar from "../components/Nav.vue";
import profileCourse from "../components/profileCourse.vue";
</script>

<template>
  <NavBar />
  <section class="taken-courses">
    <div class="container">
      <h2>My Courses</h2>
      <div class="wrapper">

        <profileCourse />
        <profileCourse class="two" />
        <profileCourse class="three" />
      </div>
    </div>
  </section>
  <section>
    <div class="container">
      <h2>My Next Lessons</h2>

      <div class="lessons">
        <div class="header">
          <span>Lesson</span>
          <span>Teacher</span>
          <span>Duration</span>
        </div>
        <div class="line">
          <div>
            <p>01. Introduction to creative writing</p>
            <p>Crative writing for beginners</p>
          </div>
          <div class="teacher">
            <div></div>
            <span>Conner Garcia</span>
          </div>
          <div>22min</div>
        </div>
        <div class="line">
          <div>
            <p>01. Introduction to creative writing</p>
            <p>Crative writing for beginners</p>
          </div>
          <div class="teacher">
            <div></div>
            <span>Conner Garcia</span>
          </div>
          <div>22min</div>
        </div>
        <div class="line">
          <div>
            <p>01. Introduction to creative writing</p>
            <p>Crative writing for beginners</p>
          </div>
          <div class="teacher">
            <div></div>
            <span>Conner Garcia</span>
          </div>
          <div>22min</div>
        </div>
        <div class="line">
          <div>
            <p>01. Introduction to creative writing</p>
            <p>Crative writing for beginners</p>
          </div>
          <div class="teacher">
            <div></div>
            <span>Conner Garcia</span>
          </div>
          <div>22min</div>
        </div>
        <div class="line">
          <div>
            <p>01. Introduction to creative writing</p>
            <p>Crative writing for beginners</p>
          </div>
          <div class="teacher">
            <div></div>
            <span>Conner Garcia</span>
          </div>
          <div>22min</div>
        </div>
        <div class="line">
          <div>
            <p>01. Introduction to creative writing</p>
            <p>Crative writing for beginners</p>
          </div>
          <div class="teacher">
            <div></div>
            <span>Conner Garcia</span>
          </div>
          <div>22min</div>
        </div>

      </div>
    </div>
  </section>
  <FooterCmp />
</template>

<style scoped>
section {
  padding: 1rem;
}

.container {
  max-width: var(--max-width);
  margin: 2rem auto;
}

.wrapper {
  display: flex;

}

.two {
  background: rgb(229, 128, 251);
}

.three {
  background: rgb(151, 177, 242);
}

.teacher>div {
  width: 40px;
  height: 40px;
  background: url("../assets/images.jpeg") center / cover;
  border-radius: 50%;
  border: 1px solid #222;
  margin-left: -10px;
}

.lessons {
  margin: 2rem auto;
  border: 1px solid #555;
  padding: 2rem;
  border-radius: 20px;
  box-shadow: 0 0 3px #506a92;

}

.lessons .header {
  font-weight: 600;
}

.teacher {
  display: flex;
  align-items: center;
}

.teacher span {
  margin-left: 15px;
}

.header,
.line {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  justify-items: center;
}

.header>span:nth-child(1),
.line>div:nth-child(1) {
  justify-self: start;
}

.line {
  align-items: center;
}

.line:not(.line:last-child) {
  border-bottom: 1px solid #888;
}

.line>div>p:nth-child(1) {
  color: #222;
  font-weight: 700;
  margin-bottom: 5px;
}

.line>div>p:nth-child(2) {
  margin-top: 0;
}
</style>