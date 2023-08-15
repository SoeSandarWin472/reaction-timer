<template>
   <p>Result is {{score}}ms</p>
   <div v-if="score<250">
        <p>U r too fast</p>
   </div>
   <div v-else-if="score>250 && score <500">
        <p>U r Normal</p>
   </div>
   <div v-else>
        <p>U r too slow! try again</p>
   </div>
</template>

<script>
export default {
    name:"ResultB",
    props:["score"]
}
</script>

<style>

</style>