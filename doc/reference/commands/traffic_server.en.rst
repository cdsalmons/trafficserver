.. Licensed to the Apache Software Foundation (ASF) under one
   or more contributor license agreements.  See the NOTICE file
  distributed with this work for additional information
  regarding copyright ownership.  The ASF licenses this file
  to you under the Apache License, Version 2.0 (the
  "License"); you may not use this file except in compliance
  with the License.  You may obtain a copy of the License at
 
   http://www.apache.org/licenses/LICENSE-2.0
 
  Unless required by applicable law or agreed to in writing,
  software distributed under the License is distributed on an
  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
  KIND, either express or implied.  See the License for the
  specific language governing permissions and limitations
  under the License.

.. _traffic-server:

==============
traffic_server
==============

.. program:: traffic_server

Description
===========

.. option:: -n COUNT, --net_threads COUNT

.. option:: -Z COUNT, --cluster_threads COUNT

.. option:: -U COUNT, --udp_threads COUNT

.. option:: -a, --accepts_thread

.. option:: -b, --accept_till_done

.. option:: -p PORT, --httpport PORT

.. option:: -P PORT, --cluster_port PORT

.. option:: -f, --disable_freelist

In order to improve performance, :program:`traffic_server` caches
commonly used data structures in a set of free object lists. This
option disables these caches, causing :program:`traffic_server` to
use :manpage:`malloc(3)` for every allocation. Though this option
should not commonly be needed, it may be beneficial in memory-constrained
environments or where the working set is highly variable.

.. option:: -o LEVEL, --dprintf_level LEVEL

.. option:: -R LEVEL, --regression LEVEL

.. option:: -r TEST, --regression_rest TEST

.. option:: -T TAGS, --debug_tags TAGS

.. option:: -B TAGS, --action_tags TAGS

.. option:: -i COUNT, --interval COUNT

.. option:: -M, --remote_management

.. option:: -C CMD, --command CMD

.. option:: -k, --clear_hostdb

.. option:: -K, --clear_cache

.. option:: -c CORE, --read_core CORE

.. option:: --accept_mss MSS

.. option:: -t MSECS, --poll_timeout MSECS

.. option:: -h, --help

   Print usage information and exit.

.. option:: -V, --version

   Print version information and exit.

Environment
===========

.. envvar:: PROXY_REMOTE_MGMT

.. envvar:: PROXY_AUTO_EXIT
