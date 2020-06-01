<template>
  <div>
      <h4>User Page</h4>
      <button class='btn btn-primary' style='margin-top:50px' @click='navigateToHome()'> Goto Home</button>
  </div>
</template>

<script>
export default {
    methods:{
        navigateToHome(){
            this.$router.push('/')
        }
    }
}
</script>

<style>

</style>