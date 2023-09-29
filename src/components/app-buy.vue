<template>
  <div class="content">
    <div class="leftCol">
      <img src="../assets/images/disk.jpg" alt="disks" />
    </div>
    <div class="rightCol">
      <h2 class="title">Купить игру Cyberpunk 2077</h2>
      <div class="title-list">В комплект входит:</div>
      <div class="list">
        <div class="item">
          <img src="../assets/images/disk-icon.svg" alt="icon" />
          <div class="text">Футляр с игровыми дисками</div>
        </div>
        <div class="item">
          <img src="../assets/images/text.svg" alt="icon" />
          <div class="text">
            Футляр с кодом для загрузки игры и дисками (pc)
          </div>
        </div>
        <div class="item">
          <img src="../assets/images/collections.svg" alt="icon" />
          <div class="text">Справочник с информацией об игровом мире</div>
        </div>
      </div>
      <div class="title-list">Выберите платформу:</div>
      <div class="list-logos">
        <img src="../assets/images/pc.svg" alt="icon" />
        <img src="../assets/images/xbox.svg" alt="icon" />
        <img src="../assets/images/stadioa.svg" alt="icon" />
        <img src="../assets/images/ps4.svg" alt="icon" />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.content {
  display: flex;
  gap: 32px;
  background-color: #000;
  .leftCol {
    overflow: hidden;
    img {
      height: 100%;
      // max-width: 100%;
    }
  }
  .rightCol {
    margin-top: 70px;
    min-width: 692px;
    .title {
      max-width: 624px;
      color: #fff;
      font-family: Archangelsk;
      font-size: 62px;
      font-style: normal;
      font-weight: 400;
      line-height: normal;
      margin: 0;
    }
    .title-list {
      color: #52bedc;
      font-family: Roboto;
      font-size: 24px;
      font-style: normal;
      font-weight: 700;
      line-height: normal;
      margin: 25px 0;
    }
    .list {
      display: flex;
      flex-direction: column;
      gap: 15px;
      margin-bottom: 70px;
      .item {
        display: flex;
        gap: 10px;
        align-items: center;
        .text {
          color: #fff;
          font-family: Roboto;
          font-size: 18px;
          font-style: normal;
          font-weight: 400;
          line-height: normal;
        }
      }
    }
    .list-logos {
      display: grid;
      grid-template-columns: 58px 178px;
      grid-template-rows: 1fr 1fr;
      grid-row-gap: 50px;
      grid-column-gap: 80px;
    }
  }
  @media (max-width: 860px) {
    flex-direction: column;
    .leftCol img {
      object-fit: cover;

      max-height: 300px;
      width: 100%;
    }
    .rightCol {
      margin-top: 0;
      padding: 70px 15px;
      min-width: unset;
    }
  }
  @media (max-width: 370px) {
   .rightCol .list-logos{
      grid-column-gap: 40px;
    }
  }
}
</style>
