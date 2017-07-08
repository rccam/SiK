Currently with mono 5.0.1.1 or 5.2.0.179beta is impossible to build because of error connectet with mono
https://github.com/mono/mono/commit/249ee0686bf87f33acf2efde76f3645ef06bb886
(EntryPoint="Mono_Unix_VersionString"  causing problem)

To fix that replace with folder https://github.com/rccam/SiK/tree/master/Mono.Posix/4.0.0.0__0738eb9f132ed756  C:\Program Files (x86)\Mono\lib\mono\gac\Mono.Posix\4.0.0.0__0738eb9f132ed756


Another ways:
  - install mono 4.2.1.102 (https://download.mono-project.com/archive/4.2.1/)
  - xbuild SIKUloader.csproj
  
Or:
  - install mono 4.2.1.102 (https://download.mono-project.com/archive/4.2.1/)
  - manual copy *.targets and *.tasks files from /Mono/lib/mono/4.5/ to /Mono/lib/mono/3.5/
  - xbuild SiKUploader.sln



Run with mono uploader.exe
