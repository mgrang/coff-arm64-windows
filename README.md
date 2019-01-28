# COFF ARM64 Windows Target

This README details my upstream LLVM work on enabling the arm64-windows target in LLVM.

### Chromium ARM64 Windows Support

http://llvmweekly.org/issue/265

http://lists.llvm.org/pipermail/llvm-dev/2018-July/124687.html

https://bugs.chromium.org/p/chromium/issues/detail?id=893460#c21

### Structured Exception Handling (SEH) patches:

https://reviews.llvm.org/D53540  [Implement support for SEH extensions __try/__except/__finally]

https://reviews.llvm.org/D56747  [Rename llvm.x86.seh.recoverfp intrinsic to llvm.eh.recoverfp]

https://reviews.llvm.org/D56748  [Rename llvm.x86.seh.recoverfp intrinsic to llvm.eh.recoverfp]

https://reviews.llvm.org/D53541  [Do not emit x86_seh_recoverfp intrinsic]

https://reviews.llvm.org/D50029	 [Enable SEH for ARM64 Windows]

https://reviews.llvm.org/D56037  [Emit the correct MCExpr relocations specifiers like VK_ABS_G0, etc]

https://reviews.llvm.org/D56029  [Support resolving signed fixups for :abs_g0_s: etc.]

### ARM64 Intrinsics patches:

https://reviews.llvm.org/D56685    [Add __byteswap intrinsics]

https://reviews.llvm.org/D56671    [Add __nop intrinsic]

https://reviews.llvm.org/D53962	   [Implement llvm.addressofreturnaddress intrinsic]

https://reviews.llvm.org/rC345808  [Implement llvm.addressofreturnaddress intrinsic]

https://reviews.llvm.org/D54068    [Implement InterlockedDecrement*_* builtins]

https://reviews.llvm.org/D54067	   [Implement InterlockedIncrement*_* builtins]

https://reviews.llvm.org/D54066	   [Implement InterlockedAnd*_* builtins]

https://reviews.llvm.org/rC346205  [Implement InterlockedXor*_* builtins]

https://reviews.llvm.org/rC346190  [Implement InterlockedOr*_* builtins]

https://reviews.llvm.org/D54062	   [Implement InterlockedCompareExchange*_* builtins]

https://reviews.llvm.org/D54046	   [Implement InterlockedExchange*_* builtins]

https://reviews.llvm.org/D53115	   [Add _ReadStatusReg and_WriteStatusReg intrinsics]

https://reviews.llvm.org/D52811	   [Add _InterlockedAdd intrinsic]

https://reviews.llvm.org/D52807	   [Add _InterlockedCompareExchangePointer_nf intrinsic]

https://reviews.llvm.org/D52838	   [Add __getReg intrinsic]

https://reviews.llvm.org/D52809	   [Add _ReadWriteBarrier intrinsic]

https://reviews.llvm.org/D53115	   [Add _ReadStatusReg and_WriteStatusReg intrinsics]

https://reviews.llvm.org/D49445	   [Add more missing MSVC ARM64 intrinsics]

https://reviews.llvm.org/D48132	   [Add ARM64 intrinsics: __yield, __wfe, __wfi, __sev, __sevl]

https://reviews.llvm.org/D36110	   [Add MS builtins __dmb, __dsb, __isb]

### ARM64 Calling Convention and other patches:

https://reviews.llvm.org/D55535	 [Emit COFF function header]

https://reviews.llvm.org/D54248	 [Add support for MSVC buffer security check]

https://reviews.llvm.org/D35531	 [Reserve X18 register by default]

https://reviews.llvm.org/D49464	 [Decide when to mark struct returns as SRet]

https://reviews.llvm.org/D34859	 [Set the data type widths and the data layout string]

https://reviews.llvm.org/D34706	 [Add support for Windows ARM64 COFF format]

https://reviews.llvm.org/D34857	 [Add initial relocation types]

https://reviews.llvm.org/D34705	 [Add support for Windows ARM64 COFF format]

https://reviews.llvm.org/D34659	 [Fix typo in COFF ARM64 Relocation Type]

https://reviews.llvm.org/D35518  [Add support to emit CodeView debug info for ARM64 COFF]
