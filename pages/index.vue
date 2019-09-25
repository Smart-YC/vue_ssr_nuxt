<template>
  <div class="container">
    <div>
      <header>
        <div class="logo">LOGO</div>
        <Header/>
      </header>
      <!-- 第一屏 -->
      <div class="content">
        <div class="furniture">
          <img src="../assets/furniture.png" alt="">
        </div>
        <img src="../assets/1.png" alt="">
      </div>
      <!-- 第二屏 -->
      <div class="content-wrap">
        <div class="content2">
          <el-carousel height="80vh" direction="vertical" :autoplay="false">
            <el-carousel-item v-for="item in 3" :key="item">
              <div class="title-wrap text-right">
                <h1>产品</h1>
                <p>PRODUCT</p>
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
                    <h3>衣架</h3>
                    <p>其他</p>
                  </div>
                </el-col>
                <el-col :span="6">
                  <div class="text-center">
                    <img src="../assets/5.png" alt="">
                    <h3>衣架</h3>
                    <p>其他</p>
                  </div>
                </el-col>
                <el-col :span="6">
                  <div class="text-center">
                    <img src="../assets/6.png" alt="">
                    <h3>衣架</h3>
                    <p>其他</p>
                  </div>
                </el-col>
              </el-row>
            </el-carousel-item>
          </el-carousel>
        </div>
      </div>
      <!-- 第三屏 -->
      <div class="content-wrap">
        <div class="content2">
          <div class="title-wrap text-left">
            <h1>我们的优势</h1>
            <p>SUPERIORITY</p>
          </div>
          <el-row :gutter="5" class="goods">
            <el-col :span="6">
              <div class="text-center">
                <img src="../assets/7.png" alt="">
              </div>
            </el-col>
            <el-col :span="16" offset="2">
              <el-row :gutter="1" class="goods">
                <el-col :span="8">
                  <p>HIGH QUALITY</p>
                  <el-divider></el-divider>
                  <img src="../assets/8.png" alt="">
                  <h4>质优价廉产品</h4>
                  <p>为了得到大众的认可，我们的产品必须做到质优价廉，我们设计产品是</p>
                </el-col>
                <el-col :span="8">
                  <p>HIGH QUALITY</p>
                  <el-divider></el-divider>
                  <img src="../assets/10.png" alt="">
                </el-col>
                <el-col :span="8">
                  <p>HIGH QUALITY</p>
                  <el-divider></el-divider>
                  <img src="../assets/11.png" alt="">
                </el-col>
              </el-row>
            </el-col>
          </el-row>
        </div>
      </div>
      <!-- 第四屏 -->
      <div class="content-wrap">
        <div class="content2">
          <div class="title-wrap text-center">
            <h1>关于</h1>
            <p>ABOUT US</p>
          </div>
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
  header {
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    width: 1200px;
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
    overflow-x: hidden;
    background-color: #E6E7E9;
  }

  .content {
    position: relative;
    height: 100vh;
  }

  .content-wrap {
    background-color: #fff;
    margin: 0 auto;
    text-align: center;
  }

  .content2 {
    width: 1200px;
    padding: 150px 0;
    display: inline-block;
    text-align: left;
  }

  .title-wrap {
    margin-bottom: 100px;
  }

  .classify {
    margin-bottom: 100px;
  }

  .goods {
    margin-bottom: 30px;
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
    top: 170px;
    left: 0;
    width: 100%;
    text-align: center;
  }

  .el-carousel__item:nth-child(2n) {
    background-color: #fff;
  }

  .el-carousel__item:nth-child(2n+1) {
    background-color: #fff;
  }
</style>
