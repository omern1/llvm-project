add_llvm_component_library(LLVMTextAPI
  Architecture.cpp
  ArchitectureSet.cpp
  InterfaceFile.cpp
  TextStubV5.cpp
  PackedVersion.cpp
  Platform.cpp
  RecordsSlice.cpp
  Symbol.cpp
  SymbolSet.cpp
  Target.cpp
  TextAPIError.cpp
  TextStub.cpp
  TextStubCommon.cpp

  ADDITIONAL_HEADER_DIRS
  "${LLVM_MAIN_INCLUDE_DIR}/llvm/TextAPI"

  LINK_COMPONENTS
  Support
  BinaryFormat
  TargetParser
)
