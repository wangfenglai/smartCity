<template>
<div id="fixed-dock">
    <div id="fiexd-bar">
      <ul>
          <li>
              <div class="flimg fli2">
                <div class="flc-zxkf">
                    <h5>联系我们</h5>
                    <div class="kefuzx shoqian">
                        <div class="sdibox sqlphone"><a href="javascript:void(0);" style="color:#fff;">010-61853955</a></div>
                    </div>
                </div>
              </div>
          </li>
          <li>
              <div class="flimg fli3">
                  <div class="flc-zxkf flc-zxkf1">
                      <h5>关注我们</h5>
                      <div><img src="../../assets/erweima.jpg" style="width:157px;height:157px;" alt=""></div>
                  </div>
              </div>
          </li>
          <li>
              <div class="flimg fli4" onclick="window.open('http://p.qiao.baidu.com/cps/chat?siteId=11681254&userId=22872480','_blank')"></div>
          </li>
          <li>
              <div class="flimg fli5 j_backtop" @click="backTop">
                  <p class="j_backtop"></p>
              </div>
          </li>
      </ul>
  </div>
</div>
  
</template>
<script>
import $ from 'jquery'
export default {
  name:"AppAside",
  data(){
      return{

      }
  },
  methods:{
      backTop(){
        //   alert(1);
        //点击事件获取当前的scrollTop
        const speed=1.2;
        var _this=this;
        var timer =setInterval(function(){
            _this.setScrolls(Math.floor(_this.getScrolls())/speed);
               if(_this.getScrolls()==0){
                   clearInterval(timer);
               } 
        },10)
      },
      getScrolls(){
          return document.documentElement.scrollTop || document.body.scrollTop
      },
      setScrolls(value){
          document.body.scrollTop=value;
          document.documentElement.scrollTop=value;
      },
  }
}
$(function(){
    $(".fli2").hover(function(){
         $(this).css({'background':"rgba(0,0,0,0.5) url("+require('../../assets/fl6.png')+ ") center no-repeat"});
          $(this).find('.flc-zxkf').stop().animate({'width':'130','height':'100','opacity':'1'},200);
    },function(){
        $(this).css({'background':"url("+require('../../assets/fl6.png')+ ") center no-repeat"});
        $(this).find('.flc-zxkf').stop().animate({'width':'0','height':'0','opacity':'0'},200);
    })
    $('.fli3').hover(function(){
        $(this).css({'background':"rgba(0,0,0,0.5) url("+require('../../assets/fl9.png')+ ") center no-repeat"});
        $(this).find('.flc-zxkf').stop().animate({'width':'240','height':'252','opacity':'1'},200);
    },function(){
        $(this).css({'background':"url("+require('../../assets/fl6.png')+ ") center no-repeat"});
        $(this).find('.flc-zxkf').stop().animate({'width':'0','height':'0','opacity':'0'},200);
    });
})
</script>
<style>
#fixed-dock{
    position:fixed;
    bottom:50%;
    right:0;
    z-index:999;
    height:326px;
    margin-bottom: -206px;
}
#fiexd-bar{
    width: 60px;
    background: rgba(0,0,0,0.4);
    border-radius:10px 0px 0px 10px;
    -webkit-transition: all .3s ease-in-out 0s;
    -moz-transition: all .3s ease-in-out 0s;
    -ms-transition: all .3s ease-in-out 0s;
    -o-transition: all .3s ease-in-out 0s;
    transition: all .3s ease-in-out 0s;
    position: absolute;
    right:0;
}
.fclose #fiexd-bar{
    right: -70px;
}
#fiexd-bar li{
    height: 60px;
    /*line-height: 60px;*/
}
.flimg {
    text-align: center;
    height: 60px;
    position: relative;
    cursor: pointer;
}
/*.fli1{
    background:url(../images/fl1.png) center no-repeat;
}*/
.fli2{
    background:url(../../assets/fl6.png) center no-repeat;
}
.fli3{
    background:url(../../assets/fl9.png) center no-repeat;
}
.fli4{
    background:url(../../assets/fl8.png) center no-repeat;
}
.fli5{
    background:url(../../assets/fl7.png) center 20% no-repeat;
}
.fli5 p{
    color: #fff;font-size: 12px;
    padding-top: 40px;
}
.flc-zxkf{
    width: 0px;
    height: 0px;
    background:rgba(0,0,0,0.4);
    border-radius:10px;
    position: absolute;
    right:61px;
    top: 0;
    opacity: 0;
}
.kefuzx{
    height: 90px;
}
.kefuzx1{
    height: 60px;
}
.flc-zxkf h5{
    font-size: 18px;
    color: #fff;
    text-align: center;
    font-weight: 500;
    height: 60px;
    line-height: 60px;
}
.zxbox{
    display:block;
    height:60px;
    line-height: 60px;
    color: #fff;
    font-size:16px;
    padding-left:20%;
}
</style>
