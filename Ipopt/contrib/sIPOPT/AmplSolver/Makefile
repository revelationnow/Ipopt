# Copyright (C) 2009, 2010 Hans Pirnay. 
# All Rights Reserved.
# This code is published under the Eclipse Public License.
#
# Author: Hans Pirnay, 2009-12-15


#############################################################################
# Do not modify anything below unless you know what you're doing.
prefix      = /home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1
exec_prefix = ${prefix}
libdir      = ${exec_prefix}/lib
bindir      = ${exec_prefix}/bin
CYGPATH_W   = echo
SRCDIR      = .
ipoptsrcdir  = $(SRCDIR)/../../../src
senssrcdir = $(SRCDIR)/../src

CXX         = g++
CXXFLAGS    = -O3 -pipe -DNDEBUG -pedantic-errors -Wparentheses -Wreturn-type -Wcast-qual -Wall -Wpointer-arith -Wwrite-strings -Wconversion -Wno-unknown-pragmas -Wno-long-long   -DIPOPT_BUILD
LDFLAGS     = $(CXXFLAGS)  -Wl,--rpath -Wl,/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib

# Include directories (we use the CYGPATH_W variables to allow compilation with Windows compilers)
#   we also need some Ipopt headers that are not installed, so we add $(ipoptsrcdir)/Algorithm and $(ipoptsrcdir)/LinAlg
#INCL = `PKG_CONFIG_PATH=/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib64/pkgconfig:/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib/pkgconfig:/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/share/pkgconfig:  --cflags ipoptamplinterface` -I`$(CYGPATH_W) $(ipoptsrcdir)/Algorithm` -I`$(CYGPATH_W) $(ipoptsrcdir)/LinAlg` -I`$(CYGPATH_W) $(senssrcdir)` $(ADDINCFLAGS)
INCL = -I`$(CYGPATH_W) /home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/include/coin`  -I/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/include/coin/ThirdParty  -I/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/include/coin/ThirdParty    -I/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/include/coin/ThirdParty         -I/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/include/coin/ThirdParty  -I`$(CYGPATH_W) $(ipoptsrcdir)/Algorithm` -I`$(CYGPATH_W) $(ipoptsrcdir)/LinAlg` -I`$(CYGPATH_W) $(senssrcdir)` $(ADDINCFLAGS)

# Linker flags
#LIBS = -lsipopt `PKG_CONFIG_PATH=/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib64/pkgconfig:/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib/pkgconfig:/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/share/pkgconfig:  --libs ipoptamplinterface`
#LIBS = -link -libpath:`$(CYGPATH_W) /home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib` libsipopt.lib libipoptamplinterface.lib libipopt.lib  -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinmumps -L/usr/lib/gcc/x86_64-linux-gnu/5 -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/5/../../.. -lgfortran -lm -lquadmath  -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinmetis  -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinblas -L/usr/lib/gcc/x86_64-linux-gnu/5 -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/5/../../.. -lgfortran -lm -lquadmath   -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinhsl -L/usr/lib/gcc/x86_64-linux-gnu/5 -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/5/../../.. -lgfortran -lm -lquadmath   -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinlapack -L/usr/lib/gcc/x86_64-linux-gnu/5 -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/5/../../.. -lgfortran -lm -lquadmath  -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinblas -L/usr/lib/gcc/x86_64-linux-gnu/5 -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/5/../../.. -lgfortran -lm -lquadmath   -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinblas -L/usr/lib/gcc/x86_64-linux-gnu/5 -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/5/../../.. -lgfortran -lm -lquadmath  -lm  -ldl  -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinasl -lm -ldl  
LIBS = -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lsipopt -lipoptamplinterface -lipopt  -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinmumps -L/usr/lib/gcc/x86_64-linux-gnu/5 -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/5/../../.. -lgfortran -lm -lquadmath  -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinmetis  -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinblas -L/usr/lib/gcc/x86_64-linux-gnu/5 -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/5/../../.. -lgfortran -lm -lquadmath   -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinhsl -L/usr/lib/gcc/x86_64-linux-gnu/5 -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/5/../../.. -lgfortran -lm -lquadmath   -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinlapack -L/usr/lib/gcc/x86_64-linux-gnu/5 -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/5/../../.. -lgfortran -lm -lquadmath  -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinblas -L/usr/lib/gcc/x86_64-linux-gnu/5 -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/5/../../.. -lgfortran -lm -lquadmath   -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinblas -L/usr/lib/gcc/x86_64-linux-gnu/5 -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/5/../../.. -lgfortran -lm -lquadmath  -lm  -ldl  -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinasl -lm -ldl  

#LIBTOOL = $(SHELL) $(top_builddir)/../libtool
#CXXLD = $(CXX)
#CXXLINK = $(LIBTOOL) --tag=CXX --mode=link $(CXXLD) $(AM_CXXFLAGS) \
#	$(CXXFLAGS) $(AM_LDFLAGS) $(LDFLAGS) -o $@

sIPOPT_LIB = libsipopt.so

sIPOPT_LIBNAME =$(sIPOPT_LIB).0.0.0

TARGET = ipopt_sens

OBJS   = SensAmplTNLP.o 

VPATH = $(SRCDIR):$(ipoptsrcdir)/Apps/AmplSolver

all: $(OBJS)

install: $(TARGET)
	if test -d $(bindir); then : ; else mkdir $(bindir); fi
	cp $(TARGET) $(bindir)

uninstall:
	rm -f $(bindir)/$(TARGET)

$(TARGET): $(OBJS) ampl_sipopt.cpp
	$(CXX) $(LDFLAGS) $(SRCDIR)/ampl_sipopt.cpp -o $(TARGET) $(OBJS) $(INCL) $(LIBS)

%.o: %.cpp 
	$(CXX) $(CXXFLAGS) $(INCL) -o $@ -c $^

clean:
	rm -f $(OBJS) $(TARGET)

distclean: clean
