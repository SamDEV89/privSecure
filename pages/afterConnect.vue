<template>
  <main id="buy">
    <section class="mission">
      <div class="container mx-auto md:my-32 my-10">
        <h2 class="text-gradient-2 md:text-4xl text-xl mb-6">Get in Early</h2>
        <p class="md:max-w-md">
          Join the Privesecure presale right away! Purchasing your first $PRSC
          tokens is now simpler than ever thanks to our step-by-step
          instructions. Simply click the connect wallet button when you are
          ready to go.
        </p>
        <div class="flex wallet-container">
           <!-- <EthModal/>
            <CardModal/>
            <UsdtModal/> -->
            <BnbModal />
          
        </div>

        <div class="mt-5">
          <p>
            1 USDT = <br />
            USDT RAISED : $1,145,382.95 OF $2,000,000
          </p>
        </div>
        <div class="progress mt-10">
          <div class="progress-done"></div>
        </div>
      </div>
    </section>

    <section>
      <div class="container mx-auto">
        <div class="flex flex-col items-center">
          <h2 class="text-gradient mb-10 text-3xl">Step 1</h2>
          <p class="md:max-w-md text-center">
            To obtain your $PRSC tokens, you will need to establish a digital
            wallet. Although we suggest using Metamask as your wallet, if you
            already have another wallet, you may be able to utilise wallet
            connect
          </p>
        </div>
        <br />
        <br />
        <div class="flex flex-col items-center">
          <h2 class="text-gradient mb-10 text-3xl">Step 2</h2>
          <p class="md:max-w-md text-center">
            After completing this, it's time to purchase BNB. On exchanges like
            Binance, this is achievable. Once you've made the purchase, send the
            BNB to your wallet.
          </p>
        </div>
        <br />
        <br />
        <div class="flex flex-col items-center">
          <h2 class="text-gradient mb-10 text-3xl">Step 3</h2>
          <p class="md:max-w-md text-center">
            A pop-up will show once you click Connect Wallet. You will be sent
            to a new page after selecting your chosen wallet. Once you are
            there, click the "Buy With BNB" button to bring up another pop-up.
            The transaction will be completed after you click purchase.
          </p>
        </div>
        <br />
        <br />
        <div class="flex flex-col items-center">
          <h2 class="text-gradient mb-10 text-3xl">Step 4</h2>
          <p class="md:max-w-md text-center">
            After the presale is over, you may access your PRSC tokens through
            the primary website (privesecure.io). Your tokens will appear in
            your wallet once the presale has ended.
          </p>
        </div>
        <!-- <div class="step-container mt-10 md:mb-10 mb-5">
          <div class="step-box">
            <img
              src="../assets/img/card.svg"
              alt="triangle alert"
              class="mb-8"
            />
          <h2 class="mx-auto text-gradient mb-5 text-2xl center">
            Buy with Card
          </h2>
            <p>This option enables you to acquire ETH, which will be 
              sent to your wallet through our partner, Transak. You 
              will then be able to buy $PRSC using this ETH. To begin, 
              click "Buy ETH With Card" and follow the on-screen instructions. 
              We propose acquiring at least $15 worth of
              ETH to satisfy the purchase minimum.</p>
          </div>
          
          <div class=" step-box">
            <img
              src="../assets/img/usdt.svg"
              alt="triangle alert"
              class="mb-8"
            />
            <h2 class="mx-auto text-gradient mb-5 text-2xl center">
            Buy PRSC with ETH
          </h2>
            <p>Once you have enough ETH in your wallet (please 
              choose option 1 to buy ETH first if you don't have ETH 
              or USDT), you can trade your ETH for PRSC. Enter the 
              minimum amount of PRSC you want to buy, and then 
              click "Convert ETH." Your wallet provider will ask you to 
              confirm the transaction and will also show you how 
              much gas costs.
            </p>
          </div>
          <div class="step-box">
            <img
              src="../assets/img/eth.svg"
              alt="triangle alert"
              class="mb-8"
            />

            <h2 class="mx-auto text-gradient mb-5 text-2xl center">
            Buy with Card
          </h2>
            <p>This option enables you to acquire ETH, which will be 
              sent to your wallet through our partner, Transak. You 
              will then be able to buy $PRSC using this ETH. To begin, 
              click "Buy ETH With Card" and follow the on-screen instructions. 
              We propose acquiring at least $15 worth of
              ETH to satisfy the purchase minimum.</p>
          </div>
          </div>-->
      </div>
    </section>
  </main>
</template>
<script>
import EnterPresale from "../components/EnterPresale.vue";
import EthModal from "../components/modal/EthModal.vue";
import UsdtModal from "../components/modal/UsdtModal.vue";
import CardModal from "../components/modal/CardModal.vue";
import BnbModal from "../components/modal/BnbModal.vue";


export default {
  components: { EnterPresale, EthModal, UsdtModal, CardModal, BnbModal },
  head() {
    return {
      title: "How to buy | PriveSecure",
    };
  },
};
</script>

<style scoped>
.mission .container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
}

.content-block .container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  place-items: top center;
  grid-gap: 2rem;
}
.wallet-container {
  gap: 2rem;
  margin-top: 2rem;
}
.content-block:last-child .text-container {
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
}

.block-1 {
  background-image: url("../assets/img/blur-left.png");
  background-position: left center;
  background-repeat: no-repeat;
}
.block-2 {
  background: url("../assets/img/blur-right.png");
  background-position: right center;
  background-repeat: no-repeat;
}

.content-block ul {
  margin-left: 0;
  padding-left: 1rem;
  margin-top: 2rem;
}

.content-block li {
  line-height: 1.6;
  margin-bottom: 1.2rem;
}

.progress {
  width: 400px;
  background: #4b4a51;
  height: 53px;
}
.progress-done {
  width: 70%;
  height: 100%;
  background: linear-gradient(146.87deg, #5f36ff 3.58%, #08ff42 88.73%);
  box-shadow: inset 0px 5px 10px #08ff42;
  border-radius: 8px;
}
.step-container {
  display: grid;
  grid-template-columns: repeat(3, minmax(5rem, 1fr));
  grid-gap: 2rem;
}
.step-box {
  background: #1e1c25;
  padding: 3rem 2rem;
  min-height: 400px;
  border-radius: 0.8rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  position: relative;
}
.step-box::before {
  content: "";
  position: absolute;
  padding: 2px;
  border-radius: inherit;
  z-index: -1;
  top: -1px;
  bottom: -1px;
  right: -1px;
  left: -1px;
  background: linear-gradient(146.87deg, #5f36ff 3.58%, #08ff42 88.73%);
}
.block-flex {
  max-width: 1000px;
  margin: 0 auto;
  padding: 0rem 3rem;
}
@media (max-width: 992px) {
  .step-container {
    grid-template-columns: 1fr 1fr;
  }
  /* .content-block{
    display: flex;
    flex-direction: column;
  } */
}

@media (max-width: 768px) {
  .container .step-container {
    grid-template-columns: auto;
  }
  .step-container {
    grid-template-columns: 1fr;
  }
  .block-flex {
    display: flex;
    flex-direction: column-reverse;
    align-items: center;
    justify-content: center;
    padding: 0rem 2rem;
  }
  .reverse {
    flex-direction: column !important;
  }
  .block-1,
  .block-2 {
    background: none;
  }

  .block-2 .img-container {
    order: 1;
  }
  .block-2 .text-container {
    order: 2;
  }

  .content-block ul {
    padding-left: 1.5rem;
  }

  .content-block h2 {
    line-height: 1.5;
  }
  .wallet-container {
    flex-direction: column;
  }
}

@media (max-width: 450px) {
  .progress {
    width: 300px;
  }
}
</style>
