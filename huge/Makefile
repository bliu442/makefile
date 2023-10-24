.PHONY:all clean

PROJECT_PWD = D:/ST/cygwin64/home/ccore/bliu/makefiles/huge

DIRS = $(PROJECT_PWD)/source/foo/src \
$(PROJECT_PWD)/source/bar/src \
$(PROJECT_PWD)/source/huge

RM = rm
RMFLAGS = -rf
RMS = $(PROJECT_PWD)/build/exes $(PROJECT_PWD)/build/libs

all:
	@set -e; \
	for dir in $(DIRS); \
	do \
		cd $$dir && $(MAKE); \
	done 
	@echo ""
	@echo ":=) Completed"
	@echo ""

clean:
	@set -e; \
	for dir in $(DIRS); \
	do \
		cd $$dir && $(MAKE) clean; \
	done; \
	$(RM) $(RMFLAGS) $(RMS)
	@echo ""
	@echo ":=) Completed"
	@echo ""

