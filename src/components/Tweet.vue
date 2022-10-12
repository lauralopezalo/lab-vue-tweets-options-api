<template>
  <div className="tweet">
    <ProfileImage :userImage="user.image" />
    <div className="body">
      <div className="top">
        <User :user="user" />
        <Timestamp :timestamp="timestamp" />
      </div>
      <Message :message="message" />
      <Actions />
    </div>
    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script>
import User from "../components/User.vue";
import ProfileImage from "../components/ProfileImage.vue";
import Timestamp from "../components/Timestamp.vue";
import Message from "../components/Message.vue";
import Actions from "../components/Actions.vue";

export default {
  name: "Tweet",
  components: {
    User,
    ProfileImage,
    Timestamp,
    Message,
    Actions,
  },
  props: {
    user: Object,
    userImage: String,
    timestamp: String,
    message: String,
  },
};
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
