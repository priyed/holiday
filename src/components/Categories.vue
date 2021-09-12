<template>
  <div class="categories">
    <span v-for="category in categories" :key="category">{{ category }}</span>
  </div>
</template>

<script>
export default {
  props: {
    categories: {
      type: Array,
      required: true,
    },
  },
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Red+Rose:wght@300;400;500&display=swap");

.categories {
  overflow: auto;
  white-space: nowrap;
  margin-top: 30px;
}

.categories::-webkit-scrollbar {
  width: 0px;
  background: transparent;
}

span {
  font-family: "Red Rose", cursive;
  font-size: 14px;
  margin-right: 20px;
  line-height: 45px;
  color: #c4c4c4;
  cursor: pointer;
  user-select: none;
  transition: all 0.3s ease;
}

span:hover {
  color: #1c8af0;
}
</style>
