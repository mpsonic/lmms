INCLUDE(BuildPlugin)
INCLUDE_DIRECTORIES(${FFTW3F_INCLUDE_DIRS})
LINK_DIRECTORIES(${FFTW3F_LIBRARY_DIRS})
LINK_LIBRARIES(${FFTW3F_LIBRARIES})
BUILD_PLUGIN(spectrumanalyzer SpectrumAnalyzer.cpp SpectrumAnalyzerControls.cpp SpectrumAnalyzerControlDialog.cpp SpectrumAnalyzer.h SpectrumAnalyzerControls.h SpectrumAnalyzerControlDialog.h MOCFILES SpectrumAnalyzerControls.h EMBEDDED_RESOURCES "${CMAKE_CURRENT_SOURCE_DIR}/*.png")
