#Chapter 22: Changing Environment Variables (export, Env:)

##English Questions

###Can you set the debug environment variable to true?
I set my DEBUG environment variable to true in the previous Chapter.
```
$ export DEBUG='True'
$ echo $DEBUG
True
```
###Can you remove the debug environment variable?
I can.
```
$ unset DEBUG
$echo $DEBUG

```
###Add your environment variables, and what they do to your Readme.md.
```
$ env
rvm_bin_path=/Users/Michael/.rvm/bin
TERM_PROGRAM=iTerm.app
GEM_HOME=/Users/Michael/.rvm/gems/ruby-2.2.4
SHELL=/bin/bash
TERM=xterm-256color
CLICOLOR=1
IRBRC=/Users/Michael/.rvm/rubies/ruby-2.2.4/.irbrc
TMPDIR=/var/folders/s5/q_pg7dz9413djgv54q5vfs640000gn/T/
Apple_PubSub_Socket_Render=/private/tmp/com.apple.launchd.aGygVRvW99/Render
OLDPWD=/Users/Michael/workspace/davinci_coders_t1_2016/homework/learn_command_line_exercises
MY_RUBY_HOME=/Users/Michael/.rvm/rubies/ruby-2.2.4
USER=Michael
_system_type=Darwin
rvm_path=/Users/Michael/.rvm
SSH_AUTH_SOCK=/private/tmp/com.apple.launchd.cxvEoA5Fhv/Listeners
__CF_USER_TEXT_ENCODING=0x1F5:0x0:0x0
rvm_prefix=/Users/Michael
PATH=/Users/Michael/.rvm/gems/ruby-2.2.4/bin:/Users/Michael/.rvm/gems/ruby-2.2.4@global/bin:/Users/Michael/.rvm/rubies/ruby-2.2.4/bin:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin:/Users/Michael/.rvm/bin
PWD=/Users/Michael/workspace/davinci_coders_t1_2016/homework/learn_command_line_exercises/Chapter_22
LANG=en_US.UTF-8
ITERM_PROFILE=Projector - Dark
_system_arch=x86_64
XPC_FLAGS=0x0
_system_version=10.11
XPC_SERVICE_NAME=0
rvm_version=1.26.11 (latest)
SHLVL=1
COLORFGBG=12;8
HOME=/Users/Michael
ITERM_SESSION_ID=w1t0p0
LOGNAME=Michael
GEM_PATH=/Users/Michael/.rvm/gems/ruby-2.2.4:/Users/Michael/.rvm/gems/ruby-2.2.4@global
RUBY_VERSION=ruby-2.2.4
_system_name=OSX
BASH_FUNC_parse_git_pair%%=() {  if ( hub rev-parse --git-dir > /dev/null 2>&1 ); then
 hub config user.name;
 fi
}
BASH_FUNC_parse_git_branch%%=() {  hub branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/(\1)/'
}
_=/usr/bin/env
```

rvm_bin_path= The path for the RVM bin

TERM_PROGRAM= Lists the program currently in use for the terminal

GEM_HOME= Tells RubyGems where to install gems

SHELL= Lists what Command Line Interface to use(bash)

TERM= Sets the terminal's capabilities for coloring text

IRBRC= A file to configure IRB in the terminal

TMPDIR= Temporary directory

OLDPWD= Shows the path for the pwd you were just in

MY_RUBY_HOME= Sets which ruby version you use, which is controlled by RVM

USER= Denotes which user is logged in

_system_type= The computer's base system

rvm_path= The path for the RVM directory

SSH_AUTH_SOCK= Contains the path for the SSH

__CF_USER_TEXT_ENCODING= Stores the preferred text encoding and language for the user

rvm_prefix= Shows the hostname using RVM

PATH= specifies a set of directories where executable programs are located

PWD= stores to current working directory

LANG= sets the langauge of the terminal

ITERM_PROFILE= stores the iTerm profile (Dark in my case)

_system_arch= The computer's architecture.

XPC_FLAGS= Not Sure

PS1= The prompt string (PS) that shows up in terminal - namely, the text prompt that shows before you type commands

_system_version= Your Operating System's version

XPC_SERVICE_NAME= Not Sure

rvm_version= The version of Ruby Version Manager

SHLVL= shows your current nested SHELL level

COLORFGBG= Sets the color scheme based on the background color in terminal

HOME= sets your home directory, which can be represented as '~' in terminal

ITERM_SESSION_ID= Stores a unique session ID for the current iTERM session

LOGNAME= Essentially the same as $USER

GEM_PATH= provides the location(s) where gems can be found

RUBY_VERSION= Shows the current version of Ruby on your computer

_system_name= The name of your operating system

_= Self-referring environment
