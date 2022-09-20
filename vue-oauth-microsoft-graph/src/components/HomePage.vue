<template>
    <div class="homepage">
        <h1>Here comes the content of the HomePage</h1>
        <div>
            <base-button class="common button1" buttonText="BaseButton with custom margin" ></base-button>
            <base-button :disabled="true" class="common button2" buttonText="BaseButton disabled" aria-disabled="disabled"></base-button>
        </div>
    </div>
</template>

<script>
import BaseButton from './BaseButton.vue'

export default {
  name: 'HomePage',
  components: {
    BaseButton
  }
}
</script>


<style>
    .homepage{
        background-color: white;
        position: static; 
        font-family: "Gill Sans", sans-serif;   
    }

    .common{
        padding: 10px;
        border: none;
        background-color: #2bb883;
        border-radius: 10px;
    }

    .common:hover{
        background-color: #8bd6b9;
    }

    .button1{
        margin: 30px;
    }
</style>