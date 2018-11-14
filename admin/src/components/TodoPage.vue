<template>
<div class="container">
  <h2>이상 징후</h2>

  <div class="input-group" style=" margin: auto;">
    <span class="input-group-btn" style="width:300px; ">
   <input type="text" class="form-control" style="text-align: center;" placeholder="조회일자">
      <button id="search" class="btn btn-primary" type="button" @click="search(date)">조회</button>
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

     <!-- <tbody v-if="search(date)!=null"> -->
     <tbody v-for="(todo,index) in todos">
      <tr>
         <td>{{todo.date}}</td>
         <td>{{todo.sVOC}}</td>
         <td><router-link to="/todos2">{{todo.cVOC}}</router-link></td>
         <td>{{todo.domain}}</td>
         <td>{{todo.key1}}</td>
         <td>{{todo.key2}}</td>
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
 th,td {
   width : 100px;
   text-align: center;
 }

</style>
<script>
export default {
  name: 'TodoPage',
  data () {
    return {
      todos: [
        {
          date:'2018.10.29 [14:18:22]',
          sVOC:'14:15:30',
          cVOC:'12',
          domain:'유선BBS',
          key1:'로그인',
          key2:'접속불가'
        },
        {
          date:'2018.10.29'+<br/>+'[14:18:22]',
          sVOC:'14:15:30',
          cVOC:'12',
          domain:'유선BBS',
          key1:'로그인',
          key2:'접속불가'
        },
        {
          date:'2018.10.29'+<br/>+'[14:18:22]',
          sVOC:'14:15:30',
          cVOC:'12',
          domain:'유선BBS',
          key1:'로그인',
          key2:'접속불가'
        }
      ]
    }
  }

  // methods:{
  //     search(date){
  //           this.todos.date === date ({date: date
  //                       });
  //         }
  //     }
//  }

}
</script>
