<template>
    <div class="homepage">
        <h1>Here comes the content of the HomePage</h1>
        <div>
            <base-button :class="{buttonprimary: true,common: true}" class="button1" buttonText="BaseButton with custom margin" ></base-button>
            <base-button :disabled="true" :class="{buttonprimary: true,common: true}" buttonText="BaseButton disabled" aria-disabled="disabled"></base-button>
        </div>
        <div>
            <base-button :class="{buttonwarn: true,common: true}" buttonText="BaseButton with color props"></base-button>
        </div>
        <div>
            <base-button :class="{buttondanger: true,common: true}" class="button1" buttonText="BaseButton with color props"></base-button>
        </div>  
        <async-button @click="handlebutton" buttonTextBis="Async Button"></async-button>
    </div>
</template>

<script>
import BaseButton from './BaseButton.vue'
import AsyncButton from './AsyncButton.vue'

export default {
  name: 'HomePage',
  components: {
    BaseButton,
    AsyncButton
  }
}
</script>


<style>
    .homepage{
        background-color: white;
        position: static; 
        font-family: "Gill Sans", sans-serif;   
    }

    .button1{
        margin: 30px;
    }
</style>