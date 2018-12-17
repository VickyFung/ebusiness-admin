<template>
	<div class="login-container">
		<h1 class="title">{{title}}</h1>
		<input type="text" placeholder="请输入用户名称" class="username" name="username"/>
		<input type="text" placeholder="请输入登录密码" class="password" name="password"/>
		<div class="tips">{{toastText}}</div>
		<button class="login-btn">登录</button>
		<p class="copyright"><span class="smallfont">{{Copyright}}</span></p>
	</div>
</template>

<script>
export default {
  name: 'login',
  data () {
    return {
      title: '后台业务管理系统',
      Copyright: 'Copyright © 2018-2018 零售后台',
      toastText: '请填写用户名称',
    }
  }
}
</script>

<style scoped lang="stylus">
	.login-container
		width: 100%
		height: 100%
		padding-top:147px
		background-color: #78DEDA
		color: #fff
		font-family: MicrosoftYaHei-Bold
		display: flex
		flex-direction: column
		align-items: center
		.title
			font-size: 14px
			letter-spacing: 2px
		.username
			width: 175px
			height: 30px
			margin-top: 36px
			background: rgba(255,255,255,1)
			border-radius: 5px
			text-align: center
		.username::-webkit-input-placeholder
			color: #C9CACA
			font-size: 9px
		.password
			width: 175px
			height: 30px
			margin-top: 15px
			background: rgba(255,255,255,1)
			border-radius: 5px
			text-align: center
		.password::-webkit-input-placeholder
			color: #C9CACA
			font-size: 9px
		.tips
			height: 25px
			width: 175px
			margin-top: 15px
			border-radius: 5px
			background:rgba(255,255,255,1)
			opacity:0.2
			font-size: 9px
			visibility: hidden
		.login-btn
			width: 175px
			height: 30px
			border-radius: 5px
			background-color: #3CBBBA
			font-size: 11px
			color: #fff
		.copyright
			flex: 1
			display: flex
			padding-bottom: 35px
			.smallfont
				display: inline-block
				align-self: flex-end
				font-size: 9px
</style>