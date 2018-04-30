# BuildTools
Build related things

I made this repo to keep track of things to help me build.

#LLVM-vs2017
Clang 6.0 doesn't currently install itself into Visual Studio 2017, It worked on 2015 but running through 2017 still used the 2015 STL.
Dropping this folder into my C:\Program Files (x86)\Microsoft Visual Studio\2017\Community\Common7\IDE\VC\VCTargets\Platforms\x64\PlatformToolsets folder (alongside v141) got it working.
It was basically just the old LLVM-vs2014 targets told to look for the 141 folders instead of 140.