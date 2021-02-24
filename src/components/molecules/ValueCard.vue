<template>
  <div class="value-content">
    <table>
      <thead>
        <tr>
          <!-- <th>No</th>
          <th>名前</th>
          <th>年齢</th>
          <th>種類</th>
          <th>好物</th> -->
          <th class="card-title-th">タイトル</th>
          <th class="card-number-th">値</th>
        </tr>
      </thead>
      <tbody>
        <!-- <tr>
          <td>
            <ul v-for="item in items" :key="item.no">
              <li style="list-style:none">{{item.no}}</li>
            </ul>
          </td>
          <td>
            <ul v-for="item in items" :key="item.name">
              <li style="list-style:none">{{item.name}}</li>
            </ul>
          </td>
          <td>
            <ul v-for="item in items" :key="item.age">
              <li style="list-style:none">{{item.age}}</li>
            </ul>
          </td>
          <td>
            <ul v-for="item in items" :key="item.kind">
              <li style="list-style:none">{{item.kind}}</li>
            </ul>
          </td>
          <td>
            <ul v-for="item in items" :key="item.favorite">
              <li style="list-style:none">{{item.favorite}}</li>
            </ul>
          </td>
        </tr> -->

        <tr>
          <td>
            <card-title :value="name"></card-title>
          </td>
          <td>
            <card-number :value="value"></card-number>
          </td>
        </tr>
        <tr>
          <td>
            <card-title :value="name"></card-title>
          </td>
          <td>
            <card-number :value="value"></card-number>
          </td>
        </tr>
        <tr>
          <td>
            <card-title :value="name"></card-title>
          </td>
          <td>
            <card-number :value="value"></card-number>
          </td>
        </tr>
        <tr>
          <td>
            <card-title :value="name"></card-title>
          </td>
          <td>
            <card-number :value="value"></card-number>
          </td>
        </tr>
        <tr>
          <td>
            <card-title :value="name"></card-title>
          </td>
          <td>
            <card-number :value="value"></card-number>
          </td>
        </tr>
        <tr>
          <td>
            <card-title :value="name"></card-title>
          </td>
          <td>
            <card-number :value="value"></card-number>
          </td>
        </tr>
        <tr>
          <td>
            <card-title :value="name"></card-title>
          </td>
          <td>
            <card-number :value="value"></card-number>
          </td>
        </tr>
        <tr>
          <td>
            <card-title :value="name"></card-title>
          </td>
          <td>
            <card-number :value="value"></card-number>
          </td>
        </tr>
        <tr>
          <td>
            <card-title :value="name"></card-title>
          </td>
          <td>
            <card-number :value="value"></card-number>
          </td>
        </tr>
        <tr>
          <td>
            <card-title :value="name"></card-title>
          </td>
          <td>
            <card-number :value="value"></card-number>
          </td>
        </tr>

      </tbody>
    </table>
  </div>
</template>
<script>
import CardTitle from "../atoms/CardTitle";
import CardNumber from "../atoms/CardNumber";
export default {
  data(){
    return {
      items:[
        {no:'1',name:'そら',age:'8',kind:'キジトラ',favorite:'犬の人形'},
        {no:'2',name:'りく',age:'7',kind:'長毛種',favorite:'人間'},
        {no:'3',name:'うみ',age:'6',kind:'ミケ',favorite:'高級ウェットフード'},
        {no:'4',name:'こうめ',age:'4',kind:'サビ',favorite:'横取りフード'}
      ]
    }
  },
  components: {
    CardTitle,
    CardNumber
  },
  props: {
    name: String,
    value: String
  }
};
</script>
<style scoped>
.value-content {
  width: 100%;
  display: inline-block;
  margin: 40px 0 0 40px;
  background-color: white;
  border: 0 solid #aaa;
  border-radius: 4px;
  box-shadow: 2px 2px 2px 2px #ccc;
  padding: 15px;
  overflow: scroll;
}

table {
  width: 100%;
}

thead th {
  border-bottom: solid 1px;
}
.card-title-th {
  width: 70%;
}
.card-number-th {
  width: 30%;
}
</style>