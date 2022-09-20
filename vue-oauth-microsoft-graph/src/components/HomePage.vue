<template>
    <div class="homepage">
        <h1>Here comes the content of the HomePage</h1>
        <div>
            <base-button :class="{buttonprimary: true}" class="common button1" buttonText="BaseButton with custom margin" ></base-button>
            <base-button :disabled="true" :class="{buttonprimary: true}" class="common button2" buttonText="BaseButton disabled" aria-disabled="disabled"></base-button>
        </div>
        <div>
            <base-button :class="{buttonwarn: true}" class="common" buttonText="BaseButton with color props"></base-button>
        </div>
        <div>
            <base-button :class="{buttondanger: true}" class="common button1" buttonText="BaseButton with color props"></base-button>
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
        border-radius: 10px;
    }

    .button1{
        margin: 30px;
    }
</style>