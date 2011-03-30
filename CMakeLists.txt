# Copyright (C) 2007-2011 LuaDist.
# Created by Peter Drahoš
# Redistribution and use of this file is allowed according to the terms of the MIT license.
# For details see the COPYRIGHT file distributed with LuaDist.
# Please note that the package source code is licensed under its own license.

PROJECT(cgilua NONE)
CMAKE_MINIMUM_REQUIRED(VERSION 2.6)
INCLUDE(dist.cmake)

# Install all files and documentation
INSTALL (FILES src/cgilua/cgilua.lua DESTINATION ${INSTALL_LMOD})
INSTALL (FILES
		src/cgilua/authentication.lua
		src/cgilua/cookies.lua
		src/cgilua/dispatcher.lua
		src/cgilua/loader.lua
		src/cgilua/lp.lua
		src/cgilua/mime.lua
		src/cgilua/post.lua
		src/cgilua/readuntil.lua
		src/cgilua/serialize.lua
		src/cgilua/session.lua
		src/cgilua/urlcode.lua
		DESTINATION ${INSTALL_LMOD}/cgilua )
INSTALL (FILES README DESTINATION ${INSTALL_DATA})
INSTALL(DIRECTORY doc/ DESTINATION ${INSTALL_DOC})
INSTALL(DIRECTORY tests/ DESTINATION ${INSTALL_TEST})
INSTALL(DIRECTORY examples/ DESTINATION ${INSTALL_EXAMPLE})
