<template>
    <el-card  shadow="never">
        <template #header>
            <div class="card-header">
                <span>请先阅读协议</span>
                <el-button type="primary" round @click="handle(scope.row.url)">我已知悉</el-button>
            </div>
        </template>
        <div class="text item">
            本测验基于MMPI，仅供个人学习使用，请勿用于其他用途
            <br>
            本测验属于专业心理测量手段，须在专业人士指导下进行使用，个人请慎用！！
            <br>
            <br>
            明尼苏达多项人格测验
            <br>
             Minnesota Multiphasic Per-sonality Inventory (MMPI) 
            <br>
             简要介绍：明尼苏达多项人格测验（MMPI）是由明尼苏达大学教授哈瑟韦 （S．R．Hathaway）和麦金力（J．C．Mckinley）于1942年制定的，它可以用于测试正常人的人格类型，也可以用于区分正常人和心理或精神疾病患者。上世 纪末，在纪术茂先生等人多年研究和实践调查的基础上，形成了适用于中国本土 的MMPI测验问卷和常模，从1980年我国即开始试用MMPI，近年来使用更为广泛， 结果证明此测验在我国使用具有一定的信度与效度，有较高的临床参考价值。
            <br>
            <br>
            指导语：本测验由许多与你有关的问题所组成，当你阅读每一个题目时，请考虑 是否符合你现在的行为、感情、态度或意见。请尽快填写你读完题目后的第一印象，不要在每一道题上花费太多时间思考。个性各有不同，答案是无所谓对与不对，好与不好的，完全不必有任何顾虑，请按照你的实际情况作答即可。
        </div>
    </el-card>
</template>

<script>
export default {
  name: 'topic',
  props: {
  },
  data() {
    return {
    }
  },
  handle(url) {
    window.location.href='/Users/chenmeng/Documents/GitHub/TransExam/src/components/test.vue'
  }
}
</script>

<style>
  .card-header {
      display: flex;
      justify-content: space-between;
      align-items: center;
  }
    
  .text {
    font-size: 14px;
  }

  .item {
    margin-bottom: 18px;
  }

  .box-card {
    max-width: 480px;
  }
</style>