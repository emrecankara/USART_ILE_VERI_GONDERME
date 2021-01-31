################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include Drivers/STM32F4xx_HAL_Driver/Src/subdir.mk
-include Core/Startup/subdir.mk
-include Core/Src/subdir.mk
-include subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 
EXECUTABLES += \
USART_ILE_VERI_GONDERME-02.elf \

SIZE_OUTPUT += \
default.size.stdout \

OBJDUMP_LIST += \
USART_ILE_VERI_GONDERME-02.list \

OBJCOPY_BIN += \
USART_ILE_VERI_GONDERME-02.bin \


# All Target
all: USART_ILE_VERI_GONDERME-02.elf secondary-outputs

# Tool invocations
USART_ILE_VERI_GONDERME-02.elf: $(OBJS) $(USER_OBJS) C:\Users\Emre\ Can\STM32CubeIDE\workspace_1.3.0\USART_ILE_VERI_GONDERME-02\STM32F407VGTX_FLASH.ld
	arm-none-eabi-gcc -o "USART_ILE_VERI_GONDERME-02.elf" @"objects.list" $(USER_OBJS) $(LIBS) -mcpu=cortex-m4 -T"C:\Users\Emre Can\STM32CubeIDE\workspace_1.3.0\USART_ILE_VERI_GONDERME-02\STM32F407VGTX_FLASH.ld" --specs=nosys.specs -Wl,-Map="USART_ILE_VERI_GONDERME-02.map" -Wl,--gc-sections -static --specs=nano.specs -mfpu=fpv4-sp-d16 -mfloat-abi=hard -mthumb -Wl,--start-group -lc -lm -Wl,--end-group
	@echo 'Finished building target: $@'
	@echo ' '

default.size.stdout: $(EXECUTABLES)
	arm-none-eabi-size  $(EXECUTABLES)
	@echo 'Finished building: $@'
	@echo ' '

USART_ILE_VERI_GONDERME-02.list: $(EXECUTABLES)
	arm-none-eabi-objdump -h -S $(EXECUTABLES) > "USART_ILE_VERI_GONDERME-02.list"
	@echo 'Finished building: $@'
	@echo ' '

USART_ILE_VERI_GONDERME-02.bin: $(EXECUTABLES)
	arm-none-eabi-objcopy  -O binary $(EXECUTABLES) "USART_ILE_VERI_GONDERME-02.bin"
	@echo 'Finished building: $@'
	@echo ' '

# Other Targets
clean:
	-$(RM) *
	-@echo ' '

secondary-outputs: $(SIZE_OUTPUT) $(OBJDUMP_LIST) $(OBJCOPY_BIN)

.PHONY: all clean dependents
.SECONDARY:

-include ../makefile.targets
