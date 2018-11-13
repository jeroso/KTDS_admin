<template>
<div class="container">
  <h2>이상 징후</h2>

  <div class="input-group" style=" margin: auto;">
    <span class="input-group-btn" style="width:300px; ">
   <input type="text" class="form-control" style="text-align: center;" placeholder="조회일자">
      <button class="btn btn-primary" type="button">조회</button>
    </span>
  </div>
  <div style="margin-top:20px;">
    <table class="table table-bordered table-hover">
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
       <td>1</td>
       <td>2</td>
       <td><router-link to="/">3</router-link></td>
       <td>4</td>
       <td>5</td>
       <td>6</td>
     </tr>
    </tbody>
    <tbody>
      <tr>
       <td>1</td>
       <td>2</td>
       <td>3</td>
       <td>4</td>
       <td>5</td>
       <td>6</td>

     </tr>
     </tbody>
     <tbody>
      <tr>
       <td>1</td>
       <td>2</td>
       <td>3</td>
       <td>4</td>
       <td>5</td>
       <td>6</td>
     </tr>
     </tbody>
    </table>
</div>
</div>
</template>

<style scoped>
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
