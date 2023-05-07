<template>
  <div class="container">
    <img src="../../assets/map.png" alt="">
    <div class="box">
      <div>
        <h2>1M+</h2>
        <p>People have joined our space</p>
      </div>
      <div>
        <h2>10k+</h2>
        <p>Tasks available</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  position: relative;
  display: flex;
  width: 100%;
}

img {
  width: 100%;
}

.box {
  position: absolute;
  width: 100%;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  display: flex;
  gap: 25px;
  justify-content: center;
  /* margin-left: 40px; */
}



h2 {
  text-align: center;
  color: rgba(255, 255, 255, 0.471);
}

p {
  white-space: nowrap;
  color: rgba(197, 197, 197, 0.623);
}

.box:hover h2 {
  color: rgba(255, 255, 255, 0.896);
}

.box:hover p {
  color: var(--color-text);
}
</style>