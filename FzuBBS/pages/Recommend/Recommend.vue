<template>
	<view class="page">
		<!--轮播图组件-->
		<swiper :indicator-dots="true" :autoplay="true" class="RecSchool">
			<swiper-item>
				<image src="../../static/RecSchool/School1.JPG" class="RecSchool"></image>
			</swiper-item>
			<swiper-item>
				<image src="../../static/RecSchool/School2.JPG" class="RecSchool"></image>
			</swiper-item>
			<swiper-item>
				<image src="../../static/RecSchool/School3.JPG" class="RecSchool"></image>
			</swiper-item>
		</swiper>
		
		<!-- 新推荐帖子 start-->
		
		<view class="page-block WorthRead">
			<view class="WorthRead-title">
				<image src="../../static/RecIcon/WorthReading.png" class="WorthRead-icon"></image>
				<view class="WorthReadWord">
						推荐阅读
				</view>
			</view>
				
			<view class="page-block RecommendRead">
				<view class="single-recommend">
					<view class="recommend-detail">
						<view v-for="TieObj in TieArray">
							<view class="recommend-title">
							{{TieObj.title}}
							</view>
							<view class="recommend-content">
							{{TieObj.content}}
							</view>
							<view class="recommend-time">
							{{TieObj.time}}
							</view>
						</view>
					</view>
				</view>
			</view>	
		</view>
		
		<!-- 新推荐帖子 end-->
		
		
		
		
	
	<!--推荐帖子详情界面-->
		<!-- <view class="page-block WorthRead">
			<view class="WorthRead-title">
				<image src="../../static/RecIcon/WorthReading.png" class="WorthRead-icon"></image>
				<view class="WorthReadWord">
					推荐阅读
				</view>
			</view>
		</view>
		
		<view class="page-block RecommendRead">
				
				<view class="single-recommend">
					<view class="recommend-detail">
						<view class="recommend-title">
							【福州大学吧】欢迎2019级考生报考福州大学
						</view>
						<view class="recommend-content">
							又是一年高考季，吧里相信会进来越来越多的19级学弟学妹前来咨询学校的各种情况。高中时代结束了，你们即将迎来属于自己的大学生活。大学时代就要来了，你们兴奋、平淡还是茫然不知所措？无论如何，学长学姐们在学校等着你们这批即将进入福州大学的新鲜血液。
						</view>
						<view class="recommend-time">
							2019-06-23 11:41
						</view>
					</view>
				</view>
			
				
				<view class="single-recommend">
					<view class="recommend-detail">
						<view class="recommend-title">
							【福州大学吧】欢迎2019级考生报考福州大学
						</view>
						<view class="recommend-content">
							又是一年高考季，吧里相信会进来越来越多的19级学弟学妹前来咨询学校的各种情况。高中时代结束了，你们即将迎来属于自己的大学生活。大学时代就要来了，你们兴奋、平淡还是茫然不知所措？无论如何，学长学姐们在学校等着你们这批即将进入福州大学的新鲜血液。
						</view>
						<view class="recommend-time">
							2019-06-23 11:41
						</view>
					</view>
				</view>
			
				
				<view class="single-recommend">
					<view class="recommend-detail">
						<view class="recommend-title">
							【福州大学吧】欢迎2019级考生报考福州大学
						</view>
						<view class="recommend-content">
							又是一年高考季，吧里相信会进来越来越多的19级学弟学妹前来咨询学校的各种情况。高中时代结束了，你们即将迎来属于自己的大学生活。大学时代就要来了，你们兴奋、平淡还是茫然不知所措？无论如何，学长学姐们在学校等着你们这批即将进入福州大学的新鲜血液。
						</view>
						<view class="recommend-time">
							2019-06-23 11:41
						</view>
					</view>
				</view>
		</view> -->
	</view>
</template>

<script>
	export default {
		data() {
			return {
				TieArray:[
					{
							
							title:"【福州大学吧】欢迎2019级考生报考福州大学",
							content:"又是一年高考季，吧里相信会进来越来越多的19级学弟学妹前来咨询学校的各种情况。高中时代结束了，你们即将迎来属于自己的大学生活。大学时代就要来了，你们兴奋、平淡还是茫然不知所措？无论如何，学长学姐们在学校等着你们这批即将进入福州大学的新鲜血液。",
							time:"2019-06-23 11:41"
						
					},
					{
							title:"【福州大学吧】欢迎2019级考生报考福州大学",
							content:"又是一年高考季，吧里相信会进来越来越多的19级学弟学妹前来咨询学校的各种情况。高中时代结束了，你们即将迎来属于自己的大学生活。大学时代就要来了，你们兴奋、平淡还是茫然不知所措？无论如何，学长学姐们在学校等着你们这批即将进入福州大学的新鲜血液。",
							time:"2019-06-23 11:41"
						
					},
					{
							title:"【福州大学吧】欢迎2019级考生报考福州大学",
							content:"又是一年高考季，吧里相信会进来越来越多的19级学弟学妹前来咨询学校的各种情况。高中时代结束了，你们即将迎来属于自己的大学生活。大学时代就要来了，你们兴奋、平淡还是茫然不知所措？无论如何，学长学姐们在学校等着你们这批即将进入福州大学的新鲜血液。",
							time:"2019-06-23 11:41"
						
					},
					{
							title:"【福州大学吧】欢迎2019级考生报考福州大学",
							content:"又是一年高考季，吧里相信会进来越来越多的19级学弟学妹前来咨询学校的各种情况。高中时代结束了，你们即将迎来属于自己的大学生活。大学时代就要来了，你们兴奋、平淡还是茫然不知所措？无论如何，学长学姐们在学校等着你们这批即将进入福州大学的新鲜血液。",
							time:"2019-06-23 11:41"
						
					}
					
				]
				
			}
		},
		methods: {
			
		},
		components:{
		}
	}
</script>

<style>
	@import url("Rec.css");
</style>