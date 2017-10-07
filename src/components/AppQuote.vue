<template>
  <blockquote>
    <h5>
      <slot name="title">My Wonderful Quote</slot>
    </h5>
    <p>
      <slot name="content">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Inventore at quod est nulla neque, molestiae aspernatur facere reprehenderit maxime fugiat.</slot>
    </p>
    <cite>
      <slot name="author">Dummy Man</slot>
    </cite>
  </blockquote>
</template>

<script>
export default {
}
</script>

<style lang="scss" scoped>
  h5 { color: #0ea29d; }
  p { font-size: 0.95rem;margin-bottom: 0.5rem; }
  cite { font-weight: bold; }
</style>
