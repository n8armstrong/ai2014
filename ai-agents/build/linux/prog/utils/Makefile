include ../../Makefile.top

LOCAL_PROG    := RunProg
LOCAL_PART    := utils
LOCAL_SRC_DIR := $(PROG_DIR)/$(LOCAL_PART)
LOCAL_INC_DIR := $(PROG_DIR)/$(LOCAL_PART)
LOCAL_AGENT_SELECT := 

LOCAL_SRC := 

LOCAL_HEADERS := 

CXX_HEADERS := \
        $(LOCAL_HEADERS)

CXX_SRC  := \
        $(LOCAL_SRC) 

TARGET_HEADERS    := ${CXX_HEADERS:%.h=$(LOCAL_INC_DIR)/%.h}
TARGET_OBJS       := ${CXX_SRC:%.cpp=$(OBJ_BASE)/%.o}
TARGET_LIB        := 
TARGET_PROG       := $(AI_BIN_DIR)/$(LOCAL_PROG)


include ../../Makefile.rules

$(AI_BIN_DIR)/RunProg: $(LOCAL_SRC_DIR)/RunProg
	sed 's?MY_LIB_PATH?'$(AI_LIB_DIR)'?' $^ > $@
	chmod +x $@

include ../../Makefile.dep
