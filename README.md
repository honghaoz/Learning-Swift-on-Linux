# Learning Swift on Linux

### How to install Swift on Ubuntu 14.04
1. `cd` to a directory (home directory)

2. download Swift distribution:   
	`curl -O https://swift.org/builds/ubuntu1404/swift-2.2-SNAPSHOT-2015-12-31-a/swift-2.2-SNAPSHOT-2015-12-31-a-ubuntu14.04.tar.gz`

3. unzip downloaded file:  
	`tar zxf swift-2.2-SNAPSHOT-2015-12-31-a-ubuntu14.04.tar.gz`

4. export to $PATH
	`export PATH=/path/to/swift-2.2-SNAPSHOT-2015-12-31-a-ubuntu14.04/usr/bin/:"${PATH}"`  
	or
	 `echo "export PATH=/path/to/swift-2.2-SNAPSHOT-2015-12-31-a-ubuntu14.04/usr/bin:\"${PATH}\"" >> .profile` (should be in `~` home directory, this will add `export` to `.profile`, which will be executed when bash is opened)
	 
5. Install necessary dependencies  
	`apt-get update`  
	and  
	`sudo apt-get install git cmake ninja-build clang uuid-dev libicu-dev icu-devtools libbsd-dev libedit-dev libxml2-dev libsqlite3-dev swig libpython-dev libncurses5-dev pkg-config`
	
6. Test Swift is installed successfully  
	`swift --version`
	
---

Ref1: [Introduction to Open Source Swift on Linux](http://www.raywenderlich.com/122189/introduction-to-open-source-swift-on-linux)  
Ref2: [Getting Started with Swift on Linux](https://www.twilio.com/blog/2015/12/getting-started-with-swift-on-linux.html)  
Ref3: [Linux compatible Swift and Swift Package Manager](http://blog.krzyzanowskim.com/2015/12/04/swift-package-manager-and-linux-compatible)

---

Questions to be searched:  
1. What is Darwin?  
2. What is `import Glibc`  
