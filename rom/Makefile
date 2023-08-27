TARGET = main.bin
SRC = main.asm
OBJ = main.p

all: $(TARGET)

$(TARGET): $(OBJ)
	p2bin -r \$$-\$$ $<

$(OBJ): $(SRC)
	asl -l $<

.PHONY: clean
clean:
	rm -f $(OBJ) $(TARGET)

.PHONY: program
program: $(TARGET)
	minipro -p W27C512@DIP28 -w main.bin -S
