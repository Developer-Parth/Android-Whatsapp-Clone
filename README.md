<!DOCTYPE html>
<html>
    <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <link href='https://fonts.googleapis.com/icon?family=Material+Icons' rel='stylesheet'/>
     <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/material-design-iconic-font/2.1.2/css/material-design-iconic-font.min.css">
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
        <title>♎WhatsApp Clone♎ | Developer Parth</title>
        <style>
            @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Lato&display=swap');
*{
    margin:0;
    padding:0;
    font-family: 'Poppins', sans-serif;
}
:root{
    --green: #008E6B;
}
html{
    scroll-behavior:smooth;
}
.container{
    width:100%;
    height:100%;
    box-sizing:border-box;
    position:absolute;
    background:#fff;
}
.header{
    width:100%;
    height:70px;
    padding:20px 0px 0px 0px;
    background:var(--green);
    color:#fff;
    position:fixed;
    z-index:100;
}
#menu{
    width:190px;
    height:210px;
    padding-top:10px;
    background:white;
    position:fixed;
    overflow:hidden;
    right:0;
    margin-top:20px;
    z-index:250;
    box-shadow:-3px 3px 5px rgba(0,0,0,.2);
}
#menu li{
    padding:8px 10px 8px 25px;
}
#menu li:active{
    background:rgba(0,0,0,.2);
}
.whatsapp{
    font-weight:500;
    margin-left:15px;
    margin-top:-10px;
    font-size:20px;
}
.ellip{
    right:15px;
    padding:8px;
    font-size:18px;
    margin-right:0px;
    border-radius:50px;
    color:#fff;
    position:fixed;
    margin-top:10px;
    z-index:200;
}
.ellip:active{
    background:rgba(255,255,255,.3);
}
.search{
    float:right;
    padding:7px 8px 7px 8px;
    font-size:18px;
    margin-right:45px;
    border-radius:50px;
    margin-top:-10px;
}
.search:active{
    background:rgba(255,255,255,.3);
}
.list{
    margin-top:10px;
    font-size:13px;
    font-weight:bold;
    text-align:center;
}
.camera{
    padding:5px;
    font-size:17px;
    color:rgba(255,255,255,.6);
    float:left;
    margin-left:5px;
    margin-top:-3px;
    border-radius:5px;
}
.camera:active{
    background:rgba(255,255,255,.2);
}
.calls{
    float:right;
    margin-right:20px;
    padding:5px;
    margin-top:-4px;
}
.calls:active{
    background:rgba(255,255,255,.3);
}
.chats{
    float:left;
    margin-left:20px;
    margin-top:-6px;
    padding-bottom:3px;
    padding:5px;
    border-bottom:2px solid #fff;
}
.chats:active{
    background:rgba(255,255,255,.3);
}
.status{
    margin-left:0px;
    margin-top:10px;
    padding:5px;
    padding-bottom:4px;
}
.status:active{
    background:rgba(255,255,255,.3);
}
.the_chats{
    width:100%;
    height:100%;
    background:#fff;
    margin-top:85px;
    display:flex;
    overflow-x:auto;
    scroll-snap-type:x mandatory;
}
.chats_container{
    scroll-snap-align:start;
    min-width:100%;
    height:100%;
    overflow-y:scroll;
    background:#fff;
    border-right:.2px solid rgba(0,0,0,.2);
}
.status_container{
    scroll-snap-align:start;
    min-width:100%;
    height:100%;
    background:#fff;
    border-right:.2px solid rgba(0,0,0,.2);
    overflow-y:scroll;
}
.calls_container{
    scroll-snap-align:start;
    min-width:100%;
    height:100%;
    background:#fff;
}
.call_info{
    width:300px;
    height:300px;
    margin-top:200px;
}
.ul_chats{
    width:100%;
    margin-top:15px;
}
.ul_chats li{
    list-style-type:none;
    margin-bottom:12px;
    padding-bottom:6px;
}
.ul_chats li:active{
    background:rgba(0,0,0,.2);
}
li a{
    text-decoration:none;
    list-style-type:none;
    color:black;
    cursor:pointer;
}
.ul_chats .icon1{
    width:50px;
    border-radius:50%;
    height:50px;
    border:none;
    outline:none;
    background:#efe7dd url(https://encrypted-tbn1.gstatic.com/images?q=tbn:ANd9GcSVvdf3mtAr8BQaBqwu2wAFbJD1dH6jtmyAK7hZRRnbFc0yc_pT);
    background-size:cover;
    margin-top:10px;
    margin-left:12px;
}
.ul_chats .icon2{
    width:50px;
    border-radius:50%;
    height:50px;
    border:none;
    outline:none;
    background:#efe7dd url(https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcT12cP23udqvCqHW_2oAvK257g3oVQkv23tOumxtpfFOhHi8a5B);
    background-size:cover;
    margin-top:10px;
    margin-left:12px;
}
.ul_chats .icon3{
    width:50px;
    border-radius:50%;
    height:50px;
    border:none;
    outline:none;
    background:#efe7dd url(https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcS1rDH_nWadT1GXFPomdutqV1PUMA8uXIWS2Js5_fq4pJ1lwG16);
    background-size:cover;
    margin-top:10px;
    margin-left:12px;
}
.ul_chats .icon4{
    width:50px;
    border-radius:50%;
    height:50px;
    border:none;
    outline:none;
    background:#efe7dd url(https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcQU2JRbbl3LBOm_an3eI5iplFhOoLESyBwUfmWDO49BS1EYuGUE);
    background-size:cover;
    margin-top:10px;
    margin-left:12px;
}
.ul_chats .icon5{
    width:50px;
    border-radius:50%;
    height:50px;
    border:none;
    outline:none;
    background:#efe7dd url(https://t0.gstatic.com/licensed-image?q=tbn:ANd9GcSUadwflQXaMZhx4HNJ9yjmPkQnKQoKRk4_yuC4WjgjjsAXdV5_QFZERdRTShHG);
    background-size:cover;
    margin-top:10px;
    margin-left:12px;
}
.ul_chats .icon6{
    width:50px;
    border-radius:50%;
    height:50px;
    border:none;
    outline:none;
    background:#efe7dd url(https://t2.gstatic.com/licensed-image?q=tbn:ANd9GcQQ840Wk_80H2JjO4wmYQ8VpNzck-GCsmu8a4HqMDNoeZNAH5Zw8qkRZc9a2C9v);
    background-size:cover;
    margin-top:10px;
    margin-left:12px;
}
.ul_chats .icon7{
    width:50px;
    border-radius:50%;
    height:50px;
    border:none;
    outline:none;
    background:#efe7dd url(https://t0.gstatic.com/licensed-image?q=tbn:ANd9GcRjhVK6JmLl4J0MwVaAQy11_-b46X7VI81sJIuwf_UEJyg_O-_uChuBqIMSel3d);
    background-size:cover;
    margin-top:10px;
    margin-left:12px;
}
.ul_chats .icon8{
    width:50px;
    border-radius:50%;
    height:50px;
    border:none;
    outline:none;
    background:#efe7dd url(https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcS0U5a32I81EyodYLVvHBNs7GSlBgmag51JRMz_0RQ2DqthEDKr);
    background-size:cover;
    margin-top:10px;
    margin-left:12px;
}
.ul_chats .icon9{
    width:50px;
    border-radius:50%;
    height:50px;
    border:none;
    outline:none;
    background:#efe7dd url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTyv0aAzhDzlUzFm_5uXSQvVp7GISukmB-2zA&usqp=CAU);
    background-size:cover;
    margin-top:10px;
    margin-left:12px;
}
.ul_chats .icon10{
    width:50px;
    border-radius:50%;
    height:50px;
    border:none;
    outline:none;
    background:#efe7dd url(https://t1.gstatic.com/licensed-image?q=tbn:ANd9GcTFNWogBmphs9qMbvplnItdr9z1nA41VxzHpdxq9n-tigPQjc3-7pPMx83rK0tk);
    background-size:cover;
    margin-top:10px;
    margin-left:12px;
}
.ul_chats .icon11{
    width:50px;
    border-radius:50%;
    height:50px;
    border:none;
    outline:none;
    background:#efe7dd url(https://upload.wikimedia.org/wikipedia/commons/e/e2/Mike_Bloomberg_Headshot.jpg);
    background-size:cover;
    margin-top:10px;
    margin-left:12px;
}
.ul_chats .icon12{
    width:50px;
    border-radius:50%;
    height:50px;
    border:none;
    outline:none;
    background:#efe7dd url(https://t3.gstatic.com/licensed-image?q=tbn:ANd9GcTkkZVfx7MDl1vS6XBHph7VvTMfETmBQWO4nsvXAq9MFO689TB9HQ7OAhS-1W4I);
    background-size:cover;
    margin-top:10px;
    margin-left:12px;
}
.ul_chats .icon13{
    width:50px;
    border-radius:50%;
    height:50px;
    border:none;
    outline:none;
    background:#efe7dd url(https://t2.gstatic.com/licensed-image?q=tbn:ANd9GcRTqPkCX1wgKlcE8FnfUjOQCyjayYR9schlFte0f_TvdXLr2F57rdYJov7oaNIe);
    background-size:cover;
    margin-top:10px;
    margin-left:12px;
}
.ul_chats .icon14{
    width:50px;
    border-radius:50%;
    height:50px;
    border:none;
    outline:none;
    background:#efe7dd url(https://t0.gstatic.com/licensed-image?q=tbn:ANd9GcS5PUoIIwZz81pF5O2LLNZUHjH7S57UlJBDyT5NIaA97Wj4mhFwUplM3-nxx3Dc);
    background-size:cover;
    margin-top:10px;
    margin-left:12px;
}
.ul_chats .icon15{
    width:50px;
    border-radius:50%;
    height:50px;
    border:none;
    outline:none;
    background:#efe7dd url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSTIGVmUB2OlzA80cf4xtLpc6QCvqdh3rNIpg&usqp=CAU);
    background-size:cover;
    margin-top:10px;
    margin-left:12px;
}
.ul_chats .person1{
    margin-top:-53px;
    margin-left:75px;
    font-weight:450;
}
.ul_chats .person2{
    margin-top:-53px;
    margin-left:75px;
    font-weight:450;
}
.ul_chats .person3{
    margin-top:-53px;
    margin-left:75px;
    font-weight:450;
}
.ul_chats .person4{
    margin-top:-53px;
    margin-left:75px;
    font-weight:450;
}
.ul_chats .person5{
    margin-top:-53px;
    margin-left:75px;
    font-weight:450;
}
.ul_chats .person6{
    margin-top:-53px;
    margin-left:75px;
    font-weight:450;
}
.ul_chats .person7{
    margin-top:-53px;
    margin-left:75px;
    font-weight:450;
}
.ul_chats .person8{
    margin-top:-53px;
    margin-left:75px;
    font-weight:450;
}
.ul_chats .person9{
    margin-top:-53px;
    margin-left:75px;
    font-weight:450;
}
.ul_chats .person10{
    margin-top:-53px;
    margin-left:75px;
    font-weight:450;
}
.ul_chats .person11{
    margin-top:-53px;
    margin-left:75px;
    font-weight:450;
}
.ul_chats .person12{
    margin-top:-53px;
    margin-left:75px;
    font-weight:450;
}
.ul_chats .person13{
    margin-top:-53px;
    margin-left:75px;
    font-weight:450;
}
.ul_chats .person14{
    margin-top:-53px;
    margin-left:75px;
    font-weight:450;
}
.ul_chats .person15{
    margin-top:-53px;
    margin-left:75px;
    font-weight:450;
}


.ul_chats .msg1{
    color:grey;
    font-size:13px;
    margin-top:-23px;
    margin-left:75px;
}
.ul_chats .msg2{
    color:grey;
    font-size:13px;
    margin-top:-23px;
    margin-left:75px;
}
.ul_chats .msg3{
    color:grey;
    font-size:13px;
    margin-top:-23px;
    margin-left:75px;
}
.ul_chats .msg4{
    color:grey;
    font-size:13px;
    margin-top:-23px;
    margin-left:75px;
}
.ul_chats .msg5{
    color:grey;
    font-size:13px;
    margin-top:-23px;
    margin-left:75px;
}
.ul_chats .msg6{
    color:grey;
    font-size:13px;
    margin-top:-23px;
    margin-left:75px;
}
.ul_chats .msg7{
    color:grey;
    font-size:13px;
    margin-top:-23px;
    margin-left:75px;
}
.ul_chats .msg8{
    color:grey;
    font-size:13px;
    margin-top:-23px;
    margin-left:75px;
}
.ul_chats .msg9{
    color:grey;
    font-size:13px;
    margin-top:-23px;
    margin-left:75px;
}
.ul_chats .msg10{
    color:grey;
    font-size:13px;
    margin-top:-23px;
    margin-left:75px;
}
.ul_chats .msg11{
    color:grey;
    font-size:13px;
    margin-top:-23px;
    margin-left:75px;
}
.ul_chats .msg12{
    color:grey;
    font-size:13px;
    margin-top:-23px;
    margin-left:75px;
}
.ul_chats .msg13{
    color:grey;
    font-size:13px;
    margin-top:-23px;
    margin-left:75px;
}
.ul_chats .msg14{
    color:grey;
    font-size:13px;
    margin-top:-23px;
    margin-left:75px;
}
.ul_chats .msg15{
    color:grey;
    font-size:13px;
    margin-top:-23px;
    margin-left:75px;
}
.ul_chats .time{
    margin-top:-23px;
    float:right;
    font-size:11px;
    font-weight:bolder;
    color:dimgrey;
    margin-right:13px;
}
.ul_chats .time_msgt{
    margin-top:-23px;
    float:right;
    font-size:11px;
    font-weight:bolder;
    color:#09EC58;
    margin-right:13px;
}
.ul_chats .time_msg1{
    margin-top:-23px;
    float:right;
    font-size:11px;
    font-weight:bolder;
    color:#09EC58;
    margin-right:13px;
}
.ul_chats .time_msg2{
    margin-top:-23px;
    float:right;
    font-size:11px;
    font-weight:bolder;
    color:#09EC58;
    margin-right:13px;
}
.ul_chats .time_msg3{
    margin-top:-23px;
    float:right;
    font-size:11px;
    font-weight:bolder;
    color:#09EC58;
    margin-right:13px;
}
.ul_chats .msgcol1{
    margin-top:-23px;
    float:right;
    font-size:11px;
    font-weight:bolder;
    width:10px;
    padding:2.5px 2px 7.5px 7px;
    height:10px;
    border-radius:50%;
    color:#fff;
    background:#09EC58;
    margin-right:13px;
}
.ul_chats .msgcol2{
    margin-top:-23px;
    float:right;
    font-size:11px;
    font-weight:bolder;
    width:10px;
    padding:2.5px 2px 7.5px 7px;
    height:10px;
    border-radius:50%;
    color:#fff;
    background:#09EC58;
    margin-right:13px;
}
.ul_chats .msgcol3{
    margin-top:-23px;
    float:right;
    font-size:11px;
    font-weight:bolder;
    width:10px;
    padding:2.5px 2px 7.5px 7px;
    height:10px;
    border-radius:50%;
    color:#fff;
    background:#09EC58;
    margin-right:13px;
}
.ul_chats .msgcol4{
    margin-top:-23px;
    float:right;
    font-size:11px;
    font-weight:bolder;
    width:10px;
    padding:2.5px 2px 7.5px 7px;
    height:10px;
    border-radius:50%;
    color:#fff;
    background:#09EC58;
    margin-right:13px;
}





.ul_status{
    width:100%;
    margin-top:15px;
}
.ul_status li{
    list-style-type:none;
    margin-bottom:12px;
    padding-bottom:6px;
}
.ul_status li:active{
    background:rgba(0,0,0,.2);
}
.icons1{
    width:53px;
    border-radius:50%;
    height:53px;
    border:3.5px solid #999999;
    outline:none;
    background:#efe7dd url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTzu5NNtYXjTgcixYVxyx5KMuQ1mX3Po9HE-w&usqp=CAU);
    background-size:cover;
    margin-top:10px;
    margin-left:12px;
}
.icons2{
    width:53px;
    border-radius:50%;
    height:53px;
    border:3.5px solid var(--green);
    outline:none;
    background:#efe7dd url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQfRSUkc_GKvOF71sbbBiwcsOpzjFGKyvFxmw&usqp=CAU);
    background-size:cover;
    margin-top:10px;
    margin-left:12px;
}
.icons3{
    width:53px;
    border-radius:50%;
    height:53px;
    border:3.5px solid var(--green);
    outline:none;
    background:#efe7dd url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRR_qUJAaNKNLsLVVZVX4e7iTG-zYTC0WTeiQ&usqp=CAU);
    background-size:cover;
    margin-top:10px;
    margin-left:12px;
}
.icons4{
    width:53px;
    border-radius:50%;
    height:53px;
    border:3.5px solid var(--green);
    outline:none;
    background:#efe7dd url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSe-bFZDvwJW0D-xrOxK5GV-WTcI2pRUXsyuA&usqp=CAU);
    background-size:cover;
    margin-top:10px;
    margin-left:12px;
}
.icons5{
    width:53px;
    border-radius:50%;
    height:53px;
    border:3.5px solid var(--green);
    outline:none;
    background:#efe7dd url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRkU-vVOPo24W1M4oSoXxvGDIFZ9KZTSrLKeg&usqp=CAU);
    background-size:cover;
    margin-top:10px;
    margin-left:12px;
}
.icons6{
    width:53px;
    border-radius:50%;
    height:53px;
    border:3.5px solid #999999;
    outline:none;
    background:#efe7dd url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRx-44eg2xPHvoHlR0gaO7DXRGKO9MGhOKRzw&usqp=CAU);
    background-size:cover;
    margin-top:10px;
    margin-left:12px;
}
.icons7{
    width:53px;
    border-radius:50%;
    height:53px;
    border:3.5px solid #999999;
    outline:none;
    background:#efe7dd url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT8BZ140TjscTxWdQ_FBN4oDB4Oev3pcU4hgQ&usqp=CAU);
    background-size:cover;
    margin-top:10px;
    margin-left:12px;
}
.icons8{
    width:53px;
    border-radius:50%;
    height:53px;
    border:3.5px solid #999999;
    outline:none;
    background:#efe7dd url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRtCQYBPxkZNSajdzTpFwnF71MfXUPVbiKPlw&usqp=CAU);
    background-size:cover;
    margin-top:10px;
    margin-left:12px;
}
.icons9{
    width:53px;
    border-radius:50%;
    height:53px;
    border:3.5px solid #999999;
    outline:none;
    background:#efe7dd url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRoVKUCMLAD3UNvsmDkMr4azr3c2D-rYJsE9g&usqp=CAU);
    background-size:cover;
    margin-top:10px;
    margin-left:12px;
}
.persons1{
    margin-top:-53px;
    margin-left:75px;
    font-weight:450;
}
.ul_status .elliph{
    margin-top:-15px;
    float:right;
    font-size:16px;
    font-weight:bolder;
    color:dimgrey;
    margin-right:20px;
}
.ul_status .msgs{
    color:grey;
    font-size:13px;
    margin-top:-22px;
    margin-left:75px;
}
.recent_update{
    color:dimgrey;
    font-weight:620;
    font-size:12px;
    margin-left:20px;
    margin-top:12px;
    margin-bottom:7px;
    opacity:.9;
}
.settings_container{
    width:100%;
    height:100%;
    position:absolute;
    box-sizing:border-box;
}
.settings_header{
    width:100%;
    padding:17px 0px 10px 0px;
    height:38px;
    color:#fff;
    background:var(--green);
}
.settings_back{
    padding:10px;
    margin-left:10px;
    font-size:20px;
    margin-top:10px;
    border-radius:50px;
}
.settings_back:active{
    background:rgba(255,255,255,.3);
}
.setting_name{
    margin-left:15px;
    font-size:18px;
    margin-top:-10px;
}
.settings_li{
    width:100%;
    height:85px;
    margin-top:10px;
    padding:10px 0px 5px 0px;
    border-bottom:.2px solid rgba(0,0,0,.2);
}
.settings_profile{
    width:65px;
    height:65px;
    border-radius:50%;
    background:dodgerblue url(https://source.unsplash.com/random);
    background-size:cover;
    border:.5px solid rgba(0,0,0,.2);
    margin-left:15px;
}
.settings_profile_name{
    margin-left:95px;
    margin-top:-53px;
    font-weight:585;
    font-size:18.5px;
    
}
.settings_profile_description{
    margin-left:95px;
    margin-top:0px;
    color:dimgrey;
    font-size:14px;
}
.settings_ul{
    width:100%;
    margin-top:5px;
}
.settings_ul li{
    list-style-type:none;
    padding:5px 10px 5px 30px;
    margin-bottom:3px;
    transition:.3s;
}
.settings_ul li:hover{
    background:rgba(0,0,0,.2);
}
.settings_ul .key{
    padding:10px 20px 10px 10px;
    font-size:20px;
    margin-top:0px;
    color:dimgrey;
}
.settings_ul .fa-key{
    margin-top:0px;
}
.settings_ul .key_name{
    font-size:18px;
    font-weight:575;
    margin-top:-45px;
    margin-left:65px;
}
.settings_ul .key_description{
    color:dimgrey;
    font-size:13px;
    margin-top:-23px;
    margin-left:63px;
}




.camera_container{
    width:100%;
    height:100%;
    position:absolute;
    box-sizing:border-box;
    background:black;
}
.camera_header{
    width:100%;
    padding:17px 0px 10px 0px;
    height:38px;
    color:#fff;
    background:black;
}
.camera_back{
    padding:10px;
    margin-right:15px;
    float:right;
    font-size:20px;
    margin-top:0px;
    border-radius:50px;
}
.camera_back:active{
    background:rgba(255,255,255,.3);
}
.record{
    position:absolute;
    bottom:50px;
    width:100%;
    height:70px;
    background:transparent;
}
.flash{
    float:left;
    font-size:25px;
    padding:10px;
    margin-left:10px;
    margin-top:5px;
    border-radius:50px;
}
.flash:active{
    background:rgba(255,255,255,.3);
}
.for_hold{
    width:53px;
    height:53px;
    border:3px solid #fff;
    border-radius:50%;
    margin-top:5px;
}
.for_hold:active{
    width:55px;
    height:55px;
    background:white;
}
.camera_switch{
    float:right;
    font-size:20px;
    padding:10px;
    margin-right:10px;
    margin-top:-55px;
    border-radius:50px;
}
.camera_switch:active{
    background:rgba(255,255,255,.3);
}
.camera_info{
    margin-top:10px;
    font-size:12px;
}
.iconsp{
    width:260px;
    height:260px;
    background:grey;
    position:fixed;
    top:130px;
    left:55px;
    border-radius:50%;
    transition:.4s;
    box-shadow:0 0 0 999px rgba(0,0,0,.4);
    z-index:300;
}
.iconsp_items{
    width:240px;
    height:30px;
    padding:10px;
    background:white;
    margin-top:260px;
    
}
.iconsp span{
    font-size:20px;
    color:var(--green);
}
.iconsp span .fa{
     padding:5px;
}
.iconsp span .fa:active{
    background:rgba(0,0,0,.3);
}
.iconsp .fa-send{
    float:left;
    margin-left:10px;
    margin-top:2px;
}
.iconsp .fa-info-circle{
    float:right;
    margin-right:10px;
    font-size:22px;
}
.iconsp .fa-phone{
    margin:0 20px;
    font-size:21px;
}
.iconsp .fa-video-camera{
    margin:0 20px;
}




.invi{
    width:100%;
    height:100vh;
    background:transparent;
    position:fixed;
    z-index:288;
    backdrop-filter:blur(1px);
}


.view_status_container{
    width:100%;
    height:100%;
    background:transparent;
    z-index:350;
    position:fixed;
}
.status_top{
    width:100%;
    height:45px;
    padding:15px 0px 5px 0px;
    color:#fff;
    position:absolute;
    background:#000;
}
.view_back{
    color:white;
    font-size:20px;
    margin-left:10px;
    margin-top:-5px;
    padding:10px;
    float:left;
}
.view_icon{
    width:45px;
    height:45px;
    background:url(https://source.unsplash.com/random);
    background-size:cover;
    border-radius:50%;
    margin-left:50px;
    margin-top:-3px;
    border:2px solid white;
}
.view_name{
    margin-top:-40px;
    margin-left:110px;
    font-weight:590;
    font-size:18px;
}
.view_ellip{
    float:right;
    margin-right:15px;
    font-size:18px;
    margin-top:-25px;
}
.line{
    width:100%;
    height:4px;
    background:white;
    margin-top:-10px;
    position:absolute;
    margin-bottom:15px;
    left:-100%;
    z-index:20;
    border-radius:10px;
    animation:line 8s linear;
}
@keyframes line{
    100% {left:0%;}
}
.line2{
    width:100%;
    height:4px;
    background:#999999;
    margin-top:-10px;
    position:absolute;
    border-radius:10px;
    margin-bottom:15px;
}
.status_down{
    position:absolute;
    bottom:30px;
    width:100%;
    height:30px;
    color:#fff;
}
.status_down .fa-angle-up{
    font-size:20px;
}
.reply{
    font-size:15px;
}


.status_down2{
    position:absolute;
    bottom:20px;
    width:100%;
    height:30px;
    color:#fff;
}
.status_down2 .fa-eye{
    font-size:18px;
    padding-top:3px;
    padding-left:5px;
    padding-right:5px;
    border-top:3px solid white;
    border-radius:10px;
}

.real_chat{
    width:100%;
    height:100%;
    position:fixed;
    background:#efe7dd url(https://user-images.githubusercontent.com/15075759/28719144-86dc0f70-73b1-11e7-911d-60d70fcded21.png);
    background-size:cover;
    z-index:100;
}
.real_chat_header{
    width:100%;
    height:40px;
    padding:10px 0px 10px 0px;
    color:#fff;
    background:var(--green);
}
.real_chat_back{
    float:left;
    margin-left:7px;
    padding:10px;
    border-radius:50px;
}
.real_chat_back:active{
    background:rgba(255,255,255,.3);
}
.real_chat_icon{
    width:40px;
    border-radius:50%;
    height:40px;
    border:3px solid white;
    background:white;
    background-size:cover;
    margin-left:40px;
}
.real_chat_name{
    margin-top:-40px;
    margin-left:95px;
    font-size:18px;
    font-weight:570;
}
.real_chat_calls{
    float:right;
    margin-right:40px;
    font-size:20px;
    margin-top:-32px;
}
.real_chat_calls .fa{
    padding:10px;
    border-radius:50px;
}
.real_chat_calls2 .fa{
    padding:10px;
    border-radius:50px;
}
.real_chat_calls .fa:active{
    background:rgba(255,255,255,.3);
}
.real_chat_calls2 .fa:active{
    background:rgba(255,255,255,.3);
}
.real_chat_calls2{
    float:right;
    margin-right:10px;
    font-size:20px;
    margin-top:-32px;
}
.real_chat_online{
    font-size:12px;
    margin-left:100px;
    margin-top:-5px;
}
.real_chat_input{
    width:80%;
    height:30px;
    padding:10px;
    background:white;
    position:absolute;
    bottom:5px;
    z-index:200;
    overflow:hidden;
    float:left;
    border-radius:50px;
    margin-left:3px;
}
.real_chat_smile{
    float:left;
    font-size:25px;
    color:dimgrey;
    padding:0px 5px 0px 5px;
    border-radius:50px;
    margin-top:-3px;
}
.real_chat_smile:active{
    background:rgba(0,0,0,.2);
}
.real_chat_input{
    display:flex;
    align-items:center;
    justify-content:center;
}
.real_chat_input input{
    outline:none;
    padding:3px;
    float:left;
    margin-top:2px;
    margin-left:3px;
    background:transparent;
    border:none;
    font-size:16px;
    width:180px;
}
.real_chat_send{
    position:absolute;
    bottom:5px;
    font-size:25px;
    color:white;
    padding:6.5px 12px 4.5px 14px;
    right:5px;
    border-radius:50%;
    background:var(--green);
}
.real_chat_mic{
    position:absolute;
    bottom:5px;
    font-size:25.5px;
    color:white;
    padding:8px 12px 2px 12px;
    right:5px;
    border-radius:50%;
    background:var(--green);
}
.real_chat_mic:active{
    background:#00BA8C;
}
.real_chat_send:active{
    background:#00BA8C;
}
.real_chat_items{
    float:right;
    margin:auto;
}
.real_link{
    padding:5px 11px 5px 11px;
    font-size:22px;
    margin-right:-10px;
    color:dimgrey;
    border-radius:50px;
}
.real_link:active{
    background:rgba(0,0,0,.2);
}
.real_cam{
    padding:8px 10px 7px 10px;
    font-size:20px;
    color:dimgrey;
    border-radius:50px;
}
.real_cam:active{
    background:rgba(0,0,0,.2);
}
.real_today{
    padding:5px 10px 10px 10px;
    width:65px;
    background:dodgerblue;
    font-size:12px;
    height:10px;
    background:#98D6F3;
    border-radius:5px;
    margin-top:10px;
    box-shadow:1px 3px 2px rgba(0,0,0,.3);
}
.real_inform{
    padding:8px 10px 15px 10px;
    width:310px;
    background:dodgerblue;
    height:auto;
    color:black;
    margin-top:-5px;
    opacity:.8;
    background:#FFEEA9;
    font-size:12px;
    border-radius:10px;
}
.conversation{
    width:100%;
    transition:1.5s;
    scroll-behavior:smooth;
    height:45%;
    overflow:scroll;
    padding:10px 0px 10px 0px;
}








.tick{
    display:inline-block ;
     font-size:15px;
     padding:2px;
     float:right;
     margin-top:-3px;
     color:#37d; 
     color:gray;
}
#schat{
     background:#dcf8c6;
     box-shadow:2px 1px 2px 0px gray;
     border-radius:7px 0px 7px 7px;
     padding:5px 5px 5px 7px;
     margin:5px 10px 5px 5px;
     float:right;
     right:10px;
     overflow:hidden;
     clear:both;
     max-width:50%;
     display:inline-block ;
}
#rchat{
     background:white;
     box-shadow:1px 1px 1px 0px gray;
     border-radius:0px 7px 7px 7px;
     padding:5px 5px 5px 7px;
     margin:5px 5px 5px 10px;
     float:left;
     clear:both;
     overflow:hidden;
     max-width:50%;
     display:inline-block;
}
#rchats{
     background:white;
     box-shadow:1px 1px 1px 0px gray;
     border-radius:0px 7px 7px 7px;
     padding:5px 5px 5px 7px;
     margin:5px 5px 5px 10px;
     float:left;
     clear:both;
     overflow:hidden;
     max-width:50%;
     display:inline-block;
}
.rtime, .stime{
  float: right;
  padding: 0 0 0 7px;
  position: relative;
  bottom: -8px;
  color: rgba(0, 0, 0, .45);
  font-size: 11px;
  display: inline-block;
}
.load_screen{
    width:100%;
    height:100%;
    display:flex;
    align-items:center;
    justify-content:center;
    background:#fff;
    position:absolute;
}
.whatsapp_logo{
    width:105px;
    height:105px;
    background:url(https://assets.stickpng.com/images/580b57fcd9996e24bc43c543.png);
    background-size:cover;
    border-radius:10px;
    margin-top:-90px;
}
.from{
    position:absolute;
    margin-left:40px;
    font-size:14.5px;
    bottom:40px;
}
.devparth{
    position:absolute;
    bottom:15px;
    font-weight:bold;
    color:#09EC58;
    margin-left:10px;
}
        </style>
    </head>
    <body>
    <div class="load_screen">
   <div class="whatsapp_logo">
   <div class="from">from</div>
   <div class="devparth">Developer Parth</div>
   </div>
    </div>
    <span class="ellip"><i class="fa fa-ellipsis-v"></i></span>
    <ul id="menu">
    <li class="l1">New group</li>
    <li class="l2">New broadcast</li>
    <li class="l3">Linked devices</li>
    <li class="l4">Starred messages</li>
    <li class="l5">Settings</li>
    </ul>
    <!--  CONTAINER  -->
    <div class="container">
    <!-- HEADER  -->
    <div class="header">
    <span class="whatsapp">WhatsApp</span>
    <span class="search"><i class="fa fa-search"></i></span><br />
    
    
    <!-- LISTS  -->
    <div class="list">
    <span class="camera"><i class="fa fa-camera"></i></span>
    <span class="chats">CHATS</span>
    <span class="status">STATUS</span>
    <span class="calls">CALLS</span>
    </div>
    
    </div>
    
    <!--  THE CHATS  -->
    <div class="the_chats">
    
    
    
    <!--  CHATS CONTAINER  -->
    <div class="chats_container">
    <!--  UL -->
    <ul class="ul_chats">
    
    <li class="li_chats1">
    <button class="icon1"></button>
    <div class="person1">Jeff Bezos</div>
    <span class="time_msgt">12:00 AM</span><br />
    <div class="msg1">Hi, we need an update to our website</div><div class="msgcol1">1</div>
    </li>
    
    <li class="li_chats2">
    <button class="icon2"></button>
    <div class="person2">Bill Gates</div>
    <span class="time_msg1">12:29 AM</span><br />
    <div class="msg2">Yes, but the alert has not yet arrived</div><div class="msgcol2">1</div>
    </li>
    
    
    <li class="li_chats3">
    <button class="icon3"></button>
    <div class="person3">Mark Zuckerberg</div>
    <span class="time_msg2">11:36 PM</span><br />
    <div class="msg3">I called you yesterday, but you did n...</div><div class="msgcol3">1</div>
    </li>
    
    
    <li class="li_chats4">
    <button class="icon4"></button>
    <div class="person4">Elon Musk</div>
    <span class="time_msg3">10:01 PM</span><br />
    <div class="msg4">Hello Dev Parth, i saw the updates </div><div class="msgcol4">1</div>
    </li>
    
    
    <li class="li_chats5">
    <button class="icon5"></button>
    <div class="person5">Larry Ellison</div>
    <span class="time">Yesterday</span><br />
    <div class="msg5">yes i saw the mail, I'm on my way from</div>
    </li>
    
    
    <li class="li_chats6">
    <button class="icon6"></button>
    <div class="person6">Lary Page</div>
    <span class="time">Yesterday</span><br />
    <div class="msg6">Hi Dev Parth, I need a loan from you!!</div>
    </li>
    
    
    <li class="li_chats7">
    <button class="icon7"></button>
    <div class="person7">Sergey Brin</div>
    <span class="time">Yesterday</span><br />
    <div class="msg7">I want you to be our frontend developer...</div>
    </li>
    
    
    <li class="li_chats8">
    <button class="icon8"></button>
    <div class="person8">Warren Buffet</div>
    <span class="time">Yesterday</span><br />
    <div class="msg8">I'm trying to send you back the $380M</div>
    </li>
    
    
    <li class="li_chats9">
    <button class="icon9"></button>
    <div class="person9">Alice Walton</div>
    <span class="time">28/12/21</span><br />
    <div class="msg9">Good job! Dev Parth, glad to see yo...</div>
    </li>
    
    
    
    <li class="li_chats10">
    <button class="icon10"></button>
    <div class="person10">Jim Walton</div>
    <span class="time">26/12/21</span><br />
    <div class="msg10">I have a serious issue with you, please...</div>
    </li>
    
    
    <li class="li_chats11">
    <button class="icon11"></button>
    <div class="person11">Michael Bloomberg</div>
    <span class="time">23/12/21</span><br />
    <div class="msg11">it was very very nice, thank you so much</div>
    </li>
    
    
    <li class="li_chats12">
    <button class="icon12"></button>
    <div class="person12">Mukesh Ambani</div>
    <span class="time">18/12/21</span><br />
    <div class="msg12">Thank you bhai😊, i'll meet you tomm...</div>
    </li>
    
    
    <li class="li_chats13">
    <button class="icon13"></button>
    <div class="person13">Rob Walton</div>
    <span class="time">17/12/21</span><br />
    <div class="msg13">Okay, no problem i'll come as soon as...</div>
    </li>
    
    
    <li class="li_chats14">
    <button class="icon14"></button>
    <div class="person14">Carlos Slim</div>
    <span class="time">11/12/21</span><br />
    <div class="msg14">are you done with the project please? </div>
    </li>
    
    
    <li class="li_chats15">
    <button class="icon15"></button>
    <div class="person15">Warren Buffet</div>
    <span class="time">8/12/21</span><br />
    <div class="msg15">i'll be back to you before 12:00 AM</div>
    </li>
    
    
    
    
    </ul>
    </div>
        
    
    <!--  STATUS CONTAINER  -->
    <div class="status_container">
    <!--  UL  -->
    <ul class="ul_status">
    <li class="li_status1">
    <button class="icons1"></button>
    <div class="persons1">My status</div><span class="elliph"><i class="fa fa-ellipsis-h"></i></span><br />
    <div class="msgs">Today, 11:30 AM</div>
    </li>
    
    
    <div class="recent_update">Recent updates</div>
    
    
    <li class="li_status2">
    <button class="icons2"></button>
    <div class="persons1">Bill Gates</div><br />
    <div class="msgs">Just know</div>
    </li>
    
    
    <li class="li_status3">
    <button class="icons3"></button>
    <div class="persons1">Jeff Bezos</div><br />
    <div class="msgs">2 minutes ago</div>
    </li>
    
    
    
    <li class="li_status4">
    <button class="icons4"></button>
    <div class="persons1">Mark Zukerberg</div><br />
    <div class="msgs">39 minutes ago</div>
    </li>
    
    
    
    <li class="li_status5">
    <button class="icons5"></button>
    <div class="persons1">Larry Page</div><br />
    <div class="msgs">53 minutes ago</div>
    </li>
    
    <div class="recent_update">Viewed updates</div>
    
    
    <li class="li_status6">
    <button class="icons6"></button>
    <div class="persons1">Elon Musk</div><br />
    <div class="msgs">Today, 10:03 AM</div>
    </li>
    
    
    
    <li class="li_status7">
    <button class="icons7"></button>
    <div class="persons1">Rob Walton</div><br />
    <div class="msgs">Today, 11:43 PM</div>
    </li>
    
    
    
    <li class="li_status8">
    <button class="icons8"></button>
    <div class="persons1">Carlos Slim</div><br />
    <div class="msgs">Yesterday, 01:03 AM</div>
    </li>
    
    
    
    
    <li class="li_status9">
    <button class="icons9"></button>
    <div class="persons1">Warren Buffet</div><br />
    <div class="msgs">Yesterday, 08:14 AM</div>
    </li>
    
    
    </ul>
    </div>
    
    
    
    
    <!--  CALLS CONTAINER  -->
    <div class="calls_container">
    <center>
    <div class="call_info">
    To start calling contacts who have<br>
    WhatsApp, tap <i class="fa fa-phone"></i> at the bottom of your screen.
    </div>
    </center>
    </div>
    
        
    </div>
    
    
    </div>
     <!-- SETTINGS -->
    <div class="settings_container">
    <div class="settings_header">
    <span class="settings_back"><i class="fa fa-arrow-left"></i></span>
    <span class="setting_name">Settings</span>
    </div>
    
    <div class="settings_li">
    <div class="settings_profile"></div>
    <div class="settings_profile_name">Dev Parth</div>
    <div class="settings_profile_description">Talented Developer</div>
    </div>
    
    <ul class="settings_ul">
    
    <li><div class="key"><i class="fa fa-key"></i></div> <div class="key_name">Account</div><br /><div class="key_description">Privacy, security, change number</div></li>
    
    <li><div class="key"><i class="fa fa-envelope"></i></div> <div class="key_name">Chats</div><br /><div class="key_description">Theme, wallpapers, chat history</div></li>
    
    <li><div class="key"><i class="fa fa-bell"></i></div> <div class="key_name">Notifications</div><br /><div class="key_description">Message, group & call tones</div></li>
    
    <li><div class="key"><i class="fa fa-bar-chart"></i></div> <div class="key_name">Storage and data</div><br /><div class="key_description">Network usage, auto-download</div></li>
    
    <li><div class="key"><i class="fa fa-question-circle-o"></i></div> <div class="key_name">Help</div><br /><div class="key_description">Help center, contact us, privacy policy</div></li>
    
    <li><div class="key"><i class="fa fa-users"></i></div> <div class="key_name">Invite a friend</div></li>
    </ul>
    
    </div>
    
    
    
    
     <!-- CAMERA  -->
    <div class="camera_container">
    <div class="camera_header">
    <span class="camera_back"><i class="fa fa-arrow-right"></i></span>
    <center>
    <div class="record">
    <div class="flash"><i class="fa fa-flash"></i></div>
    <div class="for_hold"></div>
    <div class="camera_switch"><i class="fa fa-camera"></i></div>
    <div class="camera_info">
    Hold for video, tap for photo
    </div>
    </div>  
    </center>
    </div>
    </div>
    
    
    <!--  ICONS  -->
    <center>
    <div class="iconsp">
    <div class="iconsp_items">
    <span class="iconsp_send"><i class="fa fa-send"></i></span>  
    <span class="iconsp_send"><i class="fa fa-phone"></i></span>  
    <span class="iconsp_send"><i class="fa fa-video-camera"></i></span>
    <span class="iconsp_send"><i class="fa fa-info-circle"></i></span>  
    </div>
    </div>
    </center>
    
    
    <div class="invi">
        
    </div>
    
    
    <!-- STATUS  -->
    <div class="view_status_container">
    <div class="status_top">
    <div class="line"></div>
    <div class="line2"></div>
    <span class="view_back"><i class="fa fa-arrow-left"></i></span>
    <div class="view_icon"></div>
    <div class="view_name">Abdul Majid</div>
    <span class="view_ellip"><i class="fa fa-ellipsis-v"></i></span>
    </div>
     
     <center>
     <div class="status_down">
     <i class="fa fa-angle-up"></i><br />
     <span class="reply">Reply</span>
     </div>
     
     <div class="status_down2">
     <i class="fa fa-eye"></i><br />
     <span class="reply">208</span>
     </div>
     </center>
    
    </div>
    
    
    <!--  REAL CHATS  -->
    <div class="real_chat">
    <div class="real_chat_header">
    
    <span class="real_chat_back">
    <i class="fa fa-arrow-left"></i>
    </span>
    
    <div class="real_chat_icon"></div>
    
    <div class="real_chat_name">User Name</div>
    
    <div class="real_chat_calls">
    <i class="fa fa-phone"></i>
    </div>
    <div class="real_chat_calls2">
    <i class="fa fa-video-camera"></i>
    </div>
    
    <div class="real_chat_online">online</div>
    
    </div>
    
    <div class="real_chat_input">
    <span class="real_chat_smile"><i class="fa fa-smile-o"></i></span>
    <input type="text" placeholder="Message" id="message">
    <div class="real_chat_items">
    <span class="real_link"><i class="fa fa-paperclip"></i></span>
    <span class="real_cam"><i class="fa fa-camera"></i></span>
    </div>
    </div>
    <!-- TODAY  -->
    <center>
    <div class="real_today">Today</div><br>
    <div class="real_inform">
 <i class="fa fa-lock"></i> Messages and calls are end-to-end encrypted.<br />No one outside of this chat, not even WhatsApp, can read or listen to them. Tap to learn more.
    </div>
    </center>
    
    <!-- CONVERSATIONS  -->
    <ul class="conversation">
    <div id="rchats"><span class="rechats"></span><span class="rtime"></span></div>
    
    </ul>
    
    
    
    <div class="real_chat_send">
    <i class="zmdi zmdi-mail-send"></i>
    </div>
    <div class="real_chat_mic">
    <i class="material-icons">mic</i>
    </div>
    
    </div>
    <audio controls style="display:none;" id="audio">
    <source id="audio-source"
     src="https://devnasfam.000webhostapp.com/rec.mp3" type="audio/mpeg">
     <audio controls style="display:none;" id="audio2">
    <source id="audio-source"
     src="https://devnasfam.000webhostapp.com/sen.mp3" type="audio/mpeg">
    <script>
    $(".container").hide();
    $(".ellip").hide();
    window.onload = function(){
    $(".container").show();
    $(".load_screen").fadeOut(500);
    $(".ellip").show();
    
    $(".fa-phone").click(function(){
    setTimeout(function(){
    navigator.vibrate&&navigator.vibrate(60);
    }, 50);
    });
    
    
    var span = document.querySelector(".time_msgt");
    var date = new Date();
    var HH = date.getHours();
    var MM = date.getMinutes();
    MM = (MM < 10) ? "0" + MM : MM;
    var am_pm = "PM";
    if (HH==0){
        am_pm = "PM";
    }else if (HH>=12){
        am_pm = "PM";
    }
    else{
        am_pm = "AM";
    }
    if (HH>12){
        HH=HH-12;
    }else{
        HH=HH;
    }
    var TT = HH+":"+MM+" "+am_pm;
    span.innerHTML=TT;
    }
    

    
    $(".real_chat_send").click(function(){
    var d = new Date();
 var h = d.getHours(); 
 var t = d.getMinutes();
  h = (h <10) ? "0" + h : h;
 t = (t <10) ? "0" + t : t;
 if(h>12){
    h=h-12;
 }else{
    h=h;
 }
 time= h+":"+t;
 document.querySelector("#message").focus();
  var mmssgg = document.querySelector("#message");
 mmssgg.addEventListener("focus",()=>{
     $(".conversation").css("height","45%");
 });
 mmssgg.addEventListener("focusout",()=>{
     $(".conversation").css("height","65%");
 });
 
    var val = $("#message").val();
    if (val!==""){
    var elem = $("  <div class='re' id='schat'><span class='sechat'>"+val+"</span> <span class='stime'>"+time+"<i class='material-icons tick'style='color:#aaa;'>done_all</i></span></div> ");
    $(".conversation").append(elem);
    $("#message").val("");
   // document.getElementById("audio2").play();
    var mmssgg = document.querySelector("#message").focus();
    $(".conversation").scrollTop($(".conversation")[0].scrollHeight);

    setTimeout(function(){
        //document.getElementById("audio").play();
    },1950);
    
    setTimeout(function(){
  $(".tick").css("color","#4fc3f7");
  $(".real_chat_online").text("typing...").css("color","#3d7");
   setTimeout(function(){
   if (val=="Hi"){
       $(".conversation").append("<div class='re' id='rchat'><span class='rechat'>Hello</span> <span class='rtime'>"+time+"</span></div>");
       $(".conversation").scrollTop($(".conversation")[0].scrollHeight);
       navigator.vibrate(100);
       $(".real_chat_online").text("online").css("color","#fff");
   }else if (val=="Hello"){
       $(".conversation").append("<div class='re' id='rchat'><span class='rechat'>Hi</span> <span class='rtime'>"+time+"</span></div>");$(".conversation").scrollTop($(".conversation")[0].scrollHeight);
       navigator.vibrate(100);
       $(".real_chat_online").text("online").css("color","#fff");
   }else if (val=="How are you?"){
       $(".conversation").append("<div class='re' id='rchat'><span class='rechat'>I'm fine, and you..?</span> <span class='rtime'>"+time+"</span></div>");$(".conversation").scrollTop($(".conversation")[0].scrollHeight);
       navigator.vibrate(100);
       $(".real_chat_online").text("online").css("color","#fff");
   }else if (val=="How are you"){
       $(".conversation").append("<div class='re' id='rchat'><span class='rechat'>I'm fine, and you..?</span> <span class='rtime'>"+time+"</span></div>");$(".conversation").scrollTop($(".conversation")[0].scrollHeight);
       val = val.trim();
       navigator.vibrate(100);
       $(".real_chat_online").text("online").css("color","#fff");
   }else if (val=="Fuck you"){
       $(".conversation").append("<div class='re' id='rchat'><span class='rechat'>You are in trouble😠</span> <span class='rtime'>"+time+"</span></div>");$(".conversation").scrollTop($(".conversation")[0].scrollHeight);
       navigator.vibrate(900);
       $(".real_chat_online").text("online").css("color","#fff");
   }else{
       $(".conversation").append("<div class='re' id='rchat'><span class='rechat'>Don't worry about what he is saying🤩, just upvote my code and subscribe my youtube channel🙏</span> <span class='rtime'>"+time+"</span></div>");$(".conversation").scrollTop($(".conversation")[0].scrollHeight);
       navigator.vibrate(100);
       $(".real_chat_online").text("online").css("color","#fff");
    }
   },2000);},1000);
    }
    });
    
    
    var msg = document.querySelector("#message");
    var mic = document.querySelector(".real_chat_mic");
    var send = document.querySelector(".real_chat_send");
    send.style.display="none";
    

    msg.addEventListener("input", myFun);
    function myFun(){
     if(msg.value.length>0){
         mic.style.display="none";
         send.style.display="block";
         $(".real_cam").hide();
     }else if(msg.value.length>=12){
         return false;
     }
     else{
         send.style.display="none";
         mic.style.display="block";
         $(".real_cam").show();
         $(".real_link").show();
     }
    }
    
    //TEMPORARY HIDES 
    
    $("#menu").toggle();
    $(".ellip").click(function(){
    $("#menu").toggle(300);
    $(".container").click(function(){
    $("#menu").hide(200);
    });
    });
    $(".status").click(function(){
    $(".chats_container").hide(300);
    $(".status_container").show(300);
    $(".calls_container").hide(300);
    $("#menu").css({"height":"80px"});
    $(".status").css({"border-bottom":"2px solid #fff"});
    $(".calls").css({"border-bottom":"0px"});
    $(".chats").css({"border-bottom":"0px"});
    $(".l2").hide();
    $(".l4").hide();
    $(".l3").hide();
    $(".l1").html("Status privacy");
    });
    $(".chats").click(function(){
    $(".calls_container").hide(300);
    $(".status_container").hide(300);
    $(".chats_container").show(300);
    $("#menu").css({"height":"210px"});
    $(".chats").css({"border-bottom":"2px solid #fff"});
    $(".calls").css({"border-bottom":"0px"});
    $(".status").css({"border-bottom":"0px"});
    $(".l2").show();
    $(".l4").show();
    $(".l3").show();
    $(".l1").html("New Group");
    });
    $(".calls").click(function(){
    $(".calls_container").show(300);
    $(".status_container").hide(300);
    $(".chats_container").hide(300);
    $("#menu").css({"height":"50px"});
    $(".l2").hide();
    $(".l4").hide();
    $(".l3").hide();
    $(".l1").html("<a href='https:///wa.me/2349017872620'>Contact me</a>");
    $(".l5").show();
    $(".calls").css({"border-bottom":"2px solid #fff"});
    $(".status").css({"border-bottom":"0px"});
    $(".chats").css({"border-bottom":"0px"});
    });
    
    
    //SETTINGS
    $(".settings_container").hide();
    $(".l5").click(function(){
    $(".real_chat").hide();
     $(".container").hide(400);
     $(".settings_container").slideToggle(300);
     $("#menu").fadeToggle(300);
     $(".ellip").hide();
    });
    $(".settings_back").click(function(){
    $(".settings_container").slideToggle(400);
        $(".container").show(600);
     $(".ellip").show();
    });
    
    
    //CAMERA
$(".camera_container").hide();
    $(".camera").click(function(){
     $(".container").fadeToggle(400);
     $(".camera_container").show();
     $("#menu").hide();
     $(".ellip").hide();
    });
    $(".camera_back").click(function(){
    $(".camera_container").fadeToggle(400);
        $(".container").fadeToggle(500);
     $(".ellip").show();
    });
    
    
    
    $(".iconsp").hide();
    $(".invi").hide();
    $(".icon1").click(function(){
    $(".iconsp").css({"border-radius":"0px", "background":"url(https://encrypted-tbn1.gstatic.com/images?q=tbn:ANd9GcSVvdf3mtAr8BQaBqwu2wAFbJD1dH6jtmyAK7hZRRnbFc0yc_pT)", "background-size":"cover"});
    $(".iconsp").show();
    $(".invi").show();
    $(".invi").click(function(){
    $(".iconsp").hide();
    $(".invi").hide();
    });
    });
    
    
    
    $(".icon2").click(function(){
    $(".iconsp").css({"border-radius":"0px", "background":"url(https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcT12cP23udqvCqHW_2oAvK257g3oVQkv23tOumxtpfFOhHi8a5B)", "background-size":"cover"});
    $(".iconsp").show();
    $(".invi").show();
    $(".invi").click(function(){
    $(".iconsp").hide();
    $(".invi").hide();
    });
    });
    
    
    $(".icon3").click(function(){
    $(".iconsp").css({"border-radius":"0px", "background":"url(https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcS1rDH_nWadT1GXFPomdutqV1PUMA8uXIWS2Js5_fq4pJ1lwG16)", "background-size":"cover"});
    $(".iconsp").show();
    $(".invi").show();
    $(".invi").click(function(){
    $(".iconsp").hide();
    $(".invi").hide();
    });
    });
    
    
    $(".icon4").click(function(){
    $(".iconsp").css({"border-radius":"0px", "background":"url(https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcQU2JRbbl3LBOm_an3eI5iplFhOoLESyBwUfmWDO49BS1EYuGUE)", "background-size":"cover"});
    $(".iconsp").show();
    $(".invi").show();
    $(".invi").click(function(){
    $(".iconsp").hide();
    $(".invi").hide();
    });
    });
    
    
    
    
    $(".icon5").click(function(){
    $(".iconsp").css({"border-radius":"0px", "background":"url(https://t0.gstatic.com/licensed-image?q=tbn:ANd9GcSUadwflQXaMZhx4HNJ9yjmPkQnKQoKRk4_yuC4WjgjjsAXdV5_QFZERdRTShHG)", "background-size":"cover"});
    $(".iconsp").show();
    $(".invi").show();
    $(".invi").click(function(){
    $(".iconsp").hide();
    $(".invi").hide();
    });
    });
    
    
    
    $(".icon6").click(function(){
    $(".iconsp").css({"border-radius":"0px", "background":"url(https://t2.gstatic.com/licensed-image?q=tbn:ANd9GcQQ840Wk_80H2JjO4wmYQ8VpNzck-GCsmu8a4HqMDNoeZNAH5Zw8qkRZc9a2C9v)", "background-size":"cover"});
    $(".iconsp").show();
    $(".invi").show();
    $(".invi").click(function(){
    $(".iconsp").hide();
    $(".invi").hide();
    });
    });
    
    
    
    $(".icon7").click(function(){
    $(".iconsp").css({"border-radius":"0px", "background":"url(https://t0.gstatic.com/licensed-image?q=tbn:ANd9GcRjhVK6JmLl4J0MwVaAQy11_-b46X7VI81sJIuwf_UEJyg_O-_uChuBqIMSel3d)", "background-size":"cover"});
    $(".iconsp").show();
    $(".invi").show();
    $(".invi").click(function(){
    $(".iconsp").hide();
    $(".invi").hide();
    });
    });
    
    
    
    
    $(".icon8").click(function(){
    $(".iconsp").css({"border-radius":"0px", "background":"url(https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcS0U5a32I81EyodYLVvHBNs7GSlBgmag51JRMz_0RQ2DqthEDKr)", "background-size":"cover"});
    $(".iconsp").show();
    $(".invi").show();
    $(".invi").click(function(){
    $(".iconsp").hide();
    $(".invi").hide();
    });
    });
    
    
    $(".icon9").click(function(){
    $(".iconsp").css({"border-radius":"0px", "background":"url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTyv0aAzhDzlUzFm_5uXSQvVp7GISukmB-2zA&usqp=CAU)", "background-size":"cover"});
    $(".iconsp").show();
    $(".invi").show();
    $(".invi").click(function(){
    $(".iconsp").hide();
    $(".invi").hide();
    });
    });
    
    
    $(".icon10").click(function(){
    $(".iconsp").css({"border-radius":"0px", "background":"url(https://t1.gstatic.com/licensed-image?q=tbn:ANd9GcTFNWogBmphs9qMbvplnItdr9z1nA41VxzHpdxq9n-tigPQjc3-7pPMx83rK0tk)", "background-size":"cover"});
    $(".iconsp").show();
    $(".invi").show();
    $(".invi").click(function(){
    $(".iconsp").hide();
    $(".invi").hide();
    });
    });
    
    
    $(".icon11").click(function(){
    $(".iconsp").css({"border-radius":"0px", "background":"url(https://upload.wikimedia.org/wikipedia/commons/e/e2/Mike_Bloomberg_Headshot.jpg)", "background-size":"cover"});
    $(".iconsp").show();
    $(".invi").show();
    $(".invi").click(function(){
    $(".iconsp").hide();
    $(".invi").hide();
    });
    });
    
    $(".icon12").click(function(){
    $(".iconsp").css({"border-radius":"0px", "background":"url(https://t3.gstatic.com/licensed-image?q=tbn:ANd9GcTkkZVfx7MDl1vS6XBHph7VvTMfETmBQWO4nsvXAq9MFO689TB9HQ7OAhS-1W4I)", "background-size":"cover"});
    $(".iconsp").show();
    $(".invi").show();
    $(".invi").click(function(){
    $(".iconsp").hide();
    $(".invi").hide();
    });
    });
    
    $(".icon13").click(function(){
    $(".iconsp").css({"border-radius":"0px", "background":"url(https://t2.gstatic.com/licensed-image?q=tbn:ANd9GcRTqPkCX1wgKlcE8FnfUjOQCyjayYR9schlFte0f_TvdXLr2F57rdYJov7oaNIe)", "background-size":"cover"});
    $(".iconsp").show();
    $(".invi").show();
    $(".invi").click(function(){
    $(".iconsp").hide();
    $(".invi").hide();
    });
    });
    
    $(".icon14").click(function(){
    $(".iconsp").css({"border-radius":"0px", "background":"url(https://t0.gstatic.com/licensed-image?q=tbn:ANd9GcS5PUoIIwZz81pF5O2LLNZUHjH7S57UlJBDyT5NIaA97Wj4mhFwUplM3-nxx3Dc)", "background-size":"cover"});
    $(".iconsp").show();
    $(".invi").show();
    $(".invi").click(function(){
    $(".iconsp").hide();
    $(".invi").hide();
    });
    });
    
    $(".icon15").click(function(){
    $(".iconsp").css({"border-radius":"0px", "background":"url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSTIGVmUB2OlzA80cf4xtLpc6QCvqdh3rNIpg&usqp=CAU)", "background-size":"cover"});
    $(".iconsp").show();
    $(".invi").show();
    $(".invi").click(function(){
    $(".iconsp").hide();
    $(".invi").hide();
    });
    });
    
    

    
    $(".status_down2").hide();
    $(".view_status_container").hide();
    $(".li_status1").click(function(){
    $(".view_status_container").show();
    $(".view_status_container").css({"background":"url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTzu5NNtYXjTgcixYVxyx5KMuQ1mX3Po9HE-w&usqp=CAU)", "background-size":"cover"});
    $(".view_icon").css({"background":"url(https://source.unsplash.com/random)", "background-size":"cover"});
    $(".status_down2").show();
    $(".status_down").hide();
    $(".view_name").text("My status");
    setTimeout(function(){
    $(".view_status_container").hide();
    $(".status_down").show();
    }, 8000);
    });
    $(".view_back").click(function(){
    $(".view_status_container").hide();
    });
    
    
    
    $(".li_status2").click(function(){
    $(".view_status_container").show();
    $(".view_status_container").css({"background":"url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQfRSUkc_GKvOF71sbbBiwcsOpzjFGKyvFxmw&usqp=CAU)", "background-size":"cover"});
$(".view_icon").css({"background":"url(https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcT12cP23udqvCqHW_2oAvK257g3oVQkv23tOumxtpfFOhHi8a5B)", "background-size":"cover"});
    $(".status_down2").hide();
    $(".status_down").show();
    $(".view_name").text("Bill Gates");
    setTimeout(function(){
    $(".view_status_container").hide();
    $(".status_down").show();
    }, 8000);
    });
    $(".view_back").click(function(){
    $(".view_status_container").hide();
    });
    
    
    $(".li_status3").click(function(){
    $(".view_status_container").show();
    $(".view_status_container").css({"background":"url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRR_qUJAaNKNLsLVVZVX4e7iTG-zYTC0WTeiQ&usqp=CAU)", "background-size":"cover"});
$(".view_icon").css({"background":"url(https://encrypted-tbn1.gstatic.com/images?q=tbn:ANd9GcSVvdf3mtAr8BQaBqwu2wAFbJD1dH6jtmyAK7hZRRnbFc0yc_pT)", "background-size":"cover"});
    $(".status_down2").hide();
    $(".status_down").show();
    $(".view_name").text("Jeff Bezos");
    setTimeout(function(){
    $(".view_status_container").hide();
    $(".status_down").show();
    }, 8000);
    });
    $(".view_back").click(function(){
    $(".view_status_container").hide();
    });
    
    $(".li_status4").click(function(){
    $(".view_status_container").show();
    $(".view_status_container").css({"background":"url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSe-bFZDvwJW0D-xrOxK5GV-WTcI2pRUXsyuA&usqp=CAU)", "background-size":"cover"});
$(".view_icon").css({"background":"url(https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcS1rDH_nWadT1GXFPomdutqV1PUMA8uXIWS2Js5_fq4pJ1lwG16)", "background-size":"cover"});
    $(".status_down2").hide();
    $(".status_down").show();
    $(".view_name").text("Mark Zuckerberg");
    setTimeout(function(){
    $(".view_status_container").hide();
    $(".status_down").show();
    }, 8000);
    });
    $(".view_back").click(function(){
    $(".view_status_container").hide();
    });
    
    
    $(".li_status5").click(function(){
    $(".view_status_container").show();
    $(".view_status_container").css({"background":"url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRkU-vVOPo24W1M4oSoXxvGDIFZ9KZTSrLKeg&usqp=CAU)", "background-size":"cover"});
    $(".status_down2").hide();
    $(".status_down").show();
$(".view_icon").css({"background":"url(https://t2.gstatic.com/licensed-image?q=tbn:ANd9GcQQ840Wk_80H2JjO4wmYQ8VpNzck-GCsmu8a4HqMDNoeZNAH5Zw8qkRZc9a2C9v)", "background-size":"cover"});
    $(".view_name").text("Larry Page");
    setTimeout(function(){
    $(".view_status_container").hide();
    $(".status_down").show();
    }, 8000);
    });
    $(".view_back").click(function(){
    $(".view_status_container").hide();
    });
    
    $(".li_status6").click(function(){
    $(".view_status_container").show();
    $(".view_status_container").css({"background":"url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRx-44eg2xPHvoHlR0gaO7DXRGKO9MGhOKRzw&usqp=CAU)", "background-size":"cover"});
    $(".status_down2").hide();
    $(".status_down").show();
$(".view_icon").css({"background":"url(https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcQU2JRbbl3LBOm_an3eI5iplFhOoLESyBwUfmWDO49BS1EYuGUE)", "background-size":"cover"});
    $(".view_name").text("Elon Musk");
    setTimeout(function(){
    $(".view_status_container").hide();
    $(".status_down").show();
    }, 8000);
    });
    $(".view_back").click(function(){
    $(".view_status_container").hide();
    });
    
    
    $(".li_status7").click(function(){
    $(".view_status_container").show();
    $(".view_status_container").css({"background":"url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT8BZ140TjscTxWdQ_FBN4oDB4Oev3pcU4hgQ&usqp=CAU)", "background-size":"cover"});
    $(".status_down2").hide();
    $(".status_down").show();
$(".view_icon").css({"background":"url(https://t2.gstatic.com/licensed-image?q=tbn:ANd9GcRTqPkCX1wgKlcE8FnfUjOQCyjayYR9schlFte0f_TvdXLr2F57rdYJov7oaNIe)", "background-size":"cover"});
    $(".view_name").text("Rob Walton");
    setTimeout(function(){
    $(".view_status_container").hide();
    $(".status_down").show();
    }, 8000);
    });
    $(".view_back").click(function(){
    $(".view_status_container").hide();
    });
    
    
    $(".li_status8").click(function(){
    $(".view_status_container").show();
    $(".view_status_container").css({"background":"url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRtCQYBPxkZNSajdzTpFwnF71MfXUPVbiKPlw&usqp=CAU)", "background-size":"cover"});
$(".view_icon").css({"background":"url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSTIGVmUB2OlzA80cf4xtLpc6QCvqdh3rNIpg&usqp=CAU)", "background-size":"cover"});
    $(".status_down2").hide();
    $(".status_down").show();
    $(".view_name").text("Carlos Slim");
    setTimeout(function(){
    $(".view_status_container").hide();
    $(".status_down").show();
    }, 8000);
    });
    $(".view_back").click(function(){
    $(".view_status_container").hide();
    });
    
    
    $(".li_status9").click(function(){
    $(".view_status_container").show();
    $(".view_status_container").css({"background":"url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRoVKUCMLAD3UNvsmDkMr4azr3c2D-rYJsE9g&usqp=CAU)", "background-size":"cover"});
$(".view_icon").css({"background":"url(https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcS0U5a32I81EyodYLVvHBNs7GSlBgmag51JRMz_0RQ2DqthEDKr)", "background-size":"cover"});
    $(".status_down2").hide();
    $(".status_down").show();
    $(".view_name").text("Warren Buffet");
    setTimeout(function(){
    $(".view_status_container").hide();
    $(".status_down").show();
    }, 8000);
    });
    $(".view_back").click(function(){
    $(".view_status_container").hide();
    });
    
    
    
    
    var d = new Date();
 var h = d.getHours(); 
 var t = d.getMinutes();
  h = (h <10) ? "0" + h : h;
 t = (t <10) ? "0" + t : t;
 if(h>12){
    h=h-12;
 }else{
    h=h;
 }
 time= h+":"+t;
    
    
    
    
    
    $(".real_chat").hide();
    $(".person1").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://encrypted-tbn1.gstatic.com/images?q=tbn:ANd9GcSVvdf3mtAr8BQaBqwu2wAFbJD1dH6jtmyAK7hZRRnbFc0yc_pT)", "background-size":"cover"});
    $(".real_chat_name").text("Jeff Bezos");
    $(".container").hide();
    $(".rechats").text("Hi, we need an update to our website");
    $(".time_msgt").css({"color":"dimgrey"});
    $(".msgcol1").hide();
    $(".rtime").text(time);
    });
    
    $(".msg1").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://encrypted-tbn1.gstatic.com/images?q=tbn:ANd9GcSVvdf3mtAr8BQaBqwu2wAFbJD1dH6jtmyAK7hZRRnbFc0yc_pT)", "background-size":"cover"});
    $(".real_chat_name").text("Jeff Bezos");
    $(".container").hide();
    $(".rechats").text("Hi, we need an update to our website");
    $(".time_msgt").css({"color":"dimgrey"});
    $(".msgcol1").hide();
    $(".rtime").text(time);
    });
    
    
    
    
    
    $(".person2").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcT12cP23udqvCqHW_2oAvK257g3oVQkv23tOumxtpfFOhHi8a5B)", "background-size":"cover"});
    $(".real_chat_name").text("Bill Gates");
    $(".container").hide();
    $(".rechats").text("Yes, but the alert has not yet arrived");
    $(".time_msg1").css({"color":"dimgrey"});
    $(".msgcol2").hide();
    $(".rtime").text(time);
    });
    
    $(".msg2").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcT12cP23udqvCqHW_2oAvK257g3oVQkv23tOumxtpfFOhHi8a5B)", "background-size":"cover"});
    $(".real_chat_name").text("Bill Gates");
    $(".container").hide();
    $(".rechats").text("Yes, but the alert has not yet arrived");
    $(".time_msg1").css({"color":"dimgrey"});
    $(".msgcol2").hide();
    $(".rtime").text(time);
    });
    
    
    
    
    
    $(".person3").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcS1rDH_nWadT1GXFPomdutqV1PUMA8uXIWS2Js5_fq4pJ1lwG16)", "background-size":"cover"});
    $(".real_chat_name").text("Mark Zuckerb...");
    $(".container").hide();
    $(".rechats").text("I called you yesterday, but you did not pick my call🙄");
    $(".time_msg2").css({"color":"dimgrey"});
    $(".msgcol3").hide();
    $(".rtime").text(time);
    });
    
    $(".msg3").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcS1rDH_nWadT1GXFPomdutqV1PUMA8uXIWS2Js5_fq4pJ1lwG16)", "background-size":"cover"});
    $(".real_chat_name").text("Mark Zuckerb...");
    $(".container").hide();
    $(".rechats").text("I called you yesterday, but you did not pick my call🙄");
    $(".time_msg2").css({"color":"dimgrey"});
    $(".msgcol3").hide();
    $(".rtime").text(time);
    });
    
    
    
    
    
    
    $(".person4").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcQU2JRbbl3LBOm_an3eI5iplFhOoLESyBwUfmWDO49BS1EYuGUE)", "background-size":"cover"});
    $(".real_chat_name").text("Elon Musk");
    $(".container").hide();
    $(".rechats").text("Hello Dev Parth, i saw the updates");
    $(".time_msg3").css({"color":"dimgrey"});
    $(".msgcol4").hide();
    $(".rtime").text(time);
    });
    
    $(".msg4").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcQU2JRbbl3LBOm_an3eI5iplFhOoLESyBwUfmWDO49BS1EYuGUE)", "background-size":"cover"});
    $(".real_chat_name").text("Elon Musk");
    $(".container").hide();
    $(".rechats").text("Hello Dev Parth, i saw the updates");
    $(".time_msg3").css({"color":"dimgrey"});
    $(".msgcol4").hide();
    $(".rtime").text(time);
    });
    
    
    
    
    
    
    
    $(".person5").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://t0.gstatic.com/licensed-image?q=tbn:ANd9GcSUadwflQXaMZhx4HNJ9yjmPkQnKQoKRk4_yuC4WjgjjsAXdV5_QFZERdRTShHG)", "background-size":"cover"});
    $(".real_chat_name").text("Larry Ellison");
    $(".container").hide();
    $(".rechats").text("yes i saw the mail, I'm on my from the town");
    $(".real_today").text("Yesterday");
    $(".rtime").text(time);
    });
    
    $(".msg5").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://t0.gstatic.com/licensed-image?q=tbn:ANd9GcSUadwflQXaMZhx4HNJ9yjmPkQnKQoKRk4_yuC4WjgjjsAXdV5_QFZERdRTShHG)", "background-size":"cover"});
    $(".real_chat_name").text("Larry Ellison");
    $(".container").hide();
    $(".rechats").text("yes i saw the mail, I'm on my from the town");
    $(".real_today").text("Yesterday");
    $(".rtime").text(time);
    });
    
    
    
    
    
    
    
    
    
    $(".person6").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://t2.gstatic.com/licensed-image?q=tbn:ANd9GcQQ840Wk_80H2JjO4wmYQ8VpNzck-GCsmu8a4HqMDNoeZNAH5Zw8qkRZc9a2C9v)", "background-size":"cover"});
    $(".real_chat_name").text("Larry Page");
    $(".container").hide();
    $(".rechats").text("Hi Dev Parth, I need a loan from you!!");
    $(".real_today").text("Yesterday");
    $(".rtime").text(time);
    });
    
    $(".msg6").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://t2.gstatic.com/licensed-image?q=tbn:ANd9GcQQ840Wk_80H2JjO4wmYQ8VpNzck-GCsmu8a4HqMDNoeZNAH5Zw8qkRZc9a2C9v)", "background-size":"cover"});
    $(".real_chat_name").text("Larry Page");
    $(".container").hide();
    $(".rechats").text("Hi Dev Parth, I need a loan from you!!");
    $(".real_today").text("Yesterday");
    $(".rtime").text(time);
    });
    
    
    
    
    
    
    
    
    $(".person7").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://t0.gstatic.com/licensed-image?q=tbn:ANd9GcRjhVK6JmLl4J0MwVaAQy11_-b46X7VI81sJIuwf_UEJyg_O-_uChuBqIMSel3d)", "background-size":"cover"});
    $(".real_chat_name").text("Sergey Brin");
    $(".container").hide();
    $(".rechats").text("I want you to be our frontend developer for our company");
    $(".real_today").text("Yesterday");
    $(".rtime").text(time);
    });
    
    $(".msg7").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://t0.gstatic.com/licensed-image?q=tbn:ANd9GcRjhVK6JmLl4J0MwVaAQy11_-b46X7VI81sJIuwf_UEJyg_O-_uChuBqIMSel3d)", "background-size":"cover"});
    $(".real_chat_name").text("Sergey Brin");
    $(".container").hide();
    $(".rechats").text("I want you to be our frontend developer for our company");
    $(".real_today").text("Yesterday");
    $(".rtime").text(time);
    });
    
    
    
    
    
    
    
    $(".person8").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcS0U5a32I81EyodYLVvHBNs7GSlBgmag51JRMz_0RQ2DqthEDKr)", "background-size":"cover"});
    $(".real_chat_name").text("Warren Buffet");
    $(".container").hide();
    $(".rechats").text("I'm trying to send you back the $380M");
    $(".real_today").text("Yesterday");
    $(".rtime").text(time);
    });
    
    $(".msg8").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcS0U5a32I81EyodYLVvHBNs7GSlBgmag51JRMz_0RQ2DqthEDKr)", "background-size":"cover"});
    $(".real_chat_name").text("Warren Buffet");
    $(".container").hide();
    $(".rechats").text("I'm trying to send you back the $380M");
    $(".real_today").text("Yesterday");
    $(".rtime").text(time);
    });
    
    
    
    
    
    $(".person9").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTyv0aAzhDzlUzFm_5uXSQvVp7GISukmB-2zA&usqp=CAU)", "background-size":"cover"});
    $(".real_chat_name").text("Alice Walton");
    $(".container").hide();
    $(".rechats").text("Good job! Dev Parth, glad to see your code");
    $(".real_today").text("December");
    $(".rtime").text(time);
    });
    
    $(".msg9").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTyv0aAzhDzlUzFm_5uXSQvVp7GISukmB-2zA&usqp=CAU)", "background-size":"cover"});
    $(".real_chat_name").text("Alice Walton");
    $(".container").hide();
    $(".rechats").text("Good job! Dev Parth, glad to see your code");
    $(".real_today").text("December");
    $(".rtime").text(time);
    });
    
    
    
    
    
    
    $(".person10").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://t1.gstatic.com/licensed-image?q=tbn:ANd9GcTFNWogBmphs9qMbvplnItdr9z1nA41VxzHpdxq9n-tigPQjc3-7pPMx83rK0tk)", "background-size":"cover"});
    $(".real_chat_name").text("Jim Walton");
    $(".container").hide();
    $(".rechats").text("I have a serious issue with you, please i want to see you tommorrow");
    $(".real_today").text("December");
    $(".rtime").text(time);
    });
    
    $(".msg10").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://t1.gstatic.com/licensed-image?q=tbn:ANd9GcTFNWogBmphs9qMbvplnItdr9z1nA41VxzHpdxq9n-tigPQjc3-7pPMx83rK0tk)", "background-size":"cover"});
    $(".real_chat_name").text("Jim Walton");
    $(".container").hide();
    $(".rechats").text("I have a serious issue with you, please i want to see you tommorrow");
    $(".real_today").text("December");
    $(".rtime").text(time);
    });
    
    
    
    
    $(".person11").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://upload.wikimedia.org/wikipedia/commons/e/e2/Mike_Bloomberg_Headshot.jpg)", "background-size":"cover"});
    $(".real_chat_name").text("Michael Bloo...");
    $(".container").hide();
    $(".rechats").text("it was very very nice, thank you so much");
    $(".real_today").text("December");
    $(".rtime").text(time);
    });
    
    $(".msg11").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://upload.wikimedia.org/wikipedia/commons/e/e2/Mike_Bloomberg_Headshot.jpg)", "background-size":"cover"});
    $(".real_chat_name").text("Michael Bloo...");
    $(".container").hide();
    $(".rechats").text("it was very very nice, thank you so much");
    $(".real_today").text("December");
    $(".rtime").text(time);
    });
    
    
    
    
    
    
    $(".person12").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://t3.gstatic.com/licensed-image?q=tbn:ANd9GcTkkZVfx7MDl1vS6XBHph7VvTMfETmBQWO4nsvXAq9MFO689TB9HQ7OAhS-1W4I)", "background-size":"cover"});
    $(".real_chat_name").text("Mukesh Amb...");
    $(".container").hide();
    $(".rechats").text("Thank you bhai😊, i'll meet you tommorrow");
    $(".real_today").text("December");
    $(".rtime").text(time);
    });
    
    $(".msg12").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://t3.gstatic.com/licensed-image?q=tbn:ANd9GcTkkZVfx7MDl1vS6XBHph7VvTMfETmBQWO4nsvXAq9MFO689TB9HQ7OAhS-1W4I)", "background-size":"cover"});
    $(".real_chat_name").text("Mukesh Amb...");
    $(".container").hide();
    $(".rechats").text("Thank you bhai😊, i'll meet you tommorrow");
    $(".real_today").text("December");
    $(".rtime").text(time);
    });
    
    
    
    
    $(".person13").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://t2.gstatic.com/licensed-image?q=tbn:ANd9GcRTqPkCX1wgKlcE8FnfUjOQCyjayYR9schlFte0f_TvdXLr2F57rdYJov7oaNIe)", "background-size":"cover"});
    $(".real_chat_name").text("Rob Walton");
    $(".container").hide();
    $(".rechats").text("Okay, no problem i'll come as soon as possible");
    $(".real_today").text("December");
    $(".rtime").text(time);
    });
    
    $(".msg13").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://t2.gstatic.com/licensed-image?q=tbn:ANd9GcRTqPkCX1wgKlcE8FnfUjOQCyjayYR9schlFte0f_TvdXLr2F57rdYJov7oaNIe)", "background-size":"cover"});
    $(".real_chat_name").text("Rob Walton");
    $(".container").hide();
    $(".rechats").text("Okay, no problem i'll come as soon as possible");
    $(".real_today").text("December");
    $(".rtime").text(time);
    });
    
    
    
    
    $(".person14").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://t0.gstatic.com/licensed-image?q=tbn:ANd9GcS5PUoIIwZz81pF5O2LLNZUHjH7S57UlJBDyT5NIaA97Wj4mhFwUplM3-nxx3Dc)", "background-size":"cover"});
    $(".real_chat_name").text("Carlos Slim");
    $(".container").hide();
    $(".rechats").text("are you done with the project please? ");
    $(".real_today").text("December");
    $(".rtime").text(time);
    });
    
    $(".msg14").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://t0.gstatic.com/licensed-image?q=tbn:ANd9GcS5PUoIIwZz81pF5O2LLNZUHjH7S57UlJBDyT5NIaA97Wj4mhFwUplM3-nxx3Dc)", "background-size":"cover"});
    $(".real_chat_name").text("Carlos Slim");
    $(".container").hide();
    $(".rechats").text("are you done with the project please? ");
    $(".real_today").text("December");
    $(".rtime").text(time);
    });
    
    
    
    $(".person15").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSTIGVmUB2OlzA80cf4xtLpc6QCvqdh3rNIpg&usqp=CAU)", "background-size":"cover"});
    $(".real_chat_name").text("Warren Buffet");
    $(".container").hide();
    $(".rechats").text("i'll be back to you before 12:00 AM");
    $(".real_today").text("December");
    $(".rtime").text(time);
    });
    
    $(".msg15").click(function(){
    $(".real_chat").show();
    $(".real_chat_icon").css({"background":"url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSTIGVmUB2OlzA80cf4xtLpc6QCvqdh3rNIpg&usqp=CAU)", "background-size":"cover"});
    $(".real_chat_name").text("Warren Buffet");
    $(".container").hide();
    $(".rechats").text("i'll be back to you before 12:00 AM");
    $(".real_today").text("December");
    $(".rtime").text(time);
    });
    
    
    
    $(".real_chat").click(function(){
    $("#menu").hide();
    });
    $(".real_chat_back").click(function(){
    $("#menu").hide();
    $("#schat").remove();
    $("#rchat").remove();
    $(".real_chat").hide();
    $(".container").show();
    });
    
    </script>
    
    
    </body>
</html>
