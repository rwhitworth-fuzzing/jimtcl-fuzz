`id:000040,sig:06,src:001944,op:havoc,rep:4`

```
#0  __GI_raise (sig=sig@entry=6) at ../sysdeps/unix/sysv/linux/raise.c:51
#1  0x00007f0416b043fa in __GI_abort () at abort.c:89
#2  0x00007f0416b40bd0 in __libc_message (do_abort=do_abort@entry=2, fmt=fmt@entry=0x7f0416c35dd0 "*** Error in `%s': %s: 0x%s ***\n")
    at ../sysdeps/posix/libc_fatal.c:175
#3  0x00007f0416b46f96 in malloc_printerr (action=3, str=0x7f0416c35f28 "double free or corruption (fasttop)", ptr=<optimized out>, ar_ptr=<optimized out>)
    at malloc.c:5049
#4  0x00007f0416b477de in _int_free (av=0x7f0416e69b00 <main_arena>, p=0x1ecd550, have_lock=0) at malloc.c:3905
#5  0x000000000040bdc7 in Jim_Free (ptr=0x2) at jim.c:653
#6  Jim_FreeObj (interp=<optimized out>, objPtr=0x1ed3fb0) at jim.c:2194
#7  Jim_SetResultFormatted (interp=<optimized out>, format=<optimized out>) at jim.c:15466
#8  0x000000000041163a in SetBooleanFromAny (flags=1, interp=<optimized out>, objPtr=<optimized out>) at jim.c:6127
#9  Jim_GetBoolean (interp=0x1eaf010, objPtr=0x1ed3fb0, booleanPtr=0x7ffe970ed3bc) at jim.c:6103
#10 0x00000000004222a4 in ExprBool (obj=0x1ed3fb0, interp=<optimized out>) at jim.c:8250
#11 JimExprGetTermBoolean (interp=0x1eaf010, node=<optimized out>) at jim.c:9220
#12 0x00000000004207e6 in JimExprOpAnd (interp=0x1eaf010, node=0x1eda430) at jim.c:8263
#13 0x0000000000415da2 in JimExprEvalTermNode (interp=0x1eaf010, node=0x7ffe970ecc50) at jim.c:9160
#14 0x00000000004148c2 in Jim_EvalExpression (interp=0x1eaf010, exprObjPtr=<optimized out>) at jim.c:9320
#15 0x0000000000419100 in JimExpandExprSugar (interp=0x1eaf010, objPtr=0x7ffe970ecc50) at jim.c:4933
#16 JimSubstOneToken (interp=<optimized out>, token=<optimized out>, objPtrPtr=<optimized out>) at jim.c:10187
#17 JimInterpolateTokens (interp=<optimized out>, token=<optimized out>, tokens=<optimized out>, flags=<optimized out>) at jim.c:10238
#18 0x000000000041828b in Jim_EvalObj (interp=<optimized out>, scriptObjPtr=<optimized out>) at jim.c:10481
#19 0x000000000041a4c8 in Jim_EvalFile (interp=0x1eaf010, filename=<optimized out>) at jim.c:10928
#20 0x000000000040743d in main (argc=<optimized out>, argv=0x7ffe970ed7f8) at jimsh.c:140
```

`id:000377,sig:11,src:007620,op:ext_AO,pos:476`
```
#0  __GI_raise (sig=sig@entry=6) at ../sysdeps/unix/sysv/linux/raise.c:51
#1  0x00007f1f7d7073fa in __GI_abort () at abort.c:89
#2  0x00007f1f7d743bd0 in __libc_message (do_abort=do_abort@entry=2, fmt=fmt@entry=0x7f1f7d838dd0 "*** Error in `%s': %s: 0x%s ***\n")
    at ../sysdeps/posix/libc_fatal.c:175
#3  0x00007f1f7d749f96 in malloc_printerr (action=3, str=0x7f1f7d838f08 "double free or corruption (top)", ptr=<optimized out>, ar_ptr=<optimized out>)
    at malloc.c:5049
#4  0x00007f1f7d74a7de in _int_free (av=0x7f1f7da6cb00 <main_arena>, p=0xd0f660, have_lock=0) at malloc.c:3905
#5  0x000000000041e805 in Jim_Free (ptr=0x2) at jim.c:653
#6  FreeListInternalRep (interp=<optimized out>, objPtr=<optimized out>) at jim.c:6168
#7  0x000000000041d51c in Jim_FreeObj (interp=0xce3010, objPtr=0xd0f340) at jim.c:2190
#8  FreeDictSubstInternalRep (interp=0xce3010, objPtr=0xd0bee0) at jim.c:4875
#9  0x000000000041e2af in Jim_FreeObj (objPtr=0xd0bee0, interp=<optimized out>) at jim.c:2190
#10 JimVariablesHTValDestructor (interp=0xce3010, val=0xd0c0e0) at jim.c:3812
#11 0x0000000000408a81 in Jim_FreeHashTable (ht=<optimized out>) at jim.c:921
#12 0x0000000000410afb in JimFreeCallFrame (interp=<optimized out>, cf=<optimized out>, action=<optimized out>) at jim.c:5031
#13 0x000000000040fabe in Jim_FreeInterp (i=<optimized out>) at jim.c:5539
#14 0x000000000040756c in main (argc=<optimized out>, argv=<optimized out>) at jimsh.c:156
```


`id:000452,sig:06,src:007658,op:havoc,rep:8`
```
#0  __GI_raise (sig=sig@entry=6) at ../sysdeps/unix/sysv/linux/raise.c:51
#1  0x00007f338e8cf3fa in __GI_abort () at abort.c:89
#2  0x00007f338e90bbd0 in __libc_message (do_abort=do_abort@entry=2, fmt=fmt@entry=0x7f338ea00dd0 "*** Error in `%s': %s: 0x%s ***\n")
    at ../sysdeps/posix/libc_fatal.c:175
#3  0x00007f338e911f96 in malloc_printerr (action=3, str=0x7f338ea00f08 "double free or corruption (top)", ptr=<optimized out>, ar_ptr=<optimized out>)
    at malloc.c:5049
#4  0x00007f338e9127de in _int_free (av=0x7f338ec34b00 <main_arena>, p=0x23c5ff0, have_lock=0) at malloc.c:3905
#5  0x000000000041d556 in Jim_Free (ptr=0x2) at jim.c:653
#6  Jim_FreeObj (interp=<optimized out>, objPtr=0x23c5cf0) at jim.c:2194
#7  FreeDictSubstInternalRep (interp=0x2396010, objPtr=0x23c4620) at jim.c:4875
#8  0x000000000041e2af in Jim_FreeObj (objPtr=0x23c4620, interp=<optimized out>) at jim.c:2190
#9  JimVariablesHTValDestructor (interp=0x2396010, val=0x23bf160) at jim.c:3812
#10 0x0000000000408a81 in Jim_FreeHashTable (ht=<optimized out>) at jim.c:921
#11 0x0000000000410afb in JimFreeCallFrame (interp=<optimized out>, cf=<optimized out>, action=<optimized out>) at jim.c:5031
#12 0x000000000040fabe in Jim_FreeInterp (i=<optimized out>) at jim.c:5539
#13 0x000000000040756c in main (argc=<optimized out>, argv=<optimized out>) at jimsh.c:156
```

