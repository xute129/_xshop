<template>
  <div>
    <div v-for="(item, index) in R" :key="index">R:{{item}}</div>
    
  </div>
</template>

<script>
import lifeBlue from '@/components/lifeBlue'
export default {
  components: { lifeBlue },
  data () {
    return {
      arr: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19],
      R: [],
      A: [],

    };
  },
  created () {
    this.SplitArray(5, this.arr);
    this.data('阿娇','柏芝','思慧');
  },
  methods: {
    SplitArray (N, Q) {
      for (let F = 0; F < Q.length;) {
        this.R.push(Q.slice(F, F += N))
      }
      let B = this.R
      //console.log(B)
      for (let i = 0; i < B.length; i++) {
        if (i % 2 === 0) {
          this.A.push(B[i])

        } else {
          this.A.push(B[i].reverse())
        }
       // console.log(i)
      }
    },
    //rest参数应用
    data(...args){
      console.log(args)
    },

  },

};
</script>


