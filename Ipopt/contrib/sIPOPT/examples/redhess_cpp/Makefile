# Copyright (C) 2010 Hans Pirnay
# All Rights Reserved.
# This file is distributed under the Eclipse Public License.


##########################################################################
#    You can modify this example makefile to fit for your own program.   #
#    Usually, you only need to change the five CHANGEME entries below.   #
##########################################################################

# CHANGEME: This should be the name of your executable
EXE = redhess_cpp

# CHANGEME: Here is the name of all object files corresponding to the source
#           code that you wrote in order to define the problem statement
OBJS =  redhess_cpp.o \
	MySensTNLP.o

# CHANGEME: Additional libraries
ADDLIBS =

# CHANGEME: Additional flags for compilation (e.g., include flags)
ADDINCFLAGS =

##########################################################################
#  Usually, you don't have to change anything below.  Note that if you   #
#  change certain compiler options, you might have to recompile Ipopt.   #
##########################################################################

# C++ Compiler command
CXX = g++

# C++ Compiler options
CXXFLAGS = -O3 -pipe -DNDEBUG -pedantic-errors -Wparentheses -Wreturn-type -Wcast-qual -Wall -Wpointer-arith -Wwrite-strings -Wconversion -Wno-unknown-pragmas -Wno-long-long   -DIPOPT_BUILD

# additional C++ Compiler options for linking
CXXLINKFLAGS =  -Wl,--rpath -Wl,/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib

SRCDIR = .
ipoptsrcdir  = $(SRCDIR)/../../../../src
senssrcdir = $(SRCDIR)/../../src

# Include directories (we use the CYGPATH_W variables to allow compilation with Windows compilers)
#   we also need some Ipopt headers that are not installed, so we add $(ipoptsrcdir)/Algorithm and $(ipoptsrcdir)/LinAlg
#INCL = `PKG_CONFIG_PATH=/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib64/pkgconfig:/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib/pkgconfig:/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/share/pkgconfig:  --cflags ipopt` -I`$(CYGPATH_W) $(ipoptsrcdir)/Algorithm` -I`$(CYGPATH_W) $(ipoptsrcdir)/LinAlg` -I`$(CYGPATH_W) $(senssrcdir)` $(ADDINCFLAGS)
INCL = -I`$(CYGPATH_W) /home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/include/coin`  -I/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/include/coin/ThirdParty  -I/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/include/coin/ThirdParty    -I/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/include/coin/ThirdParty        -I`$(CYGPATH_W) $(ipoptsrcdir)/Algorithm` -I`$(CYGPATH_W) $(ipoptsrcdir)/LinAlg` -I`$(CYGPATH_W) $(senssrcdir)` $(ADDINCFLAGS)

# Linker flags
#LIBS = -lsipopt `PKG_CONFIG_PATH=/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib64/pkgconfig:/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib/pkgconfig:/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/share/pkgconfig:  --libs ipopt`
#LIBS = -link -libpath:`$(CYGPATH_W) /home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib` libsipopt.lib libipopt.lib  -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinmumps -L/usr/lib/gcc/x86_64-linux-gnu/5 -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/5/../../.. -lgfortran -lm -lquadmath  -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinmetis  -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinblas -L/usr/lib/gcc/x86_64-linux-gnu/5 -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/5/../../.. -lgfortran -lm -lquadmath   -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinhsl -L/usr/lib/gcc/x86_64-linux-gnu/5 -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/5/../../.. -lgfortran -lm -lquadmath   -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinlapack -L/usr/lib/gcc/x86_64-linux-gnu/5 -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/5/../../.. -lgfortran -lm -lquadmath  -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinblas -L/usr/lib/gcc/x86_64-linux-gnu/5 -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/5/../../.. -lgfortran -lm -lquadmath   -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinblas -L/usr/lib/gcc/x86_64-linux-gnu/5 -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/5/../../.. -lgfortran -lm -lquadmath  -lm  -ldl
LIBS = -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lsipopt -lipopt  -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinmumps -L/usr/lib/gcc/x86_64-linux-gnu/5 -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/5/../../.. -lgfortran -lm -lquadmath  -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinmetis  -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinblas -L/usr/lib/gcc/x86_64-linux-gnu/5 -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/5/../../.. -lgfortran -lm -lquadmath   -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinhsl -L/usr/lib/gcc/x86_64-linux-gnu/5 -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/5/../../.. -lgfortran -lm -lquadmath   -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinlapack -L/usr/lib/gcc/x86_64-linux-gnu/5 -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/5/../../.. -lgfortran -lm -lquadmath  -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinblas -L/usr/lib/gcc/x86_64-linux-gnu/5 -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/5/../../.. -lgfortran -lm -lquadmath   -L/home/anoop/Work/Udacity/SelfDriving/ModelPredictiveController/Ipopt-3.12.1/lib -lcoinblas -L/usr/lib/gcc/x86_64-linux-gnu/5 -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/5/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/5/../../.. -lgfortran -lm -lquadmath  -lm  -ldl

# The following is necessary under cygwin, if native compilers are used
CYGPATH_W = echo

all: $(EXE)

.SUFFIXES: .cpp .c .o .obj

$(EXE): $(OBJS)
	bla=;\
	for file in $(OBJS); do bla="$$bla `$(CYGPATH_W) $$file`"; done; \
	$(CXX) $(CXXLINKFLAGS) $(CXXFLAGS) -o $@ $$bla $(ADDLIBS) $(LIBS)

clean:
	rm -rf $(EXE) $(OBJS)

.cpp.o:
	$(CXX) $(CXXFLAGS) $(INCL) -c -o $@ $<


.cpp.obj:
	$(CXX) $(CXXFLAGS) $(INCL) -c -o $@ `$(CYGPATH_W) '$<'`
