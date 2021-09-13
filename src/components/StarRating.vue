<template>
  <div class="star-rating">
    <label
      class="star-rating__star"
      :key="rating"
      v-for="rating in ratings"
      :class="{
        'is-selected': value >= rating && value != null,
        'is-disabled': disabled,
      }"
    >
      <input
        class="star-rating star-rating__checkbox"
        type="radio"
        :value="rating"
        :disabled="disabled"
      />★</label
    >
  </div>
</template>

<script>
export default {
  props: {
    value: {
      type: Number,
      required: true,
    },
    disabled: Boolean,
  },

  data: function () {
    return {
      temp_value: null,
      ratings: [1, 2, 3, 4, 5],
    };
  },

  methods: {
    set: function (value) {
      if (!this.disabled) {
        return value;
      }
    },
  },
};
</script>

<style scoped>
.star-rating {
  display: flex;
  position: absolute;
  top: 20px;
  left: 10px;
  width: auto;
  height: 12px;
  background: rgba(0, 0, 0, 0.08);
  border-radius: 14px;
  z-index: 9;
}
.star-rating__checkbox {
  position: absolute;
  overflow: hidden;
  height: 1px;
  width: 1px;
  margin: -1px;
  padding: 0;
  border: 0;
}

.star-rating__star {
  display: inline-block;
  padding: 3px;
  vertical-align: middle;
  line-height: 1;
  font-size: 0.5em;
  color: #ababab;
  -webkit-transition: color 0.2s ease-out;
  transition: color 0.2s ease-out;
}

.star-rating__star.is-selected {
  color: #fff;
}

.star-rating__star.is-disabled:hover {
  cursor: default;
}
</style>
