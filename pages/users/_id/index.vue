<template>
  <div>
    <h2>single user page suck em</h2>
    <h3>{{ $route.params.id }}</h3>
    <h3>{{ $route.params }}</h3>
  </div>
</template>

<script>
export default {
  validate(data) {
    return /^\d+$/.test(data.params.id)
  }
}
</script>
