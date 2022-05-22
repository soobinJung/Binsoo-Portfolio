<template>
<div style="font-family: BMEULJIROTTF;">
  <div style="width: 90%; padding : 0 0 20px 50px">
      <span style="font-size : 25px"> 제가 소중하게 다루는 개발책들을 소개할께요 👩‍🚀  </span>
  </div>
  <div style = "width: 97%; height: 500px; margin : 0 0 50px 30px; ">

    <div class="image-box" style = "width: 255px; height: 500px; border : 1px solid #ffadad; margin : 22px; float : left; text-align : center; border-radius : 50px">
      <div style="height : 44px; padding : 21px 0 0 0; background : rgb(253, 226, 226); border-radius : 50px 50px 0 0; font-size: 19px">C 언어 알고리즘</div>
      <img class="image-thumbnail" :src="book1" style="width: 250px; height: 300px;"/>
      <div style="padding : 10px 0 0 0"> 
        <span> 개발 시작하고 세번째로 읽은 책, <br> 어떤 문제를 마주했을 때 어떤 태도로  <br>접근해야 하는지 가르쳐준 책이에요</span>
      </div>
    </div>

    <div class="image-box" style = "width: 255px; height: 500px; border : 1px solid #ffadad; margin : 22px; float : left; text-align : center; border-radius : 50px">
      <div style="height : 44px; padding : 21px 0 0 0; background : rgb(253, 226, 226); border-radius : 50px 50px 0 0; font-size: 19px"> JAVA 알고리즘 </div>
      <img class="image-thumbnail" :src="book2" style="width: 250px; height: 300px;"/>
      <div style="padding : 10px 0 0 0"> 
        <span> C 알고리즘과 같은 문제를 <br> Java는 어떤식으로 접근하는지 <br> 호기심에 같은문제 두번 끙끙 .. </span>
      </div>
    </div>

    <div class="image-box" style = "width: 255px; height: 500px; border : 1px solid #ffadad; margin : 22px; float : left; text-align : center; border-radius : 50px">
      <div style="height : 44px; padding : 21px 0 0 0; background : rgb(253, 226, 226); border-radius : 50px 50px 0 0; font-size: 19px"> 웹 API 디자인 </div>
      <img class="image-thumbnail" :src="book3" style="width: 250px; height: 300px;"/>
      <div style="padding : 10px 0 0 0"> 
        <span> API 를 개발할 때 어떻게 개발해야 <br> 사용자가 잘 이용할 수 있을까 ? <br> 라는 고민을 할 때 꼼꼼히 읽은 책이에요 </span>
      </div>
    </div>
    

    <div class="image-box" style = "width: 255px; height: 500px; border : 1px solid #ffadad; margin : 22px; float : left; text-align : center; border-radius : 50px">
      <div style="height : 44px; padding : 21px 0 0 0; background : rgb(253, 226, 226); border-radius : 50px 50px 0 0; font-size: 19px">스프링</div>
      <img class="image-thumbnail" :src="book6" style="width: 250px; height: 300px;"/>
      <div style="padding : 10px 0 0 0"> 
        <span> 스프링을 처음 시작할 때 읽은책인데 <br> 처음에는 정말 이해 안되었던 부분들이 많았는데 다시 펼쳐보니 저는 스프링 세계에 들어와있 ..어요 !</span>
      </div>
    </div>

    <div class="image-box" style = "width: 255px; height: 500px; border : 1px solid #ffadad; margin : 22px; float : left; text-align : center; border-radius : 50px">
      <div style="height : 44px; padding : 21px 0 0 0; background : rgb(253, 226, 226); border-radius : 50px 50px 0 0; font-size: 19px">스프링 + VUE 웹개발</div>
      <img class="image-thumbnail" :src="book5" style="width: 250px; height: 300px;"/>
      <div style="padding : 10px 0 0 0"> 
        <span>제가 좋아하는 언어 <br> 두 개를 합친 책이어서 <br> 바로 결제 쓱 -, 완독 쓱 - <br>업무 적용 100% !</span>
      </div>
    </div>


    <div class="image-box" style = "width: 255px; height: 500px; border : 1px solid #ffadad; margin : 22px; float : left; text-align : center; border-radius : 50px">
      <div style="height : 44px; padding : 21px 0 0 0; background : rgb(253, 226, 226); border-radius : 50px 50px 0 0; font-size: 19px">JPA</div>
      <img class="image-thumbnail" :src="book15" style="width: 250px; height: 300px;"/>
      <div style="padding : 10px 0 0 0"> 
        <span>JPA 책을 읽고 <br> 부장님께 저희도 JPA 도입하자고  <br>  말씀드렸는데 안되나봐요 ..  </span>
      </div>
    </div>
    
    
    <div class="image-box" style = "width: 255px; height: 500px; border : 1px solid #ffadad; margin : 22px; float : left; text-align : center; border-radius : 50px">
      <div style="height : 44px; padding : 21px 0 0 0; background : rgb(253, 226, 226); border-radius : 50px 50px 0 0; font-size: 19px">객체지향 설계</div>
      <img class="image-thumbnail" :src="book4" style="width: 250px; height: 300px;"/>
      <div style="padding : 10px 0 0 0"> 
        <span> 객체지향을 코드로 <br> 구현하는 여러가지 예를 보여주는데 <br> 역할, 책임, 협력을 코드로 배웠어요 </span>
      </div>
    </div>
    

    <div class="image-box" style = "width: 255px; height: 500px; border : 1px solid #ffadad; margin : 22px; float : left; text-align : center; border-radius : 50px">
      <div style="height : 44px; padding : 21px 0 0 0; background : rgb(253, 226, 226); border-radius : 50px 50px 0 0; font-size: 19px">객체지향의 사실과 오해</div>
      <img class="image-thumbnail" :src="book7" style="width: 250px; height: 300px;"/>
      <div style="padding : 10px 0 0 0"> 
        <span>객체지향을 엘리스로 비유하여 설명해줬는데 역할, 책임, 협력을 상상하며 배웠어요 <br> 두고두고 챙겨보는 책</span>
      </div>
    </div>

    <div class="image-box" style = "width: 255px; height: 500px; border : 1px solid #ffadad; margin : 22px; float : left; text-align : center; border-radius : 50px">
      <div style="height : 44px; padding : 21px 0 0 0; background : rgb(253, 226, 226); border-radius : 50px 50px 0 0; font-size: 19px">JSP / Servlet</div>
      <img class="image-thumbnail" :src="book8" style="width: 250px; height: 300px;"/>
      <div style="padding : 10px 0 0 0"> 
        <span> 입문할 때만 보고 안보게 되더라고요 <br> jsp 를 기반으로 구현된 <br> 더 멋진 언어들이 많으니 !!!</span>
      </div>
    </div>

  

    <div class="image-box" style = "width: 255px; height: 500px; border : 1px solid #ffadad; margin : 22px; float : left; text-align : center; border-radius : 50px">
      <div style="height : 44px; padding : 21px 0 0 0; background : rgb(253, 226, 226); border-radius : 50px 50px 0 0; font-size: 19px">Git</div>
      <img class="image-thumbnail" :src="book12" style="width: 250px; height: 300px;"/>
      <div style="padding : 10px 0 0 0"> 
        <span> git 명령어 좀 이해하고 쓰고 싶었어요 <br> 덕분에 팀에서 git 도입하고 <br> 내가 메뉴얼만듬 !!</span>
      </div>
    </div>

    <div class="image-box" style = "width: 255px; height: 500px; border : 1px solid #ffadad; margin : 22px; float : left; text-align : center; border-radius : 50px">
      <div style="height : 44px; padding : 21px 0 0 0; background : rgb(253, 226, 226); border-radius : 50px 50px 0 0; font-size: 19px">대규모 시스템 설계기초</div>
      <img class="image-thumbnail" :src="book13" style="width: 250px; height: 300px;"/>
      <div style="padding : 10px 0 0 0"> 
        <span> 개발 잘하는 선배들이랑 스터디 했는데 <br> 나도 덩달아 보는 설계 구조에 대한 <br> 시야가 넓어지게 되었어요</span>
      </div>
    </div>

    <div class="image-box" style = "width: 255px; height: 500px; border : 1px solid #ffadad; margin : 22px; float : left; text-align : center; border-radius : 50px">
      <div style="height : 44px; padding : 21px 0 0 0; background : rgb(253, 226, 226); border-radius : 50px 50px 0 0; font-size: 19px">컴공지식</div>
      <img class="image-thumbnail" :src="book14" style="width: 250px; height: 300px;"/>
      <div style="padding : 10px 0 0 0"> 
        <span> 컴퓨터를 처음 배울 때 <br> 코딩으로 배워서 몰랐던 내용들을<br>  이 책이 알려줬어요</span>
      </div>
    </div>
  


    <div class="image-box" style = "width: 255px; height: 500px; border : 1px solid #ffadad; margin : 22px; float : left; text-align : center; border-radius : 50px">
      <div style="height : 44px; padding : 21px 0 0 0; background : rgb(253, 226, 226); border-radius : 50px 50px 0 0; font-size: 19px">C언어 기초</div>
      <img class="image-thumbnail" :src="book16" style="width: 250px; height: 300px;"/>
      <div style="padding : 10px 0 0 0"> 
        <span> 저한테 있어서 제일 소중한 책이에요 <br> 내 적성을 찾을 수 있도록 도와준 감사한 '컴맹을 위한 C 언어' </span>
      </div>
    </div>

    <div class="image-box" style = "width: 255px; height: 500px; border : 1px solid #ffadad; margin : 22px; float : left; text-align : center; border-radius : 50px">
      <div style="height : 44px; padding : 21px 0 0 0; background : rgb(253, 226, 226); border-radius : 50px 50px 0 0; font-size: 19px"> 알고리즘 기초 </div>
      <img class="image-thumbnail" :src="book9" style="width: 250px; height: 300px;"/>
      <div style="padding : 10px 0 0 0"> 
        <span> C 알고리즘 책을 먼저 읽었는데 <br> 이해가 가지 않아 기초부터 <br>차근차근 공부했어요 </span>
      </div>
    </div>



    <div class="image-box" style = "width: 255px; height: 500px; border : 1px solid #ffadad; margin : 22px; float : left; text-align : center; border-radius : 50px">
      <div style="height : 44px; padding : 21px 0 0 0; background : rgb(253, 226, 226); border-radius : 50px 50px 0 0; font-size: 19px">프론트엔드 이해</div>
      <img class="image-thumbnail" :src="book10" style="width: 250px; height: 300px;"/>
      <div style="padding : 10px 0 0 0"> 
        <span> 회사에서 프론트엔드 개발이 할당되는데 <br> 물어볼 곳도 없어서 .. 샀어요 <br> 덕분에 설정부터 꼼꼼히 <br> 리팩토링 할 수 있었어요 </span>
      </div>
    </div>


    <div class="image-box" style = "width: 255px; height: 500px; border : 1px solid #ffadad; margin : 22px; float : left; text-align : center; border-radius : 50px">
      <div style="height : 44px; padding : 21px 0 0 0; background : rgb(253, 226, 226); border-radius : 50px 50px 0 0; font-size: 19px">VueJs</div>
      <img class="image-thumbnail" :src="book11" style="width: 250px; height: 300px;"/>
      <div style="padding : 10px 0 0 0"> 
        <span> Vue 는 제가 자신있는 언어에요 <br> 이 책 덕분에 기초가 탄탄해져서 <br> Vue 의 왠만한 요구사항은 <br> 구현 가능해졌어요 </span>
      </div>
    </div>

  </div>
</div>
</template>

<script>
export default {
  name : "Binsoo Book"
  , data () {
    return {
      book1 : require('./../../assets/book/a1.png')
      , book2 : require('./../../assets/book/a2.png')
      , book3 : require('./../../assets/book/a3.png')
      , book4 : require('./../../assets/book/a4.png')
      , book5 : require('./../../assets/book/a5.png')
      , book6 : require('./../../assets/book/a6.png')
      , book7 : require('./../../assets/book/a7.png')
      , book8 : require('./../../assets/book/a8.png')
      , book9 : require('./../../assets/book/a9.png')
      , book10 : require('./../../assets/book/a10.png')
      , book11 : require('./../../assets/book/a11.png')
      , book12 : require('./../../assets/book/a12.png')
      , book13 : require('./../../assets/book/a13.png')
      , book14 : require('./../../assets/book/a14.png')
      , book15 : require('./../../assets/book/a15.png')
      , book16 : require('./../../assets/book/a16.png')
    }
  }
}
</script>

<style>
.image-box {
    width:380px;
    height:220px;
    overflow:hidden;
    margin:0 auto;
}

.image-thumbnail {
    width:100%;
    height:100%;
    object-fit:cover;
    padding: 30px 0 0 0;
}
</style>