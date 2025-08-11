<script setup>
import SocialPost from './molecules/SocialPost.vue'
import TestFooter from './molecules/TestFooter.vue'
</script>

<template>
  <SocialPost
    username="Username one"
    userId="usernameID1"
    avatarSrc="https://i.pravatar.cc/40"
    post="This is my post"
  />
  <SocialPost
    username="Username two"
    userId="usernameID2"
    avatarSrc="https://i.pravatar.cc/40"
    post="This is my second post"
  ></SocialPost>
  <TestFooter />
</template>
