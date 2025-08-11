<script setup>
import { reactive } from 'vue'
import SocialPost from './molecules/SocialPost.vue'
import TestFooter from './molecules/TestFooter.vue'
const posts = reactive([
  {
    username: 'Username one',
    userId: 'usernameId1',
    avatarSrc: 'https://i.pravatar.cc/40',
    post: 'This is my post',
  },
  {
    username: 'Username two',
    userId: 'usernameId2',
    avatarSrc: 'https://i.pravatar.cc/40',
    post: 'This is my second post',
  },
])
</script>

<template>
  <SocialPost
    :username="posts[0].username"
    :userId="posts[0].userId"
    :avatarSrc="posts[0].avatarSrc"
    :post="posts[0].post"
  />
  <SocialPost
    :username="posts[1].username"
    :userId="posts[1].userId"
    :avatarSrc="posts[1].avatarSrc"
    :post="posts[1].post"
  ></SocialPost>
  <TestFooter />
</template>
