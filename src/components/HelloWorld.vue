<template>
  <div class="hello">
    <header>
      <span class="head-img">
        <img alt="logo" src="../assets/alxlogo.png"/>
      </span>
      <span class="head-name">澳立新印刷</span>
    </header>

    <div class="swiper">
      <swiper :options="swiperOption" ref="mySwiper">
        <swiper-slide><img src="../assets/pic1.png" alt=""></swiper-slide>
        <swiper-slide><img src="../assets/swiper2.png" alt=""></swiper-slide>
        <swiper-slide><img src="../assets/production/swap3.png" alt=""></swiper-slide>
        <swiper-slide><img src="../assets/production/swap4.png" alt=""></swiper-slide>
      </swiper>
    </div>
    <div class="illustrate">
      <div class="bgImg"><img src="../assets/smoke.png"/></div>
      <h3>——————公司介绍——————</h3>
      <div class="pro">
        <div class="pro-item" @click="show(1)" :class="ind===1?'active':''">
          <i class="iconfont icon-factory"></i>
          <p>企业理念</p>
        </div>
        <div class="pro-item" @click="show(2)" :class="ind===2?'active':''">
          <i class="iconfont icon-bulbidealight"></i>
          <p>经营理念</p>
        </div>
        <div class="pro-item" @click="show(3)" :class="ind===3?'active':''">
          <i class="iconfont icon-wodetuandui"></i>
          <p>服务承诺</p>
        </div>
        
        <div class="pro-item" @click="show(4)" :class="ind===4?'active':''">
          <i class="iconfont icon-changjingguanli"></i>
          <p>团队管理</p>
        </div>
      </div>
      <div class="one" v-show="ind===1 && isShow">
        <p>✈&nbsp;&nbsp;没有最好，只有更好</p>
        <p>✈&nbsp;&nbsp;急客户所急，想客户所想</p>
        <p>✈&nbsp;&nbsp;追求双赢， 做到让您百分百满意、百分百放心</p>
      </div>
      <div class="two" v-show="ind===2 && isShow">
        <p>✈&nbsp;&nbsp;诚信合作，交友合作</p>
        <p>✈&nbsp;&nbsp;积极进取，不断创新</p>
        <p>✈&nbsp;&nbsp;用心服务，勇争一流</p>
      </div>
      <div class="three" v-show="ind===3 && isShow">
        <p>✈&nbsp;&nbsp;内容准确，编排美观，格式规范，字迹清晰</p>
        <p>✈&nbsp;&nbsp;保质保量，准时送货，三包售后</p>
        <p>✈&nbsp;&nbsp;设备种类丰富，可实现多种产品定制</p>
      </div>
      <div class="four" v-show="ind===4 && isShow">
        <p>本公司群英荟萃，精于印刷，有最敬业的后道加工技术人员。本团队敬业、创新、追求完美，步伐一致，时刻准备为客户提供完美的整体印刷方案为广大客户提供及时、完善的印刷技术服务。</p>
      </div>
    </div>
    <div class="production">
      <h3>——————产品介绍——————</h3>
      <ul>
        <li>
          <div><img alt="" src="../assets/production2.jpg"/></div>
          <div>彩色使用说明书</div>
        </li>
        <li>
          <div><img alt="" src="../assets/production1.jpg"/></div>
          <div>黑白使用说明书</div>
        </li>
        <li>
          <div><img alt="" src="../assets/production5.jpg"/></div>
          <div>精美硬纸贺卡</div>
        </li>
        <li>
          <div><img alt="" src="../assets/production3.jpg"/></div>
          <div>通知单/检查单/仓库领料单</div>
        </li>
        <li>
          <div><img alt="" src="../assets/production4.jpg"/></div>
          <div>通用病历</div>
        </li>
        <li>
          <div class="more">
            <span>······</span>
          </div>
        </li>
      </ul>
      <ul>
        <li style="width:100%">
          <p class="title-img">校园合作定制作业簿/写字簿</p>
        </li>
         <li>
          <div><img alt="" src="../assets/school1.jpg"/></div>
        </li>
         <li>
          <div><img alt="" src="../assets/school2.jpg"/></div>
        </li>
        <li>
          <div><img alt="" src="../assets/school3.jpg"/></div>
        </li>
        <li>
          <div><img alt="" src="../assets/school4.jpg"/></div>
        </li>
        <li>
          <div><img alt="" src="../assets/school5.jpg"/></div>
        </li>
        <li>
          <div><img alt="" src="../assets/school6.jpg"/></div>
        </li>
        <li>
          <div class="middle"></div>
        </li>
        <li>
          <div class="middle"></div>
        </li>
        <li style="width:100%">
          <p style="font-weight:600;"><span>······</span><span style="margin-left:0.7rem;">更多定制，等你决定!</span> </p>
        </li>
      </ul>
    </div>
    <div class="connection">
      <div class="item">
        <a href="tencent://message/?uin=724037534&Site=&Menu-=yes"><i class="iconfont icon-QQ"></i></a>
      </div>
      <div class="item">
        <i class="iconfont icon-weixin"></i>
        <a href="weixin://" class="linkwx">
          <img alt="qq" src="../assets/weChat.jpg" @click="bbb"/>
        </a>
        
      </div>
      <div class="item">
        <a href="tel:13534343514"><i class="iconfont icon-phone"></i></a>
      </div>
    </div>
    <footer>
      <div class="foot-logo"><img alt="logo" src="../assets/alxlogo.png"/></div>
      <div class="foot-con">
        <p class="name">澳立新印刷厂</p>
        <p><i class="iconfont icon-dizhi"></i>地址：广东省佛山市三水区芦苞镇芦湖路35-1号四合村委会白土村</p>
        <p><i class="iconfont icon-promise"></i>虚假赔偿 <i class="iconfont icon-promise"></i>欺诈赔偿</p>
        <p>© 2022 澳立新印刷厂</p>
      </div>
    </footer>
  </div>
</template>

<script>
import '../assets/font/iconfont.css'
// import CarouselContainer from '@/components/CarouselContainer'
import { Swiper, SwiperSlide } from 'swiper/vue';
import 'swiper/css';

export default {
  name: 'HelloWorld',
  data(){
    return{
      ind:1,
      isShow: true,
      list:[
        {name:"aaa"},
        {name:"bbb"},
        {name:"ccc"},
      ]
    }
  },
  components: {
      Swiper, SwiperSlide
  },
  mounted() {
    let self=this
    //延时模拟两次数据变化
    setTimeout(()=>{
      let obj={name:"ddd"}
      self.list.push(obj)
    },5000)
    setTimeout(()=>{
      let obj={name:"eee"}
      self.list[0].name="AAA"
      self.list.push(obj)
    },8000)
  },

  methods: {
    show(value){
      this.ind === value ? this.isShow = !this.isShow : this.isShow = true
      this.ind = value
    },
    bbb(){
      console.error("2222");
    }
  },

}
</script>

<style scoped lang="scss">
@font-face {
  font-family: 'fzstk';
  src: url(../assets/font/FZSTK.TTF);
}
body{
  margin: 0;
  padding: 0;
}
.hello{
  background: rgb(248, 246, 246);
  // background-image: url("../assets/world.png");
  // background-attachment: fixed;
  // background-size:  100%;
  width: 100%;
  top: 0;
  left: 0;
  bottom: 0;
}
header{
  width: 100%;
  height: 1.5rem;
  background: rgb(15, 76, 131);
  .head-img{
    height: 100%;
    float: left;
    margin-left: 00.2rem;
    margin-top: 00.1rem;
    img{
      height: 80%;
      float: left;
    }
  }
  .head-name{
    height: 1.5rem;
    float: left;
    font-size: 0.8rem;
    font-family: 'fzstk';
    font-weight: bold;
    color: white;
    line-height: 1.4rem;
    margin-left: 00.2rem;
  }
}

.swiper{
  width: 98%;
  height: 100%;
  margin: 0 auto;
  img{
    width: 100%;
  }
}

.illustrate{
  margin: 0.5rem auto;
  width: 95%;
  height: 6.8rem;
  background: #f0efef;
  border-radius: 00.2rem;
  font-size: 0.4rem;
  position: relative;
  .bgImg{
    position: absolute;
    width: 100%;
    z-index: 0;
    img{
      width: 100%;
    }
  }
  .pro{
    width: 100%;
    z-index: 1;
    position: absolute;
    .pro-item{
      // border: 1px solid rgb(175, 171, 171);
      float: left;
      width: 23%;
      margin-left: 00.1rem;
      i{ font-size: 1.3rem;}
    }
    .active{
      color: rgb(99,82,63);
      font-weight: bold;
    }
  }
  .one, .two, .three, .four{
    height: 3rem;
    width: 100%;
    text-align: left;
    position: absolute;
    border-bottom-left-radius: 0.2rem;
    border-bottom-right-radius: 0.2rem;
    bottom: 0;
    background: rgb(190, 192, 180);
    background-image: url("../assets/world.png");
    background-size: 40% 100%;
    background-position: right;
    background-repeat: no-repeat;
    p{ padding-left: 10px;}
  }
.four{
  text-indent: 2em;
}
 
}
.production{
  width: 95%;
  margin: 0.5rem auto;
  display: block;
  background: #f0efef;
  border-radius: 00.2rem;
  font-size: 00.4rem;
  ul,li{
    list-style: none;
		margin: 0;
		padding: 0;
		width: 100%;
  }
  ul{
    display: flex;
		flex-direction: row;
		flex-wrap: wrap;
		justify-content:space-between;
    li{
      width: calc(50% - 5px);
      margin: 5px 0;
      img{
        width: 90%;
        margin-bottom: 0.2rem;
      }
    }
  }
}
.connection{
  position: fixed;
  bottom: 30%;
  right: 4px;
  z-index: 10;
  color: white;
  .item{
    width: 1rem;
    height: 1rem;
    // background-color: rgb(15, 76, 131);
    background-color: rgb(190, 192, 180);
    border-radius: 00.5rem;
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
    margin-top: 00.5rem;
    i{font-size: 00.8rem;}
    img{
      position: absolute;
      z-index: -1;
      display: none;
      width: 3.5rem;
      height: 3.5rem;
    }
    .info{
      position: absolute;
      z-index: -1;
      display: none;
      width: 150px;
      height: 150px;
      background: #f0efef;
      color: black;
    }
    a{
      text-decoration: none;
      color: white;
    }
  }
  .item:hover{
    background: #f0efef;
    i{color: rgb(15, 76, 131);}
  }
  .item:hover img, .linkwx,  .info{  
    display: block;
    right: 1.2rem;
    top: -1rem;
  }
}
.more{
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100%;
  font-size: 1rem;
}

.title-img{
  width: 60%;
  margin: 0.8rem auto;
  font-size: 0.5rem;
  font-weight: bold;
  padding: 0.2rem 0.2rem 0.2rem;
  background: rgba(125,125,125,.4);
  border-radius: 0.6rem;
}
footer{
  margin-top: 00.5rem;
  height:4rem;
  width: 100%;
  background-color: rgb(15, 76, 131);
  color: white;
  .foot-logo, .foot-con{
    display: inline-block;
  }
  .foot-logo{
    width: 35%;
    img{
      width: 90%;
    }
  }
  .foot-con{
    width: 65%;
    font-size: 00.3rem;
    text-align: left;
    .name{
      font-size: 00.6rem;
      font-family: 'fzstk';
      font-weight: bold;
      margin-block-start: 0.6em;
      margin-block-end: 0.5em;
    }
  }

}
</style>
