<template>
  <div class="header" id="header">
        <div class="header_wrap">
            <div class="clearfix head-top">
                <div class="head-l fl">
                    <img alt="智慧神州" src="../../assets/logo.png">
                </div>
                <div class="fl head-r">
                    <ul>
                         <li><a class="active" href="#">首页</a></li>
                        <li><a href="#trade">商标</a></li>
                        <li><a href="#ban">版权</a></li>
                        <li><a href="#zhuan">专利</a></li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'AppHeader',
  data () {
    return {

    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

/*头部导航*/
.header {
    height: 75px;
    background: #fff;
    position: relative;
    width: 100%;
    box-shadow:0 1px 10px #ddd;
}

.header .head-top {

}

.header .head-top .head-l {
    margin-top: 8px;
}

.header .head-top .head-l img {
    /*width: ;*/
    height: 59px;
}

.header .head-top .head-r {
    margin-left: 334px;

}

.header .head-top .head-r ul li {
    float: left;
    margin-right: 72px;
}

.header .head-top .head-r ul li a {
    color: #333;
    font-size: 18px;
    line-height: 75px;

}

.header .head-top .head-r ul li a.active {
    color: #00b49d;
}

.header .logo_img {
    margin-top: 8px;
}
</style>
