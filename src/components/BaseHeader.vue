<template>

    <header class="base-header">
        <div class="header-content">
            <div @click="navigateHome" class="header-left">
                <svg class="header-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 576 512"><path d="M575.8 255.5c0 18-15 32.1-32 32.1l-32 0 .7 160.2c0 2.7-.2 5.4-.5 8.1l0 16.2c0 22.1-17.9 40-40 40l-16 0c-1.1 0-2.2 0-3.3-.1c-1.4 .1-2.8 .1-4.2 .1L416 512l-24 0c-22.1 0-40-17.9-40-40l0-24 0-64c0-17.7-14.3-32-32-32l-64 0c-17.7 0-32 14.3-32 32l0 64 0 24c0 22.1-17.9 40-40 40l-24 0-31.9 0c-1.5 0-3-.1-4.5-.2c-1.2 .1-2.4 .2-3.6 .2l-16 0c-22.1 0-40-17.9-40-40l0-112c0-.9 0-1.9 .1-2.8l0-69.7-32 0c-18 0-32-14-32-32.1c0-9 3-17 10-24L266.4 8c7-7 15-8 22-8s15 2 21 7L564.8 231.5c8 7 12 15 11 24z"/></svg>
                <a href=""><span class="home-text">Home</span></a>
            </div>
            
            <div class="header-right">
                <svg class="header-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"><path d="M399 384.2C376.9 345.8 335.4 320 288 320l-64 0c-47.4 0-88.9 25.8-111 64.2c35.2 39.2 86.2 63.8 143 63.8s107.8-24.7 143-63.8zM0 256a256 256 0 1 1 512 0A256 256 0 1 1 0 256zm256 16a72 72 0 1 0 0-144 72 72 0 1 0 0 144z"/></svg>
                <a href=""><span @click="navigateLogin" class="user-text">not yet logged in</span></a>
            </div>
        </div>
    </header>
        

</template>

<script>

const navigateLogin = () =>
{
    console.log("test")
    console.log("navigate to login mock");
}
const navigateHome = () =>
{
    console.log("navigate Home mock");
}


export default {
  name: 'BaseHeader',
  methods: {
    navigateHome,
    navigateLogin
  }
}


</script>

<style scoped>

.header-icon
{
    width: 24px;
    height: 24px;
}

.base-header {
  background-color: #cecece;
  width: 100%;
  padding: 0;
}

.header-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 12px 20px;
  max-width: 100%;
}

.header-left,
.header-right {
    
  display: flex;
  align-items: center;
  gap: 8px;
  cursor: pointer;
}

.home-icon,
.user-icon {
  color: #333;
  font-size: 16px;
}

.home-text,
.user-text {

  color: #333;
  font-size: 16px;
  font-weight: 500;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
  
}

a 
{
text-decoration: none;

}


</style>