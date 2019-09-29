# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: ysalihi <marvin@42.fr>                     +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2018/10/03 22:06:00 by ysalihi           #+#    #+#              #
#    Updated: 2018/10/03 22:06:22 by ysalihi          ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME = libft.a
SRC_C = srcs/*.c
INCLUDES_H = includes
FT_O = ft_putchar.o ft_putstr.o ft_strcmp.o ft_strlen.o ft_swap.o

.PHONY: clean fclean re all

all: $(NAME)

$(FT_O):
	gcc -Wall -Wextra -Werror -c $(SRC_C) -I $(INCLUDES_H)

$(NAME): $(FT_O)
	ar rc $(NAME) $(FT_O)
	ranlib $(NAME)

clean:
	/bin/rm -rf $(FT_O)

fclean: clean
	/bin/rm -rf $(NAME)
	
re: fclean all
