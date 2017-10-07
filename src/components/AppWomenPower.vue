<template>
  <blockquote>
    <h5>
      <slot name="title">To call woman the weaker sex is a libel; it is man's injustice to woman.</slot>
    </h5>
    <p>
      <slot name="content">If by strength is meant brute strength, then, indeed, is woman less brute than man. If by strength is meant moral power, then woman is immeasurably man's superior. Has she not greater intuition, is she not more self-sacrificing, has she not greater powers of endurance, has she not greater courage? Without her, man could not be. If nonviolence is the law of our being, the future is with woman. Who can make a more effective appeal to the heart than woman?</slot>
    </p>
    <cite>
      <slot name="author">Mohandas Karamchand Gandhi</slot>
    </cite>
  </blockquote>
</template>

<script>
export default {
}
</script>

<style lang="scss" scoped>
  h5 { color: #1779ba; }
  p { font-size: 0.95rem;margin-bottom: 0.5rem; }
  cite { font-weight: bold; }
</style>
