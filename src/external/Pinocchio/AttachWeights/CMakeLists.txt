CMAKE_MINIMUM_REQUIRED(VERSION 2.8)

SET(ATTACHWEIGHTS_INCLUDE_DIR ${CMAKE_CURRENT_SOURCE_DIR} CACHE PATH "Path to attachweights headers")

INCLUDE_DIRECTORIES(
PINOCCHIO_INCLUDE_DIR
)

ADD_EXECUTABLE( attachweights
AttachWeights.cpp
stdafx.cpp
stdafx.h
)

TARGET_LINK_LIBRARIES( attachweights
pinocchio
)
