<script>
  let showSocialMedia = false;
  import ActionButton from "./ActionButton.svelte";
  let toggleSocialMedia = () => {
    showSocialMedia = !showSocialMedia;
    console.log(showSocialMedia);
  };
</script>

<style>
  .Card__Info__Contact {
    position: relative;
    width: 100%;
    height: 64px;
    display: flex;
    padding-top: 9px;
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
    font-weight: 700;
    font-size: 12px;
    line-height: 16px;
    letter-spacing: 0.064em;
    width: 120px;
    position: absolute;
    top: 6px;
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

  .Card__Info__Contact__Action {
    position: relative;
    width: 90px;
    height: 64px;
    padding-top: 7px;
    padding-left: 26px;
  }

  .Card__Info__Contact_SocialMedia {
    position: absolute;
    background-color: #48556a;
    /* background-color: red; */
    /* opacity: 0.3; */
    width: 100%;
    height: 65px;
    top: 0;
    left: 0;
    border-radius: 0 0 10px 10px;
    display: flex;
    padding-top: 6px;
  }

  .Card__Info__Contact_SocialMedia_Links {
    width: 237px;
    display: flex;
    position: relative;
  }
  .Card__Info__Contact_SocialMedia_Links p {
    display: inline;
    margin-top: 17px;
    margin-left: 32px;
    /* SHARE */

    /* position: absolute;
width: 63px;
height: 17px;
left: 0px;
top: 0px; */

    font-family: Manrope;
    font-style: normal;
    font-weight: normal;
    font-size: 13px;
    line-height: 18px;
    letter-spacing: 0.394em;

    color: #9eafc2;
  }
  .Card__Info__Contact_SocialMedia_Links ul {
    display: flex;
    padding: 0px;
    padding-left: 17px;
    height: 20px;
  }
  .Card__Info__Contact_SocialMedia_Links ul li {
    list-style: none;
    margin: 0;
    margin-right: 16px;
    padding: auto auto;
    height: 100%;
  }

  .Card__Info__Contact_SocialMedia_Links ul li img {
    align-self: center;
  }

  .Card__Info__Contact_SocialMedia_Action {
    position: relative;
    width: 90px;
    height: 48px;
    padding-top: 10px;
    padding-left: 40px;
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

    .Card__Info__Contact_SocialMedia {
      width: 248px;
      height: 49px;
      border-radius: 10px;
      top: -76px;
      left: 265px;
    }

    .Card__Info__Contact_SocialMedia::after{
      position:absolute;
      top:45px;
      left:115px;
      content: '';
      width: 18px;
      height: 18px;
      background-color: #48556a;
      transform: rotate(45deg);
    }

    .Card__Info__Contact_SocialMedia_Links p {
      margin-top: 13px;
      margin-left: 37px;
    }

    .Card__Info__Contact_SocialMedia_Links ul {
      margin-top: 12px;
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
    <ActionButton actionHandler={toggleSocialMedia} />
  </div>
  {#if showSocialMedia === true}
    <div class="Card__Info__Contact_SocialMedia">
      <div class="Card__Info__Contact_SocialMedia_Links">
        <p>SHARE</p>
        <ul>
          <li><img src="./images/icon-facebook.svg" alt="facebook icon" /></li>
          <li>
            <img
              style="padding-top:2px"
              src="./images/icon-twitter.svg"
              alt="twitter icon" />
          </li>
          <li>
            <img src="./images/icon-pinterest.svg" alt="pinterest icon" />
          </li>
        </ul>
      </div>
      <div class="Card__Info__Contact_SocialMedia_Action">
        <ActionButton actionHandler={toggleSocialMedia} />
      </div>
    </div>
  {/if}
</div>
