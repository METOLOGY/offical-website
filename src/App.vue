<template>
  <div id="app">
    <img id="metology-logo" src="/static/img/metology-icon.png">
    <Navbar></Navbar>
    <Product></Product>
    <Records></Records>
    <Partner></Partner>
    <Member></Member>
    <FootNav></FootNav>

  </div>
</template>

<script>
import Navbar from './components/Navbar'
import Product from './components/Product'
import Records from './components/Records'
import Partner from './components/Partner'
import Member from './components/Member'
import FootNav from './components/FootNav'

export default {
  name: 'app',
  components: {
    Navbar,
    Product,
    Records,
    Partner,
    Member,
    FootNav
  }
}

</script>

<style lang="sass">
$mblue: #1158A8
$mgreen: #65BDBC

body
  overflow-x: hidden
  margin: 0px

#metology-logo
  position: absolute;
  width: 80px;
  top: 20px;
  right: 20px;
</style>
