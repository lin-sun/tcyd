<!-- 大学生认证结果 -->
<template>
	<div class="pos_rel">
		<!--S 头部-->
		<top title="认证结果" :isReturn="false"></top>
		<!--E 头部-->
		<!--S 内容-->
		<div class="l_certicate">
			<img class="l_certicate_img" src="~src/images/ico_2.png"/>
			<p class="f30 c_555" >很遗憾，您的大学生认证已过期！</p>
			<div class="mlr30 mt60 text_center">
				<a class="btn mini">重新认证</a>
				<a class="btn_border mini ml30">取消认证</a>
			</div>
		</div>

	</div>
</template>

<script>

</script>

<style lang="less" scoped>
@import (reference) "~src/style/all.less";
.l_certicate_img {
  display: block;
  width: 1.48rem;
  height: 1.98rem;
  margin: 2.1rem auto 0.44rem;
}

.l_certicate {
  p {
    .text_center;
    line-height: 0.7rem;
  }
}

.l_certicate_hint {
  .plr30;
  .ptb20;
  .bg_gray;
  .border-b;
  line-height: 1.5em;
  .f26;
  .c_999;
}

.l_certicate_mess {
  .l_title {
    line-height: 0.87rem;
    .f28;
  }
}
.fail_hint{
	width: 7.5rem;
	position: fixed;
	bottom: 0;
	left: 50%;
	margin-left: -3.75rem;
	.fail_tit{
		height: .5rem;
		position: relative;
		font-size: .26rem;
		text-align: center;
		span{
			display: inline-block;
			height: 100%;
			line-height: .5rem;
			padding: 0 .25rem;
			background: #fff;
			position: relative;
			z-index: 1;
		}
		&::after{
			display: block;
			width: 100%;
			height: 1px;
			content: '';
			position: absolute;
			top:0;
			bottom: 0;
			margin: auto;
			background-color: @line_color;
		}
	}
	.fail_con{
		padding: .34rem .34rem .34rem .54rem;
		color: #666;
		line-height: .4rem;
		position: relative;
		&::before{
			content: '';
			display: block;
			width: .14rem;
			height: .14rem;
			background: @color;
			border-radius: 50%;
			position: absolute;
			top:.44rem;
			left: .34rem;

		}
	}
}
</style>
