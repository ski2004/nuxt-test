<template>
  <div class="header-menu-box">
    <div class="header-inner">
      <h1>與您打造不同的網路夢 - xxx互動網頁設計</h1>
      <a href="https://www.menai.com.tw" class="logo">
        <img
          src="https://www.menai.com.tw/images/header/menai_logo.png"
          height="50"
          width="250"
          alt="xxx互動網頁設計"
        />
      </a>
      <!-- <a href="javascript:void(0)" class="btn-menu"></a> -->
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarHeader" aria-controls="navbarHeader" aria-expanded="true" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <nav id="navbarHeader" class="header-menu">
        <header>
          <h2>設計主選單</h2>
        </header>
        <div class="logo-mobile">
          <a href="https://www.menai.com.tw">
            <img
              src="https://www.menai.com.tw/images/header/menai_logo.png"
              height="50"
              width="250"
              alt="xxx互動網頁設計"
            />
          </a>
        </div>
        <ul class="clearfix">
          <li>
            <a href="https://www.menai.com.tw/about">
              認識我們
              <span></span>
            </a>
          </li>
          <li>
            <a href="https://www.menai.com.tw/service">
              服務項目
              <span></span>
            </a>
          </li>
          <li class="hide">
            <a href="https://www.menai.com.tw/project">
              設計案例
              <span></span>
            </a>
          </li>
          <li>
            <a href="https://www.menai.com.tw/article">
              設計 X 狂想
              <span></span>
            </a>
          </li>
          <li>
            <a href="https://www.menai.com.tw/contact">
              詢價/聯絡
              <span></span>
            </a>
          </li>
        </ul>
        <div class="btn-box">
          <a href="javascript:void(0)" class="btn-menu-close"></a>
        </div>
      </nav>
      <!-- end header-menu -->
    </div>
    <!-- end header-inner -->
  </div>
</template>
<style>
/*--header--*/
.header-menu-box {
  width: 100%;
  position: relative;
}

.header-menu-box .header-inner {
  width: 1200px;
  position: absolute;
  left: 50%;
  margin-left: -600px;
  z-index: 999;
}

.header-menu-box .header-inner h1 {
  display: none;
}

.header-menu-box .header-inner a.logo {
  float: left;
  display: block;
  width: 250px;
  height: 50px;
  margin: 43px 0 0 0;
}

.header-menu-box .header-inner .header-menu {
  float: right;
}

.header-menu-box .header-inner .header-menu header {
  display: none;
}

.header-menu-box .header-inner .header-menu .logo-mobile {
  display: none;
}

.header-menu-box .header-inner .header-menu ul li {
  float: left;
  margin: 57px 0 0 32px;
}

.header-menu-box .header-inner .header-menu ul li a {
  display: block;
  color: #fff;
  font-size: 1em;
}

.header-menu-box .header-inner .header-menu ul li a:hover span {
  opacity: 1;
  margin: 12px 0 0 0;
}

.header-menu-box .header-inner .header-menu ul li a span {
  display: block;
  width: 100%;
  height: 1px;
  opacity: 0;
  background: #fff;
  margin: 5px 0 0 0;
  transition: all 0.3s linear;
}

.header-menu-box-clone {
  width: 100%;
  height: 65px;
  position: fixed;
  z-index: 9999;
  background: rgba(0, 0, 0, 0.75);
  top: -65px;
  transition: all 0.3s linear;
}

.header-menu-box-clone .header-inner {
  width: 1200px;
  height: 65px;
  margin: 0 auto;
}

.header-menu-box-clone .header-inner h1 {
  display: none;
}

.header-menu-box-clone .header-inner a.logo {
  float: left;
  width: 175px;
  height: 35px;
  margin: 15px 0 0 0;
}

.header-menu-box-clone .header-inner a.logo img {
  width: 100%;
  height: auto;
}

.header-menu-box-clone .header-inner .header-menu {
  float: right;
}

.header-menu-box-clone .header-inner .header-menu header {
  display: none;
}

.header-menu-box-clone .header-inner .header-menu .logo-mobile {
  display: none;
}

.header-menu-box-clone .header-inner .header-menu ul li {
  float: left;
  margin: 20px 0 0 32px;
}

.header-menu-box-clone .header-inner .header-menu ul li a {
  display: block;
  color: #bababa;
  font-size: 0.875em;
  transition: all 0.5s ease;
}

.header-menu-box-clone .header-inner .header-menu ul li a:hover {
  color: #fff;
}

.header-menu-box-clone .header-inner .header-menu ul li a span {
  display: none;
}

.header-menu-box-clone.visible {
  top: 0;
}

@media screen and (max-width: 970px) {
  /*--header--*/
  .header-menu-box {
    width: 100%;
    position: relative;
  }
  .header-menu-box .header-inner {
    width: 100%;
    position: absolute;
    left: 0;
    margin-left: 0;
    z-index: 999;
  }
  .header-menu-box .header-inner h1 {
    display: none;
  }
  .header-menu-box .header-inner a.logo {
    float: none;
    display: block;
    width: 300px;
    height: 46px;
    margin: 70px auto 0 auto;
  }
  .header-menu-box .header-inner a.logo img {
    width: 100%;
    height: auto;
  }
  .header-menu-box .header-inner .btn-menu {
    display: block;
    position: absolute;
    top: 70px;
    right: 20px;
    width: 50px;
    height: 50px;
    /* // background: url("../images/header/btn_menu.png") no-repeat; */
    background-size: 50px 50px;
  }
  .header-menu-box .header-inner .header-menu {
    float: none;
    display: none;
    position: fixed;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    background: rgba(0, 0, 0, 0.9);
  }
  .header-menu-box .header-inner .header-menu header {
    display: none;
  }
  .header-menu-box .header-inner .header-menu .logo-mobile {
    display: block;
    width: 300px;
    margin: 70px auto 80px;
  }
  .header-menu-box .header-inner .header-menu .logo-mobile img {
    width: 100%;
    height: auto;
  }
  .header-menu-box .header-inner .header-menu .btn-menu-close {
    display: inline-block;
    width: 20px;
    height: 20px;
    padding: 15px;
    /* background: url("../images/header/btn_close.png") no-repeat center center; */
    background-size: 20px 20px;
    border: 1px solid #fff;
    border-radius: 50%;
  }
  .header-menu-box .header-inner .header-menu ul li {
    float: left;
    width: 100%;
    text-align: center;
    margin: 0 0 65px 0;
  }
  .header-menu-box .header-inner .header-menu ul li a {
    display: block;
    color: #bababa;
    font-size: 1.5em;
    transition: all 0.5s ease;
  }
  .header-menu-box .header-inner .header-menu ul li a:hover {
    color: #fff;
  }
  .header-menu-box .header-inner .header-menu ul li a span {
    display: none;
  }
}
</style>
