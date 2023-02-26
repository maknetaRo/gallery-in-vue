<script setup></script>

<template>
  <header class="header">
    <h2 class="main-title">galleria.</h2>
    <button class="btn">Start Slideshow</button>
  </header>
</template>
<style scoped>
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 40px;
  border-bottom: 1px solid #e5e5e5;
}
.main-title {
  display: inline-flex;
  height: 32px;
  width: 100%;
}
.btn {
  display: inline-flex;
  flex-wrap: nowrap;
  white-space: nowrap;
  justify-content: flex-end;
  background: transparent;
  border: none;
  outline-color: #7d7d7d;

  font-weight: 700;
  text-transform: uppercase;
  color: #7d7d7d;
  letter-spacing: 2px;
  max-width: 130px;
  width: 100%;
  font-size: 12px;
  line-height: 15px;
}

@media (max-width: 500px) {
  .header {
    padding: 24px;
  }
  .btn {
    font-size: 9px;
    line-height: 11px;
  }
}
</style>
