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

<style>
  @media only screen and (min-width: 640px) {
    .link {

    }
  }
  body {
    display: flex;
    justify-content: center;
    align-items: center;
    font-family: Tahoma, Verdana, sans-serif;
    background: linear-gradient(to right, rgba(34,0,36,1) 0%, rgba(109,9,121,1) 50%, rgba(255,139,0,1) 100%) fixed;
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
</style>
