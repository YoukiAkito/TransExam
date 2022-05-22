<template>
    <el-card  shadow="never">

		<el-form name="config" action="#">
            <template #header>
			    <div class="card-header">
				    <input type="radio" name="gender" value="M" onclick="set_gender(0);" checked>Male&nbsp;
				    <input type="radio" name="gender" value="F" onclick="set_gender(1);">Female<br>

				    <input type="radio" name="testform" value="L" onclick="use_long_form(true);" checked>Long Form&nbsp;
				    <input type="radio" name="testform" value="S" onclick="use_long_form(false);">Short Form<br>

			    </div>
            </template>
		</el-form>

		<div onclick="document.write(questions[0]);">

		</div>

		<el-form name="questions" action="#">
			<div onclick="doc_write_all_questions();">
				<br>
				<input type="button" value="Score" onclick="score_rb(document.forms.questions);">
				<br><br>
			</div>
		</el-form>
    </el-card>
</template>

<script>
import '/Users/chenmeng/Documents/GitHub/TransExam/static/data.js'
import '/Users/chenmeng/Documents/GitHub/TransExam/static/script.js'

export default {
  name: 'test',
  props: {
  },
  data() {
    return {
    }
  }
}
</script>