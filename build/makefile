# Compiler and flags
CXX = g++
CXXFLAGS = -Wall -std=c++11

# Output binary
TARGET = ../bin/main

# Source files
SRC = ../src/main.cpp

# Object files
OBJ = $(SRC:.cpp=.o)

# Default target to build
all: $(TARGET)

$(TARGET): $(OBJ)
	$(CXX) $(OBJ) -o $(TARGET) $(LDFLAGS)

# Rule to create object files
../src/%.o: ../src/%.cpp
	$(CXX) $(CXXFLAGS) -c $< -o $@

# Clean up (platform-independent way)
clean:
	$(RM) $(OBJ) $(TARGET)
