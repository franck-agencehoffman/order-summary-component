<template>
  <div class="card">
    <img class="card-img" src="@/assets/card-img.svg" alt="Card Image">
    <div class="card-content">
      <h3 class="card-title">Order Summary</h3>

      <p class="card-text">You can now listen to millions of songs, audiobooks, and podcasts on any device anywhere you like!</p>

      <div class="card-subscription">
        <img src="@/assets/icon-music.svg" alt="Subscription Icon" class="subscription-icon">
        <div class="subscription-infos">
          <p class="subscription-name"><strong>Annual Plan</strong></p>
          <p class="subscription-price">$59.99/year</p>
        </div>
        <a href="#" class="subscription-edit">Change</a>
      </div>

      <button type="button" class="card-proceed-btn">Proceed to Payment</button>

      <a href="#" class="card-cancel-btn">Cancel Order</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "Card"
}
</script>

<style lang="scss" scoped>
  .card {
    position: relative;
    overflow: hidden;
    z-index: 1;
    width: 100%;
    max-width: 450px;
    border-radius: 20px;
    background: #ffffff;
    box-shadow: 0 40px 40px -20px rgba(13, 48, 189, 0.151826);

    @media (max-width: 375px) {
      margin: 20px;
    }

    .card-img {
      display: block;
      width: 100%;
    }

    .card-content {
      padding: 45px 48px 48px;

      @media (max-width: 375px) {
        padding: 32px 24px;
      }
    }

    .card-title {
      margin-bottom: 17px;
      font-family: 'Red Hat Display';
      font-style: normal;
      font-weight: 900;
      font-size: 28px;
      line-height: 37px;
      text-align: center;
      color: #1f2e55;

      @media (max-width: 375px) {
        margin-bottom: 16px;
        font-size: 22px;
        line-height: 29px;
      }
    }

    .card-text {
      margin-bottom: 20px;
      font-family: 'Red Hat Display';
      font-style: normal;
      font-weight: 500;
      font-size: 16px;
      line-height: 26px;
      text-align: center;
      color: #717fa6;

      @media (max-width: 375px) {
        margin-bottom: 24px;
        font-size: 15px;
        line-height: 25px;
      }
    }

    .card-subscription {
      display: flex;
      align-items: center;
      width: 100%;
      margin-bottom: 32px;
      padding: 25px 24px;
      border-radius: 11px;
      background: #f7f9ff;

      @media (max-width: 375px) {
        margin-bottom: 24px;
        padding: 17px 16px 16px;
      }

      .subscription-icon {
        width: 48px;
        height: 48px;
      }

      .subscription-infos {
        flex: 1;
        padding-left: 20px;
        text-align: left;
      }

      .subscription-name {
        margin-bottom: 6px;
        font-family: 'Red Hat Display';
        font-style: normal;
        font-weight: 900;
        font-size: 16px;
        line-height: 21px;
        color: #1f2e55;

        @media (max-width: 375px) {
          margin-bottom: 3px;
          font-size: 14px;
          line-height: 19px;
        }
      }

      .subscription-price {
        font-family: 'Red Hat Display';
        font-style: normal;
        font-weight: 500;
        font-size: 16px;
        line-height: 21px;
        color: #717fa6;

        @media (max-width: 375px) {
          font-size: 14px;
          line-height: 19px;
        }
      }

      .subscription-edit {
        font-family: 'Red Hat Display';
        font-style: normal;
        font-weight: bold;
        font-size: 14px;
        line-height: 19px;
        text-decoration-line: underline;
        color: #382ae1;

        @media (max-width: 375px) {
          font-size: 13px;
          line-height: 17px;
        }
      }
    }

    .card-proceed-btn {
      width: 100%;
      margin-bottom: 32px;
      padding: 15px;
      font-family: 'Red Hat Display';
      font-style: normal;
      font-weight: 900;
      font-size: 15px;
      line-height: 20px;
      color: #FFFFFF;
      border-radius: 11px;
      background: #382ae1;
      box-shadow: 0 20px 20px rgba(56, 42, 225, 0.190291);

      @media (max-width: 375px) {
        margin-bottom: 24px;
        font-size: 15px;
        line-height: 20px;
      }
    }

    .card-cancel-btn {
      font-family: 'Red Hat Display';
      font-style: normal;
      font-weight: 900;
      font-size: 15px;
      line-height: 20px;
      text-align: center;
      text-decoration-line: none;
      color: #717fa6;

      @media (max-width: 375px) {
        font-size: 15px;
        line-height: 20px;
      }
    }
  }
</style>
