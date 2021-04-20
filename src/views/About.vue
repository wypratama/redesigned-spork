<template>
  <div class="about">
    <div id="nav">
      <router-link to="/">Tahap 1</router-link> |
      <router-link to="/about">Tahap 2</router-link> |
      <router-link to="/tahap-3">Tahap 3</router-link>
    </div>
    <h1>Search</h1>
    <input type="text" name="" id="" v-model="search">
    <button @click="searchText">Search</button>
    <div>
      <span>Result</span>
      <p>Found {{ foundWord }} occurances of the word "{{search}}" in the below text.</p>
    </div>
    <p>
      Turtles are reptiles of the order Chelonii[2] or Testudines characterised by a special bony or cartilaginous shell developed from their ribs and acting as a shield.[3] "Turtle" may either refer to the order as a whole, or to particular turtles which make up a form taxon that is not monophyletic.
    </p>
    <p>
      The order Chelonii or Testudines includes both extant (living) and extinct species. The earliest known turtles date from 220 million years ago,[4] making turtles one of the oldest reptile groups and a more ancient group than lizards, snakes or crocodiles. Of the many species alive today, some are highly endangered.[5]
    </p>
    <p>
      Like all other extant reptiles, turtles are ectotherms their internal temperature varies according to the ambient environment, commonly called cold-blooded. However, because of their high metabolic rate, leatherback sea turtles have a body temperature that is noticeably higher than that of the surrounding water.

Like other amniotes (reptiles, dinosaurs, birds, and mammals), they breathe air and do not lay eggs underwater, although many species live in or around water. The largest turtles are aquatic.
    </p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      search: '',
      foundWord: 0,
      searchData: `Turtles are reptiles of the order Chelonii[2] or Testudines characterised by a special bony or cartilaginous shell developed from their ribs and acting as a shield.[3] "Turtle" may either refer to the order as a whole, or to particular turtles which make up a form taxon that is not monophyletic.

The order Chelonii or Testudines includes both extant (living) and extinct species. The earliest known turtles date from 220 million years ago,[4] making turtles one of the oldest reptile groups and a more ancient group than lizards, snakes or crocodiles. Of the many species alive today, some are highly endangered.[5]

Like all other extant reptiles, turtles are ectotherms their internal temperature varies according to the ambient environment, commonly called cold-blooded. However, because of their high metabolic rate, leatherback sea turtles have a body temperature that is noticeably higher than that of the surrounding water.

Like other amniotes (reptiles, dinosaurs, birds, and mammals), they breathe air and do not lay eggs underwater, although many species live in or around water. The largest turtles are aquatic.`
    }
  },
  methods: {
    searchText () {
      // console.log(this.search)
      // console.log(this.$el.getElementsByTagName('p').map(el => el))
      const data = this.searchData.match(this.search)
      this.foundWord = data.length
      console.log(data.length)
    } 
  }
}
</script>