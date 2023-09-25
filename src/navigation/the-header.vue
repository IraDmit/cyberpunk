<template>
  <header >
    <div class="header-wrp container">
      <div class="logo">
        <img
          src="../assets/images/Cyberpunk_2077_logo 1.svg"
          alt="../assets/images/Cyberpunk_2077_logo 1.svg"
        />
      </div>
      <ul class="header-logos">
        <li class="messenger">
          <img
            src="../assets/images/youtube.svg"
            alt="../assets/images/youtube.svg"
          />
        </li>
        <li class="messenger">
          <img src="../assets/images/vk.svg" alt="../assets/images/vk.svg" />
        </li>
        <li class="messenger">
          <img
            src="../assets/images/facebook.svg"
            alt="../assets/images/facebook.svg"
          />
        </li>
        <li class="messenger">
          <img
            src="../assets/images/twitter.svg"
            alt="../assets/images/twitter.svg"
          />
        </li>
        <li class="messenger">
          <img
            src="../assets/images/twitch.svg"
            alt="../assets/images/twitch.svg"
          />
        </li>
        <li class="messenger">
          <img
            src="../assets/images/instagram.svg"
            alt="../assets/images/instagram.svg"
          />
        </li>
      </ul>
    </div>
  </header>
</template>

<style lang="scss" scoped>
header {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 1;
  width: 100%; 
  .header-wrp {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .header-logos {
    display: flex;
    gap: 40px;
    margin-left: auto;
  }
}
</style>
