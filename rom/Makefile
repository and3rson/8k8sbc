TARGET = main.bin
SRC = main.asm
OBJ = main.p

all: $(TARGET)

$(TARGET): $(OBJ)
	p2bin -r \$$-\$$ $<

$(OBJ): $(SRC)
	asl -l $<

clean:
	rm -f $(OBJ) $(TARGET)
