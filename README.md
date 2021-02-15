# Photo_wall_carousel_effect
Photo wall carousel effect
前端照片墙，轮播特效。带背景音乐，除了常见图片，还支持动态图轮播
值得注意事项

1.如需关掉自动旋转，需要注释掉9～16行和24行代码即可
@keyframes run{   /*这里我们要他旋转360度，那么就不用那么麻烦写关键帧了。开始0  结束360，然后循环即可*/
            0%{
                transform: rotateY(0deg);
            }
            100%{
                transform: rotateY(360deg);
            }
        }
        
2.此行代码是控制旋转速度的，修改60s参数即可
 animation: run 60s linear infinite; /*animation linear是匀速运动，infinite是无限循环*/
 
3.在微信里和safaris浏览器打开都是有背景音乐的。google浏览器打开可能会没有背景音乐。如果没有背景音乐打开可以换个浏览器或者自行百度google浏览器的设置问题
