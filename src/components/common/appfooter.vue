<template>
<footer>
<div class="header_wrap">
        <div class="footer-all clearfix">
            <!--  <div class="foot-l fl">
                  <img src="./images/logo.png" alt="智慧神州" title="智慧神州">
              </div>-->
            <div class="foot-c fl">
                <h3>企业信息</h3>
                <ul>
                    <li>公司名称：智慧神州信息技术有限公司</li>
                    <li>公司地址：北京市海淀区上地九街9号</li>
                    <li>联系电话：010-61853955</li>
                    <!--<li><a href="./contact.html" style="color:#fff;">关于我们</a></li>-->
                </ul>
            </div>
            <div class="foot-r fl">
                <h3>联系我们</h3>
                <div class="img-wei">
                    <img src="../../assets/erweima.jpg" title="公众号二维码">
                </div>
            </div>
        </div>
        <div class="copyright">
            <div class="center">
                <span class="smart">©版权所有 不得转载 智慧神州信息技术有限公司 2017</span>
                <span class="record">京ICP备15022251号-1</span>
            </div>
        </div>
    </div>
</footer>
</template>
<script>
export default {
  name: 'AppFooter',
  data () {
    return {}
  }
}
</script>
<style>
footer {
    border-top: 1px solid #aaa;
    background: #8f8f8f;
}

footer .footer-all {
    margin-top: 24px;
    margin-bottom: 24px;
}

/*
footer .footer-all .foot-l {
    width: 260px;
}

footer .footer-all .foot-l img {
    width: 150px;
}
*/

footer .footer-all .foot-c {
    margin-left: 227px;
    color:#fff;

}

footer .footer-all .foot-c h3 {
    font-size: 18px;
    font-weight: bold;
    color: #fff;
    text-align: center;
}

footer .footer-all .foot-c ul {
    font-size: 15px;
}

footer .footer-all .foot-c ul li {
    margin-top: 15px;
    color: #fff;
    line-height: 20px;
}

footer .footer-all .foot-r {
    margin-left: 240px;
}

footer .footer-all .foot-r h3 {
    font-size: 18px;
    font-weight: bold;
    color: #fff;
    text-align: center;
}

footer .footer-all .foot-r .img-wei {
    width: 100px;
    margin-top: 20px;
}

footer .footer-all .foot-r .img-wei img {
    width: 98px;
}

footer .copyright {
    border-top:1px solid #fff;
    padding: 10px 0;

    font-size: 14px;
    color: #fff;
   /* height: 44px;
    line-height: 44px;*/
   /* background: #eeeeee;*/
}

footer .copyright .center {
    margin-left: 227px;
}

footer .copyright .record {
    margin-left: 150px;
}
</style>
