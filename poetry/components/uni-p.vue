<template>
	<view>
		<view v-for="(item, index) in paragraphs" :key="index">
			<p class="uni-p">
			  {{item.paragraph}}
			</p>
		</view>
	</view>
</template>

<script>
	export default {
		name:"UniP",
		data() {
			return {
				
			};
		},
		props: {
			paragraphs: {
				type: Array,
				default: function(e) {
					return []
				}
			}
		},
	}
</script>

<style>
.uni-p{
	text-align: left;
	text-indent: 2em;
	line-height:25px;
	font-family:'MicrosoftYaHei';
	font-size:medium;
	padding: 4px 0;
}
</style>
