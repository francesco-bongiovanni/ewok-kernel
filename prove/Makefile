PROJ_FILES = ../../

-include $(PROJ_FILES)/Makefile.conf

all:
	gnatprove -P prove.gpr --RTS=$(CONFIG_ADA_RUNTIME)/arm-eabi/lib/gnat/zfp-stm32f4 --mode=all -U

check:
	gnatprove -P prove.gpr --RTS=$(CONFIG_ADA_RUNTIME)/arm-eabi/lib/gnat/zfp-stm32f4 --mode=check_all -U

flow:
	gnatprove -P prove.gpr --RTS=$(CONFIG_ADA_RUNTIME)/arm-eabi/lib/gnat/zfp-stm32f4 --mode=flow -U

prove:
	gnatprove -P prove.gpr --RTS=$(CONFIG_ADA_RUNTIME)/arm-eabi/lib/gnat/zfp-stm32f4 --mode=prove -U

test:
	gnatprove -P prove.gpr --RTS=$(CONFIG_ADA_RUNTIME)/arm-eabi/lib/gnat/zfp-stm32f4 --mode=all -u test.ads test.adb

clean:
	rm -rf $(PROJ_FILES)/kernel/prove/gnatprove/*.ali

distclean:
	rm -rf $(PROJ_FILES)/kernel/prove/gnatprove

