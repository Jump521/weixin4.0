<template>
  <!--左语音-->
  <div class="left audioLeft js-audio" @click="childAudio($event,msg)">
    <a href="javascript:;"><img class="headImg" :src="msg.headImage" alt=""></a>
    <p class="con audioLeft">
                <span class="auto-voice">
                    <img class="imgActive Ico co" src="../../../static/imgs/au3.png" alt="">
                    <img class="co" src="../../../static/imgs/au1.png" alt="">
                    <img class="co" src="../../../static/imgs/au2.png" alt="">
                </span>
      <audio class="audioPlay" :src="msg.sound.url"></audio>
    </p>
    <div class="red">
      <p :class="{shows:msg.fla}"></p>
      <span class="js-long">{{msg.sound.duration}}</span><b>"</b>
    </div>
  </div>
</template>
<script>
  import $ from "jquery";
    export default{
        data(){
            return {
                msg:this.leftSound
            }
        },
        props:['leftSound'],
        methods:{
          childAudio(data,msg){
            this.$emit("audio-play",data,msg);
          },
        }
    }
</script>
<style>

</style>
