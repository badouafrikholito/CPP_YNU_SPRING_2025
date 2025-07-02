 CC=g++
CFLAGS=-std=c++17 -Iinclude/
SRC_DIR=src/
OBJ_DIR=obj/
BIN_DIR=bin/
SRCS=$(wildcard $(SRC_DIR)*.cpp)
OBJS=$(patsubst $(SRC_DIR)%.cpp,$(OBJ_DIR)%.o,$(SRCS))
TARGET=$(BIN_DIR)USMS

all: $(TARGET)

$(TARGET): $(OBJS)
	@mkdir -p $(BIN_DIR)
	$(CC) $(OBJS) -o $@

$(OBJ_DIR)%.o: $(SRC_DIR)%.cpp
	@mkdir -p $(OBJ_DIR)
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	rm -rf $(OBJ_DIR) $(BIN_DIR)

.PHONY: all clean