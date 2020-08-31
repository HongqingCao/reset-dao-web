<template>
<div class="navbar-warpper">
  <nav class="navbar navbar-expand-md navbar-dark navbar-transparent fixed-top sticky-navigation" id="calay-navbar">
      <a class="navbar-brand" href="index.html">
        <img src="@/assets/logo.png"/>
      </a>
      <button class="navbar-toggler navbar-toggler-right text-white" type="button" data-toggle="collapse" 
              data-target="#navbarCollapse" aria-controls="navbarCollapse" aria-expanded="false" aria-label="Toggle navigation">
          <span data-feather="grid"></span>
          <span class="icon-bar"></span>
         <span class="icon-bar"></span>
         <span class="icon-bar"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarCollapse">
          <ul class="navbar-nav ml-auto">
              <li class="nav-item" v-for="item in navList" :key="item.id">
                  <a class="nav-link page-scroll" :class="{'active': isActive==item.id}">{{ item.title }}</a>
              </li>
              <li class="nav-item lan-item">
                <a class="nav-link lan" :class="{'active': lanIsActive=='EN'}">EN</a>
                <a class="nav-link lan" :class="{'active': lanIsActive=='CN'}">CN</a>
              </li>
          </ul>
      </div>
  </nav>
</div>
    
</template>
<script>
export default {
  name:'navbar',
  data() {
    return {
      isActive:'gov',
      lanIsActive:'EN',
      navList:[
        {id:'gov', title:' GOV', ref:''},
        {id:'projects', title:'PROJECTS', ref:''},
        {id:'community', title:'COMMUNITY', ref:''},
        {id:'Web3', title:'(Connect Web3)', ref:''}
      ]
    }
  }
}
</script>
<style lang="scss">
.navbar-warpper {
  .navbar {
    height:110px; 
    background-color: rgb(521,32,59);

    .navbar-nav {
      li {
        padding: 8px;
        .nav-link {
          color: white;
          padding: 8px 22px 8px 22px;
          border-radius: 22px;
          font-size: 14px;
          
          &.active {
          background-color: #e31d33;
          }
          &:hover {
            background-color: #e31d33;
          }
        }
        &.lan-item {
          padding-left: 90px;
          .lan {
            color: white;
            float: left;
            font-size: 14px;
            padding: 8px;
            border-radius: 0;
            margin-right: 5px;
            &.active {
              background-color: #e31d33;
            }
          }
        }
      }
    }
  }
}
</style>