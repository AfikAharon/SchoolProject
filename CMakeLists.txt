cmake_minimum_required(VERSION 3.12)
project(secondProject)

set(CMAKE_CXX_STANDARD 14)

add_executable(secondProject main.cpp serverPackage/MyParralelServer.cpp serverPackage/Server.h serverPackage/MySerialServer.cpp serverPackage/MySerialServer.h clientPackage/ClientHandler.h clientPackage/MyTestClientHandler.cpp clientPackage/MyTestClientHandler.h solverPackage/Solver.h cachePackage/CacheManager.h cachePackage/FileCacheManager.cpp cachePackage/FileCacheManager.h solverPackage/StringReverser.cpp solverPackage/StringReverser.h searchPackage/BestFirstSearch searchPackage/State.h searchPackage/Searcher.h searchPackage/Searchable.h utils/Point.h test/MatrixDomain.h searchPackage/BFS.h searchPackage/DFS.h searchPackage/AStar.h utils/MyPriorQueue.h utils/SearchSolver.h clientPackage/MyClientHandler.h problemPackage/ProblemCreator.h problemPackage/MatrixProblem.h problemPackage/MatrixProblem.cpp searchPackage/SearchableMatrix.h serverPackage/MainBoot.h)

SET(CMAKE_CXX_FLAGS -pthread)