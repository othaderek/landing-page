<template>
  <div id="app">
    <Header />
    <Links/>
  </div>
</template>

<script>
import Links from './components/Links'
import Header from './components/layout/Header'

export default {
  name: 'App',
  components: {
    Links,
    Header
  }
}
</script>

<style lang="scss">
  $desktop:1200px;
  $laptop:1024px;
  $tablet:768px;
  $phone:375px;

  body {
    display: flex;
    justify-content: center;
    align-items: center;
    font-family: Tahoma, Verdana, sans-serif;
    background: linear-gradient(to right, rgba(34,0,36,1) 0%, rgba(109,9,121,1) 50%, rgba(255,139,0,1) 100%) fixed;
    width: 100%;
    position: relative;
  }
  .link {
    display: inline-block;
    border: 2px solid white;
    color: #fff;
    padding: 7px 20px;
    cursor: pointer;
    height: auto;
    width: auto;
    margin-bottom: 10px;
    min-width: 640px;
    max-width: 640px;
    min-height: 45px;
    max-height: 50px;
  }
  .text{
    vertical-align: middle;
    text-align: center;
    font: Roboto;
  }
  .link:hover {
    background: #fff;
    color: rgba(34,0,36,1);
  }

  @media only screen and (max-width: $phone){
    body{
      min-width: $phone;
    }
  }
  @media only screen and (max-width: $tablet){
    body{
      min-width: $tablet;
    }
  @media only screen and (max-width: $phone){
      .link{
        min-width: 200px;
      }
    }
  @media only screen and (max-width: $tablet){
      .link{
        min-width: 600px;
      }
    }
  }
</style>
