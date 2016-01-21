# THIS DOES NOT WORK

# compiler
CC = g++

# flags
CFLAGS = -std=c++11

# name of file
TARGET = room-explorer

all: $(TARGET)

$(TARGET): main.o
	$(CC) $(CFLAGS) -o $(TARGET) main.o
    
# main
main.o: game.o player.o menutext.h
	$(CC) $(CFLAGS) -c

# game
game.o: locationdata.o coordlist.o

# locationdata
locationdata.o: locationdata.h locationdata.cpp tile.o

# tile
tile.o: tile.h tile.cpp location.o player.o node.o item.o key.o menutext.o linkedList.o

# location
location.o: location.h location.cpp linkedList.o 

# linkedList
linkedList.o: linkedList.h linkedList.cpp 
