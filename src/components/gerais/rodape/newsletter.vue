<template lang="html">
  <section id="containerNewsletter" >
    <div class="row">
      <div class="small-12 columns">
        <div class="newsletter-container">
          <div class="newsletter-container-icon">
            <img :src="require('@/assets/img/geral/news.png')" alt="">
          </div>
          <p class="newsletter-container-t1">
            Nós enviamos e-mails incríveis
          </p>
          <p class="newsletter-container-t2">
            Saiba primeiro dos nossos lançamentos, <br class="mob"/> dicas e promoções exclusivas
          </p>
          <form id="newsletter" class="newsletter-container-form" action="index.html" method="post" @submit.prevent="submitNews()">

            <input type="email" name="" value="" placeholder="Digite seu melhor e-mail" 
            v-model="email"
            :class="{error: emailError}"
            @keyup="emailError = false"
            >

            <div class="newsletter-boxButton">
              <button type="submit" name="button">
                <transition name="fadeCheck">
                  <span class="material-icons" v-if="check">check</span>
                </transition>
                {{ textBt }}
              </button>
              <preloader v-if="newsShowLoader" class="preloaderNews"/>
            </div>
          </form>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  components: {
    preloader: () => import("@/components/gerais/preloader.vue"),
  },
  data() {
    return {
      email: "",
      textBt: "Participar",
      check: false,
      emailError: false,
      newsShowLoader: false,
    };
  },
  methods: {
    submitNews() {
      if (this.email != "") {
        this.newsShowLoader = true;

        this.$requestSend(
          "post",
          "/v2/front/newsletter",
          { email: this.email },
          (success, response) => {
            if (success && response.data.sucesso) {
              this.check = true;
              this.textBt = "Cadastrado!";

              this.email = "";
              this.newsShowLoader = false;

              setTimeout(() => {
                this.check = false;
              }, 1000);

              setTimeout(() => {
                this.textBt = "Participar";
              }, 5000);
            } else {
              this.textBt = "Erro ao cadastrar";
              this.newsShowLoader = false;
              setTimeout(() => {
                this.textBt = "Participar";
              }, 5000);
            }
          }
        );
        return;
      }
      this.emailError = this.email == "";
    },
  },
};
</script>

<style lang="css" scoped>
#containerNewsletter {
  background-image: url("../../../assets/newwhite/bgnews.jpg");
  background-position: center top;
  background-repeat: no-repeat;
  background-size: 1920px;
  height: 300px;
  display: flex;
  justify-content: center;
  align-items: center;
  color: #fff;
  overflow: hidden;
}
.newsletter-container {
  padding: 0 45px;
  display: block;
  text-align: center;
}
.newsletter-container-icon {
  margin-bottom: 5px;
}
.newsletter-container-t1 {
  margin-right: 30px;
  line-height: 1.125;
  margin-bottom: 3px;
  font-weight: 700;
  font-size: 18px;
}
.newsletter-container-t2 {
  margin-top: 0;
  line-height: 20px;
  font-size: 13px;
  margin-bottom: 1rem;
}
.newsletter-container-form input {
  width: 500px;
  color: #999 !important;
  font-size: 12px;
  height: 45px;
  display: block;
  border-radius: none;
  border: 0px;
  padding: 12px 12px 12px 20px;
  fill: #000000;
  background-color: #ffffff;
  transition: all 0.4s ease;
  font-style: normal !important;
}

.newsletter-container-form input.error {
  border-color: red;
  box-shadow: 2px 2px 8px rgba(255, 0, 0, 0.3);
}
.newsletter-container-form input::placeholder {
  transition: 200ms;
}
.newsletter-container-form input.error::placeholder {
  color: #ff0000;
  opacity: 1;
}
.newsletter-container-form input[type="text"] {
  max-width: 338px;
}

.newsletter-container-form button[type="submit"] {
  display: block;
  opacity: 100 !important;
  width: 300px;
  padding: 16px 0px 16px 0px;
  border-radius: none;
  border:none;
  font-weight: bold;
  background: #ff9326;
  color: #fff;
  font-size: 12px;
  margin: 10px auto;
  cursor: pointer;
  text-transform: uppercase;
}
.newsletter-container-form button[type="submit"] span.material-icons {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: #214861;
  display: flex;
  align-items: center;
  justify-content: center;
}
.fadeCheck-leave-to,
.fadeCheck-enter {
  opacity: 0;
}
.fadeCheck-leave-active,
.fadeCheck-enter-active {
  transition: 300ms;
}

/********************* TABLET *********************/
@media (min-width: 768px) and (max-width: 1023px) {
  .newsletter-container {
    padding: 0;
  }
  .newsletter-container-form button {
    min-width: 125px;
  }
}

/********************* MOBILE *********************/
@media (max-width: 767px) {
  .newsletter-boxButton {
    width: 100%;
  }
  .newsletter-container {
    padding: 0;
    flex-direction: column;
    align-items: flex-start;
  }
  .newsletter-container-t1 {
    max-width: unset;
    margin-bottom: 10px;
    text-align: center;
    margin-right: 0;
    width: 100%;
  }
  .newsletter-container-form {
    flex-direction: column;
    align-items: center;
  }
  .newsletter-container-form input[type] {
    width: 300px;
    margin: 0 auto 5px auto;
  }
  .newsletter-container-form button[type="submit"] {
    margin-top: 10px;
    max-width: 200px;
    width: 100%;
  }
}
</style>
