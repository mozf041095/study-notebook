# gfortran的使用

## 编译
### 命令行编译
* 注意：
> gfortran 默认会将 .f, .for, .fpp, .ftn, .F, .FOR, .FPP 和 .FTN 结尾的文件作为固定格式处理，
> 而将.f90, .f95, .f03, .F90, .F95 和 .F03 结尾的文件作为自由格式来处理。
* 固定格式： `gfortran helloworld.f -o helloworld`
> 传统的 Fortran 程序（也就是以 Fortran 77 为代表的）只能用大写字符书写，而且每行前六个字符为特定用途所保留。
> 第一列为字符 C 或 * 所保留，用来表征整行都是注释。第二列到第六列是为标号预留的。代码从第七列开始，到72列结束（73列及以后将被直接忽略，可作注释）。
* 自由格式： `gfortran helloworldff.f90 -o helloworldff`
> 注释以感叹号（！）开始直到行尾，其中语句、标号都可从任一列开始。
* 固定转自由： `mv helloworldff.f90 helloworldff.for |  gfortran -ffree-form helloworldff.for -o helloworldff`
* 自由转固定： `mv helloworld.f helloworld.f90 | gfortran helloworld.f90 -ffixed-form -o helloworld`
* 多文件： `gfortran caller.f called.f -o caller`
* 汇编： `gfortran -S helloworld.f`
### 注意
* gfortran是gcc的一个前端，以下等价：
`gfortran helloworld.f -o helloworld`与`gcc helloworld.f -o helloworld -lgfortran -lgfortranbegin`
## 引用
1. [Fortran 编程中相关文件后缀](http://www.cnblogs.com/djcsch2001/archive/2012/01/12/2321062.html)
