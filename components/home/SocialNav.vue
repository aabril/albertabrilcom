<template>
	<div class="social-nav social-footer">
		<ul>
			<li>
				<a href="https://www.linkedin.com/in/albertabril" target="_blank">
          <i class="fa fa-linkedin"></i>
        </a>
			</li>
			<li>
				<a href="https://twitter.com/desmondo" target="_blank"><i class="fa fa-twitter"></i></a>
			</li>
			<li>
				<a href="http://github.com/aabril" target="_blank"><i class="fa fa-github"></i></a>
			</li>
			<li>
				<a href="https://plus.google.com/u/0/+AlbertAbrilCerd%C3%A0" target="_blank"><i class="fa fa-google-plus"></i></a>
			</li>
			<li>
				<a href="mailto:albert.abril@gmail.com" target="_blank"><i class="fa fa-at"></i></a>
			</li>
		</ul>
	</div>
</template>

<script>
export default {
  props: [ ],
  layout: 'default' // you can set a custom layout for the error page
}
</script>

<style lang="less">
@import url('https://maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css');

@color_1: #757A86;
@color_2: #6534ff;

.social-nav {
	position: relative;
	z-index: 100;
	display: inline-block;
	margin-top: 30px;
	opacity: 1;
	ul {
		margin: 0;
		padding: 0;
		li {
			position: relative;
			display: block;
			float: left;
			margin: 0 5px 0;
			text-align: center;
			-webkit-transition: all 0.3s cubic-bezier(0, 0, 0.58, 1);
			transition: all 0.3s cubic-bezier(0, 0, 0.58, 1);
			a {
				font-size: .9em;
				line-height: 35px !important;
				position: relative;
				display: inline-block;
				width: 35px;
				height: 35px;
				margin: 0 5px;
				text-align: center;
				color: @color_1;
				-webkit-transition: all 0.3s cubic-bezier(0, 0, 0.58, 1);
				transition: all 0.3s cubic-bezier(0, 0, 0.58, 1);
				-webkit-backface-visibility: hidden;
				&:before {
					font-size: 1.5em;
					position: absolute;
					top: 0;
					left: 0;
					display: inline-block;
					width: 100%;
					height: 100%;
					content: '';
					border: 1px solid rgba(0, 0, 0, 0.3);
					background: transparent;
					border-radius: 2px;
					-webkit-transition: all 0.3s cubic-bezier(0, 0, 0.58, 1);
					transition: all 0.3s cubic-bezier(0, 0, 0.58, 1);
					-webkit-transform: rotate(45deg);
					transform: rotate(45deg);
				}
				&:hover {
					color: @color_2;
					&:before {
						border: 1px solid #6534ff;
						background: transparent;
						-webkit-transform: rotate(135deg);
						transform: rotate(135deg);
					}
				}
				i {
					position: relative;
					top: 0;
					left: 0;
				}
			}
		}
	}
}
.social-nav.social-footer {
	position: absolute;
	bottom: 32px;
	left: 36px;
	-webkit-transition: all 0.6s ease;
	transition: all 0.6s ease;
}
</style>
