UNIT_TESTS = common_stringutil
check_PROGRAMS = common_stringutil
common_stringutil_SOURCES = Common/StringUtilTest.cpp
common_stringutil_CPPFLAGS = -I$(top_srcdir)
common_stringutil_LDADD = $(GTEST_LIBS)

UNIT_TESTS += common_histogram
check_PROGRAMS += common_histogram
common_histogram_SOURCES = Common/HistogramTest.cpp
common_histogram_CPPFLAGS = -I$(top_srcdir)
common_histogram_LDADD = $(GTEST_LIBS)

UNIT_TESTS += common_bitutil
check_PROGRAMS += common_bitutil
common_bitutil_SOURCES = Common/BitUtilTest.cpp
common_bitutil_CPPFLAGS = -I$(top_srcdir)
common_bitutil_LDADD = $(GTEST_LIBS)

UNIT_TESTS += common_kmer
check_PROGRAMS += common_kmer
common_kmer_SOURCES = Common/KmerTest.cpp
common_kmer_CPPFLAGS = -I$(top_srcdir)
common_kmer_LDADD = $(top_builddir)/Common/libcommon.a $(GTEST_LIBS)

UNIT_TESTS += common_sequence
check_PROGRAMS += common_sequence
common_sequence_SOURCES = Common/Sequence.cc
common_sequence_CPPFLAGS = -I$(top_srcdir)
common_sequence_LDADD = $(top_builddir)/Common/libcommon.a $(GTEST_LIBS)

UNIT_TESTS += common_KmerIterator
check_PROGRAMS += common_KmerIterator
common_KmerIterator_SOURCES = Common/KmerIteratorTest.cpp
common_KmerIterator_CPPFLAGS = -I$(top_srcdir)
common_KmerIterator_LDADD = $(top_builddir)/Common/libcommon.a $(GTEST_LIBS)

UNIT_TESTS += common_sam
check_PROGRAMS += common_sam
common_sam_SOURCES = Common/SAM.cc
common_sam_CPPFLAGS = -I$(top_srcdir)
common_sam_LDADD = $(top_builddir)/Common/libcommon.a $(GTEST_LIBS)

UNIT_TESTS += BloomFilter
check_PROGRAMS += BloomFilter
BloomFilter_SOURCES = Konnector/BloomFilter.cc
BloomFilter_CPPFLAGS = -I$(top_srcdir) -I$(top_srcdir)/Common
BloomFilter_CXXFLAGS = $(AM_CXXFLAGS) $(OPENMP_CXXFLAGS)
BloomFilter_LDADD = $(top_builddir)/Common/libcommon.a $(GTEST_LIBS)

UNIT_TESTS += Konnector_DBGBloom
check_PROGRAMS += Konnector_DBGBloom
Konnector_DBGBloom_SOURCES = Konnector/DBGBloomTest.cpp
Konnector_DBGBloom_CPPFLAGS = -I$(top_srcdir) -I$(top_srcdir)/Common
Konnector_DBGBloom_CXXFLAGS = $(AM_CXXFLAGS) $(OPENMP_CXXFLAGS)
Konnector_DBGBloom_LDADD = $(top_builddir)/Common/libcommon.a $(GTEST_LIBS)

UNIT_TESTS += Konnector_DBGBloomAlgorithms
check_PROGRAMS += Konnector_DBGBloomAlgorithms
Konnector_DBGBloomAlgorithms_SOURCES = Konnector/DBGBloomAlgorithmsTest.cpp
Konnector_DBGBloomAlgorithms_CPPFLAGS = -I$(top_srcdir) -I$(top_srcdir)/Common
Konnector_DBGBloomAlgorithms_CXXFLAGS = $(AM_CXXFLAGS) $(OPENMP_CXXFLAGS)
Konnector_DBGBloomAlgorithms_LDADD = \
	$(top_builddir)/Common/libcommon.a \
	$(GTEST_LIBS)

UNIT_TESTS += graph_ConstrainedBFSVisitor
check_PROGRAMS += graph_ConstrainedBFSVisitor
graph_ConstrainedBFSVisitor_SOURCES = Graph/ConstrainedBFSVisitorTest.cpp
graph_ConstrainedBFSVisitor_CPPFLAGS = -I$(top_srcdir) -I$(top_srcdir)/Common
graph_ConstrainedBFSVisitor_LDADD = $(top_builddir)/Common/libcommon.a $(GTEST_LIBS)

UNIT_TESTS += graph_BidirectionalBFS
check_PROGRAMS += graph_BidirectionalBFS
graph_BidirectionalBFS_SOURCES = Graph/BidirectionalBFSTest.cpp
graph_BidirectionalBFS_CPPFLAGS = -I$(top_srcdir) -I$(top_srcdir)/Common
graph_BidirectionalBFS_LDADD = $(top_builddir)/Common/libcommon.a $(GTEST_LIBS)

UNIT_TESTS += graph_AllPathsSearch
check_PROGRAMS += graph_AllPathsSearch
graph_AllPathsSearch_SOURCES = Graph/AllPathsSearchTest.cpp
graph_AllPathsSearch_CPPFLAGS = -I$(top_srcdir) -I$(top_srcdir)/Common
graph_AllPathsSearch_LDADD = $(top_builddir)/Common/libcommon.a $(GTEST_LIBS)

UNIT_TESTS += graph_HashGraph
check_PROGRAMS += graph_HashGraph
graph_HashGraph_SOURCES = Graph/HashGraphTest.cpp
graph_HashGraph_CPPFLAGS = -I$(top_srcdir) -I$(top_srcdir)/Common
graph_HashGraph_LDADD = $(top_builddir)/Common/libcommon.a $(GTEST_LIBS)

UNIT_TESTS += graph_ConstrainedBidiBFSVisitor
check_PROGRAMS += graph_ConstrainedBidiBFSVisitor
graph_ConstrainedBidiBFSVisitor_SOURCES = \
	Graph/ConstrainedBidiBFSVisitorTest.cpp
graph_ConstrainedBidiBFSVisitor_CPPFLAGS = -I$(top_srcdir) -I$(top_srcdir)/Common
graph_ConstrainedBidiBFSVisitor_LDADD = $(top_builddir)/Common/libcommon.a $(GTEST_LIBS)

UNIT_TESTS += Konnector_konnector
check_PROGRAMS += Konnector_konnector
Konnector_konnector_SOURCES = \
	Konnector/konnectorTest.cpp
Konnector_konnector_CPPFLAGS = -I$(top_srcdir) -I$(top_srcdir)/Common
Konnector_konnector_CXXFLAGS = $(AM_CXXFLAGS) $(OPENMP_CXXFLAGS)
Konnector_konnector_LDADD = \
	$(top_builddir)/Align/libalign.a \
	$(top_builddir)/Common/libcommon.a $(GTEST_LIBS)

##Tests for log kmer counting / Counting bloom filter

TESTS = $(UNIT_TESTS)
