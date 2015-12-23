jsGintoki.github

 Github jekyll 中有解决方案（http://www.tuicool.com/articles/jM367r3）
 

$ gem sources --remove http://rubygems.org/

$ gem sources -a http://ruby.taobao.org/

$ gem sources -l

*** CURRENT SOURCES ***
http://ruby.taobao.org    

$ gem install rack   在自己的Mac10.10.5 电脑上失败

然后继续执行 gem install jekyll 即可。等待片刻，会提示21 gems installed。jekyll 安装完毕。

尝试了很多中方法，一直提示：

“
ERROR: Error installing nokogiri:

ERROR: Failed to build gem native extension.

/System/Library/Frameworks/Ruby.framework/Versions/2.0/usr/bin/ruby extconf.rb”

根据查询，gem update 2.3.0一直无法解决

后来重新安装ruby成功：(http://www.mamicode.com/info-detail-224375.html)

rvm install ruby 2.1.1

 sudo gem install jekyll
 




