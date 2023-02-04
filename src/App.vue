<script setup>
import HelloWorld from './components/HelloWorld.vue'
import count  from './components/count.vue'
import reactiveproxy from './components/reactiveproxy.vue'
import methods from './components/methods.vue';
import updatetiming from './components/updatetiming.vue';
import deepreactivity from './components/deepreactivity.vue';
import computed from './components/computed.vue';
</script>

<template>
  <header>
    <div class="wrapper">
      <HelloWorld msg="You did it!" />
    </div>
  </header>

  <main>
    <count />
    <reactiveproxy />
    <methods />
    <updatetiming />
    <deepreactivity />
    <computed />
  </main>
</template>
