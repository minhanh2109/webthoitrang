# webthoitrang
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, Helvetica, sans-serif;
}
li{
    list-style: none;
}
a{
    text-decoration: none;
    color: #000;
}
header{
    display: flex;
    justify-content: space-between;
    padding: 12px 50px;
    height: 70px;
    align-items: center;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    z-index: 1;
    background: rgba(255, 255, 255, 0.3);
}
header.sticky{
    background: rgba(255, 255, 255, 1);
}
header:hover{
    background: rgba(255, 255, 255, 1);
}
.logo{
    flex: 1;
}
.menu{
    flex: 3;
    display: flex;
}
.menu > li {
    padding: 0 12px;
    position: relative;
}
.menu > li:hover .sub-menu {
    visibility: visible;
    top: 45px;
}
.sub-menu{
    position: absolute;
    width: 150px;
    border: 1px solid #ccc;
    padding: 10px 0 10px 20px;
    visibility: hidden;
    top: 60px;
    transition: 0.3s;
    z-index: 1;
    background: #fff;
}
.sub-menu ul{
    padding-left: 20px;
}
.sub-menu ul a{
    font-weight: normal!important;
    font-size: 12px!important;
}
.menu li a{
    font-size: 12px;
    font-weight: bold!important;
    display: block;
    line-height: 20px;
}
.others {
    flex: 1;
    display: flex;
}
.others > li{
    padding: 0 12px;
    position: relative;
}
.others > li::after{
    content: "";
    display: block;
    width: 1px;
    height: 50%;
    background: #ccc;
    position: absolute;
    right: 0;
    top: 50%;
    transform: translateY(-50%);
}
.others > li:last-child::after{
    display: none;
}
.others > li:first-child{
    position: relative;
}
.others > li:first-child input{
    width: 100%;
    border: none;
    border-bottom: 1px solid #333;
    background: transparent;
    outline: none;
}
.others > li:first-child i {
    position: absolute;
    right: 10px;
}
#Slider{
    padding-bottom:30px ;
    border-bottom: 2px solid #000;
    overflow: hidden;
}
.aspect-ratio-169 {
    display: block;
    position: relative;
    padding-top: 56.25%;
    transition: 0.3s;
}
.aspect-ratio-169 img {
    display: block;
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
}
.dot-container{
    position: absolute;
    height: 30px;
    width: 100%;
    display: flex;
    align-items: center;
    text-align: center;
    justify-content: center;
}
.dot{
    height: 16px;
    width: 16px;
    background-color: #ccc;
    border-radius: 50%;
    margin-right: 12px;
}
.dot.active{
    background-color: #333;
}
/*..............appp....................*/
.app-container{
    text-align: center;
    align-items: center;
    padding: 150px 0 50px 0;
}
.app-google{
    margin: 50px;
} 
.app-google img{
    height: 50px;
}
.app-container p{
    line-height: 20px;
    letter-spacing: 1px;
    font-size: 17px;
    color: #000;
    font-weight: bold;
}
.app-container input{
    margin-top: 50px;
    border: none;
    border-bottom: 1px solid #000;
    padding-bottom: 20px;
    width: 400px;
    text-align: center;
    outline: none;
}
/*..............footer....................*/
footer{
    text-align: center;
}
.footer-top{
    display: flex;
    text-align: center;
    justify-content: center;
    align-items: center;
    margin-bottom: 20px;
    height: 70px;
}
.footer-top img{
    height: 50px;
}
.footer-top li{
    padding: 0 12px;
    position: relative;
}
.footer-top li::after{
    content: "";
    display: block;
    width: 1px;
    height: 80%;
    background: #ccc;
    position: absolute;
    right: 0;
    top: 50%;
    transform: translateY(-50%);
}
.footer-top li:last-child::after{
    display: none;
}
.footer-top li:last-child a{
    margin-right: 12px;
    color: #333;
}
.footer-center{
    text-align: center;
}
.footer-bottom{
    margin: 20px 0;
    text-align: center;
}
