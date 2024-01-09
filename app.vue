<template>
  <div>
    {{ data?.message }}
    <NuxtLayout>
    <!-- 路由出口 -->
    <NuxtPage></NuxtPage>
    </NuxtLayout>
  </div>
</template>

<script setup lang="ts">
  // const { message } = await $fetch('/api/hello') 
  // const {message} = await $fetch('/api/hello',{query:{name: 'tom'}})
  const {data,pending,error} = await useFetch('/api/hello')
  console.log(data,pending,error,'999');
</script>