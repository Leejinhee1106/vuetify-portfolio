<template>
    <v-container>
        <h2>뷰 이벤트</h2>
        <p>
        - 이벤트 처리는 지시문을 통해 이루어지므로 v-on을 사용합니다 <br/>
        </p>
        <hr class="my-4"/>
        <p>{{ "count" + count }}</p>
        <button v-on:click="count--">Count 감소</button>
        <v-btn v-on:click="count++" color="primary" variant="elevated">Count 증가</v-btn>
        <hr class="my-4"/>
        <v-row>
            <v-col cols="12" md="4">
                <div id="lightDiv">
                    <div v-show="lightOn"></div>
                    <img src="../../assets/img_lightBulb.svg">
                </div>
                <v-btn v-on:click="lightOn = !lightOn">Switch on/off</v-btn>
            </v-col>

            <v-col cols="12" md="4">
            <h2>Count Input Events</h2>
            <input type="text" v-on:input="inputCount++" placeholder="Start Writing..">
            <p>{{ inputCount }} input events occurred</p>
            </v-col>

            <v-col cols="12" md="4">
                <div class="color" 
                v-on:mousemove="colorVal = Math.floor(Math.random() * 360)"
                v-bind:style="{ backgroundColor: 'hsl(' + colorVal + ', 60%, 60%)' }">
                </div>
                <p>background-color : hsl(<strong>{{ colorVal }}</strong>)</p>
            </v-col>
        </v-row>
        <hr class="my-4"/>
    </v-container>
</template>

<script>
export default {
    data(){
        return{
            count:0,
            lightOn: false,
            inputCount: 0,
            colorVal:50,
        }
    }
}
</script>

<style>
#lightDiv{
    position: relative;
    width: 150px;
    height: 150px;
}
#lightDiv > img{
    position: relative;
    width: 100%;
    height: 100%;
}
#lightDiv > div{
    position: absolute;
    top: 10%;
    left: 10%;
    width: 80%;
    height: 80%;
    border-radius: 50%;
    background: yellow;
}
.color{
    width:200px;
    height: 80px;
}
</style>

