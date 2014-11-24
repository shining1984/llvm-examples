LLVM_CONFIG = llvm-config
LLVM_CXXFLAGS += $(shell $(LLVM_CONFIG) --cxxflags)
LLVM_LDFLAGS := $(shell $(LLVM_CONFIG) --ldflags)
LLVM_LIBS = $(shell $(LLVM_CONFIG) --libs bitwriter core support)

llvm_model_src = ModuleMaker.cpp


test_model:
	g++ $(llvm_model_src) $(LLVM_CXXFLAGS) $(LLVM_LIBS) $(LLVM_LDFLAGS) -lpthread -ldl -o ModuleMaker




