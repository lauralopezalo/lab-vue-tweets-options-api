<template>
  <img :src="userImage" className="profile"/>
</template>

<script>
export default {
    name: "userImage",
    props: {
        userImage: String,
    },

}
</script>

<style>

</style>