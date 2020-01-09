# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: rafrodri <rafrodri@student.42.fr>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2020/01/06 15:12:29 by rafrodri          #+#    #+#              #
#    Updated: 2020/01/09 16:47:03 by rafrodri         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

SRCS =		ft_isalnum.c ft_isalpha.c ft_tolower.c ft_strncmp.c\
			ft_isascii.c ft_isdigit.c ft_isprint.c ft_strlen.c ft_toupper.c

OBJS =		${SRCS:.c=.o}

NAME =		libft.a

CC =		gcc
RM =		rm -f

CFLAGS =	-Wall -Wextra -Werror

.c.o:
			${CC} ${CFLAGS} -c $< -o ${<:.c=.o}

${NAME}:	${OBJS}
			ar rc ${NAME} ${OBJS}

all:		${NAME}

clean:		
			${RM} ${OBJS}

fclean:		clean
			${RM} ${NAME}

re: 		fclean all

.PHONY: 	all clean fclean re