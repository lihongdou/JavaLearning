* [一\.Maven配置](#%E4%B8%80maven%E9%85%8D%E7%BD%AE)
  * [1\.本机Maven配置](#1%E6%9C%AC%E6%9C%BAmaven%E9%85%8D%E7%BD%AE)
    * [（1）下载Maven](#1%E4%B8%8B%E8%BD%BDmaven)
    * [（2）解压](#2%E8%A7%A3%E5%8E%8B)
    * [（3）解压配置settings\.xml，修改用户仓库为自定义地址](#3%E8%A7%A3%E5%8E%8B%E9%85%8D%E7%BD%AEsettingsxml%E4%BF%AE%E6%94%B9%E7%94%A8%E6%88%B7%E4%BB%93%E5%BA%93%E4%B8%BA%E8%87%AA%E5%AE%9A%E4%B9%89%E5%9C%B0%E5%9D%80)
    * [（4）配置环境变量](#4%E9%85%8D%E7%BD%AE%E7%8E%AF%E5%A2%83%E5%8F%98%E9%87%8F)
    * [（4）查看是否配置成功](#4%E6%9F%A5%E7%9C%8B%E6%98%AF%E5%90%A6%E9%85%8D%E7%BD%AE%E6%88%90%E5%8A%9F)
* [二\.Maven与Idea的整合](#%E4%BA%8Cmaven%E4%B8%8Eidea%E7%9A%84%E6%95%B4%E5%90%88)
  * [1\.当前项目maven设置](#1%E5%BD%93%E5%89%8D%E9%A1%B9%E7%9B%AEmaven%E8%AE%BE%E7%BD%AE)
  * [2\.默认所有项目maven设置](#2%E9%BB%98%E8%AE%A4%E6%89%80%E6%9C%89%E9%A1%B9%E7%9B%AEmaven%E8%AE%BE%E7%BD%AE)
# 一.Maven配置
## 1.本机Maven配置
### （1）下载Maven
官网下载地址:[http://maven.apache.org/download.cgi](http://maven.apache.org/download.cgi)  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106150508926.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
### （2）解压
解压 maven 压缩包 到一个路径（尽量编码路径中不要包含中文）  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106150907690.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
* bin：含有mvn运行的脚本  
* boot：含有plexus-classworlds类加载器框架  
* lib：含有Maven运行时所需要的java类库  
* conf：含有settings.xml配置文件  
 settings.xml 中默认的用户库: ${user.home}/.m2/repository[通过maven下载的jar包都会存储到此仓库中]    
### （3）解压配置settings.xml，修改用户仓库为自定义地址
 ![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106151309717.png)
### （4）配置环境变量
此电脑——右键——属性——高级系统设置——环境变量——系统变量——新建——变量名和变量值  
在系统变量PATH中引入你配置的变量名: **;%MAVEN_HOME%\bin**
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106151742765.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106152015804.png)
### （4）查看是否配置成功
打开cmd窗口或者桌面**shift+右键**打开powershell窗口，输入  
> mvn -v  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106152726185.png)
# 二.Maven与Idea的整合
## 1.当前项目maven设置
File --> Settings  
搜索 maven，选择路径，会自动根据 settings.xml文件设置的 jar 保存路径来设置  
也可以自定义 maven 下载的 jar 保存路径  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106153839613.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
自动引入及源码下载配置修改  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106154503205.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
## 2.默认所有项目maven设置
File --> Other Settings --> Setting for new projects  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106154645377.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
搜索 maven，选择路径，会自动根据 settings.xml文件设置的 jar 保存路径来设置  
也可以自定义 maven 下载的 jar 保存路径  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106153839613.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
自动引入及源码下载配置修改  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106154503205.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
到此maven本地及idea配置完成！  
**情况说明：**  
    1. 出现jar不下载或者下载到一半卡住进度条不动，一般是maven仓库有问题，换个仓库解决  
    2.idea里面出现所有jar报红，一般也是仓库问题，建议手动清空仓库，重新下载或者换个仓库都行  
    3.出现单个jar无法下载，或者单个jar报红，一般都是因为下载不完整，进仓库找到 jar位置，删除，重下，保证网络畅通
