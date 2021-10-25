<template>
  <div container>
    <div avatar-container>
      <img avatar :src="url" >
    </div>
    <div main>
      <div v-for="(link, index) in links" v-bind:key="index">
        <a :href="link.url" target="_blank" v-text="link.label" />
      </div>
      <p description v-text="description"></p>
    </div>
  </div>
</template>
<script>

  export default {
    name: 'App',
    data: () => ({
      url: "https://images.unsplash.com/photo-1535713875002-d1d0cf377fde?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxjb2xsZWN0aW9uLXBhZ2V8MXw3NjA4Mjc3NHx8ZW58MHx8fHw%3D&w=1000&q=80",
      links: [
        {
          label: 'Tictok',
          url: 'http://google.com',
        },
        {
          label: 'instargram',
          url: 'http://google.com',
        },
        {
          label: 'Snapchat',
          url: 'http://google.com',
        },
        {
          label: 'Twitter',
          url: 'http://google.com',
        },
      ],
      description: "Loren ipsum dolor sit amet, consectetur adipiscing elite, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
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
    padding: 15px;
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
    text-align: left;
    a {
      color: #e8e3dd;
      font-family: new-spirit, serif;
      font-weight: 500;
      font-style: normal;
      font-size: 42px;
    }
  }
  [description] {
    font-family: 'Courier New';
  }
</style>
