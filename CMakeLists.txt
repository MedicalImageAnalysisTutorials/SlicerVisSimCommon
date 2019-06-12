cmake_minimum_required(VERSION 3.5)

project(SlicerVisSimCommon)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "http://slicer.org/slicerWiki/index.php/Documentation/4.10/Extensions/SlicerVisSimCommon")
set(EXTENSION_CATEGORY "VisSimTools")
set(EXTENSION_CONTRIBUTORS "Ibraheem Al-Dhamari (VisSim, Uni-Koblenz)")
set(EXTENSION_DESCRIPTION "Common tools for VisSIm extensions")
set(EXTENSION_ICONURL "http://www.example.com/Slicer/Extensions/SlicerVisSimCommon.png")
set(EXTENSION_SCREENSHOTURLS "http://www.example.com/Slicer/Extensions/SlicerVisSimCommon/Screenshots/1.png")
set(EXTENSION_DEPENDS VisSimCommon) # Specified as a space separated string, a list or 'NA' if any

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(VisSimCommon)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_GENERATE_CONFIG})
include(${Slicer_EXTENSION_CPACK})
