# set up a personal webpage on github step by step
1) set up a webpage development environement on my windows 10 laptop according to  https://github.com/github/personal-website
My Gemfile file: <br>
	> source 'https://rubygems.org' <br>
	> gem 'github-pages', group: :jekyll_plugins<br>
	> gem "jekyll-github-metadata"<br>
	> gem "jekyll-octicons"<br>
	> gem "jemoji"<br>
	> gem 'wdm'<br>
	> gem "webrick"<br>

2) Result of "bundle exec jekyll serve": <br>
C:\Users\echnhog\begood-chenhong.github.io>bundle exec jekyll serve

	    `H:/` is not a directory.
	    Bundler will use `C:/Users/echnhog/AppData/Local/Temp/bundler20210530-44340-qxpppt44340' as your home directory temporarily.
	    Configuration file: C:/Users/echnhog/begood-chenhong.github.io/_config.yml
	                Source: C:/Users/echnhog/begood-chenhong.github.io
	           Destination: C:/Users/echnhog/begood-chenhong.github.io/_site
	     Incremental build: disabled. Enable with --incremental
	          Generating...
	       GitHub Metadata: No GitHub API authentication could be found. Some fields may be missing or have incorrect data.
	                        done in 5.117 seconds.
	     Auto-regeneration: enabled for 'C:/Users/echnhog/begood-chenhong.github.io'
	        Server address: http://127.0.0.1:4000
	      Server running... press ctrl-c to stop.
	    Terminate batch job (Y/N)?
	    ^CThe system cannot open the device or file specified.
	    Terminate batch job (Y/N)? Y

	    C:\Users\echnhog\begood-chenhong.github.io>bundle exec jekyll serve
	    `H:/` is not a directory.
	    Bundler will use `C:/Users/echnhog/AppData/Local/Temp/bundler20210530-2176-sw17ec2176' as your home directory temporarily.
	    Configuration file: C:/Users/echnhog/begood-chenhong.github.io/_config.yml
	                Source: C:/Users/echnhog/begood-chenhong.github.io
	           Destination: C:/Users/echnhog/begood-chenhong.github.io/_site
	     Incremental build: disabled. Enable with --incremental
	          Generating...
	       GitHub Metadata: No GitHub API authentication could be found. Some fields may be missing or have incorrect data.
	                        done in 6.742 seconds.
	     Auto-regeneration: enabled for 'C:/Users/echnhog/begood-chenhong.github.io'
	        Server address: http://127.0.0.1:4000
	      Server running... press ctrl-c to stop.

3) Then the webpage can be reviewed locally.

4) Commit local changes to github.

I mainly refer to these documents and links:
a) https://pages.github.com/
b) https://github.com/github/personal-website
c) https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll


> Written with [StackEdit](https://stackedit.io/).
