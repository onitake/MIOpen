[//]: # (This file is a tempory place to update missing environment varibles in DebugAndLogging.md)
[//]: # (DebugAndLogging.md contains 88 env vars; Develop contains 157. Below is the difference)
1. MIOPEN_CONV_PRECISE_ROCBLAS_TIMING : Boolean 0/1, disable/enable convolution time precision; when enabled rocBLAS needs extra warm-up call for accurate timing 

2. MIOPEN_CUSTOM_CACHE_DIR : string, set custommized cache directory specified by the user

3. MIOPEN_DEBUG_AMD_ASM_KERNELS_PERF_FILTERING: commented out for now
4. MIOPEN_DEBUG_AMD_WINOGRAD_RXS_F2X3_PERF_VALS  [//]: # introduced for winograd kernel debug and testing. It allows you to override PerformanceConfig of the kernel. (PerformanceConfig contains one parameter : n_groups).

5. MIOPEN_DEBUG_AMD_WINOGRAD_RXS_F3X2_PERF_VALS  [//]: # same as above but for 3x2 kernel

6. MIOPEN_DEBUG_CK_BLOCK_SYNC_LDS_WITHOUT_SYNC_VMEM: Boolean 0/1; Compiler Flag; to sync LDS(Local Data Share); [//]: # (Followup)

7. MIOPEN_DEBUG_CK_USE_AMD_BUFFER_ADDRESSING : Boolean 0/1; Compiler Flag; Buffer addressing; [//]: # (Followup)

8. MIOPEN_DEBUG_COMGR_COMPILER_OPTIONS_INSERT: String, debug compiler options when building HIP

9. MIOPEN_DEBUG_COMGR_HIP_BUILD_FATBIN: Boolean 0/1; Build HIP and compile source to Fatbin

10. MIOPEN_DEBUG_COMGR_HIP_PCH_ENFORCE: Boolean 0/1; Store PCH Enforced status if PCH is supported [//]: # (Followup)

11. MIOPEN_DEBUG_COMGR_LOG_CALLS: Binary, if enabled, prints build logs onto console even if CMGR or HIPRTC call returns success

12. MIOPEN_DEBUG_COMGR_LOG_OPTIONS : logging options
0: Off.
1: Logs each option on a separate line.
2: Logs all options altogether, on single line.

13. MIOPEN_DEBUG_COMGR_LOG_SOURCE_NAMES : Boolean, when enabled, log source file name and size etc, e.g. hip.pch

14. MIOPEN_DEBUG_COMGR_LOG_SOURCE_TEXT: Int; Set logging information text file content/container size

15. MIOPEN_DEBUG_COMPILE_ONLY: Boolean 0/1, If enabled, running kernels on GPU is disabled and Search skipped

16. MIOPEN_DEBUG_CONVOLUTION_ATTRIB_FP16_ALT_IMPL : Please refer to MI200AlternateImplementation.md

17. MIOPEN_DEBUG_CONVOLUTION_DETERMINISTIC : to skip certain solvers that utilize atomic-addinstruction, which cause non-deterministirc results run-to-run. 
 /// * 0: Default.
/// * 1: skip the non-deterministic solvers.

18. MIOPEN_DEBUG_CONV_CK_IGEMM_FWD_V6R1_DLOPS_NCHW


MIOPEN_DEBUG_CONV_DIRECT_ASM_1X1UV2_PERF_VALS : String; configuation for 1x1 convolution with stride 2 GPU kernel in Assembly. 
MIOPEN_DEBUG_CONV_DIRECT_ASM_1X1UV2_SEARCH_OPTIMIZED
MIOPEN_DEBUG_CONV_DIRECT_ASM_1X1U_PERF_VALS
MIOPEN_DEBUG_CONV_DIRECT_ASM_1X1U_SEARCH_OPTIMIZED: Boolean, narrow search space in optimized mode
MIOPEN_DEBUG_CONV_DIRECT_ASM_3X3U_PERF_VALS
MIOPEN_DEBUG_CONV_DIRECT_ASM_WRW1X1_PERF_VALS
MIOPEN_DEBUG_CONV_DIRECT_ASM_WRW1X1_SEARCH_OPTIMIZED
MIOPEN_DEBUG_CONV_DIRECT_ASM_WRW3X3_PERF_VALS
MIOPEN_DEBUG_CONV_DIRECT_ASM_WRW3X3_SEARCH_OPTIMIZED
MIOPEN_DEBUG_CONV_DIRECT_NAIVE_CONV_BWD : Boolean, to choose naive convolution backward solver
MIOPEN_DEBUG_CONV_DIRECT_NAIVE_CONV_FWD : Boolean, to choose naive convolution forward solver
MIOPEN_DEBUG_CONV_DIRECT_NAIVE_CONV_WRW : What is WRW
MIOPEN_DEBUG_CONV_DIRECT_OCL_WRW2_SEARCH_OPTIMIZED : Boolean
MIOPEN_DEBUG_CONV_IMMED_FALLBACK : Boolean, disable fallback solution when disabled
MIOPEN_DEBUG_CONV_IMPLICIT_GEMM_ASM_BWD_GTC_XDLOPS_NHWC
MIOPEN_DEBUG_CONV_IMPLICIT_GEMM_ASM_FWD_GTC_XDLOPS_NHWC
MIOPEN_DEBUG_CONV_IMPLICIT_GEMM_ASM_PK_ATOMIC_ADD_FP16
MIOPEN_DEBUG_CONV_IMPLICIT_GEMM_ASM_WRW_GTC_XDLOPS_NHWC
MIOPEN_DEBUG_CONV_IMPLICIT_GEMM_BLOCK_SYNC_LDS_WITHOUT_SYNC_VMEM
MIOPEN_DEBUG_CONV_IMPLICIT_GEMM_HIP_BWD_V4R1_XDLOPS_PERF_VALS
MIOPEN_DEBUG_CONV_IMPLICIT_GEMM_XDLOPS : Tensor core (XDLOPS)
MIOPEN_DEBUG_CONV_IMPLICIT_GEMM_XDLOPS_EMULATE
MIOPEN_DEBUG_CONV_MLIR_IGEMM_BWD
MIOPEN_DEBUG_CONV_MLIR_IGEMM_BWD_XDLOPS
MIOPEN_DEBUG_CONV_MLIR_IGEMM_FWD
MIOPEN_DEBUG_CONV_MLIR_IGEMM_FWD_XDLOPS
MIOPEN_DEBUG_CONV_MLIR_IGEMM_WRW
MIOPEN_DEBUG_CONV_MLIR_IGEMM_WRW_XDLOPS
MIOPEN_DEBUG_DISABLE_FIND_DB
MIOPEN_DEBUG_DISABLE_SQL_WAL
MIOPEN_DEBUG_DYNAMIC_REDUCTION
MIOPEN_DEBUG_ENFORCE_DEVICE : String: user specified device name

MIOPEN_DEBUG_HIP_DUMP: Boolean, when enabled, add -gline-tables-only and -save-temps parameters when building HIP

MIOPEN_DEBUG_HIP_VERBOSE: Boolean, when enabled, add -v (verbose) parameter when building HIP

MIOPEN_DEBUG_IMPLICIT_GEMM_FIND_ALL_SOLUTIONS

MIOPEN_DEBUG_IMPLICIT_GEMM_NON_XDLOPS_INLINE_ASM: Boolean, enable inline ASM for certain AMD products
MIOPEN_DEBUG_IMPLICIT_GEMM_XDLOPS_INLINE_ASM : Boolean, unused (?)
[//]: # (Followup)

MIOPEN_DEBUG_LOGGING_QUIETING_DISABLE
MIOPEN_DEBUG_OPENCL_ENFORCE_CODE_OBJECT_OPTION
MIOPEN_DEBUG_OPENCL_WAVE64_NOWGP
MIOPEN_DEBUG_SAVE_TEMP_DIR : Boolean, when enabled, log build info currently avaible for compiling HIP
MIOPEN_DEBUG_SRAM_EDC_DISABLED

MIOPEN_DEBUG_USE_HIPRTC : Boolean, When enabled, use HIPRTC to build HIP 

MIOPEN_DEVICE_ARCH : String, declared in multiple places
[//]: # (Followup)

MIOPEN_DEVICE_CU: Int, number of computing units

MIOPEN_DISABLE_CACHE: defined in cache.md

MIOPEN_DRIVER_PAD_BUFFERS_2M : Boolean, When enabled, Padding buffers allocations to be multiplication of 2M
[//]: # (Followup)

MIOPEN_DRIVER_USE_GPU_REFERENCE: Boolean, when enabled, use GPU as reference
[//]: # (Followup)

MIOPEN_EXPERIMENTAL_GCN_ASM_PATH

MIOPEN_FIND_ENFORCE: String, 
[//]: # (Followup)

MIOPEN_FIND_MODE : defined in find_and_immediate.md

MIOPEN_SYSTEM_DB_PATH : String, path of system db files

MIOPEN_USER_DB_PATH : String, path of user db files

MIOPEN_VERIFY_CACHE_PATH: String, Path of MIOpen cache, default is ~/.cache/miopen/tests
