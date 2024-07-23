<template>
  <main>
    <div class="container">
      <header>
        <h1>Notes</h1>
        <button>+</button>
      </header>
      <div class="cards-container">
        <div class="card">
          <p class="main-text">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Tempore corporis omnis
            laboriosam dicta dignissimos pariatur, cumque quis. Obcaecati, provident possimus.</p>
          <p class="date">04/27/2024</p>
        </div>
      </div>
    </div>
  </main>
</template>

<style scoped>
main {
  height: 100vh;
  width: 100vw;
}

.container {
  max-width: 1000px;
  padding: 10px;
  margin: 0 auto;
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

h1 {
  font-weight: bold;
  margin-bottom: 25px;
  font-size: 3.5rem;
}

button {
  border: none;
  padding: 10px;
  width: 3rem;
  height: 3rem;
  cursor: pointer;
  background-color: black;
  border-radius: 100%;
  color: white;
  font-size: 1.5rem;
}

.card {
  width: 15rem;
  height: 15rem;
  background-color: darkorange;
  padding: 10px;
  border-radius: 15px;
  display: flex;
  justify-content: space-between;
  margin-right: 20px;
  margin-bottom: 20px;
}

.date {
  font-size: 0.75rem;
  font-weight: bold;
}

.cards-container {
  display: flex;
  flex-wrap: wrap;
}
</style>