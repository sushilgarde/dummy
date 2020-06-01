<template>
  <div>
    <form style='border: 1px solid; width: 300px; padding: 40px; margin: 200px auto'>
        Username: <input type="text" v-model='username'> <br> <br>
        Session Id: <input type="text" v-model='sessionId'> <br> <br>
        <button class='btn btn-primary' @click='joinSession()'>Join Session</button>
    </form>
  </div>
</template>

<script>
export default {
    data(){
        return{
            username: '',
            sessionId: ''
        }
    },
    methods:{
        joinSession(){
            this.$router.push({
                path: '/session',
                query:{
                    sessionId: this.sessionId,
                    username: this.username
                }
            })
        }
    }
}
</script>

<style>

</style>