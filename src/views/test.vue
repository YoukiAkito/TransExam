<template>
	<el-card shadow="never">
		<el-form>
			<div class="card-header">
				<input type="radio" id="gender" value="M" onclick="set_gender(0);" checked />Male&nbsp;
				<input type="radio" id="gender" value="F" onclick="set_gender(1);" />Female<br />
				<input type="radio" id="testform" value="L" onclick="use_long_form(true);" checked />Long
				Form&nbsp;
				<input type="radio" id="testform" value="S" onclick="use_long_form(false);" />Short Form<br />
			</div>
		</el-form>
		<el-form>
			<div>
				<br/>
				<input type="button" value="Score" onclick="score_rb(document.forms.questions);" />
				<br/><br/>
			</div>
		</el-form>
	</el-card>
</template>

<script>
import './data'
import './script'
export default {
	name: "test",
	props: {},
	data() {
		return {}
	},
	mounted: function () {
		document.write(questions[0]);
		doc_write_all_questions();
		score_rb(document.forms.questions);
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

#app {
	font-family: Avenir, Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #2c3e50;
	margin-top: 60px;
}
</style>
