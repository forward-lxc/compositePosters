<template>
  <div id="appindex">
    <div class="viewWrap">
      <router-view></router-view>
    </div>
  </div>
</template>

<script>

export default {
  name: 'app',
  data () {
    return {
    }
  },
  methods:{
        // TimeDown(id, endDateStr) {
        //     //结束时间
        //     var endDate = new Date(endDateStr);
        //     //当前时间
        //     var nowDate = new Date();
        //     //相差的总秒数
        //     var totalSeconds = parseInt((endDate - nowDate) / 1000);
        //     //天数
        //     var days = Math.floor(totalSeconds / (60 * 60 * 24));
        //     //取模（余数）
        //     var modulo = totalSeconds % (60 * 60 * 24);
        //     //小时数
        //     var hours = Math.floor(modulo / (60 * 60));
        //     modulo = modulo % (60 * 60);
        //     //分钟
        //     var minutes = Math.floor(modulo / 60);
        //     //秒
        //     var seconds = modulo % 60;
        //     console.log("距结束：" + days + "天" + hours + ":" + minutes + ":" + seconds + "")
        //     //输出到页面
        //     // document.getElementById(id).innerHTML = "距结束：" + days + "天" + hours + ":" + minutes + ":" + seconds + "";
        //     //延迟一秒执行自己
        //     //setTimeout(function () {
        //     //    TimeDown(id, endDateStr);
        //     //}, 1000)
        // }
        },
        mounted(){
          // setInterval(()=>{
          //   this.TimeDown(1,"2019/08/14 23:00:00")
          // },1000)
          
        }
}
</script>

<style lang="stylus" src="STYLUS/main.styl"></style>

<style lang="stylus">
#appindex
  min-width: 1180px
  .viewWrap
    background-color: $color-white
    min-height: calc(110vh - 110px)
    min-width: 1170px
.fade-enter-active, .fade-leave-active
  transition: opacity .3s
.fade-enter, .fade-leave-to
  opacity: 0
</style>
