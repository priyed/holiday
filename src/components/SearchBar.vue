<template>
  <div class="search_form">
    <img src="../assets/search_icon.svg" alt="" />
    <input
      type="text"
      name=""
      id="search"
      placeholder="Search for the best location"
    />
  </div>
</template>

<style scoped>
.search_form {
  width: 100%;
  height: 59px;
  background: #fbfafa;
  border: 1px solid rgba(0, 0, 0, 0.2);
  border-radius: 20px;
  margin: 30px auto;
  padding: 0 20px;
  display: flex;
  align-items: center;
}
img {
  width: 20px;
  height: 20px;
}

input {
  border: none;
  background: none;
  width: 100%;
  color: #c4c4c4;
  margin-left: 10px;
  padding: 10px;
}

input::placeholder {
  color: #c4c4c4;
  font-size: 14px;
  line-height: 45px;
}

input:focus {
  border: none;
  outline: none;
  background: none;
}
</style>
