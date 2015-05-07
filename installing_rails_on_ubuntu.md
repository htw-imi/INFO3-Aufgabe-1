It's best to install Ruby and Rails with the Ruby Version Manager.
From my experience it's the easiest and most efficient way. 

Before we get started you should get Curl and some other libraries 
in order to setup your system:

(you can actually skip this step. rvm will install all this automatically)

```shell
xyz@ubuntu:~$ sudo apt-get install curl git-core patch
   build-essential bison zlib1g-dev libssl-dev libxml2-dev
   libxml2-dev sqlite3 libsqlite3-dev autotools-dev
   libxslt1-dev libyaml-0-2 autoconf automake libreadline6-dev
   libyaml-dev libtool
```
   
I have experienced that the following packages are also necessary, especially if 
you work with postgresql

postgresql
libpq-dev

Also, you need to download node.js or something similar. Node.js is just fine. Please
see the webpage for details and download: (I actually just needed this in one tutorial
that I did. I have worked with Rails without Node.js installed. Some gems require it.)

http://nodejs.org/

Now you can begin with the installation of RVM:

xyz@ubuntu:~$ curl -L https://get.rvm.io | bash -s stable

Now you should restart your terminal/bash/shell or read in the RVM script
as follows:

xyz@ubuntu:~$ source ~/.rvm/scripts/rvm

Test whether you have succesfully installed RVM with the following code:

xyz@ubuntu:~$ rvm -v

The shell should show something like this: 

rvm 1.23.8 (stable) by Wayne E. Seguin <wayneeseguin@gmail.com>, 
Michal Papis <mpapis@gmail.com> [https://rvm.io/]

Now you can install Ruby:

xyz@ubuntu:~$ rvm list known

to see a list of known ruby versions. Choose one, you can copy it and paste it in the next step:

xyz@ubuntu:~$ rvm install [your-desired-ruby-version]

Next, we just make sure that the gem packet manager is up to date:

xyz@ubuntu:~$ gem update

You can go ahead now and install Rails: 

xyz@ubuntu:~$ gem install rails

Check if all went alright by typing: 

xyz@ubuntu:~$ rails -v

It should print something like this:

Rails 4.0.0 or some other version.

