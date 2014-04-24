[Optimize Options - Using the GNU Compiler Collection (GCC)](http://gcc.gnu.org/onlinedocs/gcc/Optimize-Options.html)
-O
-O1
Optimize. Optimizing compilation takes somewhat more time, and a lot more memory for a large function.
With -O, the compiler tries to reduce code size and execution time, without performing any optimizations that take a great deal of compilation time.

-O turns on the following optimization flags:

          -fauto-inc-dec 
          -fcompare-elim 
          -fcprop-registers 
          -fdce 
          -fdefer-pop 
          -fdelayed-branch 
          -fdse 
          -fguess-branch-probability 
          -fif-conversion2 
          -fif-conversion 
          -fipa-pure-const 
          -fipa-profile 
          -fipa-reference 
          -fmerge-constants
          -fsplit-wide-types 
          -ftree-bit-ccp 
          -ftree-builtin-call-dce 
          -ftree-ccp 
          -ftree-ch 
          -ftree-copyrename 
          -ftree-dce 
          -ftree-dominator-opts 
          -ftree-dse 
          -ftree-forwprop 
          -ftree-fre 
          -ftree-phiprop 
          -ftree-slsr 
          -ftree-sra 
          -ftree-pta 
          -ftree-ter 
          -funit-at-a-time
-O also turns on -fomit-frame-pointer on machines where doing so does not interfere with debugging. 

-O2
Optimize even more. GCC performs nearly all supported optimizations that do not involve a space-speed tradeoff. As compared to -O, this option increases both compilation time and the performance of the generated code.
-O2 turns on all optimization flags specified by -O. It also turns on the following optimization flags:

          -fthread-jumps 
          -falign-functions  -falign-jumps 
          -falign-loops  -falign-labels 
          -fcaller-saves 
          -fcrossjumping 
          -fcse-follow-jumps  -fcse-skip-blocks 
          -fdelete-null-pointer-checks 
          -fdevirtualize -fdevirtualize-speculatively 
          -fexpensive-optimizations 
          -fgcse  -fgcse-lm  
          -fhoist-adjacent-loads 
          -finline-small-functions 
          -findirect-inlining 
          -fipa-sra 
          -fisolate-erroneous-paths-dereference 
          -foptimize-sibling-calls 
          -fpartial-inlining 
          -fpeephole2 
          -freorder-blocks  -freorder-functions 
          -frerun-cse-after-loop  
          -fsched-interblock  -fsched-spec 
          -fschedule-insns  -fschedule-insns2 
          -fstrict-aliasing -fstrict-overflow 
          -ftree-switch-conversion -ftree-tail-merge 
          -ftree-pre 
          -ftree-vrp
Please note the warning under -fgcse about invoking -O2 on programs that use computed gotos. 

-O3
Optimize yet more. -O3 turns on all optimizations specified by -O2 and also turns on the -finline-functions, -funswitch-loops, -fpredictive-commoning, -fgcse-after-reload, -ftree-loop-vectorize, -ftree-slp-vectorize, -fvect-cost-model, -ftree-partial-pre and -fipa-cp-clone options. 
-O0
Reduce compilation time and make debugging produce the expected results. This is the default. 
-Os
Optimize for size. -Os enables all -O2 optimizations that do not typically increase code size. It also performs further optimizations designed to reduce code size.
-Os disables the following optimization flags:

          -falign-functions  -falign-jumps  -falign-loops 
          -falign-labels  -freorder-blocks  -freorder-blocks-and-partition 
          -fprefetch-loop-arrays

-Ofast
Disregard strict standards compliance. -Ofast enables all -O3 optimizations. It also enables optimizations that are not valid for all standard-compliant programs. It turns on -ffast-math and the Fortran-specific -fno-protect-parens and -fstack-arrays. 
-Og
Optimize debugging experience. -Og enables optimizations that do not interfere with debugging. It should be the optimization level of choice for the standard edit-compile-debug cycle, offering a reasonable level of optimization while maintaining fast compilation and a good debugging experience.
If you use multiple -O options, with or without level numbers, the last such option is the one that is effective.
