<template>
  <div container>
    <div avatar-container>
      <img avatar src="https://images.unsplash.com/photo-1535713875002-d1d0cf377fde?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxjb2xsZWN0aW9uLXBhZ2V8MXw3NjA4Mjc3NHx8ZW58MHx8fHw%3D&w=1000&q=80" >
    </div>
    <div main>
      <div v-for="(link, index) in links" v-bind:key="index">
        dddd
      </div>
    </div>
  </div>
</template>
<script>

  export default {
    name: 'App',
    data: () => ({
      links: [
        {
          label: 'Tictok',
          links: 'google.com',
        },
        {
          label: 'instargram',
          links: 'google.com',
        },
        {
          label: 'Snapchat',
          links: 'google.com',
        },
        {
          label: 'Twitter',
          links: 'google.com',
        },
      ]
  })
  }
</script>

<style lang="scss">
  body {
    background: #2c6622;
    color: #fff;
    font-family: Helvetica;
    text-align: center;
  }
  [container] {
    padding: 20px 15px;
  }
  [avatar-container] {
    height: 40vh;
    display: flex;
    justify-content: flex-end;
    align-items: flex-end;
  }
  [avatar] {
      width: 150px;
      height: 150px;
      border-radius: 50%;
    }
  [main] {
    flex: 1;
    font-family: new-spirit, serif;
    font-weight: 500;
    font-style: normal;
  }
</style>
