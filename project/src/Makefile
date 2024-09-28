FLAGS = -Wall -Werror -Wextra
BUILD_DIR = ../build/

build_db: modules_db.c modules.c levels.c status_events.c shared.c
	gcc $(FLAGS) -c modules_db.c modules.c levels.c status_events.c shared.c
	gcc modules.o levels.o status_events.o shared.o modules_db.o -o $(BUILD_DIR)database 
	$(BUILD_DIR)database
clean:
	rm -f *.o
	rm -f ./database

all: database