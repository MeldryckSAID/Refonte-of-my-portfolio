<template>
  <div>
    <form
      action="https://formsubmit.co/meldryck.d.said@gmail.com"
      method="POST"
    >
      <div class="grid-container">
        <div>
          <input
            type="text"
            name="nom"
            :placeholder="isInputFilled(input1) ? '' : 'Votre Nom'"
            id="input1"
            v-model="input1"
            class="form_input"
            @focus="addShadow"
            @blur="removeShadow"
          />
        </div>
        <div>
          <input
            class="form_input"
            type="text"
            name="Prénom"
            :placeholder="isInputFilled(input2) ? '' : 'Votre Prénom'"
            id="input2"
            v-model="input2"
            @focus="addShadow"
            @blur="removeShadow"
          />
        </div>

        <div>
          <input
            class="form_input"
            type="email"
            name="email"
            :placeholder="isInputFilled(input3) ? '' : 'E-mail'"
            id="input3"
            v-model="input3"
            @focus="addShadow"
            @blur="removeShadow"
          />
        </div>
        <div class="mb-4 flex flex-col">
          <select
            class="form_select"
            name="Type"
            v-model="selectedOption"
            required
            id="input4"
           
          >
            <option class="" value="option" disabled selected>
              Choisissez une option
            </option>
            <option class="" value="particulier">Particulier</option>
            <option class="" value="entreprise">Entreprise</option>
            <option class="" value="agence">Agence</option>
          </select>
        </div>
      </div>

      <div class="message">
        <textarea
          :placeholder="isInputFilled(input3) ? '' : 'Votre message:'"
          class="myTextArea"
          id="textarea"
          name="message"
          v-model="textareaContent"
       
        ></textarea>
      </div>
      <div class="form__button">
        <button class="buttof" libelle="Send" type="submit">
          <Mybutton>Envoyez</Mybutton>
        </button>
      </div>
    </form>
  </div>
</template>

<style lang="scss">
.grid-container {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 20px;
  justify-items: center;
}
.form_input {

  margin-bottom: 1.5rem;
  padding-left: 1.5rem;
  border: 2px solid $D;
  border-radius: rem(15);
  text-align: justify;
  text-align: start;
  font-family: $secondary-font;
  font-size: 20px;

  &::placeholder {
    text-align: start;
    font-family: $secondary-font;
    font-size: 20px;
    font-weight: 800;
  }
}
.form_select {
  margin-bottom: 1.5rem;
  padding-left: 1.5rem;
  border: 2px solid $D;
  border-radius: rem(15);
  font-family: $secondary-font;
  font-size: 20px;
  width: 301px;
  &::placeholder {
    text-align: start;
    font-family: $secondary-font;
    font-size: 20px;
    font-weight: 400;
  }
}
.message {
  display: flex;
  justify-content: center;
  margin: 20px;
}
.myTextArea {
  width: 614px;
  height: 218.161px;
  padding-left: 1.5rem;
  font-family: $secondary-font;
  font-size: 14px;
  font-weight: 500;
  flex-shrink: 0;
  border: 2px solid $D;
  border-radius: rem(15);
  &::placeholder {
    text-align: start;
    font-family: $secondary-font;
    font-size: 20px;
    font-weight: 800;
  }
}

.form__button {
  display: flex;
  justify-content: center;
  .buttof {
    border: none;
  }
}
</style>

<script setup>
import { ref } from "vue";

const selectedOption = ref("option");

const isInputFilled = (input) => {
  return input !== "";
};


const input1 = ref("");
const input2 = ref("");
const input3 = ref("");
const input5 = ref("");
const textareaContent = ref("");
</script>
