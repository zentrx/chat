# chat
nativefier version of google chat with instructions on how to build. 

# install
in order to install this, grab the latest release and the exe, and place the exe in ./chat
it's just too big to store on git apparently.
the pre-compiled version is windows-x64

# build
if you want to build it yourself you'll need nodejs and nativefier installed.
here's the nativefier command. for non-windows and non-64 bit versions, you can adjust the platform (osx, linux) and arch (ia32, arm64)

nativefier 'https://chat.google.com/' --name Chat --internal-urls ".*?\.google\.*?" --icon "icon.ico"
