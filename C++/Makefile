MAIN=test.cpp
COMPILER=g++
APP=main.exe
MINIWIN_H=miniwin.hpp
MINIWIN_LIB=miniwin.o
MINIWIN_SRC=miniwin.cpp
WIN_FLAGS=-mwindows
run: $(APP)
	./$(APP)

$(APP): $(MAIN) $(MINIWIN_H) $(MINIWIN_LIB)
	$(COMPILER) -o $(APP) $(MINIWIN_LIB) $(MAIN) $(WIN_FLAGS)

$(MINIWIN_LIB): $(MINIWIN_H) $(MINIWIN_SRC)
	$(COMPILER) -c $(MINIWIN_SRC) -o $(MINIWIN_LIB)

clean: 
	del $(APP) $(MINIWIN_LIB)