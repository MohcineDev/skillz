<script setup>
</script>

<template>

  <div class="test-container">
    <header>
      <h1>Full Stack Developer Assessment</h1>
      <p>Please answer the following questions to the best of your ability.</p>
    </header>

    <form id="test-form">
      <!-- Frontend Section -->
      <section class="section">
        <h2>Frontend (HTML/CSS/JS)</h2>
        <div class="question">
          <label for="html-question">What is the purpose of the 'alt' attribute in an <img> tag?</label>
          <textarea id="html-question" name="html-question"></textarea>
        </div>
        <!-- Add more questions for frontend -->
      </section>

      <!-- Backend Section -->
      <section class="section">
        <h2>Backend (Node.js/Express)</h2>
        <div class="question">
          <label for="node-question">Explain how to create a REST API using Node.js and Express.</label>
          <textarea id="node-question" name="node-question"></textarea>
        </div>
        <!-- Add more backend questions -->
      </section>

      <!-- Coding Challenge -->
      <section class="section">
        <h2>Coding Challenge</h2>
        <div class="question">
          <label for="coding-challenge">Write a function in JavaScript to reverse a string.</label>
          <textarea id="coding-challenge" name="coding-challenge"></textarea>
        </div>
      </section>

      <button type="submit">Submit Test</button>
    </form>
  </div>


</template>


<style scoped>
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  background-color: #f4f7fa;
}

.test-container {
  width: 80%;
  max-width: 800px;
  margin: 0 auto;
  background-color: white;
  padding: 20px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

header {
  text-align: center;
}

h1 {
  color: #333;
}

.section {
  margin-bottom: 20px;
}

h2 {
  font-size: 1.5rem;
  margin-bottom: 10px;
}

label {
  font-weight: bold;
  display: block;
}

textarea {
  width: 100%;
  height: 100px;
  padding: 10px;
  border: 1px solid #ddd;
  border-radius: 5px;
}

button {
  background-color: #4CAF50;
  color: white;
  padding: 10px 20px;
  border: none;
  cursor: pointer;
  font-size: 1rem;
  margin-top: 20px;
  border-radius: 5px;
}

button:hover {
  background-color: #45a049;
}

</style>