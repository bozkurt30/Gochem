<template>
  <nav>
    <ul>
      <li v-for="nav in navItems" :key="nav.id">
        <a :href="nav.path"><i :class="nav.icon" />{{ nav.label }}</a>
      </li>
    </ul>
  </nav>
</template>
<script>
export default {
  data () {
    return {
      navItems: [
        {
          label: 'Anasayfa',
          path: '/home',
          icon: 'flaticon-sydney-opera-house'
        },
        {
          label: 'Hakkımızda',
          path: '/home',
          icon: 'flaticon-info'
        },
        {
          label: 'Ürünler',
          path: '/home',
          icon: 'flaticon-product'
        },
        {
          label: 'Sektörler',
          path: '/home',
          icon: 'flaticon-support'
        },
        {
          label: 'Belgeler',
          path: '/home',
          icon: 'flaticon-deal'
        },
        {
          label: 'Makaleler',
          path: '/home',
          icon: 'flaticon-content'
        },
        {
          label: 'İletişim',
          path: '/home',
          icon: 'flaticon-mail'
        }
      ]
    }
  }
}
/*
.flaticon-sydney-opera-house:before { content: "\f100"; }
.flaticon-contract:before { content: "\f101"; }
.flaticon-mail:before { content: "\f102"; }
.flaticon-support:before { content: "\f103"; }
.flaticon-info:before { content: "\f104"; }
.flaticon-content:before { content: "\f105"; }
.flaticon-pin:before { content: "\f106"; }
.flaticon-play-button:before { content: "\f107"; }
.flaticon-product:before { content: "\f108"; }
.flaticon-deal:before { content: "\f109"; }
*/
</script>
<style lang="less" scoped>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  text-align: center;
  padding-top: 1.4rem;

}

li {
  display: inline-block;
}

li a {
  font-size: .8rem;
  display: inline-block;
  color: white;
  text-align: center;
  padding: .5rem 1.2rem;
  text-decoration: none;
}

/* Change the link color to #111 (black) on hover */
li a:hover {
color: darkred;
 [class^="flaticon-"]:before{
color: darkred;
  }
}

li:not(:last-child) {
  border-right: 0.5px solid white;
}
[class^="flaticon-"]:before{

    font-size: .6rem;
    padding-right: .3rem;
    font-style: normal;
    margin-left: 0;
    color: white;
}
</style>
