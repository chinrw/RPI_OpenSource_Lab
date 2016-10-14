
## Step2

[chin39@virtual build2]$ cmake -DUSE_MYMATH=OFF   
-- The C compiler identification is GNU 6.2.1  
-- The CXX compiler identification is GNU 6.2.1  
-- Check for working C compiler: /usr/bin/cc  
-- Check for working C compiler: /usr/bi.n/cc -- works  
-- Detecting C compiler ABI info  
-- Detecting C compiler ABI info - done  
-- Detecting C compile features  
-- Detecting C compile features - done  
-- Check for working CXX compiler: /usr/bin/c++  
-- Check for working CXX compiler: /usr/bin/c++ -- works  
-- Detecting CXX compiler ABI info  
-- Detecting CXX compiler ABI info - done  
-- Detecting CXX compile features  
-- Detecting CXX compile features - done  
-- Configuring done  
-- Generating done  
-- Build files have been written to: /home/chin39/Dropbox/GitHub/test/build2  

[chin39@virtual build2]$ make
Scanning dependencies of target Tutorial  
[ 50%] Building CXX object CMakeFiles/Tutorial.dir/tutorial.cxx.o  
[100%] Linking CXX executable Tutorial  
[100%] Built target Tutorial  

[chin39@virtual build2]$ ./Tutorial 4  
The square root of 4 is 2  


[chin39@virtual build2]$ cmake -DUSE_MYMATH=ON ..  
-- The C compiler identification is GNU 6.2.1  
-- The CXX compiler identification is GNU 6.2.1  
-- Check for working C compiler: /usr/bin/cc  
-- Check for working C compiler: /usr/bin/cc -- works  
-- Detecting C compiler ABI info  
-- Detecting C compiler ABI info - done  
-- Detecting C compile features  
-- Detecting C compile features - done  
-- Check for working CXX compiler: /usr/bin/c++  
-- Check for working CXX compiler: /usr/bin/c++ -- works  
-- Detecting CXX compiler ABI info  
-- Detecting CXX compiler ABI info - done  
-- Detecting CXX compile features  
-- Detecting CXX compile features - done  
-- Configuring done  
-- Generating done  
-- Build files have been written to: /home/chin39/Dropbox/GitHub/test/build2  

[chin39@virtual build2]$ make  
Scanning dependencies of target MathFunctions  
[ 25%] Building CXX object MathFunctions/CMakeFiles/MathFunctions.dir/mysqrt.cxx.o  
[ 50%] Linking CXX static library libMathFunctions.a  
[ 50%] Built target MathFunctions  
Scanning dependencies of target Tutorial  
[ 75%] Building CXX object CMakeFiles/Tutorial.dir/tutorial.cxx.o  
[100%] Linking CXX executable Tutorial  
[100%] Built target Tutorial  

[chin39@virtual build2]$ ./Tutorial 4  
The square root of 4 is 3  

## Step3

[chin39@virtual build3]$ cmake ..  
-- Configuring done  
-- Generating done  
-- Build files have been written to: /home/chin39/Dropbox/GitHub/test/build3  
[chin39@virtual build3]$ make  
Scanning dependencies of target MathFunctions  
[ 25%] Building CXX object MathFunctions/CMakeFiles/MathFunctions.dir/mysqrt.cxx.o  
[ 50%] Linking CXX static library libMathFunctions.a  
[ 50%] Built target MathFunctions  
Scanning dependencies of target Tutorial  
[ 75%] Building CXX object CMakeFiles/Tutorial.dir/tutorial.cxx.o  
[100%] Linking CXX executable Tutorial  
[100%] Built target Tutorial  
[chin39@virtual build3]$ ctest  
Test project /home/chin39/Dropbox/GitHub/test/build3  
    Start 1: TutorialRuns  
1/5 Test #1: TutorialRuns .....................   Passed    0.00 sec  
    Start 2: TutorialComp25  
2/5 Test #2: TutorialComp25 ...................   Passed    0.00 sec  
    Start 3: TutorialNegative  
3/5 Test #3: TutorialNegative .................   Passed    0.00 sec  
    Start 4: TutorialSmall  
4/5 Test #4: TutorialSmall ....................   Passed    0.00 sec  
    Start 5: TutorialUsage  
5/5 Test #5: TutorialUsage ....................   Passed    0.00 sec  

100% tests passed, 0 tests failed out of 5  

Total Test time (real) =   0.01 sec  

## Step4

[chin39@virtual build4]$ cmake ..  
-- The C compiler identification is GNU 6.2.1  
-- The CXX compiler identification is GNU 6.2.1  
-- Check for working C compiler: /usr/bin/cc  
-- Check for working C compiler: /usr/bin/cc -- works  
-- Detecting C compiler ABI info  
-- Detecting C compiler ABI info - done  
-- Detecting C compile features
-- Detecting C compile features - done  
-- Check for working CXX compiler: /usr/bin/c++  
-- Check for working CXX compiler: /usr/bin/c++ -- works  
-- Detecting CXX compiler ABI info  
-- Detecting CXX compiler ABI info - done  
-- Detecting CXX compile features  
-- Detecting CXX compile features - done  
-- Looking for log  
-- Looking for log - not found  
-- Looking for exp  
-- Looking for exp - not found  
-- Configuring done  
-- Generating done  
-- Build files have been written to: /home/chin39/Dropbox/GitHub/test/build4  
[chin39@virtual build4]$ make  
Scanning dependencies of target MathFunctions  
[ 25%] Building CXX object MathFunctions/CMakeFiles/MathFunctions.dir/mysqrt.cxx.o  
[ 50%] Linking CXX static library libMathFunctions.a  
[ 50%] Built target MathFunctions  
Scanning dependencies of target Tutorial  
[ 75%] Building CXX object CMakeFiles/Tutorial.dir/tutorial.cxx.o  
[100%] Linking CXX executable Tutorial  
[100%] Built target Tutorial  
[chin39@virtual build4]$ ./Tutorial 4  
Computing sqrt of 4 to be 2.5  
Computing sqrt of 4 to be 2.05  
Computing sqrt of 4 to be 2.00061  
Computing sqrt of 4 to be 2  
Computing sqrt of 4 to be 2  
Computing sqrt of 4 to be 2  
Computing sqrt of 4 to be 2  
Computing sqrt of 4 to be 2  
Computing sqrt of 4 to be 2  
Computing sqrt of 4 to be 2  
The square root of 4 is 2  

## Step5

[chin39@virtual build5]$ cmake ..  
-- The C compiler identification is GNU 6.2.1  
-- The CXX compiler identification is GNU 6.2.1  
-- Check for working C compiler: /usr/bin/cc  
-- Check for working C compiler: /usr/bin/cc -- works  
-- Detecting C compiler ABI info  
-- Detecting C compiler ABI info - done  
-- Detecting C compile features  
-- Detecting C compile features - done  
-- Check for working CXX compiler: /usr/bin/c++  
-- Check for working CXX compiler: /usr/bin/c++ -- works  
-- Detecting CXX compiler ABI info  
-- Detecting CXX compiler ABI info - done  
-- Detecting CXX compile features  
-- Detecting CXX compile features - done  
-- Looking for log  
-- Looking for log - not found  
-- Looking for exp  
-- Looking for exp - not found  
-- Configuring done  
-- Generating done  
-- Build files have been written to: /home/chin39/Dropbox/GitHub/test/build5  
[chin39@virtual build5]$ make  
Scanning dependencies of target MakeTable  
[ 14%] Building CXX object MathFunctions/CMakeFiles/MakeTable.dir/MakeTable.cxx.o  
[ 28%] Linking CXX executable MakeTable  
[ 28%] Built target MakeTable  
[ 42%] Generating Table.h  
Scanning dependencies of target MathFunctions  
[ 57%] Building CXX object MathFunctions/CMakeFiles/MathFunctions.dir/mysqrt.cxx.o  
[ 71%] Linking CXX static library libMathFunctions.a  
[ 71%] Built target MathFunctions  
Scanning dependencies of target Tutorial  
[ 85%] Building CXX object CMakeFiles/Tutorial.dir/tutorial.cxx.o  
[100%] Linking CXX executable Tutorial  
[100%] Built target Tutorial  
[chin39@virtual build5]$ ./Tutorial 4  
Computing sqrt of 4 to be 2.5  
Computing sqrt of 4 to be 2.05  
Computing sqrt of 4 to be 2.00061  
Computing sqrt of 4 to be 2  
Computing sqrt of 4 to be 2  
Computing sqrt of 4 to be 2  
Computing sqrt of 4 to be 2  
Computing sqrt of 4 to be 2  
Computing sqrt of 4 to be 2  
Computing sqrt of 4 to be 2  
The square root of 4 is 2  
