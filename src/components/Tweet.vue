<template>

  <div className="tweet">
        <ProfileImage image="user.image" />
      <div className="body">
        <div className="top">       
            <User/>
            <Timestamp/>
            <Message/>
            <Actions/>
            <i class="fas fa-ellipsis-h"></i>
        </div>  
      </div>  
  </div>  
 
</template>

<script>
import { stringifyStyle } from "@vue/shared";
import ProfileImage from "./ProfileImage.vue";
import User from "./User.vue";
import Message from "./Message.vue";
import Timestamp from './Timestamp.vue';
import Actions from "./Actions.vue";



export default {
  components: { Timestamp, Actions ,Profileimage,User, Message,},
  name: "Tweet",
  props: {
    user:String,
    timestamp:String,
    message:String,
    name:String,
    handle:String,
    profileimage: String,

    
  }
  
}
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
