<template>
  <v-app :style="back">
    <div style="margin-right: 75%;margin-top: 5%" >
    <router-link  to="/GotoFloor">
      <img src="../../../static/icon/教室图标.png" height="60" width="60"/>
    </router-link>
    </div>


    <div style="margin-left: 75%;margin-top: -13%" >
    <router-link  to="/Personal">
      <img src="../../../static/icon/主地图图标.png" height="50" width="50"/>
    </router-link>

    </div>
    
    <h3>	
        <input v-model="message" placeholder="60">
    </h3>
    

    <div style="margin-right: 0%;margin-top: 124%" >     
    <router-link  to="/GotoClass">
      <img src="../../../static/icon/确认按钮.png" height="50" width="223"/>
    </router-link>
    </div>

    </v-app>
</template>



<script>
    export default {
        
        data() {
            return {
                back: {
                    backgroundImage: "url(" + require("../../../static/picture/画板.png") + ")",
                    backgroundRepeat: "no-repeat",
                    backgroundSize: "100% 100% ",
                    backgroundPosition: "fixed",
                    height:"100% " ,
                    width: "100%",
                },
            }
        },
    }
</script>


<style>
h3
{
	position:absolute;
	left:140px;
	top:325px;
	color:rgb(10, 10, 10);
}
	
</style>
