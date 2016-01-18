#好看的直方图1.0
##代码一
    data=c(4.51,10.69,9.33,7.34,5.09,11.68,4.47,8.53,13.99,5.22,4.22,9.23,7.86)
	labs=c("Species1","Species2","Species3", "Species4", "Species5", "Species6", "Species7", "Species8", "Species9", "Species10", "Species11", "Species12", "Species13")
	barplot(data,col=c("steelblue","steelblue","steelblue","mediumturquoise","mediumturquoise","mediumturquoise","mediumturquoise", "mediumturquoise","mediumturquoise","sandybrown","hotpink","hotpink","hotpink"),ylim=c(0,14),width=1,space=1,ylab="%(......)",las=1)
	text(x=seq(1.5,25.5,by=2),y=-0.15, srt = 45, adj = 1, labels = labs,xpd = TRUE)
	abline(h=c(2,4,6,8,10,12,14),col="#00000088",lwd=2)
	abline(h=0)

效果图：
<br>![](http://upload.plob.ybzhao.com/wp-content/uploads/2012/08/1.jpg)

##代码二
    labs=c("Species1","Species2","Species3", "Species4", "Species5", "Species6", "Species7", "Species8", "Species9", "Species10", "Species11", "Species12", "Species13")
	mydata<-cbind(c(2017,400,5013,308),c(640,2998,1798,4530),c(560,300,750,922),c(4654,323,3432,710),c(249,3246,2490,3604),c(746,200,990,3871),c(150,2419,1700,937),c(9801,741,144,1118),c(1651,5778,8056,1040),c(196,345,456,2108),c(246,413,214,1605),c(495,107,1582,820),c(885,501,1618,1881))
	barplot(mydata,col=c("royalblue","firebrick","yellowgreen","darkorchid","darkorchid"),width=1,space=1,border=NA,legend.text=c("Name1","Name2","Name3","Name4"),args.legend=list(x="topright"))
	abline(h=0)
	text(x=seq(1.5,25.5,by=2),y=-300, srt = 45, adj = 1, labels = labs,xpd = TRUE)

效果图：
<br>![](http://upload.plob.ybzhao.com/wp-content/uploads/2012/08/2.jpg)

#箱线图
    finaldata<-data.frame(ZM,OS,SB,AT,GM,PT,VV,WS,TC,MS,OT,CR,PP) 
	####其中ZM,OS,SB,AT,GM,PT,VV,WS,TC,MS,OT,CR,PP分别是从13个文件中读取的数据
	boxplot(finaldata,col=c("steelblue","steelblue","steelblue","mediumturquoise","mediumturquoise","mediumturquoise","mediumturquoise","mediumturquoise","mediumturquoise","sandybrown" ,"hotpink","hotpink","hotpink"),ylab="Length of AA",las=1, font.lab=2)
效果图：
<br>![](http://upload.plob.ybzhao.com/wp-content/uploads/2012/08/3.jpg)