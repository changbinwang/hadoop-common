# Licensed to the Apache Software Foundation (ASF) under one
# or more contributor license agreements.  See the NOTICE file
# distributed with this work for additional information
# regarding copyright ownership.  The ASF licenses this file
# to you under the Apache License, Version 2.0 (the
# "License"); you may not use this file except in compliance
# with the License.  You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

AM_CFLAGS=-I$(srcdir)/impl -Wall -g -Werror

# Define the programs that need to be built
bin_PROGRAMS = container-executor
check_PROGRAMS = test-container-executor

TESTS = test-container-executor

# Define the sources for the common files
common_SOURCES = impl/configuration.c impl/container-executor.c

# Define the sources for the real executable
container_executor_SOURCES = $(common_SOURCES) impl/main.c

# Define the sources for the test executable
test_container_executor_SOURCES = $(common_SOURCES) test/test-container-executor.c
