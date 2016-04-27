#
# Copyright (C) 2016, Dermot Tynan, Kalopa Research. <dtynan@kalopa.com>
#
# This program is free software: you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published
# by the Free Software Foundation, either version 3 of the License, or
# (at your option) any later version.
#
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
# General Public License for more details.
#
# You should have received a copy of the GNU General Public License
# along with this program in a file called LICENSE.  If not, see
# <http://www.gnu.org/licenses/>.
#
CFLAGS=`pkg-config --cflags gtk+-3.0 glib-2.0` -O -Wall
LDFLAGS=`pkg-config --libs gtk+-3.0 glib-2.0`
SRCS=	main.c object.c command.c channel.c grafix.c
OBJS=	$(SRCS:.c=.o)

all:	roboview

clean:
	rm -f roboview $(OBJS)

roboview: $(OBJS)
	$(CC) -o roboview $(OBJS) $(LDFLAGS)

$(OBJS): roboview.h
