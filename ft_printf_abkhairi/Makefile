# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: abkhairi <marvin@42.fr>                    +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2023/02/15 09:59:55 by abkhairi          #+#    #+#              #
#    Updated: 2023/02/23 15:17:00 by abkhairi         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME = libftprintf.a

SOURCES = ft_dectohexptr.c ft_dectohex.c ft_dectohe.c ft_printf.c ft_putchar.c \
	ft_putnbr.c ft_putnbru.c ft_putstring.c

OBJECTS = $(SOURCES:.c=.o)

CC = cc

CFLAGS = -Wall -Wextra -Werror

all : $(NAME)

$(NAME) : $(OBJECTS)
	ar -rc $(NAME) $(OBJECTS)

%.o: %.c ft_printf.h
	$(CC) -c $(CFLAGS) $<

clean:
	rm -f $(OBJECTS)

fclean: clean
	rm -f $(NAME)

re: fclean all 
