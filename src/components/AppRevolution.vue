<template>
  <blockquote>
    <h5>
      <slot name="title">Revolution did not necessarily involve sanguinary strife. It was not a cult of bomb and pistol.</slot>
    </h5>
    <p>
      <slot name="content">The people generally get accustomed to the established order of things and begin to tremble at the very idea of a change. It is this lethargical spirit that needs be replaced by the revolutionary spirit. The spirit of Revolution should always permeate the soul of humanity, so that the reactionary forces may not accumulate to check its eternal onward march. Old order should change, always and ever, yielding place to new, so that one good order may not corrupt the world. It is in this sense that we raise the shout "Long Live Revolution".</slot>
    </p>
    <cite>
      <slot name="author">Bhagat Singh</slot>
    </cite>
  </blockquote>
</template>

<script>
export default {
}
</script>

<style lang="scss" scoped>
  h5 { color: #cc4b37; }
  p { font-size: 0.95rem;margin-bottom: 0.5rem; }
  cite { font-weight: bold; }
</style>
