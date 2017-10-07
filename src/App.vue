<template>
  <div class="grid-container">
    <div class="grid-x grid-margin-x">
      <div class="cell">
        <app-quote v-for="quote in quotes">
          <template slot="title" v-if="quote.title">
            {{ quote.title }}
          </template>
          <template slot="content" v-if="quote.content">
            {{ quote.content }}
          </template>
          <template slot="author" v-if="quote.author">
            {{ quote.author }}
          </template>
        </app-quote>
      </div>
    </div>
  </div>
</template>

<script>
import AppQuote from "./components/AppQuote.vue";

export default {
  data() {
    return {
      quotes: [
        {
          title: 'Revolution did not necessarily involve sanguinary strife. It was not a cult of bomb and pistol.',
          content: 'The people generally get accustomed to the established order of things and begin to tremble at the very idea of a change. It is this lethargical spirit that needs be replaced by the revolutionary spirit. The spirit of Revolution should always permeate the soul of humanity, so that the reactionary forces may not accumulate to check its eternal onward march. Old order should change, always and ever, yielding place to new, so that one good order may not corrupt the world. It is in this sense that we raise the shout "Long Live Revolution."',
          author: 'Bhagat Singh'
        },
        {
          title: 'If I had foreseen Hiroshima and Nagasaki, I would have torn up my formula in 1905.',
          content: 'America is a democracy and has no Hitler, but I am afraid for her future; there are hard times ahead for the American people, troubles will be coming from within and without. America cannot smile away their Negro problem nor Hiroshima and Nagasaki. There are cosmic laws.',
          author: 'Albert Einstein'
        },
        {
          title: 'To call woman the weaker sex is a libel; it is man\'s injustice to woman.',
          content: 'If by strength is meant brute strength, then, indeed, is woman less brute than man. If by strength is meant moral power, then woman is immeasurably man\'s superior. Has she not greater intuition, is she not more self-sacrificing, has she not greater powers of endurance, has she not greater courage? Without her, man could not be. If nonviolence is the law of our being, the future is with woman. Who can make a more effective appeal to the heart than woman?',
          author: 'Mohandas Karamchand Gandhi'
        },
      ]
    };
  },
  components: { AppQuote }
}
</script>

<style lang="scss" scoped>
  
</style>
