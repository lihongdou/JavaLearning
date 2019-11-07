**文章目录**
* [一：IDEA常用配置](#%E4%B8%80idea%E5%B8%B8%E7%94%A8%E9%85%8D%E7%BD%AE)
  * [常用工具栏显示](#%E5%B8%B8%E7%94%A8%E5%B7%A5%E5%85%B7%E6%A0%8F%E6%98%BE%E7%A4%BA)
  * [更改idea主题设置](#%E6%9B%B4%E6%94%B9idea%E4%B8%BB%E9%A2%98%E8%AE%BE%E7%BD%AE)
  * [代码编辑器主题风格](#%E4%BB%A3%E7%A0%81%E7%BC%96%E8%BE%91%E5%99%A8%E4%B8%BB%E9%A2%98%E9%A3%8E%E6%A0%BC)
  * [设置背景颜色为豆沙绿](#%E8%AE%BE%E7%BD%AE%E8%83%8C%E6%99%AF%E9%A2%9C%E8%89%B2%E4%B8%BA%E8%B1%86%E6%B2%99%E7%BB%BF)
  * [关闭Intellij IDEA自动更新](#%E5%85%B3%E9%97%ADintellij-idea%E8%87%AA%E5%8A%A8%E6%9B%B4%E6%96%B0)
  * [设置最近打开的项目及窗口打开方式（按需修改）](#%E8%AE%BE%E7%BD%AE%E6%9C%80%E8%BF%91%E6%89%93%E5%BC%80%E7%9A%84%E9%A1%B9%E7%9B%AE%E5%8F%8A%E7%AA%97%E5%8F%A3%E6%89%93%E5%BC%80%E6%96%B9%E5%BC%8F%E6%8C%89%E9%9C%80%E4%BF%AE%E6%94%B9)
  * [自动编译](#%E8%87%AA%E5%8A%A8%E7%BC%96%E8%AF%91)
  * [全局JDK配置](#%E5%85%A8%E5%B1%80jdk%E9%85%8D%E7%BD%AE)
  * [tab页面多行显示的设置](#tab%E9%A1%B5%E9%9D%A2%E5%A4%9A%E8%A1%8C%E6%98%BE%E7%A4%BA%E7%9A%84%E8%AE%BE%E7%BD%AE)
  * [行号显示和方法间的分隔符](#%E8%A1%8C%E5%8F%B7%E6%98%BE%E7%A4%BA%E5%92%8C%E6%96%B9%E6%B3%95%E9%97%B4%E7%9A%84%E5%88%86%E9%9A%94%E7%AC%A6)
  * [设置忽略大小写提示](#%E8%AE%BE%E7%BD%AE%E5%BF%BD%E7%95%A5%E5%A4%A7%E5%B0%8F%E5%86%99%E6%8F%90%E7%A4%BA)
  * [修改代码中注释的字体颜色](#%E4%BF%AE%E6%94%B9%E4%BB%A3%E7%A0%81%E4%B8%AD%E6%B3%A8%E9%87%8A%E7%9A%84%E5%AD%97%E4%BD%93%E9%A2%9C%E8%89%B2)
  * [快捷键设置为跟Eclipse一样](#%E5%BF%AB%E6%8D%B7%E9%94%AE%E8%AE%BE%E7%BD%AE%E4%B8%BA%E8%B7%9Feclipse%E4%B8%80%E6%A0%B7)
  * [设置编辑器字体大小](#%E8%AE%BE%E7%BD%AE%E7%BC%96%E8%BE%91%E5%99%A8%E5%AD%97%E4%BD%93%E5%A4%A7%E5%B0%8F)
  * [文件编码的设置](#%E6%96%87%E4%BB%B6%E7%BC%96%E7%A0%81%E7%9A%84%E8%AE%BE%E7%BD%AE)
  * [鼠标滚轮调整代码文字大小](#%E9%BC%A0%E6%A0%87%E6%BB%9A%E8%BD%AE%E8%B0%83%E6%95%B4%E4%BB%A3%E7%A0%81%E6%96%87%E5%AD%97%E5%A4%A7%E5%B0%8F)
  * [自动导包和优化](#%E8%87%AA%E5%8A%A8%E5%AF%BC%E5%8C%85%E5%92%8C%E4%BC%98%E5%8C%96)
  * [生成类注释模板（全局）](#%E7%94%9F%E6%88%90%E7%B1%BB%E6%B3%A8%E9%87%8A%E6%A8%A1%E6%9D%BF%E5%85%A8%E5%B1%80)
  * [生成方法注释模板(只能当前项目)](#%E7%94%9F%E6%88%90%E6%96%B9%E6%B3%95%E6%B3%A8%E9%87%8A%E6%A8%A1%E6%9D%BF%E5%8F%AA%E8%83%BD%E5%BD%93%E5%89%8D%E9%A1%B9%E7%9B%AE)
  * [设置Java代码的注释风格](#%E8%AE%BE%E7%BD%AEjava%E4%BB%A3%E7%A0%81%E7%9A%84%E6%B3%A8%E9%87%8A%E9%A3%8E%E6%A0%BC)
  * [生成serialVersionUID](#%E7%94%9F%E6%88%90serialversionuid)
  * [设置鼠标悬浮事件](#%E8%AE%BE%E7%BD%AE%E9%BC%A0%E6%A0%87%E6%82%AC%E6%B5%AE%E4%BA%8B%E4%BB%B6)
  * [隐藏\.idea文件夹和\.iml等文件](#%E9%9A%90%E8%97%8Fidea%E6%96%87%E4%BB%B6%E5%A4%B9%E5%92%8Ciml%E7%AD%89%E6%96%87%E4%BB%B6)
  * [Tomcat Server（当前项目配置）](#tomcat-server%E5%BD%93%E5%89%8D%E9%A1%B9%E7%9B%AE%E9%85%8D%E7%BD%AE)
  * [Git配置（全局）](#git%E9%85%8D%E7%BD%AE%E5%85%A8%E5%B1%80)
* [二：实用插件推荐](#%E4%BA%8C%E5%AE%9E%E7%94%A8%E6%8F%92%E4%BB%B6%E6%8E%A8%E8%8D%90)
  * [Lombok plugin](#lombok-plugin)
  * [彩虹括号Rainbow Brackets](#%E5%BD%A9%E8%99%B9%E6%8B%AC%E5%8F%B7rainbow-brackets)
  * [快捷键提示插件](#%E5%BF%AB%E6%8D%B7%E9%94%AE%E6%8F%90%E7%A4%BA%E6%8F%92%E4%BB%B6)
  * [翻译插件](#%E7%BF%BB%E8%AF%91%E6%8F%92%E4%BB%B6)
  * [热部署插件JRebel](#%E7%83%AD%E9%83%A8%E7%BD%B2%E6%8F%92%E4%BB%B6jrebel)
  * [Maven Helper](#maven-helper)
  * [Properties to YAML Converter](#properties-to-yaml-converter)
  * [阿里巴巴代码规范插件p3c\-pmd](#%E9%98%BF%E9%87%8C%E5%B7%B4%E5%B7%B4%E4%BB%A3%E7%A0%81%E8%A7%84%E8%8C%83%E6%8F%92%E4%BB%B6p3c-pmd)
**注：软件版本：2019.2.4**
# 一：IDEA常用配置
## 常用工具栏显示
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106213611463.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
## 更改idea主题设置
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106164750376.png)
## 代码编辑器主题风格
编辑器风格修改个人并不推荐完全由自己来配置，因为网上提供了很多优秀的主题风格，我们可以导入自己喜欢的主题，然后在其基础上进行微调，推荐主题下载网站[http://www.riaway.com](http://www.riaway.com)，安装下载主题步骤:  
>1.从主菜单打开你的编辑器选择File->Import Setting.选择你下载的Jar文件;  
2.等待重启之后进行配置打开File->Settings->Editor->Colors and fonts 然后选择你安装的主题即可完成  
## 设置背景颜色为豆沙绿
在File->Settings->Editor->Color Scheme->General  
豆沙绿：R:199,  G: 237,  B:204
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191107160620183.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
## 关闭Intellij IDEA自动更新
在File->Settings->Appearance & Behavior->System Settings->Updates下取消Automatically check updates for勾选  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106163547457.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
## 设置最近打开的项目及窗口打开方式（按需修改）
File ->Appearance& Behavior ->System Settings
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106181407429.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
## 自动编译
![在这里插入图片描述](https://img-blog.csdnimg.cn/2019110618053168.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
## 全局JDK配置
File ->Other Settings -> Structure for new Projects-> Project  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106181014439.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
File ->Other Settings -> Structure for new Projects-> SDKs  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106181042157.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
## tab页面多行显示的设置
File -> Settings -> Editor -> Editor Tabs  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106181850821.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
## 行号显示和方法间的分隔符
File -> Settings -> Editor -> General ->Appearance  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191107111810172.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
## 设置忽略大小写提示
File -> Settings -> Editor -> General ->Code Completion  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191107112125287.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
>IntelliJ IDEA 的代码提示和补充功能有一个特性：区分大小写。如上图标注所示，默认就是 First letter only 区分大小写的。  
区分大小写的情况是这样的：比如我们在 Java 代码文件中输入 stringBuffer，IntelliJ IDEA - 默认是不会帮我们提示或是代码补充的，但是如果我们输入StringBuffer 就可以进行代码提示和补充。 
如果想不区分大小写的话，取消勾选该选项即可。（2017版本的IEDA中是改为 None 选项） 
## 修改代码中注释的字体颜色
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191107114156970.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
>Doc Comment –> Text：修改文档注释的字体颜色  
>Block comment：修改多行注释的字体颜色  
>Line comment：修改当行注释的字体颜色   

推荐颜色如下：  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191107113917882.png)

## 快捷键设置为跟Eclipse一样
很多人可能并不习惯IDEA的快捷键，为了方便，这里我们将快捷键设置为跟 Eclipse一样。  
具体步骤: File -> Settings -> Keymap - > 选择Eclipse  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106190806734.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
## 设置编辑器字体大小
File->Settings->Editor->Font 设置字体 大小 行间距  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106170116560.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
## 文件编码的设置
File->Settings->Editor->File Encodings  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106170555881.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
勾选上Transparent native-to-ascii conversion，如果没有勾选属性文件中的中文,会被转为ASCII码  
**全局编码设置**  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106190953203.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
## 鼠标滚轮调整代码文字大小
File->Settings->General ->Change font Size  
![在这里插入图片描述](https://img-blog.csdnimg.cn/2019110617115210.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
## 自动导包和优化
File -> Editor -> Auto Import  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106175200245.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
>Insert imports on paste:复制代码的时候，对于导入的包是否需要进行询问的一个选项。  
    ASK(有需要导入的包名时会弹提示框，问你要不要导入)  
    NONE(有需要导入的包名时不会弹提示框，也不会自动导入)  
    ALL(有需要导入的包名时会自动导入，不会弹提示框)  
Show import popup:当输入的类的声明没被导入时，会弹出一个选择的对话框  
Optimize imports on fly:自动优化包导入，移除不需要的包  
Add unambiguous imports on the fly:这个就是自动导入功能了，当你输入类名后声明就被自动导入了  
## 生成类注释模板（全局）
File ->Other Settings -> Structure for new Projects-> Editor-> File And Code templates  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191107095858102.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
在右边空白处，编写自己的模板即可，注意Scheme是模板的生效范围，可选变量在description有介绍，附图中本人使用的模板（${USER}为计算机用户名，可以自行修改）。  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191107100511239.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
设置完成后，创建类时自动生成注释，效果如下  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191107100905315.png)
## 生成方法注释模板(只能当前项目)
File–Setting–Editor-Live Templates。  
添加模板组  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191107104312168.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191107104352747.png)
在 JAVA分组中创建 Template
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191107104441444.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191107105022312.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
点击Edit variables按钮编辑参数表达式及返回值表达式  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191107105126116.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
params表达式如下  
> groovyScript("def result=''; def params=\"${_1}\".replaceAll('[\\\\[|\\\\]|\\\\s]', '').split(',').toList(); for(i = 0; i < params.size(); i++) {result+=' * @param ' + params[i] + ((i < params.size() - 1) ? '\\n' : '')}; return result", methodParameters()) 

点击change修改模板方法适用范围  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191107105306868.png)
模板参数如下  
```
*
 * @description: TODO
$params$
 * @return: $return$
 * @author: lhd
 * @date: $date$ $time$
 */
 ```
   点击应用,查看效果 在方法上 敲 **/**** + **Enter** 效果如下  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191107110017751.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
## 设置Java代码的注释风格
File->Settings->Editor->Code Style -> java,取消注释位置在首行
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191107154713668.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
## 生成serialVersionUID
默认情况下Intellij IDEA关闭了继承了Java.io.Serializable的类生成serialVersionUID的警告，如果需要提示生成serialVersionUID，那么需要做以下设置:在File->Settings->Editor->Inspections下勾选中Java->Serialization issues->Serializable class without ‘serialVersionUID’，将光标放到类名上按Atl＋Enter键就会提示生成serialVersionUID了  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106175732141.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
## 设置鼠标悬浮事件
File->Settings->Editor->General  
该功能的作用时, 当鼠标悬浮在类上时,显示对应的源码.如果需要,按照图中所示进行设置  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106175905865.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
## 隐藏.idea文件夹和.iml等文件
IntelliJ IDEA项目会自动生成一个.idea文件夹和.iml文讲，看着实在是碍眼，所以对以上文件进行隐藏处理  
在File->Settings->Editor->File Types下的”Ignore files and folders”一栏添加 *.idea;*.iml;等配置如下图所示  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106163942881.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
## Tomcat Server（当前项目配置）
配置Tomcat方法：File -> Settings -> Build Deployment -> Application Servers -> **+**   ->Tomcat Server  
选择tomcat所在路径然后应用    
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106214949752.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
## Git配置（全局）
File ->Other Settings -> Structure for new Projects-> Version Control -> Git
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106220956152.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)


# 二：实用插件推荐
## Lombok plugin
File->Settings->Plugins  
开发神器，可以简化你的实体类，让你i不再写get/set方法，还能快速的实现builder模式，以及链式调用方法，总之就是为了简化实体类而生的插件。  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106185344639.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
## 彩虹括号Rainbow Brackets
彩虹颜色的括号  看着很舒服 敲代码效率变高。可以很清楚明白的区分各个括号的范围  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191106185639468.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpaG9uZ2RvdQ==,size_16,color_FFFFFF,t_70)
## 快捷键提示插件
Key promoter是在你通过非快捷键方式使用某功能时 为你提供快捷键建议 在开始记不住快捷键的情况下 强烈推荐安装  

## 翻译插件
翻译插件 TranslationPlugin,支持支持中英互译、单词朗读,详细安装文档请参考:[TranslationPlugin介绍与安装手册  ](https://github.com/YiiGuxing/TranslationPlugin)  
## 热部署插件JRebel
JRebel热部署插件安装和使用请参考:[JRebel热部署插件安装和使用](https://youmeek.gitbooks.io/intellij-idea-tutorial/content/jrebel-setup.html)    
## Maven Helper
Maven 辅助插件 用于查找Maven依赖冲突非常好用的一款插件 安装步骤请参考:[Maven Helper安装使用](https://my.oschina.net/u/136229/blog/678918)   
## Properties to YAML Converter
在开发SpringBoot项目时，会需要把Properties的配置格式改为 YAML格式，Properties to YAML Converter提供了很好的支持  
## 阿里巴巴代码规范插件p3c-pmd
详细安装和使用请参考:[阿里巴巴代码规范插件p3c-pmd](https://mp.weixin.qq.com/s/lBDe60LFpdXoi2xbA-L2Qg?)  

参考链接：https://blog.csdn.net/m_m254282520/article/details/78900238





