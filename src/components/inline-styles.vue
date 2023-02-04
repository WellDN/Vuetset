<script>
    data() {
        return {
            styleObject: {
            color: 'red',
            fontSize: '13px'
            }
        }
    }
</script>

<template>
    <div :style="styleObject"></div>
    <div :style="{ display: ['-webkit-box', '-ms-flexbox', 'flex'] }"></div>
</template>
