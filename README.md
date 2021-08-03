# chat
nativefier version of google chat with instructions on how to build. 

# install
in order to install this, grab the latest release and the exe, and place the exe in ./chat
it's just too big to store on git apparently.
the pre-compiled version is windows-x64

# build
if you want to build it yourself you'll need nodejs and nativefier installed.
here's the nativefier command. for non-windows and non-64 bit versions, you can adjust the platform (osx, linux) and arch (ia32, arm64)

nativefier --name 'Chat' 'https://chat.google.com/' --icon icon.ico --user-agent 'Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:70.0) Gecko/20100101 Firefox/70.0' --internal-urls ".*?\.google\.*?" --platform windows --arch x64
