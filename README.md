# termux-mono-aarch64-api22

-AOT cache

cd /data/data/com.termux/files/usr/local/lib/mono/4.5
mono --aot csc.exe
mono --aot mcs.exe
mono --aot Microsoft.CodeAnalysis.CSharp.dll
mono --aot Microsoft.CodeAnalysis.dll
mono --aot mscorlib.dll
mono --aot System.Collections.Immutable.dll
mono --aot System.Reflection.Metadata.dll

-profile

echo export PATH=/data/data/com.termux/files/usr/local/bin:$PATH >> ~/.bash_profile
