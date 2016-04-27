#
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
