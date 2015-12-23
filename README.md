jsGintoki.github

https://help.github.com/articles/using-jekyll-with-pages/


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
 
 继续执行 
 
 sudo gem install github pages失败 提示need ruby>=2.2.2 OMG
 
 rvm install ruby 2.2.2
 
 sudo gem uninstall jekyll
 
 sudo gem install github-pages

 输出：43 gems installed
 
----------好像成功了,失败了多次以后，已经不相信了，继续尝试：

Setting up Jekyll 几步OK，通过

bundle exec jekyll serve 又失败，提示：

/Library/Ruby/Site/2.0.0/rubygems/dependency.rb:296:in `to_specs': Could not find 'bundler' (>= 0.a) among 75 total gem(s) (Gem::LoadError)

	from /Library/Ruby/Site/2.0.0/rubygems/dependency.rb:307:in `to_spec'
	
	from /Library/Ruby/Site/2.0.0/rubygems/core_ext/kernel_gem.rb:47:in `gem'
	
	from /usr/bin/bundle:22:in `<main>'
	
	好吧，晚上继续搞吧
	
参考：	http://jekyllrb.com/docs/quickstart/

~ $ gem install jekyll

~ $ jekyll new myblog

~ $ cd myblog

~/myblog $ jekyll serve

# => Now browse to http://localhost:4000





