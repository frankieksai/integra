<template>
    <div class="parallax-container">
      <div class="section no-pad-bot">
        <div class="container">
          <br />
          <br />
          <h1 class="header center blue-text darken-4">{{headerText}}</h1>
          <br />
          <br />
          <div class="row center">
            <h5
              class="header col s12 white-text"
            >{{text}}</h5>
          </div>
        </div>
      </div>
      <div class="parallax">
        <img
          :src='imgUrl'
          alt
        />
      </div>
    </div>
</template>
<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
    props: {
        header: {
            type: String
        },
        text: {
            type: String
        },
        img: {
            type: String,
            required: true
        }
    },
    computed: {
        headerText(){
            return this.header || ''
        },
        Text(){
            return this.text || ''
        },
        imgUrl(){
            return this.img
        }
    }
})
</script>