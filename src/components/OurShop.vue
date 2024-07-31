<template >
  <div class="ourShop">
    <div class="container-fluid">
      <div class="row">
        <div class="col-lg-5 col-md-12 col-sm-12 p-0">
          <img src="@/assets/images/Explore.png" class="img-fluid-w-50" />
        </div>
        <div class="col-lg-7 col-md-12 col-sm-12">
          <div
            class="h-100 d-flex align-items-start justify-content-center flex-column"
          >
            <div class="titles">
              <h3 class="title-welcome">Wecome to Our shop</h3>
              <p class="desc">The coffee you want, when you want it</p>
            </div>
            <div class="row">
              <div class="col-lg-6 col-12">
                <div class="card-contain">
                  <div class="image">
                    <img
                      src="@/assets/images/Link → h2-custom-icon-6.png.png"
                      alt=""
                    />
                  </div>
                  <div
                    class="d-flex align-items-start justify-content-center flex-column"
                  >
                    <h5 class="mb-0">quality</h5>
                    <span class=""
                      >Lorem Ipsum is simply dummy text of the printing and
                      typesetting industry.</span
                    >
                  </div>
                </div>
              </div>
              <div class="col-lg-6 col-12">
                <div class="card-contain">
                  <div class="image">
                    <img
                      src="@/assets/images/Link → h2-custom-icon-8.png.png"
                      alt=""
                    />
                  </div>
                  <div
                    class="d-flex align-items-start justify-content-center flex-column"
                  >
                    <h5 class="mb-0">Easy</h5>
                    <span class=""
                      >Lorem Ipsum is simply dummy text of the printing and
                      typesetting industry.</span
                    >
                  </div>
                </div>
              </div>
              <div class="col-lg-6 col-12">
                <div class="card-contain">
                  <div class="image">
                    <img
                      src="@/assets/images/Link → h2-custom-icon-7.png.png"
                      alt=""
                    />
                  </div>
                  <div
                    class="d-flex align-items-start justify-content-center flex-column"
                  >
                    <h5 class="mb-0">taste</h5>
                    <span class=""
                      >Lorem Ipsum is simply dummy text of the printing and
                      typesetting industry.</span
                    >
                  </div>
                </div>
              </div>
              <div class="col-lg-6 col-12">
                <div class="card-contain">
                  <div class="image">
                    <img
                      src="@/assets/images/Link → h2-custom-icon-5.png.png"
                      alt=""
                    />
                  </div>
                  <div
                    class="d-flex align-items-start justify-content-center flex-column"
                  >
                    <h5 class="mb-0">quick</h5>
                    <span class=""
                      >Lorem Ipsum is simply dummy text of the printing and
                      typesetting industry.</span
                    >
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss"
scoped>
.titles {
  width: 100%;

  display: flex;
  justify-content: center;
  align-items: start;
  flex-direction: column;
}
.title-welcome {
  color: #3b2f2f;
  font-size: 2rem;
  font-weight: 700;
}
.desc {
  color: #3b2f2f;
  font-size: 1.7rem;
  font-weight: 400;
}
.card-contain {
  display: flex;
  align-items: center;
  justify-content: start;
  gap: 1rem;
  padding: 1rem 0;
}
.image {
  background-color: #6f4336;
  border-radius: 50px;
  padding: 1rem;
}
h5 {
  color: #004876;
  font-weight: 700;
}
</style>