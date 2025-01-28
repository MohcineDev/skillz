<script>
</script>

<template>
  <div class="card">
    <div class="img"></div>
    <h3>Teach your kids math in simple way</h3>
    <div class="stats">
      <div>
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
            d="M3 8.689c0-.864.933-1.406 1.683-.977l7.108 4.061a1.125 1.125 0 0 1 0 1.954l-7.108 4.061A1.125 1.125 0 0 1 3 16.811V8.69ZM12.75 8.689c0-.864.933-1.406 1.683-.977l7.108 4.061a1.125 1.125 0 0 1 0 1.954l-7.108 4.061a1.125 1.125 0 0 1-1.683-.977V8.69Z"
          />
        </svg>

        <span>42 lessons</span>
      </div>
      <div class="rating">
        <svg
          v-for="item in 5"
          :key="item.id"
          xmlns="http://www.w3.org/2000/svg"
          fill="orange"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="none"
          class="size-6"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M11.48 3.499a.562.562 0 0 1 1.04 0l2.125 5.111a.563.563 0 0 0 .475.345l5.518.442c.499.04.701.663.321.988l-4.204 3.602a.563.563 0 0 0-.182.557l1.285 5.385a.562.562 0 0 1-.84.61l-4.725-2.885a.562.562 0 0 0-.586 0L6.982 20.54a.562.562 0 0 1-.84-.61l1.285-5.386a.562.562 0 0 0-.182-.557l-4.204-3.602a.562.562 0 0 1 .321-.988l5.518-.442a.563.563 0 0 0 .475-.345L11.48 3.5Z"
          />
        </svg>
      </div>
    </div>
  </div>
</template>
<style scoped>
.card {
  border: 1px solid #aaa;
  margin: 10px;
  border-radius: 15px;
  padding: 8px;
  text-align: left;
  background: #fff;
  box-shadow: 0 0 3px #aaa;
}

.stats {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.stats > div {
  display: flex;
  align-items: center;
}
.img {
  width: 100%;
  height: 140px;
  background-image: url("../assets/Skillz_Bridge.png");
  background-size: cover;
  background-repeat: no-repeat;
}
img {
  width: 150px;
}
svg {
  width: 15px;
}
</style>