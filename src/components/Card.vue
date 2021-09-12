<template>
  <div class="card-container">
    <div class="card" v-for="location in locations" :key="location.id">
      <img :src="location.image" :alt="location.name" />
      <h4>{{ location.name }}</h4>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      locations: [
        {
          id: "323849083mndjhfiwuo2ur",
          name: "Paris",
          description:
            "The magnetic City of Light draws visitors from around the globe who come to see iconic attractions like the Eiffel Tower, the Louvre and the Arc de Triomphe. But what travelers really fall in love with are the city's quaint cafes, vibrant markets, trendy shopping districts and unmistakable je ne sais quoi charm",
          image: [require("../assets/images/paris.png")],
          ratings: 5,
        },
        {
          id: ";kf;kdjfiep82p857puvlur",
          name: "Maldives",
          description:
            "With crystal white sands and sheltered lagoons, the Maldives redefines paradise. For those seeking relaxation, our all-inclusive Maldives holidays help you make the most of some of the world's best beach resorts. Meanwhile, adventure lovers can experience world-class diving, surfing, fishing, kayaking and more. With over 1,000 coral islands to enjoy, there's no shortage of things to see or do on trips to the Maldives.",
          image: [require("../assets/images/maldives.png")],
          ratings: 4,
        },
        {
          id: "29834i;dfpoiar8498",
          name: "London",
          description:
            "It's little wonder London, England is one of the world's top tourist destinations, attracting upward of 20 million visitors each year from around the world. Britains's capital city is a vibrant arts and entertainment center (its theaters are always busy). London offers one of the planets's greatest concentrations of cultural attractions.",
          image: [require("../assets/images/london.jpg")],
          ratings: 4,
        },
        {
          id: "ep98q2yidh;wyupafauhu",
          name: "Tokyo",
          description:
            "Simply setting foot in Japan's cosmopolitan capital is an experience within itself. A city known for its bustling streets and flashing neon signs, Tokyo has an electric energy and plenty of attractions to discover. Foodies won't be let down by the city's fresh sushi and hearty ramen",
          image: [require("../assets/images/tokyo.jpg")],
          ratings: 3,
        },
      ],
    };
  },
};
</script>

<style scoped>
.card-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  margin-bottom: 50px;
  z-index: -10;
}

.card {
  width: 159px;
  height: 344px;
  border-radius: 30px;
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 7px;
  overflow: hidden;
  cursor: pointer;
  transition: all 0.3s ease-in-out;
}

.card:hover {
  transform: scale(1.03);
}

img {
  width: 100%;
  height: 100%;
  cursor: pointer;
}
h4 {
  font-family: "Red Rose", cursive;
  font-style: normal;
  font-weight: normal;
  font-size: 20px;
  line-height: 45px;
  color: #fff;
  position: absolute;
  bottom: 10px;
  margin: 0 auto;
  z-index: 10;
  cursor: pointer;
}
</style>
