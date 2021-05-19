# termux-mono-aarch64-api22
See https://github.com/IanusInferus/termux-mono for details.
## Installation
```consloe
# Deploy
cd $PREFIX
wget https://github.com/mxpro1996/termux-mono-aarch64-api22/releases/download/arm64_api22/mono-termux.6.12.0.122-arm64-android22.tar.xz
tar xf mono-termux.6.12.0.122-arm64-android22.tar.xz
# AOT_cache
cd $PREFIX/local/lib/mono/4.5
mono --aot csc.exe
mono --aot mcs.exe
mono --aot Microsoft.CodeAnalysis.CSharp.dll
mono --aot Microsoft.CodeAnalysis.dll
mono --aot mscorlib.dll
mono --aot System.Collections.Immutable.dll
mono --aot System.Reflection.Metadata.dll
# profile 
echo export PATH=/data/data/com.termux/files/usr/local/bin:$PATH >> ~/.bash_profile
```
