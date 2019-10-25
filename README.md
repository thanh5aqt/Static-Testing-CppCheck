Câu lệnh trên teminal
cppcheck --enable=all --inconclusive --std=posix test.cpp Juliet_Test_Suite_v1.3_for_C_Cpp Juliet_Test_Suite_v1.3_for_C_Cpp 2> err.txt

--enable=<id>        Enable additional checks. The available ids are:
                          * all
                                  Enable all checks. It is recommended to only
                                  use --enable=all when the whole program is
                                  scanned, because this enables unusedFunction.

 --inconclusive       Allow that Cppcheck reports even though the analysis is
                         inconclusive.
                         There are false positives with this option. Each result
                         must be carefully investigated before you know if it is
                         good or bad.
 --std=<id>           Set standard.
                         The available options are:
                          * posix
                                 POSIX compatible code

2> err.txt write error to a file 

Tất cả các phát hiện sau khi chạy cppcheck:
	10522(error)
used when bugs are found
	125480(style)
stylistic issues related to code cleanup (unused functions, redundant code, constness, and such)
	3931(warning)
suggestions about defensive programming to prevent bugs
	214(performance)
Suggestions for making the code faster. These suggestions are only based on
common knowledge. It is not certain you’ll get any measurable difference in
speed by fixing these messages.
	870(portability)
portability warnings. 64-bit portability. code might work different on different
compilers. etc.


