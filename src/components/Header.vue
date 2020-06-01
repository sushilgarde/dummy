<template>
  <div>
    <nav class="nav nav-pills">
        <router-link to='/' tag='li' active-class="active" exact><a>Home</a></router-link>
        <router-link to='/user' tag='li' active-class="active"><a>User</a></router-link>
    </nav>
    <hr>
  </div>
</template>

<script>
export default {

}
</script>

<style>
nav{
    width: 600px;
    margin: 0 auto;
}
</style>