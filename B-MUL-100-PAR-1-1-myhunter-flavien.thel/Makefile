##
## EPITECH PROJECT, 2020
## makefile
## File description:
## makefile
##

NAME	=	my_hunter

CC	=	gcc

RM	=	rm -f

SOURCE	=	./src/

CSFML   =       -lcsfml-graphics -lcsfml-window -lcsfml-system -lcsfml-audio

CREATE	=	./src/create/

SRC	=	$(CREATE)clock.c		\
		$(CREATE)clock_2.c		\
		$(CREATE)clock_fifth.c		\
		$(CREATE)sprite_fifth.c		\
		$(CREATE)sprite_first.c		\
		$(CREATE)sprite_fourth.c	\
		$(CREATE)sprite_second.c	\
		$(CREATE)sprite_third.c		\
		main.c			\
		destroy.c		\
		display_window.c 	\
		init_menu.c		\
		menu.c			\
		menu_event.c		\
		display.c		\
		first.c			\
		init.c			\
		move_first.c		\
		target_gestion.c	\
		text_gestion.c		\
		life.c			\
		game_over.c		\
		redirection.c 		\
		move_second.c		\
		second.c		\
		rand_float.c		\
		text_level.c		\
		move_third.c		\
		third.c			\
		fourth.c		\
		move_fourth.c		\
		destroy_fifth.c		\
		display_fifth.c		\
		fifth.c			\
		move_fifth.c		\
		win.c			\
		text_win.c 

OBJ	=	$(SRC:.c=.o)

LDFlAGS	=	-L ./lib/ -lmy

CPPFLAGS	=	-I ./include/

CFLAGS	=	-Wall -Wextra

all: $(NAME)

$(NAME):	$(OBJ)
	make -C lib/my
	$(CC) $(CFLAGS) -o $(NAME) $(SRC) $(CPPFLAGS) $(LDFlAGS) $(CSFML) -g
	$(RM) -f *.gcda *.gcno

clean:
	make clean -C lib/my
	$(RM) $(NAME)
	$(RM) $(OBJ) *~ \#*\#

fclean: clean
	make fclean -C lib/my

re: fclean all

.PHONY:	all fclean re
