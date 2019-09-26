<template>
  <div class="container">
    <div>
      <div class="nav">
        <header >
          <div class="logo">LOGO</div>
          <Header/>
        </header>
      </div>
      <!-- 第一屏 -->
      <div class="content" id="main">
        <div class="furniture">
          <img src="../assets/furniture.png" alt="">
        </div>
        <img src="../assets/1.png" width="100%" alt="">
      </div>
      <!-- 第二屏 -->
      <div class="content-wrap" id="product">
        <div class="content2">
          <el-carousel height="100vh" direction="vertical" :autoplay="false">
            <el-carousel-item v-for="item in 3" :key="item">
              <div class="title-wrap text-right">
                <h1>产品</h1>
                <p>PRODUCT</p>
                <hr>
              </div>
              <el-row class="classify">
                <el-button size="medium">家具</el-button>
                <el-button size="medium">装饰</el-button>
                <el-button size="medium">橘子</el-button>
                <el-button size="medium">其他</el-button>
                <el-button size="medium" class="black-btn">MORE</el-button>
              </el-row>
              <el-row :gutter="20" class="goods">
                <el-col :span="6">
                  <div class="text-center">
                    <img src="../assets/3.png" alt="">
                    <h3>衣架</h3>
                    <p>其他</p>
                  </div>
                </el-col>
                <el-col :span="6">
                  <div class="text-center">
                    <img src="../assets/4.png" alt="">
                    <h3>吊灯</h3>
                    <p>其他</p>
                  </div>
                </el-col>
                <el-col :span="6">
                  <div class="text-center">
                    <img src="../assets/5.png" alt="">
                    <h3>台灯</h3>
                    <p>其他</p>
                  </div>
                </el-col>
                <el-col :span="6">
                  <div class="text-center">
                    <img src="../assets/6.png" alt="">
                    <h3>凳子</h3>
                    <p>其他</p>
                  </div>
                </el-col>
              </el-row>
            </el-carousel-item>
          </el-carousel>
        </div>
      </div>
      <!-- 第三屏 -->
      <div class="content-wrap" id="news">
        <div class="content2">
          <div class="title-wrap text-left">
            <h1>我们的优势</h1>
            <p>SUPERIORITY</p>
            <hr>
          </div>
          <el-row :gutter="5" class="goods">
            <el-col :span="6">
              <div class="text-center">
                <img src="../assets/7.png" alt="">
              </div>
            </el-col>
            <el-col :span="16" :offset="2">
              <el-row :gutter="1" class="goods">
                <el-col :span="8">
                  <p>HIGH QUALITY</p>
                  <el-divider></el-divider>
                  <img src="../assets/8.png" alt="">
                  <h4>质优价廉产品</h4>
                  <p class="describe">为了得到大众的认可，我们的产品必须做到质优价廉，我们设计产品时，始终将顾客的需求放在心里。</p>
                  <img style="margin-bottom: 5px" src="../assets/9.png" alt="">
                </el-col>
                <el-col :span="8">
                  <p>HIGH QUALITY</p>
                  <el-divider></el-divider>
                  <img src="../assets/10.png" alt="">
                  <h4>益于人类，益于地球</h4>
                  <p class="describe">我们持续发展壮大的同时，致力于对地球家园和大众带来全面的积极影响。</p>
                  <img style="margin-bottom: 5px" src="../assets/9.png" alt="">
                </el-col>
                <el-col :span="8">
                  <p>HIGH QUALITY</p>
                  <el-divider></el-divider>
                  <img src="../assets/11.png" alt="">
                  <h4>某某与员工共同成长</h4>
                  <p class="describe">员工是我们持续发展的关键，我们把每个人都当成有发展潜力的人才。</p>
                  <img style="margin-bottom: 5px" src="../assets/9.png" alt="">
                </el-col>
              </el-row>
              <h4>企业愿景和经营理念</h4>
              <p>“为大众创造更加美好的日常生活”，这是宜家的愿景。我们的经营理念是“提供种类繁多、美观实用、老百
                姓买得起的家居用品”。通过优化我们的整个价值链，与供应商建立长期合作关系，投资高度自动化和大规模
                生产等方式，我们努力为顾客提供物美价优的产品。我们的愿景不局限于家居装饰。我们希望通过努力，为大
                众创造更美好的日常生活。​​
              </p>
            </el-col>
          </el-row>
          <div class="superiority">
            <img src="../assets/superiority.png" alt="">
          </div>
        </div>
      </div>
      <!-- 第四屏 -->
      <div class="content-wrap" id="about">
        <img src="../assets/12.png" width="100%" alt="">
        <div class="title-wrap text-center" style="position: absolute;top: 80px;left: 48%">
          <h1>关于</h1>
          <p>ABOUT US</p>
          <hr>
        </div>
        <div style="position: absolute;top: 200px;left: 55%;width: 23%">
          <h3>FURNITUR</h3>
          <br>
          <p style="line-height: 25px">自创立以来，伴随改革开放，历经市场洗礼，家居和中国家具产业的发
            已经不可同日而语，但是这个愿景始终未变，而且日益增强。追，
            精益制造，设计时尚，品牌翘楚，是我们各项工作的出发点，表明浪度
            握了家居产业的本质而不会偏离发展方向；对行业和消费者有价值，是
            们工作的核心，表明浪度一贯负责任的发展方式，这是浪度的企业社会
            任，也是浪度不断与时俱进，推动中国家具工业转型升级的源动力。
            当前家居行业正在面临一场巨变：互联网深入行业，信息进入网络传播
            消费者主权高企，审美风格日益多元。作为家居业的从业者和领先者，
            度深知面对互联网的变革趋势，正确的态度是在把握家居行业本质的基
            上，掌握互联网的技术手段，改变自己，拥抱变革，激情转型，协同共
            2014年，浪度进入转型期，为3-5年上市的战略目标进行全面的梳理和
            统的效率提升，依托16载对行业深刻理解和中国驰名商标的品牌实力，浪
            度对家居行业的发展方向越来越清晰，对自身的变革越来越有信心。
            对家居行业我们充满信心，对振兴中国家具工业我们充满斗志。但我们也
            深知未来之路不会一帆风顺，浪度将继续与员工、供应商、消费者等利益
            相关方携手，相互支持，同舟共济，担负引领中国家居行业转型升级的重
            担，一起为中国家具享誉世界而努力奋斗！</p>
          <br><br>
          <el-button class="black-btn" size="medium">查看更多</el-button>
        </div>
      </div>
      <!-- 第五屏 -->
      <div class="content-wrap" id="relation">
        <img src="../assets/13.png" width="100%" alt="">
        <div class="title-wrap text-right" style="position: absolute;top: 80px;right: 20%">
          <h1>留言</h1>
          <p>MESSAGE</p>
          <hr>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  import Logo from '~/components/Logo.vue'
  import Header from '~/components/Header.vue'

  export default {
    components: {
      Logo, Header
    }
  }
</script>

<style>
  .nav{
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    z-index: 9989;
    box-sizing: border-box;
    background-color: #E6E7E9;
  }
  header {
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    height: 60px;
    width: 1200px;
  }

  hr {
    width: 30px;
    border: grey 1px solid;
    display: inline-block;
  }

  h4 {
    color: #47494e;
    font-weight: normal;
    font-size: 16px;
    line-height: 30px;
  }

  p {
    font-size: 14px;
    line-height: 20px;
    color: grey;
  }

  .text-center {
    text-align: center;
  }

  .text-left {
    text-align: left;
  }

  .text-right {
    text-align: right;
  }

  .logo {
    font-size: 20px;
    line-height: 60px;
  }

  .container {
    margin: 0 auto;
    overflow: hidden;
    background-color: #E6E7E9;
  }

  .content {
    position: relative;
    height: 100vh;
  }

  .content > img {
    margin-top: 50px;
  }

  .content-wrap {
    background-color: #fff;
    margin: 0 auto;
    text-align: center;
    height: 100vh;
    padding-top: 60px;
    position: relative;
  }

  .content2 {
    width: 1200px;
    display: inline-block;
    text-align: left;
  }

  .title-wrap {
    margin-bottom: 100px;
  }

  .classify {
    margin-bottom: 100px;
  }

  .goods img {
    margin-bottom: 30px;
  }

  .goods h3 {
    margin-bottom: 15px;
  }

  .black-btn {
    background-color: #000;
    color: #fff;
  }

  .furniture {
    position: absolute;
    top: 180px;
    left: 0;
    width: 100%;
    text-align: center;
  }

  .superiority {
    position: absolute;
    top: 300px;
    left: 15%;
    width: 100%;
  }

  .describe {
    height: 64px;
  }

  .el-carousel__item:nth-child(2n) {
    background-color: #fff;
  }

  .el-carousel__item:nth-child(2n+1) {
    background-color: #fff;
  }
</style>
