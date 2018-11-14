<template>
<div class="container">

  <button type="button" class="btn btn-info pull-left" onclick="history.back()"style="margin-bottom:20px;" >목록</button>
  <div style="margin-top:20px;">
    <table class="table table-bordered" >
    <thead>
     <tr>
       <th>탐지 일시</th>
       <th>최초 VOC</th>
       <th>관련 VOC 건수</th>
       <th>도메인</th>
       <th>키워드1</th>
       <th>키워드2</th>
     </tr>
     </thead>
     <tbody>
     <tr>
       <td>2018.10.29</br>[14:18:22]</td>
       <td>14:15:30</td>
       <td>유선BSS</td>
       <td>로그인</td>
       <td>접속불가</td>
       <td>...</td>
     </tr>
    </tbody>
    </table>
</div>

  <div style="margin-top:40px;">
      <h4>이상징후 발견 VOC 목록</h4>
    <table class="table table-bordered">
    <thead>
     <tr>
       <th>상담 ID</th>
       <th>접수구분</th>
       <th>접수시간</th>
       <th>요청자</th>
       <th>요청자 조직</th>
       <th>내용</th>
     </tr>
     </thead>
     <tbody>
     <tr>
       <td>SRM18070385441</td>
       <td>CALL</td>
       <td>14:18:22</td>
       <td>홍길동</td>
       <td>조직명</td>
       <td>상담사 작성 내용..</td>
     </tr>
    </tbody>
    </table>
  </div>
</div>
</template>

<style scoped>
th {
  background-color: rgb(153, 152, 149);
}

td{

    valign : middle;
}

 th,td {
   width : 100px;
   text-align: center;

 }

</style>
<script>
  export default {
    data(){
      return {
        msg:'Example Vue'
      };
    },
    mounted() {
      console.log('Component mounted.')
    }
  }
</script>
