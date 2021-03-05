<template>
  <div class="dashboard-container">
    <div class="dashboard-text">name: {{ name }}</div>
    <img
      height="1000"
      src="../../../image/C7181A414BCD2616311C70B0813F3134.png"
    />
  </div>
</template>

<script>
import { mapGetters } from "vuex";

export default {
  name: "Dashboard",
  computed: {
    ...mapGetters(["name"]),
  },
};
</script>

<style lang="scss" scoped>
.dashboard {
  &-container {
    margin: 30px;
  }
  &-text {
    font-size: 30px;
    line-height: 46px;
  }
}
</style>
