<template >
  <div class="marquee">
    <marquee behavior="scroll" direction="left" loop>
      <div class="d-flex align-items-center">
        <div class="d-flex align-items-center gap-2" v-for="i in 30" :key="i">
          <span class="coffee">coffee</span>

          <img src="@/assets/images/Group (1).png" class="mx-3" />
        </div>
      </div>
    </marquee>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
.marquee {
  width: 100%;
  margin-block: 3rem;
}
.coffee {
  color: #6f4336;
  font-weight: 400;
  font-size: 1.2rem;
}
</style>