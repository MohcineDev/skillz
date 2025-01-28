<script setup>
</script>

<template>
  <header>
    <div class="left">
      <div class="title">
        <p><span>50% OFF</span> LEARN FROM TODAY</p>
      </div>
      <h1>
        Lorem ipsum dolor sit amet, consectet vero dignissimos voluptate in
        commodi.
      </h1>
      <p>
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Enim qui harum
        cumque a tenetur in recusandae officia minima voluptas earum. cumque a
        tenetur in recusandae officia minima voluptas earum. cumque a tenetur in
        recusandae officia minima voluptas earum.
      </p>
      <div class="wrapper">
        <a href="" class="courses"
          >Explore Courses
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            class="size-6"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M13.5 4.5 21 12m0 0-7.5 7.5M21 12H3"
            />
          </svg>
        </a>
        <div class="demo">
          <i>
            <svg
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke-width="1.5"
              stroke="currentColor"
              class="size-6"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="m15.75 10.5 4.72-4.72a.75.75 0 0 1 1.28.53v11.38a.75.75 0 0 1-1.28.53l-4.72-4.72M4.5 18.75h9a2.25 2.25 0 0 0 2.25-2.25v-9a2.25 2.25 0 0 0-2.25-2.25h-9A2.25 2.25 0 0 0 2.25 7.5v9a2.25 2.25 0 0 0 2.25 2.25Z"
              />
            </svg>
          </i>

          <a href="">Watch Demo</a>
        </div>
      </div>
    </div>
    <div class="right">
      <img src="../assets/undraw_finance_m6vw.svg" alt="" />
    </div>
  </header>
</template>    

<style scoped>
header {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  margin: 4rem 20px;
  align-items: center;
  justify-content: center;
}
.wrapper {
  display: flex;
  align-items: center;
  margin: 20px 0;
}
.demo {
  margin: 0 20px;
  display: flex;
  align-items: center;
}
.demo i {
  margin: 10px;
  background: rgb(253, 182, 49);
  width: 30px;
  height: 30px;
  border-radius: 50%;
  display:flex;
  color:#fff;
  align-items:center;
  justify-content:center;
}
.demo a {
  text-decoration-line: underline;
  text-decoration-style: solid;
  text-decoration-color: var(--blue);
}
.wrapper a.courses {
  background: var(--blue);
  padding: 5px 10px;
  color: #eee;
  border-radius: 10px;
  display: flex;
  align-items: center;
}
.wrapper a.courses svg {
  margin-left: 5px;
}

.left {
}
img {
  width: 80%;
}
header > div {
  margin: 2rem;
}
.right {
  display: flex;
  align-items: center;
  justify-content: center;
}
h1 {
  font-weight: 700;
  font-size: 2.5rem;
}
.left .title {
  color: var(--red);
}
.left .title span {
  background-color: var(--red);
  color: #eee;
  border-radius: 20px;
  padding: 5px 10px;
  margin-right: 5px;
}
svg {
  width: 20px;
  height: 20px;
}
</style>