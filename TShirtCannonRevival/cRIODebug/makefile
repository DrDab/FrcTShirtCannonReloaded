################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include src/subdir.mk
-include subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(CC_DEPS)),)
-include $(CC_DEPS)
endif
ifneq ($(strip $(C++_DEPS)),)
-include $(C++_DEPS)
endif
ifneq ($(strip $(C_UPPER_DEPS)),)
-include $(C_UPPER_DEPS)
endif
ifneq ($(strip $(CXX_DEPS)),)
-include $(CXX_DEPS)
endif
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
ifneq ($(strip $(CPP_DEPS)),)
-include $(CPP_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 

# All Target
all: TShirtCannonRevival.so

# Tool invocations
TShirtCannonRevival.so: $(OBJS) $(USER_OBJS)
	@echo 'Building target: $@'
	@echo 'Invoking: Thunder cRIO Tools Partial Linker'
	powerpc-wrs-vxworks-g++ -nostdlib -L"C:\Program Files (x86)\FRC_Toolchain\mingw\powerpc-wrs-vxworks\wind_base\/../lib" -mcpu=603 -mstrict-align -mlongcall -static -r -Xlinker -X -o "TShirtCannonRevival.so" $(OBJS) $(USER_OBJS) $(LIBS)
	@echo 'Finished building target: $@'
	@echo ' '
	$(MAKE) --no-print-directory post-build

# Other Targets
clean:
	-$(RM) $(CC_DEPS)$(C++_DEPS)$(EXECUTABLES)$(OBJS)$(C_UPPER_DEPS)$(CXX_DEPS)$(C_DEPS)$(CPP_DEPS) TShirtCannonRevival.so
	-@echo ' '

post-build:
	-powerpc-wrs-vxworks-nm "C:/Users/YukiLeopard/Documents/frc2020offseason/FrcTShirtCannonReloaded/TShirtCannonRevival/cRIODebug/TShirtCannonRevival.so" | tclsh "C:\Program Files (x86)\FRC_Toolchain\mingw\powerpc-wrs-vxworks\wind_base\/host/resource/hutils/tcl/munch.tcl" -c ppc | sed "s/extern void\(.*\);/extern void \1 __attribute__((externally_visible));/" > "C:/Users/YukiLeopard/Documents/frc2020offseason/FrcTShirtCannonReloaded/TShirtCannonRevival/cRIODebug/ctdt.c"  && powerpc-wrs-vxworks-gcc -c "C:/Users/YukiLeopard/Documents/frc2020offseason/FrcTShirtCannonReloaded/TShirtCannonRevival/cRIODebug/ctdt.c" -o ctdt.o -DCPU=PPC603 -DTOOL_FAMILY=gnu -DTOOL=gnu -D_WRS_KERNEL -fmessage-length=0  -mcpu=603 -mstrict-align -mlongcall &&  powerpc-wrs-vxworks-g++ "C:/Users/YukiLeopard/Documents/frc2020offseason/FrcTShirtCannonReloaded/TShirtCannonRevival/cRIODebug/ctdt.o" "C:/Users/YukiLeopard/Documents/frc2020offseason/FrcTShirtCannonReloaded/TShirtCannonRevival/cRIODebug/TShirtCannonRevival.so" -o "C:/Users/YukiLeopard/Documents/frc2020offseason/FrcTShirtCannonReloaded/TShirtCannonRevival/cRIODebug/TShirtCannonRevival.so.out" -DCPU=PPC603 -DTOOL_FAMILY=gnu -DTOOL=gnu -D_WRS_KERNEL -fmessage-length=0  -mcpu=603 -mstrict-align -mlongcall -r -Wl,-X -static -T "C:\Program Files (x86)\FRC_Toolchain\mingw\powerpc-wrs-vxworks\wind_base\\..\share\ldscripts\dkm.ld" &&  powerpc-wrs-vxworks-stripsyms.bat "C:/Users/YukiLeopard/Documents/frc2020offseason/FrcTShirtCannonReloaded/TShirtCannonRevival/cRIODebug/TShirtCannonRevival.so.out" "C:\Program Files (x86)\FRC_Toolchain\mingw\powerpc-wrs-vxworks\wind_base\\..\lib\libstdc++.a" "C:\Program Files (x86)\FRC_Toolchain\mingw\powerpc-wrs-vxworks\wind_base\\..\lib\libsupc++.a" "C:\Program Files (x86)\FRC_Toolchain\mingw\powerpc-wrs-vxworks\wind_base\\..\..\lib\gcc\powerpc-wrs-vxworks\4.8.2\libgcc.a"
	-@echo ' '

.PHONY: all clean dependents post-build

-include ../makefile.targets
