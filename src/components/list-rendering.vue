<script>
    data() {
        return {
            parentMessage: 'Parent',
            items: [{ message: 'Foo' }, { message: 'Bar' }]
        }
    }

    //v-for with an object
    data() {
  return {
    myObject: {
      title: 'How to do lists in Vue',
      author: 'Jane Doe',
      publishedAt: '2016-04-10'
    }
  }
}


</script>

<template>
<li v-for="(item, index) in items">
  {{ parentMessage }} - {{ index }} - {{ item.message }}
</li>

<ul>
  <li v-for="value in myObject">
    {{ value }}
  </li>
</ul>


<li v-for="(value, key) in myObject">
  {{ key }}: {{ value }}
</li>


<li v-for="(value, key, index) in myObject">
  {{ index }}. {{ key }}: {{ value }}
</li>

</template>
