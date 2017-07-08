Currently with mono 5.0.1.1 or 5.2.0.179beta is impossible to build because of error connectet with mono
https://github.com/mono/mono/commit/249ee0686bf87f33acf2efde76f3645ef06bb886
(EntryPoint="Mono_Unix_VersionString"  causing problem)

Another way to xbuild SiKUploader.sln is to manuakl copy *.targets and *.tasks files from /Mono/lib/mono/4.5/ to /Mono/lib/mono/3.5/

Run with mono uploader.exe
