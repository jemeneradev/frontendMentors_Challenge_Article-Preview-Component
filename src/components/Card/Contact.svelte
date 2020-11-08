<style>
  .Card__Info__Contact {
    position: relative;
    width: 100%;
    height: 64px;
    display: flex;
  }

  .Card__Info__Contact .Card__Info__Contact__User {
    position: relative;
    width: 237px;
    margin: 0;
    padding: 0;
  }

  .Card__Info .Card__Info__Contact__User .Card__Info__Contact__User__Avatar {
    position: relative;
    width: 120px;
    height: 64px;
  }

  .Card__Info
    .Card__Info__Contact__User
    .Card__Info__Contact__User__Avatar
    img {
    width: 40px;
    border-radius: 50%;
    position: absolute;
    top: 3px;
    left: 32px;
  }

  .Card__Info__Contact__User .Card__Info__Contact__User__Details {
    position: relative;
  }
  .Card__Info__Contact__User .Card__Info__Contact__User__Details h1 {
    font-family: Manrope;
    font-style: normal;
    font-weight: 600;
    font-size: 12px;
    line-height: 16px;
    letter-spacing: 0.064em;
    width: 120px;
    position: absolute;
    top: 5px;
    left: 8px;
    margin: 0;
    color: #48556a;
  }
  .Card__Info__Contact__User .Card__Info__Contact__User__Details h2 {
    font-family: Manrope;
    font-style: normal;
    font-weight: normal;
    font-size: 12px;
    line-height: 16px;
    letter-spacing: 0.064em;
    width: 120px;
    position: absolute;
    top: 26px;
    left: 8px;
    margin: 0;
    color: #9eafc2;
  }

  /* 28 Jun 2020 */

  .Card__Info__Contact .Card__Info__Contact__Action {
    position: relative;
    width: 90px;
    height: 64px;
  }

  .Card__Info .Card__Info__Contact__Action .Card__Info__Contact__Action__Share {
    width: 32px;
    height: 32px;
    background-color: blue;
    border-radius: 50%;
    margin: 0;
    top: 8px;
    left: 26px;
  }
  .Card__Info
    .Card__Info__Contact__Action
    .Card__Info__Contact__Action__Share
    img {
    margin: 0;
    margin-left: 9px;
    margin-top: 9px;
  }

  @media screen and (min-width: 1440px) {
    .Card__Info__Contact {
      height: 70px;
    }
    .Card__Info__Contact .Card__Info__Contact__User {
      width: 347px;
    }
    .Card__Info
      .Card__Info__Contact__User
      .Card__Info__Contact__User__Avatar
      img {
      left: 40px;
    }
  }
</style>

<div class="Card__Info Card__Info__Contact">
  <div class="Card__Info__Contact Card__Info__Contact__User">
    <figure class="Card__Info__Contact__User Card__Info__Contact__User__Avatar">
      <img src="./images/avatar-michelle.jpg" alt="avatar: michelle" />
      <!--  <figcaption>Fig.1 - Trulli, Puglia, Italy.</figcaption> -->
    </figure>
    <div class="Card__Info__Contact__User Card__Info__Contact__User__Details">
      <h1>Michelle Appleton</h1>
      <h2>28 Jun 2020</h2>
    </div>
  </div>
  <div class="Card__Info__Contact Card__Info__Contact__Action">
    <div class="Card__Info__Contact__Action Card__Info__Contact__Action__Share">
      <img src="./images/icon-share.svg" alt="share arrow" />
    </div>
  </div>
</div>
