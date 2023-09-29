<template>
  <div>
    <div class="first-row">
      <div class="container">
        <div class="logos">
          <img
            src="../assets/images/Cyberpunk_2077_logo 1.svg"
            alt="main logo"
            class="mainLogo"
          />
          <img src="../assets/images/SDPR.svg" alt="SDPR" class="SDPR" />
        </div>
        <div class="text">
          <span>Лицензия</span>
          <span>Политика конфиденциальности</span>
        </div>
      </div>
    </div>
    <div class="second-row">
      <span>CD PROJEKT®, Cyberpunk®, Cyberpunk 2077®</span>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.first-row {
  background-color: #fff;
  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 13px 0;
    .logos,
    .text {
      display: flex;
      gap: 32px;
      cursor: pointer;
    }
    .text {
      font-family: Roboto;
      font-size: 18px;
      font-style: normal;
      font-weight: 400;
      line-height: normal;
    }
  }
}
.second-row {
  background-color: #000;
  color: #fff;
  text-align: center;
  font-family: Roboto;
  font-size: 12px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
  padding: 13px 0;
}
@media (max-width: 860px) {
  .first-row {
    flex-direction: column;
    .container {
      padding: 0;
      display: flex;
      flex-direction: column;
    }
    .logos {
      flex-direction: column;
      padding: 40px 15px 25px 15px;
      .mainLogo {
        width: 200px;
        height: 50px;
      }
      .CDPR {
        width: 116.25px;
        height: 50px;
      }
    }
    .text {
      width: 100%;
      background-color: #e6e6e6;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 25px 15px;
    }
  }
}
</style>
