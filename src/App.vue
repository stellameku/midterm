<template>
  <div id="app">
    <div class="topnav">
      <img src = "./assets/nthulogo.png" width = "50" height="50">
      <span >國立清華大學藝術學院</span>
      
      <el-menu :default-active="activeIndex" class="el-menu-demo" 
      mode="horizontal" @select="handleSelect " background-color="#7D0BA5" text-color="#fff" active-text-color="#fff">
  <el-menu-item index="1">HOME</el-menu-item>
  <el-submenu index="2">
    <template slot="title">關於學院</template>
    <el-menu-item index="2-1">學院簡介</el-menu-item>
    <el-menu-item index="2-2">未來展望</el-menu-item>
    <el-menu-item index="2-3">姐妹學校</el-menu-item>
    <el-submenu index="2-4">
      <template slot="title">招生資訊</template>
      <el-menu-item index="2-4-1">學院學士班</el-menu-item>
      <el-menu-item index="2-4-2">音樂系</el-menu-item>
      <el-menu-item index="2-4-3">藝設系</el-menu-item>
    </el-submenu>
  </el-submenu>
  <el-menu-item index="3" >師資</el-menu-item>
  <el-menu-item index="4" >藝術學報</el-menu-item>
  <el-menu-item index="5" >聯絡</el-menu-item>

</el-menu>
  </div>

    <div class="circle"></div> 
    <div class="circle2"></div> 
   

   <div class="section"> 
      <div class="block">
        <el-carousel trigger="click" height="500px">
          <el-carousel-item >
            <img src="./assets/img1.png" width = 100%  height=100%>
          </el-carousel-item>
          <el-carousel-item class="p">
            <img src="./assets/kotak2.png" width = 100%  height=100%>
          </el-carousel-item>

          <el-carousel-item class="p">
            <img src="./assets/img3.png" width = 100%  height=100%>
          </el-carousel-item>
        </el-carousel>
      </div>

     <div class="words">
      <h2>關於學院</h2>
      <br><br>
      <p>本院稟持著「美學博雅、創藝美緻」的美育精神，培養優秀的美術創作、工藝設計、音樂表演、音樂理論教育以及科技藝術跨域創作人才為宗旨，人才兼具藝術賞析與創作能力，且善盡社會責任，共同把美感、創意帶入清華生活，在清華創造音樂心靈饗宴，開創科技藝術跨域DNA，期望未來能成為台灣「藝術領航者」與「藝術跨域工作者」</p>     
      </div>
     <br><br><br><br><br><br>
     <div class="news">
       <h2>最新訊息</h2>
       <br><br>
      <div class="row">
        <div class="column1">
          <div class="kotak3">
            <img src="./assets/kotak1.jpg" width="100%" height="100%"><br>
            <p>國際跨領域學術論壇  </p><br><br><br>
            <el-button>Read More</el-button>
          </div>        
        </div>

        <div class="column1">
          <div class="kotak3">
            <img src="./assets/kotak2.png" width="100%" height="100%"><br>
            <p>華山烏梅劇場「Face to face」</p><br><br><br>
            <el-button>Read More</el-button>
          </div>        
        </div>
      </div><br><br><br><br><br><br><br><br>

      <div class="row">
        <div class="column">
          <div class="kotak3">
            <img src="./assets/kotak3.jpg" width="100%" height="100%"><br>
            <p>會議日期：2020年12月3日  </p><br><br><br>
            <el-button>Read More</el-button>
          </div>        
        </div>
  
        <div class="column">
          <div class="kotak3">
            <img src="./assets/kotak4.jpg" width="100%" height="100%"><br>
            <p>主旨:本校《清華藝術學報》</p><br><br><br>
            <el-button>Read More</el-button>      
          </div>
        </div>

        <div class="column">
          <div class="kotak3">
            <img src="./assets/kotak5.jpg" width="100%" height="100%"><br>
            <p>【獲獎】《那顆Ｇ1咻！》</p><br><br><br>
            <el-button>Read More</el-button>      
          </div>       
        </div>
      </div><br><br><br><br><br><br><br><br>

      <div class="row">
          <h2>學院相關網站</h2><br><br><br><br><br>
          <div class="column1">
            <div class="kotakTua">
            <div class="kotakBawah">
              <div class="column">
                <img src="./assets/left1.jpg" width="120px" height="120px"><br>
              </div>
              <div class="column">
                <img src="./assets/left2.jpg" width="120px" height="120px"><br>
              </div>
              <div class="column">
                <img src="./assets/left3.jpg" width="120px" height="120px"><br>
              </div>
            </div> 
            </div>
            </div>
             
            <br><br><br><br><br><br>
            <div class="column1">
            <div class="kotakSdg">
            <div class="kotakBawah">
              <div class="column">
                <img src="./assets/right1.jpg" width="120px" height="120px"><br>
              </div>
              <div class="column">
                <img src="./assets/right2.jpg" width="120px" height="120px"><br>
              </div>
              <div class="column">
                <img src="./assets/right3.jpg" width="120px" height="120px"><br>
              </div>
            </div> 
            </div> 


              
            </div>       
          </div>

        </div>
   </div>
   <br><br><br><br><br><br><br><br>
   <div class="footer">
    <p>Made by <span style="color:#7D0BA5">AiBao-Lin</span> ,2020</p>
 
  </div>
  </div>
  
  



</template>

<script>
export default {
    data() {
      return {
        activeIndex: '1',
        activeIndex2: '1'
      };
    },
    methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      }
    }
  }
</script>

<style lang="sass">

*
  margin: 0
  box-sizing: border-box
  font-family: "San Fransisco UI"

.el-menu
  float: right

.el-carousel__item
  h3
    color: #475669
    font-size: 14px
    opacity: 0.75
    line-height: 150px
    margin: 0

  &:nth-child(2n)
    background-color: #99a9bf

  &:nth-child(2n+1)
    background-color: #d3dce6
  
.el-button
  letter-spacing: 2px
  font-size: 12px
  font-family: "San Fransisco UI"


.circle
  position: absolute
  width: 500px
  height: 500px
  left: -280px
  top: 650px
  background-color: #F4D6FF
  z-index: -1
  border-radius: 100%

.circle2
  position: absolute
  width: 225px
  height: 450px
  top: 1200px
  right: 0px
  background-color: #9837BA
  z-index: -1
  border-bottom-left-radius: 450px
  border-top-left-radius: 450px


.section
  text-align: center
  letter-spacing: 7px


.column
  float: left
  width: 33.33%

.column1
  float: left
  width: 50%
  

/* Clear floats after the columns

.row:after
  content: ""
  display: table
  clear: both

/* Responsive layout - makes the three columns stack on top of each other instead of next to each other
@media screen and (max-width: 600px)
  .column, .column1
    width: 100%

.kotak3
  margin: 25px
  text-align: center

  p
    margin: 25px

  
.kotakSdg
  background-color: #D8B3E5
  width: 444px
  height: 250px
  float: right

  .kotakBawah
    position: relative
    right: 20px
  
.news 
  h2
    color: #7D0BA5

  p
  color: #857878


  .kotakBawah
    background-color: #FDF5FF
    width: 400px
    height: 150px
    margin: 120px
    position: absolute  

    .column
      img
        padding: 25px;
   


  .kotakTua
    background-color: #7D0BA5
    overflow: visible
    width: 444px
    height: 250px
    position: relative
  

  .kotak3
    background-color: #FDF5FF

.words
  
  p
  padding: 40px
  color: #857878

  h2
    color: #7D0BA5
  

.section
  

  span
    color: #7D0BA5
    font-size: 100%

  img
    vertical-align: middle
    float: right
  
  

/* Add a color background color to the top navigation

.topnav
  background-color: #7D0BA5
  overflow: hidden
  letter-spacing: 5px
  height: 15%
  font-size: Large

  img
    vertical-align: middle
    margin: 5px

  span
    font-size: 150%
    color: white

  a
    float: right
    color: #fff
    text-align: center
    padding: 14px 16px
    text-decoration: none
    font-size: 14px
    letter-spacing: 2px

    &:hover
      background-color: #F4D6FF
      color: black

.footer 
  height: 15vh;
  width: 100%;
  background-color: #E9CCF3;
  letter-spacing: 5px
  text-align: center
  padding: 30px
  
  p
    color: white



/* Style the links inside the navigation bar

/* Change the color of links on hover



</style>
