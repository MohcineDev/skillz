<script setup>
</script>

<template>
  <div class="card">
    <div class="title">
      <span>Marketing</span>
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="#222" class="size-6">
        <path fill-rule="evenodd"
          d="M6.32 2.577a49.255 49.255 0 0 1 11.36 0c1.497.174 2.57 1.46 2.57 2.93V21a.75.75 0 0 1-1.085.67L12 18.089l-7.165 3.583A.75.75 0 0 1 3.75 21V5.507c0-1.47 1.073-2.756 2.57-2.93Z"
          clip-rule="evenodd" />
      </svg>
    </div>
    <h2>Creative Writing for Beginners</h2>
    <div class="Progress">
      <span>Progress</span>
      <span> 8 / 20 lessons</span>
    </div>
    <progress id="file" value="32" max="100">32%</progress>
    <div class="card-footer">
      <div class="others">
        <div></div>
        <div></div>
        <div></div>
      </div>
      <button>Continue</button>
    </div>
  </div>
</template>

<style scoped>
Progress {
  width: 100%;
}

.Progress {
  display: flex;
  justify-content: space-between;
}

.card {
  box-shadow: 0 0 3px #506a92;
  background: rgb(243, 243, 100);
  margin: 1rem;
  padding: 20px;
  border-radius: 15px;
  border: 2px solid #222;
}

.title,
.card-footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.title span {
  padding: 2px 5px;
  border-radius: 5px;
}

.title svg {
  width: 20px;
}

.title span {
  background: #222;
  color: #fff;
}

.others {
  display: flex;
}

.others div {
  width: 40px;
  height: 40px;
  background: url("../assets/images.jpeg") center / cover;
  border-radius: 50%;
  border: 1px solid #222;
  margin-left: -10px;
}

button {
  border-radius: 5px;
  color: #222;
  padding: 5px 10px;
  background: var(--red-light);
  border: none;
  color: #eee;
}
</style>