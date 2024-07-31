<template >
  <div class="footer">
    <div class="container">
      <div class="row border-bottom">
        <div class="col-lg-4 col-sm-12">
          <ul>
            <p>Menu</p>
            <li>Get inspired</li>
            <li>Our products</li>
            <li>For a better world</li>
            <li>Contact</li>
            <li>Blog</li>
          </ul>
        </div>
        <div class="col-lg-4 col-sm-12">
          <ul>
            <p>CafeLocatotion</p>
            <li>lorem ipsum</li>
          </ul>
        </div>
        <div class="col-lg-4 col-sm-12">
          <ul>
            <p>Contact</p>
            <li>Do you have a question? Send it to us!</li>
            <p class="mt-5">000000000</p>
          </ul>
        </div>
      </div>
      <div class="row mt-5">
        <div class="col-12">
          <div class="d-flex justify-content-between">
            <p class="mb-0">Privacy policy</p>
            <div class="d-flex gap-3 align-items-center">
              <img src="@/assets/images/Link.png" style="cursor: pointer" />
              <img src="@/assets/images/Link (1).png" style="cursor: pointer" />
              <img src="@/assets/images/Link (2).png" style="cursor: pointer" />
            </div>
          </div>
        </div>
      </div>
    </div>
    <img src="@/assets/images/Group 1000010753.png" class="imageFoter" />
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss"
scoped>
.footer {
  margin-top: 10rem;
  position: relative;
  width: 100%;

  background: #004876;
  color: white;

  display: flex;
  justify-content: center;
  align-items: center;

  .imageFoter {
    position: absolute;
    // bottom: 0;
    // right: 0;
    // width: 100%;
  }
}
ul {
  list-style: none;
  p {
    font-size: 1.2rem;
    font-weight: 600;
  }
  li {
    font-size: 0.9rem;
    margin: 0.8rem 0;
    cursor: pointer;
  }
}
</style>