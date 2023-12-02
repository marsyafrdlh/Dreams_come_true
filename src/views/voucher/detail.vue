<template>
    <div>
        <div class="container">
            <div class="row">
                <div class="mr40 mt20">
                    <router-link to="/list-voucher">
                        <img src="../../assets/icons/back.svg">
                    </router-link>
                </div>
                <div>
                    <h1 class="m0">Detail Voucher</h1>
                    <p class="mt5 mb20 tc-green">Your voucher details</p>
                </div>
            </div>
            <hr class="uline-grey">
            <div class="mt50 right">
                <img :src="urlImg" width="50%">
                <div class="mp ">
                    <p class="mp abu">CERIA3</p>
                    <h2 class="mp">BOMBASTIS 11.11</h2>
                    <p class="detail-title-bold mp">Voucher Description</p>
                    <P class="mp abu desk">Lorem ipsum dolor sit amet consectetur adipisicing elit. Rem, deleniti alias impedit debitis voluptatem eligendi itaque ea inventore magni adipisci aperiam eius, nemo esse distinctio porro! Rerum error harum quos maiores, molestiae ea inventore? Porro veritatis voluptatem velit nam magni necessitatibus explicabo? Asperiores rem aspernatur pariatur excepturi quisquam et numquam.</P>
                    
                    <div class="container">
                        <div class="in">
                            <p class="detail-title-bold space">Voucher Category : </p>
                            <p class="abu">CERIA3</p>
                        </div>
                        <div class="in">
                            <p class="detail-title-bold space">Min Transaction : </p>
                            <p class="abu">Rp 50.000</p>
                        </div>
                        <div class="in">
                            <p class="detail-title-bold space">Amount : </p>
                            <p class="abu">Rp 15.000</p>
                        </div>
                    </div>
                </div>
            </div>

            <div class="exp">
                <div class="container2">
                    <p class="detail-title-bold">Voucher Status</p>
                    <hr class="tebal">
                    <label class="label-green c">Activae</label>
                </div>
                <div class="container2">
                    <p class="detail-title-bold">Valid From</p>
                    <hr class="tebal">
                    <label class="label-green c">07-06-2021</label>
                </div>
                <div class="container2">
                    <p class="detail-title-bold">Valid Until</p>
                    <hr class="tebal">
                    <label class="label-green c">09-06-2021</label>
                </div>
            </div>
        </div>
        <div class="admin container">
            <p>Create By Admin</p>
            <p>Create By Admin</p>
        </div>
    </div>
</template>

<script>
import List from "../voucher/list.vue"

export default {
	name: 'detail-user',
    List,
    data() {
        return {
            urlImg:  require('../../assets/images/voucher image.jpeg'),
        };
    },
}

</script>

<style>


.exp{
    display: flex;   
}

.c{
    width:100px;
    display: flex;
}

body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
}

.tebal{
    border: 1px solid black;
    width: 100%;
    margin: 0;
    margin-bottom: 16px;
    margin-top: -10px;
}

.container2 {
    margin-right: 60px;
   
}

.container {
    margin-left: 30px;
   
}

.space{
    margin-right: 10px;
}

.desk{
    line-height: 2;
}

.in {
    display: flex;
    margin-bottom: -20px;
}

.right{
    float: right;
    text-align: left;
    display: flex;
}

.mp{
    margin-left: 30px;
    margin-bottom: 20px;
}

.abu{
    color: darkgray;
}

.admin{
    margin-top: 40px;
    
}
</style>