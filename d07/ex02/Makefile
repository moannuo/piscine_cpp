.PHONY: all clean fclean re

CC = clang++

FLAGS = -Wall -Wextra -Werror -std=c++98

NAME = array

SRC = Array.cpp

OBJ = $(SRC:.cpp=.o)

all: $(NAME)

$(NAME): $(OBJ)
	$(CC) $(FLAGS) -o $@ $^

%.o:%.cpp
	$(CC) $(FLAGS) -c -o $@ $<

clean:
	rm -rf $(OBJ)

fclean: clean
	rm -rf $(NAME)

re: fclean all
