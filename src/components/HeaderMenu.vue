<template>
  <div class="container">
      <div class="header">
        <h1><a href=""><img src="../../public/images/header_images/new_logo.svg" alt=""></a></h1>
        <div class="gnd">
          <ul class="nav_icon">
            <li>
              <a href="">
                <i class="fa-solid fa-magnifying-glass"></i>
                
                
              </a>
            </li>
            <li>
              <a href="">
                <i class="fa-regular fa-user"></i>
                <i class="fal fa-user" aria-hidden="true"></i>
                
              </a>
            </li>
            <li>
              <a href="">
                <i class="fa-brands fa-facebook"></i>
              </a>
            </li>
            <li>
              <a href="">

              </a>
            </li>
            <li>
              <a href="">

              </a>
            </li>
          </ul>
          <ul class="nav_menu">
            <li><a href="">제이에이코리아</a></li>
            <li><a href="">투명경영</a></li>
            <li><a href="">교육사업</a></li>
            <li><a href="">기관소식</a></li>
            <li><a href="">후원하기</a></li>
          </ul>
        </div>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
  .header{
    height: 121px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: skyblue;
  }

  .header h1 img{
    width: 218px;
  }

  .gnd{
    margin-right: 222px;
  }
  .gnd .nav_icon{
    padding-top: 18px;
    display: flex;
    justify-content: end;
    align-items: center;
  }
  .gnd .nav_icon i{
    font-size: 20px;
   
  }
  .gnd .nav_menu{
    display: flex;
    justify-content: center;
    align-items: center;
  }
  
  .gnd .nav_menu a{
    font-size: 19px;
    font-weight: bold;
  }
</style>