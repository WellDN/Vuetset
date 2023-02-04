<script setup>
    defineProps({
  msg: {
    type: String,
    required: true
  }
})

</script>

<template>
    <div class="greetings">
        <span> Message: {{ msg }} </span>

        <p>Using text interpolation: {{ rawHtml }}</p>
        <p>Using v-html directive: <span v-html="rawHtml"></span></p>
        <span style="color:red">this should be red.</span>
        <div :id="dynamicId">v-bind shortand </div>
        <button :disabled="isButtonDisabled">button </button>
        <p v-if="seen">Now you see me </p>
        <a :href="url"></a>
        <a @click="doSomething"></a>
        <a :[attributeName]="url"> </a>
        <a @[eventName]="doSomething"> </a>
        <form @submit.prevent="onSubmit"> </form>
        </div>
    </template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
