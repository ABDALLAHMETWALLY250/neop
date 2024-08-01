<template>
  <div class="ourProducts">
    <div class="titles">
      <span class="first_title">Our Products</span>
      <h4 class="second_title">Special to Try</h4>
    </div>
    <nav>
      <div class="nav nav-tabs my-4" id="nav-tab" role="tablist">
        <button
          class="nav-link active"
          id="nav-home-tab"
          data-bs-toggle="tab"
          data-bs-target="#nav-home"
          type="button"
          role="tab"
          aria-controls="nav-home"
          aria-selected="true"
        >
          All categories
        </button>
        <button
          class="nav-link"
          id="nav-special-offers-tab"
          data-bs-toggle="tab"
          data-bs-target="#nav-special-offers"
          type="button"
          role="tab"
          aria-controls="nav-special-offers"
          aria-selected="false"
        >
          Special offers
        </button>
        <button
          class="nav-link"
          id="nav-best-seller-tab"
          data-bs-toggle="tab"
          data-bs-target="#nav-best-seller"
          type="button"
          role="tab"
          aria-controls="nav-best-seller"
          aria-selected="false"
        >
          Best seller
        </button>
        <button
          class="nav-link"
          id="nav-roasting-tab"
          data-bs-toggle="tab"
          data-bs-target="#nav-roasting"
          type="button"
          role="tab"
          aria-controls="nav-roasting"
          aria-selected="false"
        >
          Roasting
        </button>
        <button
          class="nav-link"
          id="nav-coffee-tab"
          data-bs-toggle="tab"
          data-bs-target="#nav-coffee"
          type="button"
          role="tab"
          aria-controls="nav-coffee"
          aria-selected="false"
        >
          Coffee
        </button>
        <button
          class="nav-link"
          id="nav-coffee-equipment-tab"
          data-bs-toggle="tab"
          data-bs-target="#nav-coffee-equipment"
          type="button"
          role="tab"
          aria-controls="nav-coffee-equipment"
          aria-selected="false"
        >
          Coffee equipment
        </button>
      </div>
    </nav>
    <div class="tab-content container" id="nav-tabContent">
      <div
        class="tab-pane fade show active d-flex justify-content-center gap-5 flex-wrap align-items-center"
        id="nav-home"
        role="tabpanel"
        aria-labelledby="nav-home-tab"
        tabindex="0"
      >
        <div class="cards">
          <div class="out_card">
            <div class="card">
              <img
                src="@/assets/images/image 11.png"
                alt="Brazilian Roasted Coffee"
                class="product-image"
              />
            </div>
          </div>
          <div class="product-details">
            <h2 class="text-center">Brazilian Roasted Coffee</h2>
            <p class="author text-center">Amir Samantha</p>
            <div class="rating text-center">
              <span>&#9733;</span>
              <span>&#9733;</span>
              <span>&#9733;</span>
              <span>&#9733;</span>
              <span>&#9733;</span>
            </div>
          </div>
        </div>

        <div class="cards">
          <div class="out_card">
            <div class="card">
              <img
                src="@/assets/images/image 5.png"
                alt="Brazilian Roasted Coffee"
                class="product-image"
              />
            </div>
          </div>
          <div class="product-details">
            <h2 class="text-center">Brazilian Roasted Coffee</h2>
            <p class="author text-center">Amir Samantha</p>
            <div class="rating text-center">
              <span>&#9733;</span>
              <span>&#9733;</span>
              <span>&#9733;</span>
              <span>&#9733;</span>
              <span>&#9733;</span>
            </div>
          </div>
        </div>

        <div class="cards">
          <div class="out_card">
            <div class="card">
              <img
                src="@/assets/images/image 6.png"
                alt="Brazilian Roasted Coffee"
                class="product-image"
              />
            </div>
          </div>
          <div class="product-details">
            <h2 class="text-center">Brazilian Roasted Coffee</h2>
            <p class="author text-center">Amir Samantha</p>
            <div class="rating text-center">
              <span>&#9733;</span>
              <span>&#9733;</span>
              <span>&#9733;</span>
              <span>&#9733;</span>
              <span>&#9733;</span>
            </div>
          </div>
        </div>

        <div class="cards">
          <div class="out_card">
            <div class="card">
              <img
                src="@/assets/images/cofe.png"
                alt="Brazilian Roasted Coffee"
                class="product-image"
              />
            </div>
          </div>
          <div class="product-details">
            <h2 class="text-center">Brazilian Roasted Coffee</h2>
            <p class="author text-center">Amir Samantha</p>
            <div class="rating text-center">
              <span>&#9733;</span>
              <span>&#9733;</span>
              <span>&#9733;</span>
              <span>&#9733;</span>
              <span>&#9733;</span>
            </div>
          </div>
        </div>
      </div>
      <div
        class="tab-pane fade"
        id="nav-special-offers"
        role="tabpanel"
        aria-labelledby="nav-special-offers-tab"
        tabindex="0"
      >
        <h4>Coming Soon</h4>
      </div>
      <div
        class="tab-pane fade"
        id="nav-best-seller"
        role="tabpanel"
        aria-labelledby="nav-best-seller-tab"
        tabindex="0"
      >
        <h4>Coming Soon</h4>
      </div>
      <div
        class="tab-pane fade"
        id="nav-roasting"
        role="tabpanel"
        aria-labelledby="nav-roasting-tab"
        tabindex="0"
      >
        <h4>Coming Soon</h4>
      </div>
      <div
        class="tab-pane fade"
        id="nav-coffee"
        role="tabpanel"
        aria-labelledby="nav-coffee-tab"
        tabindex="0"
      >
        <h4>Coming Soon</h4>
      </div>
      <div
        class="tab-pane fade"
        id="nav-coffee-equipment"
        role="tabpanel"
        aria-labelledby="nav-coffee-equipment-tab"
        tabindex="0"
      >
        <h4>Coming Soon</h4>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.titles {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  gap: 2.5rem;
}
.first_title {
  color: #3b2f2f;
  font-weight: 400;
  font-size: 1.2rem;
}
.second_title {
  color: #3b2f2f;
  font-size: 2rem;
  font-weight: 700;
}
</style>
