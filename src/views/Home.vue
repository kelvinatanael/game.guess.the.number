<template>
  <div class="content-home">
    <div class="content-home-itens">
      <div class="content-home-itens-title">
        <h2>QUAL É O NÚMERO?</h2>
      </div>
      <div class="content-home-itens-number">
        <div class="content-text" :class="typeNumber.style">
          <p>{{typeNumber.text}}</p>
        </div>
        <div class="content-numbers" :class="typeNumber.style">
          <svg class="first-element" :class="[arrayNumbers[0] ? `number-${arrayNumbers[0]}` : 'number-0']" viewBox="0 0 75 135" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path class="a" d="M17.269 14.8295H57.5517L71.4885 1.59469C70.1985 0.597611 68.5846 3.8147e-06 66.8301 3.8147e-06H7.63794C5.89411 3.8147e-06 4.29303 0.589093 3.00726 1.57233L17.269 14.8295Z"/>
            <path class="b" d="M1.71614 2.8155C0.644493 4.1311 0 5.80888 0 7.63687V59.4298C0 62.3986 1.69695 64.9659 4.17155 66.2293L15.8425 57.4825V15.947L1.71614 2.8155Z"/>
            <path class="c" d="M58.6244 16.2662V57.4704L70.2954 66.2173C72.77 64.9539 74.4669 62.3866 74.4669 59.4177V7.62484C74.4669 5.80751 73.8299 4.14251 72.7721 2.83224L58.6244 16.2662Z"/>
            <path class="d" d="M17.269 120.169H57.5517L71.4885 133.405C70.1985 134.4 68.5846 135 66.8301 135H7.63793C5.8941 135 4.29302 134.409 3.00726 133.426L17.269 120.169Z"/>
            <path class="e" d="M1.71614 132.194C0.644493 130.88 0 129.203 0 127.374V75.5812C0 72.6124 1.69695 70.0461 4.17155 68.7817L15.8425 77.5285V119.064L1.71614 132.194Z"/>
            <path class="f" d="M58.6244 118.721V77.5165L70.2954 68.7696C72.77 70.0341 74.4669 72.6003 74.4669 75.5692V127.362C74.4669 129.178 73.8299 130.843 72.7721 132.156L58.6244 118.721Z"/>
            <path class="g" d="M57.4494 59.39H17.0175L6.24985 67.3273L17.0175 75.2656H32.4329H42.034H57.4494L68.217 67.3273L57.4494 59.39Z"/>
          </svg>
          <svg class="second-element" :class="[arrayNumbers[1] ? `number-${arrayNumbers[1]}` : 'd-none']" viewBox="0 0 75 135" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path class="a" d="M17.269 14.8295H57.5517L71.4885 1.59469C70.1985 0.597611 68.5846 3.8147e-06 66.8301 3.8147e-06H7.63794C5.89411 3.8147e-06 4.29303 0.589093 3.00726 1.57233L17.269 14.8295Z"/>
            <path class="b" d="M1.71614 2.8155C0.644493 4.1311 0 5.80888 0 7.63687V59.4298C0 62.3986 1.69695 64.9659 4.17155 66.2293L15.8425 57.4825V15.947L1.71614 2.8155Z"/>
            <path class="c" d="M58.6244 16.2662V57.4704L70.2954 66.2173C72.77 64.9539 74.4669 62.3866 74.4669 59.4177V7.62484C74.4669 5.80751 73.8299 4.14251 72.7721 2.83224L58.6244 16.2662Z"/>
            <path class="d" d="M17.269 120.169H57.5517L71.4885 133.405C70.1985 134.4 68.5846 135 66.8301 135H7.63793C5.8941 135 4.29302 134.409 3.00726 133.426L17.269 120.169Z"/>
            <path class="e" d="M1.71614 132.194C0.644493 130.88 0 129.203 0 127.374V75.5812C0 72.6124 1.69695 70.0461 4.17155 68.7817L15.8425 77.5285V119.064L1.71614 132.194Z"/>
            <path class="f" d="M58.6244 118.721V77.5165L70.2954 68.7696C72.77 70.0341 74.4669 72.6003 74.4669 75.5692V127.362C74.4669 129.178 73.8299 130.843 72.7721 132.156L58.6244 118.721Z"/>
            <path class="g" d="M57.4494 59.39H17.0175L6.24985 67.3273L17.0175 75.2656H32.4329H42.034H57.4494L68.217 67.3273L57.4494 59.39Z"/>
          </svg>
          <svg class="third-element" :class="[arrayNumbers[2] ? `number-${arrayNumbers[2]}` : 'd-none']" viewBox="0 0 75 135" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path class="a" d="M17.269 14.8295H57.5517L71.4885 1.59469C70.1985 0.597611 68.5846 3.8147e-06 66.8301 3.8147e-06H7.63794C5.89411 3.8147e-06 4.29303 0.589093 3.00726 1.57233L17.269 14.8295Z"/>
            <path class="b" d="M1.71614 2.8155C0.644493 4.1311 0 5.80888 0 7.63687V59.4298C0 62.3986 1.69695 64.9659 4.17155 66.2293L15.8425 57.4825V15.947L1.71614 2.8155Z"/>
            <path class="c" d="M58.6244 16.2662V57.4704L70.2954 66.2173C72.77 64.9539 74.4669 62.3866 74.4669 59.4177V7.62484C74.4669 5.80751 73.8299 4.14251 72.7721 2.83224L58.6244 16.2662Z"/>
            <path class="d" d="M17.269 120.169H57.5517L71.4885 133.405C70.1985 134.4 68.5846 135 66.8301 135H7.63793C5.8941 135 4.29302 134.409 3.00726 133.426L17.269 120.169Z"/>
            <path class="e" d="M1.71614 132.194C0.644493 130.88 0 129.203 0 127.374V75.5812C0 72.6124 1.69695 70.0461 4.17155 68.7817L15.8425 77.5285V119.064L1.71614 132.194Z"/>
            <path class="f" d="M58.6244 118.721V77.5165L70.2954 68.7696C72.77 70.0341 74.4669 72.6003 74.4669 75.5692V127.362C74.4669 129.178 73.8299 130.843 72.7721 132.156L58.6244 118.721Z"/>
            <path class="g" d="M57.4494 59.39H17.0175L6.24985 67.3273L17.0175 75.2656H32.4329H42.034H57.4494L68.217 67.3273L57.4494 59.39Z"/>
          </svg>
        </div>
        <button class="btn-new-game" @click="resetFields()" v-if="typeNumber.inputDisabled || typeNumber.correct">
          <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
            <g id="refresh_24px">
            <path id="icon/navigation/refresh_24px" d="M16.2364 7.7625C15.1482 6.675 13.6548 6 11.9962 6C8.67917 6 6 8.685 6 12C6 15.315 8.67917 18 11.9962 18C14.7955 18 17.1295 16.0875 17.7974 13.5H16.2364C15.621 15.2475 13.955 16.5 11.9962 16.5C9.51219 16.5 7.49343 14.4825 7.49343 12C7.49343 9.5175 9.51219 7.5 11.9962 7.5C13.242 7.5 14.3527 8.0175 15.1632 8.835L12.7467 11.25H18V6L16.2364 7.7625Z" fill="white"/>
            </g>
          </svg>
          <p>NOVA PARTIDA</p>
        </button>
      </div>
      <form class="content-home-itens-form" ref="formNumber">
        <div class="content-input" :class="{'content-input-disabled': typeNumber.inputDisabled || typeNumber.correct}">
          <input type="number" name="input_number" placeholder="Digite o palpite" min="1" max="300" v-on:input="checkInputNumber($event)" :value="valNumber" required/>
          <button type="button" :class="{'disabled-btn': !isValid}" class="content-input-btn" @click="typeNumber.correct || !numberApi ? getNumberApi() : checkNumber()">Enviar</button>
        </div>
      </form>
    </div>  
  </div>
</template>
<script>
import axios from 'axios';

export default {
  data() {
    return {
      isValid: false,
      valNumber: null,
      numberApi: null,
      typeNumber: {},
      arrayNumbers: [],
    };
  },
  methods: {
    // CHECK INPUT NUMBER
    checkInputNumber(e){
      this.$refs.formNumber.reportValidity() ? this.isValid = true : this.isValid = false;
      this.valNumber = e.target.value;
    },
    // GET DATA API
    getNumberApi() {
      axios.get('https://us-central1-ss-devops.cloudfunctions.net/rand?min=1&max=300').then(resp => {
        this.numberApi = resp.data.value;
        this.checkNumber();
      }).catch((error) => {
          // CALL FUNCTION CREATE OBJECT TYPE NUMBER
          this.createObjectTypeNumber('ERRO', 'text-red', false, true);

          this.valNumber = error.response.data.StatusCode;
          // CALL FUNCTION CREATE NUMBERS
          this.createNumbers();
        });
    },
    //CREATE OBJECT TYPE NUMBER
    createObjectTypeNumber(text, style, correct, disabled){
      this.typeNumber = {
        text: text,
        style: style,
        correct: correct,
        inputDisabled: disabled
      }
    },
    // CREATE NUMBERS
    createNumbers() {
      this.arrayNumbers = this.valNumber.toString().split('');

      // RESET VARIABLES
      this.valNumber = null;
      if (this.typeNumber.correct){
        this.numberApi = null;
      }
    },
    // CHECKING NUMBER
    checkNumber(){
      console.log(this.numberApi);
      // VERIFY NUMBER IS SMALLER
      if (this.numberApi < this.valNumber){
        // CALL FUNCTION CREATE OBJECT TYPE NUMBER
        this.createObjectTypeNumber('É menor', 'text-orange', false, false);
        
        // CALL FUNCTION CREATE NUMBERS
        this.createNumbers();
        return;
      } 
      // VERIFY NUMBER IS BIGGER
      else if (this.numberApi > this.valNumber){
        // CALL FUNCTION CREATE OBJECT TYPE NUMBER
        this.createObjectTypeNumber('É maior', 'text-orange', false, false);

        // CALL FUNCTION CREATE NUMBERS
        this.createNumbers();
        return;
      } 
      //NUMBER IS EQUAL
      else {
        // CALL FUNCTION CREATE OBJECT TYPE NUMBER
        this.createObjectTypeNumber('Você acertou!!!!', 'text-green', true, false);

        // CALL FUNCTION CREATE NUMBERS
        this.createNumbers();
      }
    },
    // RESET FIELDS
    resetFields() {
      this.isValid = false;
      this.valNumber = null;
      this.numberApi = null;
      this.typeNumber = {};
      this.arrayNumbers = [];
    }
  },
}
</script>
<style lang="scss">
.content-home {
  min-height: 100vh;
  background: linear-gradient(to bottom, var(--gray-4), var(--white));
  &-itens {
    padding: 50px 0px;
    @media (max-width: 991px){
      padding: 60px 20px 30px 20px;
    }
    &-title {
      margin-bottom: 50px;
      h2 {
        position: relative;
        font-size: 36px;
        font-family: 'Font Montserrat Bold';
        color: var(--orange);
        padding-bottom: 25px;
        margin: 0;
        @media (max-width: 991px){
          font-size: 24px;
          padding-bottom: 15px;
        }
        &::after {
          content: '';
          display: block;
          width: 255px;
          height: 1px;
          background: var(--gray-2);
          position: absolute;
          left: 50%;
          transform: translateX(-50%);
          bottom: 0;
          @media (max-width: 991px){
            width: 205px;
          }
        }
      }
    }
    &-number {
      position: absolute;
      left: 50%;
      top: 50%;
      transform: translate(-50%, -50%);
      width: 100%;
      .content-text {
        margin-bottom: 30px;
        p {
          font-size: 16px;
          font-family: 'Font Montserrat Bold';
          margin: 0;
        }
      }
      .content-numbers {
        .first-element, .second-element, .third-element {
          fill: #DDDDDD;
          width: 75px;
          height: 135px;
          margin-right: 12px;
          @media (max-width: 991px){
            width: 56px;
            height: 100px;
          }
        }
        .number-0 {
          .a,.b, .c, .d, .e, .f{
            fill: #262A34;
          }
        }
        .number-1 {
          .c, .f{
            fill: #262A34;
          }
        }
        .number-2 {
          .a, .c, .d, .e, .g{
            fill: #262A34;
          }
        }
        .number-3 {
          .a, .c, .d, .f, .g{
            fill: #262A34;
          }
        }
        .number-4 {
          .b, .c,.f,.g{
            fill: #262A34;
          }
        }
        .number-5 {
          .a, .b, .d, .f, .g{
            fill: #262A34;
          }
        }
        .number-6 {
          .a, .b, .d, .e, .f, .g{
            fill: #262A34;
          }
        }
        .number-7 {
          .a, .c,.f {
            fill: #262A34;
          }
        }
        .number-8 {
          .a, .b, .c, .d, .e, .f, .g {
            fill: #262A34;
          }
        }
        .number-9 {
          .a, .b, .c, .d, .f, .g {
            fill: #262A34;
          }
        }
      }
      .text-orange {
        color: var(--orange-2);
      }
      .text-green {
        color: var(--green);
        .number-0 {
          .a,.b, .c, .d, .e, .f{
            fill: var(--green);
          }
        }
        .number-1 {
          .c, .f{
            fill: var(--green);
          }
        }
        .number-2 {
          .a, .c, .d, .e, .g{
            fill: var(--green);
          }
        }
        .number-3 {
          .a, .c, .d, .f, .g{
            fill: var(--green);
          }
        }
        .number-4 {
          .b, .c,.f,.g{
            fill: var(--green);
          }
        }
        .number-5 {
          .a, .b, .d, .f, .g{
            fill: var(--green);
          }
        }
        .number-6 {
          .a, .b, .d, .e, .f, .g{
            fill: var(--green);
          }
        }
        .number-7 {
          .a, .c,.f {
            fill: var(--green);
          }
        }
        .number-8 {
          .a, .b, .c, .d, .e, .f, .g {
            fill: var(--green);
          }
        }
        .number-9 {
          .a, .b, .c, .d, .f, .g {
            fill: var(--green);
          }
        }
      }
      .text-red {
        color: var(--red);
        .number-0 {
          .a,.b, .c, .d, .e, .f{
            fill: var(--red);
          }
        }
        .number-1 {
          .c, .f{
            fill: var(--red);
          }
        }
        .number-2 {
          .a, .c, .d, .e, .g{
            fill: var(--red);
          }
        }
        .number-3 {
          .a, .c, .d, .f, .g{
            fill: var(--red);
          }
        }
        .number-4 {
          .b, .c,.f,.g{
            fill: var(--red);
          }
        }
        .number-5 {
          .a, .b, .d, .f, .g{
            fill: var(--red);
          }
        }
        .number-6 {
          .a, .b, .d, .e, .f, .g{
            fill: var(--red);
          }
        }
        .number-7 {
          .a, .c,.f {
            fill: var(--red);
          }
        }
        .number-8 {
          .a, .b, .c, .d, .e, .f, .g {
            fill: var(--red);
          }
        }
        .number-9 {
          .a, .b, .c, .d, .f, .g {
            fill: var(--red);
          }
        }
      }
      .btn-new-game {
        width: 100%;
        max-width: 130px;
        height: 42px;
        display: flex;
        justify-content: center;
        align-items: center;
        background: linear-gradient(to bottom, #434854, #9E9E9E);
        border: 0;
        border-radius: 4px;
        margin: 30px auto;
        transition: 500ms;
        &:hover,&:focus {
          cursor: pointer;
        }
        p {
          font-size: 12px;
          font-family: 'Font Roboto Bold';
          color: var(--white);
          text-transform: uppercase;
          padding: 0;
          margin: 0;
        }
      }
    }
    &-form {
      position: absolute;
      bottom: 60px;
      left: 50%;
      transform: translateX(-50%);
      width: calc(100% - 40px);
      @media (max-width: 991px){
        bottom: 30px;
      }
      .content-input {
        display: flex;
        align-items: center;
        justify-content: center;
        input {
          width: calc(100% - 81px);
          max-width: 217px;
          height: 40px;
          background: var(--white);
          border: 1px solid var(--gray-2);
          border-radius: 4px;
          padding: 0;
          padding-left: 12px;
          font-size: 12px;
          font-family: 'Font Roboto Regular';
          color: #222222;
          outline: none;
          -moz-appearance: textfield;
          appearance: textfield;
          -webkit-appearance: textfield;
          &::-webkit-inner-spin-button { 
            -webkit-appearance: none; 
          }
          &::-webkit-input-placeholder { /* Chrome/Opera/Safari */
            color: #9E9E9E;
          }
          &::-moz-placeholder { /* Firefox 19+ */
            color: #9E9E9E;
          }
          &:-ms-input-placeholder { /* IE 10+ */
            color: #9E9E9E;
          }
          &:-moz-placeholder { /* Firefox 18- */
            color: #9E9E9E;
          }
          &:not(:placeholder-shown){
            border: 1px solid var(--orange-2)
          }
        }
        &-btn {
          width: 70px;
          height: 42px;
          display: flex;
          justify-content: center;
          align-items: center;
          background: var(--orange);
          border: 1px solid var(--orange);
          border-radius: 4px;
          font-size: 12px;
          font-family: 'Font Roboto Bold';
          color: var(--white);
          text-transform: uppercase;
          margin-left: 11px;
          transition: 500ms;
          &:hover,&:focus {
            cursor: pointer;
            background: var(--white);
            color: var(--orange);
          }
        }
        &-disabled {
          pointer-events: none;
          input {
            background: var(--gray-3);
            border: 1px solid var(--gray-2);
          }
          .content-input-btn {
            background: var(--gray);
            border: 1px solid var(--gray);
            color: var(--white);
          }
        }
      }
    }
  }
  .disabled-btn {
    pointer-events: none;
    background: var(--gray);
    border: 1px solid var(--gray);
    color: var(--white);
  }
}
</style>