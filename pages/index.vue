<template>
  <div>
    <h1 class="title">Home Page</h1>
    <div class="content-container">
      <Movie-card
        name="Avatar part 2"
        imgUrl="https://upload.wikimedia.org/wikipedia/en/5/54/Avatar_The_Way_of_Water_poster.jpg"
        imgAlt="Avatar Part 2 thumbnail"
        releaseDate="December 16, 2022"
      />
      <Movie-card
        name="Avatar part 2"
        imgUrl="https://upload.wikimedia.org/wikipedia/en/5/54/Avatar_The_Way_of_Water_poster.jpg"
        imgAlt="Avatar Part 2 thumbnail"
        releaseDate="December 16, 2022"
      />
      <!-- <h1>{{ getPopularList() }}</h1> -->
      <!-- <h1 v-for="popular in getPopularList" :key="popular">
        {{ popular }}
      </h1> -->
    </div>
  </div>
</template>

<script>

import apis from "@/store/api.js"
let requestOne = axios.get(apis.POPULAR_MOVIES)

export default {
  name: "IndexPage",
  methods: {
    axios.all([requestOne]).then(axios.spread((...responses) => {
  const responseOne = responses[0]
  const responseTwo = responses[1]
  const responesThree = responses[2]
  // use/access the results
})).catch(errors => {
  // react on errors.
})
  },
};
</script>
