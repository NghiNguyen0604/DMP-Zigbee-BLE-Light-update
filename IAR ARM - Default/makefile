################################################################################
# Automatically-generated file. Do not edit!
################################################################################

export WINEDEBUG=-all

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include zll-utility-client/subdir.mk
-include zll-identify-server/subdir.mk
-include zll-commissioning-common/subdir.mk
-include zll-commissioning-client/subdir.mk
-include zcl-framework-core/subdir.mk
-include update-tc-link-key/subdir.mk
-include strong-random/subdir.mk
-include spidisplay/subdir.mk
-include simple-main/subdir.mk
-include serial/EFR32/subdir.mk
-include serial/subdir.mk
-include scan-dispatch/subdir.mk
-include nvm3/EFR32/subdir.mk
-include nvm3/subdir.mk
-include network-steering/subdir.mk
-include mbedtls/EFR32/subdir.mk
-include kit-drivers/subdir.mk
-include interpan/subdir.mk
-include idle-sleep/subdir.mk
-include identify/subdir.mk
-include hal-library/EFR32/subdir.mk
-include groups-client/subdir.mk
-include green-power-common/subdir.mk
-include green-power-client/subdir.mk
-include glib/EFR32/subdir.mk
-include glib/subdir.mk
-include form-and-join/subdir.mk
-include find-and-bind-initiator/subdir.mk
-include external-generated-files/subdir.mk
-include emlib/subdir.mk
-include emdrv/subdir.mk
-include ember-minimal-printf/subdir.mk
-include efr32/subdir.mk
-include eeprom/subdir.mk
-include dmp-ui-demo/subdir.mk
-include debug-jtag-stub/EFR32/subdir.mk
-include debug-basic-library/EFR32/subdir.mk
-include counters/subdir.mk
-include coexistence-stub/EFR32/subdir.mk
-include ccm-encryption/subdir.mk
-include basic/subdir.mk
-include antenna-stub/subdir.mk
-include adc/EFR32/subdir.mk
-include subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(ASM_UPPER_DEPS)),)
-include $(ASM_UPPER_DEPS)
endif
ifneq ($(strip $(MSA_UPPER_DEPS)),)
-include $(MSA_UPPER_DEPS)
endif
ifneq ($(strip $(ASM_DEPS)),)
-include $(ASM_DEPS)
endif
ifneq ($(strip $(S79_DEPS)),)
-include $(S79_DEPS)
endif
ifneq ($(strip $(S_DEPS)),)
-include $(S_DEPS)
endif
ifneq ($(strip $(S_UPPER_DEPS)),)
-include $(S_UPPER_DEPS)
endif
ifneq ($(strip $(MSA_DEPS)),)
-include $(MSA_DEPS)
endif
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
ifneq ($(strip $(S79_UPPER_DEPS)),)
-include $(S79_UPPER_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 

# All Target
all:
	$(MAKE) --no-print-directory pre-build
	$(MAKE) --no-print-directory main-build

# Main-build Target
main-build: DynamicMultiprotocolSwitchSoc.out

# Tool invocations
DynamicMultiprotocolSwitchSoc.out: $(OBJS) $(USER_OBJS)
	@echo 'Building target: $@'
	@echo 'Invoking: IAR Linker for ARM'
	@echo 'Adding linker inputs to ilinkCommandLine_DynamicMultiprotocolSwitchSoc.out.xcl'
	echo. $(foreach file,$(OBJS), $(file)) >> ilinkCommandLine_DynamicMultiprotocolSwitchSoc.out.xcl
	echo. $(foreach file,$(USER_OBJS), $(file)) >> ilinkCommandLine_DynamicMultiprotocolSwitchSoc.out.xcl
	@echo 'Invoking linker reading args from file: ilinkCommandLine_DynamicMultiprotocolSwitchSoc.out.xcl'
	ilinkarm -f "C:\Users\DELL\SimplicityStudio\v5_workspace\DynamicMultiprotocolSwitchSoc\IAR ARM - Default\ilinkCommandLine_DynamicMultiprotocolSwitchSoc.out.xcl" 
	ielftool --srec --verbose "DynamicMultiprotocolSwitchSoc.out" "DynamicMultiprotocolSwitchSoc.s37"  
	ielftool --ihex --verbose "DynamicMultiprotocolSwitchSoc.out" "DynamicMultiprotocolSwitchSoc.hex"  
	ielftool --bin --verbose "DynamicMultiprotocolSwitchSoc.out" "DynamicMultiprotocolSwitchSoc.bin"
	@echo 'Finished building target: $@'
	@echo ' '
	$(MAKE) --no-print-directory post-build

# Other Targets
clean:
	-$(RM) $(ASM_UPPER_DEPS)$(MSA_UPPER_DEPS)$(EXECUTABLES)$(OBJS)$(ASM_DEPS)$(S79_DEPS)$(S_DEPS)$(S_UPPER_DEPS)$(MSA_DEPS)$(C_DEPS)$(S79_UPPER_DEPS) DynamicMultiprotocolSwitchSoc.out
	-@echo ' '

pre-build:
	-cmd //c 'C:\Users\DELL\SIMPLI~1\V5_WOR~1\DYNAMI~2/DynamicMultiprotocolSwitchSoc-prebuild.bat' 'DynamicMultiprotocolSwitchSoc' 'C:/Users/DELL/SimplicityStudio/v5_workspace/DynamicMultiprotocolSwitchSoc' 'C:/Program Files (x86)/IAR Systems/Embedded Workbench 7.5/arm' 'C:\SiliconLabs\SimplicityStudio\v5'
	-@echo ' '

post-build:
	-cmd //c 'C:\Users\DELL\SIMPLI~1\V5_WOR~1\DYNAMI~2/DynamicMultiprotocolSwitchSoc-postbuild.bat' 'DynamicMultiprotocolSwitchSoc' 'C:/Users/DELL/SimplicityStudio/v5_workspace/DynamicMultiprotocolSwitchSoc' 'C:/Program Files (x86)/IAR Systems/Embedded Workbench 7.5/arm' 'C:\SiliconLabs\SimplicityStudio\v5'
	-@echo ' '

.PHONY: all clean dependents main-build pre-build post-build

-include ../makefile.targets
