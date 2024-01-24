<template>
  <nav class="flex flex-1 items-center w-full h-6 p-4 gap-2">
    <Button variant="ghost" size="icon"><Pin color="red" :size="24" /></Button>
    <Button variant="default">Home</Button>
    <Button variant="ghost">Create</Button>
    <div class="relative flex grow">
      <Input class="pl-8" type="text" placeholder="Search" />
      <Search
        class="absolute left-2 top-1/2 transform -translate-y-1/2"
        color="gray"
        :size="16"
      />
    </div>
    <Button variant="ghost" size="icon"
      ><Bell color="grey" :size="24"
    /></Button>
    <Button variant="ghost" size="icon"
      ><MessageCircleMore color="grey" :size="24"
    /></Button>
    <Button variant="ghost" size="icon"
      ><Avatar>
        <AvatarImage
          src="https://i.pinimg.com/75x75_RS/cb/33/89/cb338912f19cf08b50bbdc85c3218ec8.jpg"
        /> </Avatar
    ></Button>
    <Button variant="ghost" size="smIcon"
      ><ChevronDown color="grey" :size="20"
    /></Button>
  </nav>
</template>
<script lang="ts" setup>
import {
  Pin,
  Search,
  Bell,
  MessageCircleMore,
  ChevronDown,
} from "lucide-vue-next";
import { AvatarImage } from "radix-vue";
</script>
