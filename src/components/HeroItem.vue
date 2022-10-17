
<template>
  <div class="item">
      
    <div class="details">
      <div class="container">
        <i>
          <slot name="icon"></slot>
        </i>
        <h3>
          <slot name="heading"></slot>
        </h3>
      </div>
      <slot class="paragraph"></slot>
    </div>
  </div>
</template>

<style scoped>

.item {
  margin: 2rem auto;
  display: flex;
  flex-direction: row;
  background-color: gray;
  min-width: 83vw;
  min-height: 75vh;
}

.details {
  flex: 1;
  margin-left: 0;
  margin-top: 70vh; 
  place-content: left;
}

.container {
  display: flex;
  flex-direction: row;
  place-items: left center;
  place-content: left center;
}

i {
  display: flex;
  place-items: center;
  place-content: left center;
  margin-left: -1rem;
  width: 32px; 
  height: 32px;

  color: var(--color-text);
}

h3 {
  font-size: 1.2rem;
  font-weight: 500;
  margin-bottom: 0.4rem;
  color: var(--color-heading);
}

@media (min-width: 1024px) {
  .item {
    margin-top: 1rem;
    padding: 0.4rem 0 1rem calc(var(--section-gap) / 2);
    min-width: 18%;
    min-height: 82vh;
    border-right: 1px solid var(--color-border);
  }

  .item:hover {
    width: 28%;
  }

  i {
    top: calc(50% - 25px);
    left: -26px;
    position: absolute;
    /* border: 1px solid var(--color-border); */
    border-radius: 8px;
    width: 50px;
    height: 50px;
  }


  /* .item:before {
    content: ' ';
    border-left: 1px solid var(--color-border);
    position: absolute;
    left: 0;
    bottom: calc;
    height: calc(50% - 25px);
  }

  .item:after {
    content: ' ';
    border-left: 1px solid var(--color-border);
    position: absolute;
    left: 0;
    top: calc(50% + 25px);
    height: calc(50% - 25px);
  }

  .item:first-of-type:before {
    display: none;
  }

  .item:last-of-type:after {
    display: none;
  } */
}
</style>
