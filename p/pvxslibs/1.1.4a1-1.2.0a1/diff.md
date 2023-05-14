# Comparing `tmp/pvxslibs-1.1.4a1.tar.gz` & `tmp/pvxslibs-1.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvxslibs-1.1.4a1.tar", last modified: Mon Apr  3 14:37:29 2023, max compression
+gzip compressed data, was "pvxslibs-1.2.0a1.tar", last modified: Sun May 14 15:50:35 2023, max compression
```

## Comparing `pvxslibs-1.1.4a1.tar` & `pvxslibs-1.2.0a1.tar`

### file list

```diff
@@ -1,202 +1,264 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:37:29.885774 pvxslibs-1.1.4a1/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-03 14:37:29.885774 pvxslibs-1.1.4a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:37:29.837772 pvxslibs-1.1.4a1/bundle/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:37:29.857773 pvxslibs-1.1.4a1/bundle/libevent/
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/arc4random.c
--rw-r--r--   0 runner    (1001) docker     (123)    82779 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/buffer.c
--rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/buffer_iocp.c
--rw-r--r--   0 runner    (1001) docker     (123)    19640 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/bufferevent-internal.h
--rw-r--r--   0 runner    (1001) docker     (123)    27396 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/bufferevent.c
--rw-r--r--   0 runner    (1001) docker     (123)    18675 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/bufferevent_async.c
--rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/bufferevent_filter.c
--rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/bufferevent_mbedtls.c
--rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/bufferevent_openssl.c
--rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/bufferevent_pair.c
--rw-r--r--   0 runner    (1001) docker     (123)    30253 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/bufferevent_ratelim.c
--rw-r--r--   0 runner    (1001) docker     (123)    18434 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/bufferevent_sock.c
--rw-r--r--   0 runner    (1001) docker     (123)    30751 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/bufferevent_ssl.c
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/changelist-internal.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:37:29.857773 pvxslibs-1.1.4a1/bundle/libevent/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/cmake/VersionViaGit.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:37:29.837772 pvxslibs-1.1.4a1/bundle/libevent/compat/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:37:29.857773 pvxslibs-1.1.4a1/bundle/libevent/compat/sys/
--rw-r--r--   0 runner    (1001) docker     (123)    16674 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/compat/sys/queue.h
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/defer-internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/devpoll.c
--rw-r--r--   0 runner    (1001) docker     (123)    15972 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/epoll.c
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/epoll_sub.c
--rw-r--r--   0 runner    (1001) docker     (123)    41360 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/epolltable-internal.h
--rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/evbuffer-internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/evconfig-private.h.cmake
--rw-r--r--   0 runner    (1001) docker     (123)   159252 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/evdns.c
--rw-r--r--   0 runner    (1001) docker     (123)    16969 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/event-config.h.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    18994 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/event-internal.h
--rw-r--r--   0 runner    (1001) docker     (123)   105353 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/event.c
--rw-r--r--   0 runner    (1001) docker     (123)     7706 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/event_iocp.c
--rw-r--r--   0 runner    (1001) docker     (123)    14730 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/event_tagging.c
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/evmap-internal.h
--rw-r--r--   0 runner    (1001) docker     (123)    29011 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/evmap.c
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/evport.c
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/evrpc-internal.h
--rw-r--r--   0 runner    (1001) docker     (123)    29379 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/evrpc.c
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/evsignal-internal.h
--rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/evthread-internal.h
--rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/evthread.c
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/evthread_pthread.c
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/evthread_win32.c
--rw-r--r--   0 runner    (1001) docker     (123)    77363 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/evutil.c
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/evutil_rand.c
--rw-r--r--   0 runner    (1001) docker     (123)    18286 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/evutil_time.c
--rw-r--r--   0 runner    (1001) docker     (123)    29185 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/ht-internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/http-internal.h
--rw-r--r--   0 runner    (1001) docker     (123)   134861 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/http.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:37:29.857773 pvxslibs-1.1.4a1/bundle/libevent/include/
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/evdns.h
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:37:29.865773 pvxslibs-1.1.4a1/bundle/libevent/include/event2/
--rw-r--r--   0 runner    (1001) docker     (123)    39726 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event2/buffer.h
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event2/buffer_compat.h
--rw-r--r--   0 runner    (1001) docker     (123)    36204 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event2/bufferevent.h
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event2/bufferevent_compat.h
--rw-r--r--   0 runner    (1001) docker     (123)     9416 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event2/bufferevent_ssl.h
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event2/bufferevent_struct.h
--rw-r--r--   0 runner    (1001) docker     (123)    29722 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event2/dns.h
--rw-r--r--   0 runner    (1001) docker     (123)    12595 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event2/dns_compat.h
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event2/dns_struct.h
--rw-r--r--   0 runner    (1001) docker     (123)    63084 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event2/event.h
--rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event2/event_compat.h
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event2/event_struct.h
--rw-r--r--   0 runner    (1001) docker     (123)    50138 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event2/http.h
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event2/http_compat.h
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event2/http_struct.h
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event2/keyvalq_struct.h
--rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event2/listener.h
--rw-r--r--   0 runner    (1001) docker     (123)    21775 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event2/rpc.h
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event2/rpc_compat.h
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event2/rpc_struct.h
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event2/tag.h
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event2/tag_compat.h
--rw-r--r--   0 runner    (1001) docker     (123)    10457 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event2/thread.h
--rw-r--r--   0 runner    (1001) docker     (123)    29427 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event2/util.h
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event2/visibility.h
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/event2/watch.h
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/evhttp.h
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/evrpc.h
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/include/evutil.h
--rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/iocp-internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/ipv6-internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/kqueue-internal.h
--rw-r--r--   0 runner    (1001) docker     (123)    15128 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/kqueue.c
--rw-r--r--   0 runner    (1001) docker     (123)    22077 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/listener.c
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/log-internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/log.c
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/mbedtls-compat.h
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/minheap-internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/mm-internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/openssl-compat.h
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/poll.c
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/ratelim-internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/select.c
--rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/signal.c
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/ssl-compat.h
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/strlcpy-internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/strlcpy.c
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/time-internal.h
--rw-r--r--   0 runner    (1001) docker     (123)    17817 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/util-internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/watch.c
--rw-r--r--   0 runner    (1001) docker     (123)    68318 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/wepoll.c
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/wepoll.h
--rw-r--r--   0 runner    (1001) docker     (123)    10626 2023-04-03 14:36:43.000000 pvxslibs-1.1.4a1/bundle/libevent/win32select.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:37:29.865773 pvxslibs-1.1.4a1/configure/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/configure/CONFIG_PVXS_VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:37:29.841772 pvxslibs-1.1.4a1/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:37:29.865773 pvxslibs-1.1.4a1/python/pvxslibs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/python/pvxslibs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:37:29.865773 pvxslibs-1.1.4a1/python/pvxslibs/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/python/pvxslibs/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/python/pvxslibs/path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:37:29.865773 pvxslibs-1.1.4a1/python/pvxslibs/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/python/pvxslibs/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/python/pvxslibs/test/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/python/pvxslibs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:37:29.865773 pvxslibs-1.1.4a1/python/pvxslibs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-03 14:37:29.000000 pvxslibs-1.1.4a1/python/pvxslibs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-03 14:37:29.000000 pvxslibs-1.1.4a1/python/pvxslibs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 14:37:29.000000 pvxslibs-1.1.4a1/python/pvxslibs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 14:37:29.000000 pvxslibs-1.1.4a1/python/pvxslibs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-03 14:37:29.000000 pvxslibs-1.1.4a1/python/pvxslibs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-03 14:37:29.000000 pvxslibs-1.1.4a1/python/pvxslibs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 14:37:29.885774 pvxslibs-1.1.4a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)    23933 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:37:29.877774 pvxslibs-1.1.4a1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/bitmask.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/bitmask.h
--rw-r--r--   0 runner    (1001) docker     (123)    37692 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/client.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14171 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/clientconn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/clientdiscover.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19960 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/clientget.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9858 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/clientimpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/clientintrospect.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    28183 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/clientmon.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/clientreq.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/config.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11010 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/conn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/conn.h
--rw-r--r--   0 runner    (1001) docker     (123)    36781 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/data.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    22826 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/dataencode.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/datafmt.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/dataimpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/describe.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/describe.h@
--rw-r--r--   0 runner    (1001) docker     (123)    29603 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/evhelper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9068 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/evhelper.h
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/instcounters.h
--rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/log.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/nt.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:37:29.841772 pvxslibs-1.1.4a1/src/os/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:37:29.877774 pvxslibs-1.1.4a1/src/os/WIN32/
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/os/WIN32/osdSockExt.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:37:29.881774 pvxslibs-1.1.4a1/src/os/default/
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/os/default/osdSockExt.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/osgroups.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/osiSockExt.h
--rw-r--r--   0 runner    (1001) docker     (123)    15947 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/pvaproto.h
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/pvrequest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/pvrequest.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:37:29.881774 pvxslibs-1.1.4a1/src/pvxs/
--rw-r--r--   0 runner    (1001) docker     (123)    36668 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/pvxs/client.h
--rw-r--r--   0 runner    (1001) docker     (123)    28570 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/pvxs/data.h
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/pvxs/log.h
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/pvxs/netcommon.h
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/pvxs/nt.h
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/pvxs/server.h
--rw-r--r--   0 runner    (1001) docker     (123)    23748 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/pvxs/sharedArray.h
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/pvxs/sharedpv.h
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/pvxs/source.h
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/pvxs/srvcommon.h
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/pvxs/unittest.h
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/pvxs/util.h
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/pvxs/version.h
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/pvxs/versionNum.h@
--rw-r--r--   0 runner    (1001) docker     (123)    22858 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/server.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11718 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/serverchan.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14231 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/serverconn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/serverconn.h
--rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/serverget.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/serverintrospect.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18115 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/servermon.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/serversource.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    20228 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/sharedarray.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16312 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/sharedpv.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13742 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/type.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/udp_collector.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/udp_collector.h
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/unittest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21784 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/util.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-04-03 14:36:40.000000 pvxslibs-1.1.4a1/src/utilpvt.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:50:35.618606 pvxslibs-1.2.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-14 15:50:35.618606 pvxslibs-1.2.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:50:35.594605 pvxslibs-1.2.0a1/bundle/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:50:35.602605 pvxslibs-1.2.0a1/bundle/libevent/
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/arc4random.c
+-rw-r--r--   0 runner    (1001) docker     (123)    83114 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/buffer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/buffer_iocp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19626 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/bufferevent-internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27436 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/bufferevent.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18675 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/bufferevent_async.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/bufferevent_filter.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/bufferevent_mbedtls.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13519 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/bufferevent_openssl.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/bufferevent_pair.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30252 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/bufferevent_ratelim.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18434 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/bufferevent_sock.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30783 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/bufferevent_ssl.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/changelist-internal.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:50:35.602605 pvxslibs-1.2.0a1/bundle/libevent/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/cmake/VersionViaGit.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:50:35.594605 pvxslibs-1.2.0a1/bundle/libevent/compat/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:50:35.602605 pvxslibs-1.2.0a1/bundle/libevent/compat/sys/
+-rw-r--r--   0 runner    (1001) docker     (123)    16674 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/compat/sys/queue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/defer-internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/devpoll.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16650 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/epoll.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/epoll_sub.c
+-rw-r--r--   0 runner    (1001) docker     (123)    41360 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/epolltable-internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/evbuffer-internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/evconfig-private.h.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)   159597 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/evdns.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17249 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/event-config.h.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    18994 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/event-internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)   106153 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/event.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7706 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/event_iocp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14730 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/event_tagging.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/evmap-internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29039 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/evmap.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/evport.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/evrpc-internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29379 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/evrpc.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/evsignal-internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/evthread-internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/evthread.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/evthread_pthread.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/evthread_win32.c
+-rw-r--r--   0 runner    (1001) docker     (123)    78492 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/evutil.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/evutil_rand.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18286 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/evutil_time.c
+-rw-r--r--   0 runner    (1001) docker     (123)    29185 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/ht-internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/http-internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)   139062 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/http.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:50:35.602605 pvxslibs-1.2.0a1/bundle/libevent/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/evdns.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:50:35.606606 pvxslibs-1.2.0a1/bundle/libevent/include/event2/
+-rw-r--r--   0 runner    (1001) docker     (123)    39726 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/buffer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/buffer_compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36204 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/bufferevent.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/bufferevent_compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9822 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/bufferevent_ssl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/bufferevent_struct.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30066 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/dns.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12595 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/dns_compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/dns_struct.h
+-rw-r--r--   0 runner    (1001) docker     (123)    63771 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/event.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/event_compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/event_struct.h
+-rw-r--r--   0 runner    (1001) docker     (123)    52659 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/http.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/http_compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/http_struct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/keyvalq_struct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/listener.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21775 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/rpc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/rpc_compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/rpc_struct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/tag.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/tag_compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10457 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/thread.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29427 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/visibility.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/watch.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/event2/ws.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/evhttp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/evrpc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/include/evutil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/iocp-internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/ipv6-internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/kqueue-internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15128 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/kqueue.c
+-rw-r--r--   0 runner    (1001) docker     (123)    22132 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/listener.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/log-internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/log.c
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/mbedtls-compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/minheap-internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/mm-internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/openssl-compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/poll.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/ratelim-internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/select.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/sha1.c
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/sha1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/signal.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/signalfd.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/ssl-compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/strlcpy-internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/strlcpy.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/time-internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/util-internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/watch.c
+-rw-r--r--   0 runner    (1001) docker     (123)    68318 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/wepoll.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/wepoll.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10626 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/win32select.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-05-14 15:50:06.000000 pvxslibs-1.2.0a1/bundle/libevent/ws.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:50:35.606606 pvxslibs-1.2.0a1/configure/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/configure/CONFIG_PVXS_VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:50:35.610606 pvxslibs-1.2.0a1/ioc/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/channel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/channel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/credentials.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/credentials.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/dbentry.h
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/dberrormessage.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/dberrormessage.h
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/dbeventcontextdeleter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/dblocker.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/dbmanylocker.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/demo.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/dummygroup.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/dummysingle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/field.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/field.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/fieldconfig.h
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/fielddefinition.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/fielddefinition.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/fieldname.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/fieldname.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/fieldnamecomponent.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/fieldsubscriptionctx.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/fieldsubscriptionctx.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/group.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/group.h
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/groupconfig.h
+-rw-r--r--   0 runner    (1001) docker     (123)    46068 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/groupconfigprocessor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/groupconfigprocessor.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/groupdefinition.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/groupprocessorcontext.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/groupprocessorcontext.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23270 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/groupsource.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/groupsource.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/groupsourcehooks.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/groupsrcsubscriptionctx.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/iochooks.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/iocshargument.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/iocshcommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/iocshindex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23388 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/iocsource.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/iocsource.h
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/localfieldlog.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/localfieldlog.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:50:35.610606 pvxslibs-1.2.0a1/ioc/pvxs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/pvxs/iochooks.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/securityclient.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/securityclient.h
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/securitylogger.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18417 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/singlesource.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/singlesource.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/singlesourcehooks.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/singlesrcsubscriptionctx.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/singlesrcsubscriptionctx.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/subscriptionctx.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/typeutils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/typeutils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/ioc/yajlcallbackhandler.h
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:50:35.594605 pvxslibs-1.2.0a1/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:50:35.610606 pvxslibs-1.2.0a1/python/pvxslibs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/python/pvxslibs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:50:35.610606 pvxslibs-1.2.0a1/python/pvxslibs/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/python/pvxslibs/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/python/pvxslibs/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:50:35.610606 pvxslibs-1.2.0a1/python/pvxslibs/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/python/pvxslibs/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/python/pvxslibs/test/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/python/pvxslibs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:50:35.610606 pvxslibs-1.2.0a1/python/pvxslibs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-14 15:50:35.000000 pvxslibs-1.2.0a1/python/pvxslibs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-05-14 15:50:35.000000 pvxslibs-1.2.0a1/python/pvxslibs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 15:50:35.000000 pvxslibs-1.2.0a1/python/pvxslibs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 15:50:35.000000 pvxslibs-1.2.0a1/python/pvxslibs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-14 15:50:35.000000 pvxslibs-1.2.0a1/python/pvxslibs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-14 15:50:35.000000 pvxslibs-1.2.0a1/python/pvxslibs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 15:50:35.618606 pvxslibs-1.2.0a1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26129 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:50:35.618606 pvxslibs-1.2.0a1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/bitmask.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/bitmask.h
+-rw-r--r--   0 runner    (1001) docker     (123)    40674 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/client.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14167 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/clientconn.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/clientdiscover.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19988 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/clientget.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/clientimpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/clientintrospect.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28142 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/clientmon.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/clientreq.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19459 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/config.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11010 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/conn.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/conn.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37194 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/data.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22826 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/dataencode.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/datafmt.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/dataimpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/describe.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/describe.h@
+-rw-r--r--   0 runner    (1001) docker     (123)    29891 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/evhelper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/evhelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/log.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/nt.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:50:35.594605 pvxslibs-1.2.0a1/src/os/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:50:35.618606 pvxslibs-1.2.0a1/src/os/WIN32/
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/os/WIN32/osdSockExt.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:50:35.618606 pvxslibs-1.2.0a1/src/os/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/os/default/osdSockExt.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/osgroups.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/osiSockExt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15947 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/pvaproto.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/pvrequest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/pvrequest.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:50:35.618606 pvxslibs-1.2.0a1/src/pvxs/
+-rw-r--r--   0 runner    (1001) docker     (123)    36817 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/pvxs/client.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28570 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/pvxs/data.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/pvxs/log.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/pvxs/netcommon.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/pvxs/nt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/pvxs/server.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23748 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/pvxs/sharedArray.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/pvxs/sharedpv.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/pvxs/source.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/pvxs/srvcommon.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/pvxs/unittest.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/pvxs/util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/pvxs/version.h
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/pvxs/versionNum.h@
+-rw-r--r--   0 runner    (1001) docker     (123)    24515 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/server.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11718 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/serverchan.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14442 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/serverconn.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/serverconn.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/serverget.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/serverintrospect.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20469 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/servermon.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/serversource.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20228 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/sharedarray.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/sharedpv.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13742 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/type.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19587 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/udp_collector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/udp_collector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/unittest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22583 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/util.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-05-14 15:50:04.000000 pvxslibs-1.2.0a1/src/utilpvt.h
```

### Comparing `pvxslibs-1.1.4a1/LICENSE` & `pvxslibs-1.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/MANIFEST.in` & `pvxslibs-1.2.0a1/MANIFEST.in`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 include src/*.h
 include src/*.h@
 include src/*.cpp
 include src/pvxs/*.h
 include src/pvxs/*.h@
 include src/os/default/*.cpp
 include src/os/WIN32/*.cpp
+include ioc/*.h
+include ioc/*.cpp
+include ioc/pvxs/*.h
 
 include bundle/libevent/LICENSE
 include bundle/libevent/cmake/VersionViaGit.cmake
 include bundle/libevent/*.h
 include bundle/libevent/*.h.cmake
 include bundle/libevent/include/*.h
 include bundle/libevent/compat/sys/*.h
```

### Comparing `pvxslibs-1.1.4a1/PKG-INFO` & `pvxslibs-1.2.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvxslibs
-Version: 1.1.4a1
+Version: 1.2.0a1
 Summary: PVXS libraries packaged for python
 Home-page: https://mdavidsaver.github.io/pvxs
 Author: Michael Davidsaver
 Author-email: mdavidsaver@gmail.com
 License: BSD
 Keywords: epics scada
 Platform: UNKNOWN
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/LICENSE` & `pvxslibs-1.2.0a1/bundle/libevent/LICENSE`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/arc4random.c` & `pvxslibs-1.2.0a1/bundle/libevent/arc4random.c`

 * *Files 2% similar despite different names*

```diff
@@ -71,16 +71,15 @@
 #include <stdlib.h>
 #include <string.h>
 #endif
 
 /* Add platform entropy 32 bytes (256 bits) at a time. */
 #define ADD_ENTROPY 32
 
-/* Re-seed from the platform RNG after generating this many bytes. */
-#define BYTES_BEFORE_RESEED 1600000
+#define REKEY_BASE (1024*1024) /* NB. should be a power of 2 */
 
 struct arc4_stream {
 	unsigned char i;
 	unsigned char j;
 	unsigned char s[256];
 };
 
@@ -339,18 +338,21 @@
 #ifdef TRY_SEED_SYSCTL_BSD
 	if (0 == arc4_seed_sysctl_bsd())
 		ok = 1;
 #endif
 	return ok ? 0 : -1;
 }
 
+static inline unsigned int
+arc4_getword(void);
 static int
 arc4_stir(void)
 {
 	int     i;
+	ARC4RANDOM_UINT32 rekey_fuzz; 
 
 	if (!rs_initialized) {
 		arc4_init();
 		rs_initialized = 1;
 	}
 
 	if (0 != arc4_seed())
@@ -373,15 +375,17 @@
 	 * to processor words.
 	 *
 	 * We add another sect to the cargo cult, and choose 12*256.
 	 */
 	for (i = 0; i < 12*256; i++)
 		(void)arc4_getbyte();
 
-	arc4_count = BYTES_BEFORE_RESEED;
+	rekey_fuzz = arc4_getword();
+	/* rekey interval should not be predictable */
+	arc4_count = REKEY_BASE + (rekey_fuzz % REKEY_BASE);
 
 	return 0;
 }
 
 
 static void
 arc4_stir_if_needed(void)
@@ -410,15 +414,15 @@
 }
 
 static inline unsigned int
 arc4_getword(void)
 {
 	unsigned int val;
 
-	val = arc4_getbyte() << 24;
+	val = (unsigned)arc4_getbyte() << 24;
 	val |= arc4_getbyte() << 16;
 	val |= arc4_getbyte() << 8;
 	val |= arc4_getbyte();
 
 	return val;
 }
 
@@ -463,27 +467,29 @@
 	arc4_stir_if_needed();
 	val = arc4_getword();
 	ARC4_UNLOCK_();
 	return val;
 }
 #endif
 
+#ifndef EVENT__HAVE_ARC4RANDOM_BUF
 ARC4RANDOM_EXPORT void
 arc4random_buf(void *buf_, size_t n)
 {
 	unsigned char *buf = buf_;
 	ARC4_LOCK_();
 	arc4_stir_if_needed();
 	while (n--) {
 		if (--arc4_count <= 0)
 			arc4_stir();
 		buf[n] = arc4_getbyte();
 	}
 	ARC4_UNLOCK_();
 }
+#endif  /* #ifndef EVENT__HAVE_ARC4RANDOM_BUF */
 
 #ifndef ARC4RANDOM_NOUNIFORM
 /*
  * Calculate a uniformly distributed random number less than upper_bound
  * avoiding "modulo bias".
  *
  * Uniformity is achieved by generating new random numbers until the one
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/buffer.c` & `pvxslibs-1.2.0a1/bundle/libevent/buffer.c`

 * *Files 1% similar despite different names*

```diff
@@ -154,25 +154,15 @@
 {
 	struct evbuffer_chain *chain;
 	size_t to_alloc;
 
 	if (size > EVBUFFER_CHAIN_MAX - EVBUFFER_CHAIN_SIZE)
 		return (NULL);
 
-	size += EVBUFFER_CHAIN_SIZE;
-
-	/* get the next largest memory that can hold the buffer */
-	if (size < EVBUFFER_CHAIN_MAX / 2) {
-		to_alloc = MIN_BUFFER_SIZE;
-		while (to_alloc < size) {
-			to_alloc <<= 1;
-		}
-	} else {
-		to_alloc = size;
-	}
+	to_alloc = size + EVBUFFER_CHAIN_SIZE;
 
 	/* we get everything in one chunk */
 	if ((chain = mm_malloc(to_alloc)) == NULL)
 		return (NULL);
 
 	memset(chain, 0, EVBUFFER_CHAIN_SIZE);
 
@@ -184,14 +174,37 @@
 	chain->buffer = EVBUFFER_CHAIN_EXTRA(unsigned char, chain);
 
 	chain->refcnt = 1;
 
 	return (chain);
 }
 
+static struct evbuffer_chain *
+evbuffer_chain_new_membuf(size_t size)
+{
+	size_t to_alloc;
+
+	if (size > EVBUFFER_CHAIN_MAX - EVBUFFER_CHAIN_SIZE)
+		return (NULL);
+
+	size += EVBUFFER_CHAIN_SIZE;
+
+	/* get the next largest memory that can hold the buffer */
+	if (size < EVBUFFER_CHAIN_MAX / 2) {
+		to_alloc = MIN_BUFFER_SIZE;
+		while (to_alloc < size) {
+			to_alloc <<= 1;
+		}
+	} else {
+		to_alloc = size;
+	}
+
+	return evbuffer_chain_new(to_alloc - EVBUFFER_CHAIN_SIZE);
+}
+
 static inline void
 evbuffer_chain_free(struct evbuffer_chain *chain)
 {
 	EVUTIL_ASSERT(chain->refcnt > 0);
 	if (--chain->refcnt > 0) {
 		/* chain is still referenced by other chains */
 		return;
@@ -322,15 +335,15 @@
 	buf->total_len += chain->off;
 }
 
 static inline struct evbuffer_chain *
 evbuffer_chain_insert_new(struct evbuffer *buf, size_t datlen)
 {
 	struct evbuffer_chain *chain;
-	if ((chain = evbuffer_chain_new(datlen)) == NULL)
+	if ((chain = evbuffer_chain_new_membuf(datlen)) == NULL)
 		return NULL;
 	evbuffer_chain_insert(buf, chain);
 	return chain;
 }
 
 void
 evbuffer_chain_pin_(struct evbuffer_chain *chain, unsigned flag)
@@ -845,15 +858,15 @@
 
 	/* If there's data in the first pinned chain, we need to allocate
 	 * a new chain and copy the data over. */
 	if (chain->off) {
 		struct evbuffer_chain *tmp;
 
 		EVUTIL_ASSERT(pinned == src->last_with_datap);
-		tmp = evbuffer_chain_new(chain->off);
+		tmp = evbuffer_chain_new_membuf(chain->off);
 		if (!tmp)
 			return -1;
 		memcpy(tmp->buffer, chain->buffer + chain->misalign,
 			chain->off);
 		tmp->off = chain->off;
 		*src->last_with_datap = tmp;
 		src->last = tmp;
@@ -1414,15 +1427,15 @@
 		size_t old_off = chain->off;
 		buffer = chain->buffer + chain->misalign + chain->off;
 		tmp = chain;
 		tmp->off = size;
 		size -= old_off;
 		chain = chain->next;
 	} else {
-		if ((tmp = evbuffer_chain_new(size)) == NULL) {
+		if ((tmp = evbuffer_chain_new_membuf(size)) == NULL) {
 			event_warn("%s: out of memory", __func__);
 			goto done;
 		}
 		buffer = tmp->buffer;
 		tmp->off = size;
 		buf->first = tmp;
 	}
@@ -1651,15 +1664,15 @@
 	}
 	case EVBUFFER_EOL_CRLF: {
 		ev_ssize_t start_pos = it.pos;
 		/* Look for a LF ... */
 		if (evbuffer_strchr(&it, '\n') < 0)
 			goto done;
 		extra_drain = 1;
-		/* ... optionally preceeded by a CR. */
+		/* ... optionally preceded by a CR. */
 		if (it.pos == start_pos)
 			break; /* If the first character is \n, don't back up */
 		/* This potentially does an extra linear walk over the first
 		 * few chains.  Probably, that's not too expensive unless you
 		 * have a really pathological setup. */
 		memcpy(&it2, &it, sizeof(it));
 		if (evbuffer_ptr_subtract(buffer, &it2, 1)<0)
@@ -1762,18 +1775,17 @@
 	} else {
 		chain = *buf->last_with_datap;
 	}
 
 	/* If there are no chains allocated for this buffer, allocate one
 	 * big enough to hold all the data. */
 	if (chain == NULL) {
-		chain = evbuffer_chain_new(datlen);
+		chain = evbuffer_chain_insert_new(buf, datlen);
 		if (!chain)
 			goto done;
-		evbuffer_chain_insert(buf, chain);
 	}
 
 	if ((chain->flags & EVBUFFER_IMMUTABLE) == 0) {
 		/* Always true for mutable buffers */
 		EVUTIL_ASSERT(chain->misalign >= 0 &&
 		    (ev_uint64_t)chain->misalign <= EVBUFFER_CHAIN_MAX);
 		remain = chain->buffer_len - (size_t)chain->misalign - chain->off;
@@ -1804,15 +1816,15 @@
 
 	/* we need to add another chain */
 	to_alloc = chain->buffer_len;
 	if (to_alloc <= EVBUFFER_CHAIN_MAX_AUTO_SIZE/2)
 		to_alloc <<= 1;
 	if (datlen > to_alloc)
 		to_alloc = datlen;
-	tmp = evbuffer_chain_new(to_alloc);
+	tmp = evbuffer_chain_new_membuf(to_alloc);
 	if (tmp == NULL)
 		goto done;
 
 	if (remain) {
 		memcpy(chain->buffer + chain->misalign + chain->off,
 		    data, remain);
 		chain->off += remain;
@@ -1854,18 +1866,17 @@
 	if (datlen > EV_SIZE_MAX - buf->total_len) {
 		goto done;
 	}
 
 	chain = buf->first;
 
 	if (chain == NULL) {
-		chain = evbuffer_chain_new(datlen);
+		chain = evbuffer_chain_insert_new(buf, datlen);
 		if (!chain)
 			goto done;
-		evbuffer_chain_insert(buf, chain);
 	}
 
 	/* we cannot touch immutable buffers */
 	if ((chain->flags & EVBUFFER_IMMUTABLE) == 0) {
 		/* Always true for mutable buffers */
 		EVUTIL_ASSERT(chain->misalign >= 0 &&
 		    (ev_uint64_t)chain->misalign <= EVBUFFER_CHAIN_MAX);
@@ -1894,15 +1905,15 @@
 			buf->n_add_for_cb += (size_t)chain->misalign;
 			datlen -= (size_t)chain->misalign;
 			chain->misalign = 0;
 		}
 	}
 
 	/* we need to add another chain */
-	if ((tmp = evbuffer_chain_new(datlen)) == NULL)
+	if ((tmp = evbuffer_chain_new_membuf(datlen)) == NULL)
 		goto done;
 	buf->first = tmp;
 	if (buf->last_with_datap == &buf->first && chain->off)
 		buf->last_with_datap = &tmp->next;
 
 	tmp->next = chain;
 
@@ -2023,15 +2034,15 @@
 	} else {
 		/* Okay, we're going to try to resize this chain: Not doing so
 		 * would waste at least 1/8 of its current allocation, and we
 		 * can do so without having to copy more than
 		 * MAX_TO_COPY_IN_EXPAND bytes. */
 		/* figure out how much space we need */
 		size_t length = chain->off + datlen;
-		struct evbuffer_chain *tmp = evbuffer_chain_new(length);
+		struct evbuffer_chain *tmp = evbuffer_chain_new_membuf(length);
 		if (tmp == NULL)
 			goto err;
 
 		/* copy the data over that we had so far */
 		tmp->off = chain->off;
 		memcpy(tmp->buffer, chain->buffer + chain->misalign,
 		    chain->off);
@@ -2069,20 +2080,19 @@
 
 	ASSERT_EVBUFFER_LOCKED(buf);
 	EVUTIL_ASSERT(n >= 2);
 
 	if (chain == NULL || (chain->flags & EVBUFFER_IMMUTABLE)) {
 		/* There is no last chunk, or we can't touch the last chunk.
 		 * Just add a new chunk. */
-		chain = evbuffer_chain_new(datlen);
+		chain = evbuffer_chain_insert_new(buf, datlen);
 		if (chain == NULL)
 			return (-1);
-
-		evbuffer_chain_insert(buf, chain);
-		return (0);
+		else
+			return (0);
 	}
 
 	used = 0; /* number of chains we're using space in. */
 	avail = 0; /* how much space they have. */
 	/* How many bytes can we stick at the end of buffer as it is?  Iterate
 	 * over the chains at the end of the buffer, tring to see how much
 	 * space we have in the first n. */
@@ -2112,15 +2122,15 @@
 	 * them. Either add a new chain with enough space, or replace all
 	 * empty chains with one that has enough space, depending on n. */
 	if (used < n) {
 		/* The loop ran off the end of the chains before it hit n
 		 * chains; we can add another. */
 		EVUTIL_ASSERT(chain == NULL);
 
-		tmp = evbuffer_chain_new(datlen - avail);
+		tmp = evbuffer_chain_new_membuf(datlen - avail);
 		if (tmp == NULL)
 			return (-1);
 
 		buf->last->next = tmp;
 		buf->last = tmp;
 		/* (we would only set last_with_data if we added the first
 		 * chain. But if the buffer had no chains, we would have
@@ -2144,15 +2154,15 @@
 
 		for (; chain; chain = next) {
 			next = chain->next;
 			EVUTIL_ASSERT(chain->off == 0);
 			evbuffer_chain_free(chain);
 		}
 		EVUTIL_ASSERT(datlen >= avail);
-		tmp = evbuffer_chain_new(datlen - avail);
+		tmp = evbuffer_chain_new_membuf(datlen - avail);
 		if (tmp == NULL) {
 			if (rmv_all) {
 				ZERO_CHAIN(buf);
 			} else {
 				buf->last = *buf->last_with_datap;
 				(*buf->last_with_datap)->next = NULL;
 			}
@@ -3050,15 +3060,15 @@
 evbuffer_file_segment_materialize(struct evbuffer_file_segment *seg)
 {
 	const unsigned flags = seg->flags;
 	const int fd = seg->fd;
 	const ev_off_t length = seg->length;
 	const ev_off_t offset = seg->file_offset;
 
-	if (seg->contents)
+	if (seg->contents || seg->is_mapping)
 		return 0; /* already materialized */
 
 #if defined(EVENT__HAVE_MMAP)
 	if (!(flags & EVBUF_FS_DISABLE_MMAP)) {
 		off_t offset_rounded = 0, offset_leftover = 0;
 		void *mapped;
 		if (offset) {
@@ -3066,15 +3076,19 @@
 			 * to have an offset that isn't a round  */
 			long page_size = get_page_size();
 			if (page_size == -1)
 				goto err;
 			offset_leftover = offset % page_size;
 			offset_rounded = offset - offset_leftover;
 		}
+#if defined(EVENT__HAVE_MMAP64)
+		mapped = mmap64(NULL, length + offset_leftover,
+#else
 		mapped = mmap(NULL, length + offset_leftover,
+#endif
 		    PROT_READ,
 #ifdef MAP_NOCACHE
 		    MAP_NOCACHE | /* ??? */
 #endif
 #ifdef MAP_FILE
 		    MAP_FILE |
 #endif
@@ -3209,20 +3223,18 @@
 	int can_use_sendfile = 0;
 
 	EVBUFFER_LOCK(buf);
 	EVLOCK_LOCK(seg->lock, 0);
 	if (buf->flags & EVBUFFER_FLAG_DRAINS_TO_FD) {
 		can_use_sendfile = 1;
 	} else {
-		if (!seg->contents) {
-			if (evbuffer_file_segment_materialize(seg)<0) {
-				EVLOCK_UNLOCK(seg->lock, 0);
-				EVBUFFER_UNLOCK(buf);
-				return -1;
-			}
+		if (evbuffer_file_segment_materialize(seg)<0) {
+			EVLOCK_UNLOCK(seg->lock, 0);
+			EVBUFFER_UNLOCK(buf);
+			return -1;
 		}
 	}
 	EVLOCK_UNLOCK(seg->lock, 0);
 
 	if (buf->freeze_end)
 		goto err;
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/buffer_iocp.c` & `pvxslibs-1.2.0a1/bundle/libevent/buffer_iocp.c`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 	/** How many chains are pinned; how many of the fields in buffers
 	 * are we using. */
 	int n_buffers;
 	WSABUF buffers[MAX_WSABUFS];
 };
 
-/** Given an evbuffer, return the correponding evbuffer structure, or NULL if
+/** Given an evbuffer, return the corresponding evbuffer structure, or NULL if
  * the evbuffer isn't overlapped. */
 static inline struct evbuffer_overlapped *
 upcast_evbuffer(struct evbuffer *buf)
 {
 	if (!buf || !buf->is_overlapped)
 		return NULL;
 	return EVUTIL_UPCAST(buf, struct evbuffer_overlapped, buffer);
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/bufferevent-internal.h` & `pvxslibs-1.2.0a1/bundle/libevent/bufferevent-internal.h`

 * *Files 1% similar despite different names*

```diff
@@ -481,16 +481,16 @@
 
 
 /** Internal: Given a bufferevent, return its corresponding
  * bufferevent_private. */
 #define BEV_UPCAST(b) EVUTIL_UPCAST((b), struct bufferevent_private, bev)
 
 #ifdef EVENT__DISABLE_THREAD_SUPPORT
-#define BEV_LOCK(b) EVUTIL_NIL_STMT_
-#define BEV_UNLOCK(b) EVUTIL_NIL_STMT_
+#define BEV_LOCK(b) (void)(b)
+#define BEV_UNLOCK(b) (void)(b)
 #else
 /** Internal: Grab the lock (if any) on a bufferevent */
 #define BEV_LOCK(b) do {						\
 		struct bufferevent_private *locking =  BEV_UPCAST(b);	\
 		EVLOCK_LOCK(locking->lock, 0);				\
 	} while (0)
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/bufferevent.c` & `pvxslibs-1.2.0a1/bundle/libevent/bufferevent.c`

 * *Files 0% similar despite different names*

```diff
@@ -497,15 +497,15 @@
 		impl_events &= ~EV_WRITE;
 
 	bufev->enabled |= event;
 
 	if (impl_events && bufev->be_ops->enable(bufev, impl_events) < 0)
 		r = -1;
 	if (r)
-		event_debug(("%s: cannot enable 0x%hx on %p", __func__, event, bufev));
+		event_debug(("%s: cannot enable 0x%hx on %p", __func__, event, (void *)bufev));
 
 	bufferevent_decref_and_unlock_(bufev);
 	return r;
 }
 
 int
 bufferevent_set_timeouts(struct bufferevent *bufev,
@@ -581,15 +581,15 @@
 
 	BEV_LOCK(bufev);
 	bufev->enabled &= ~event;
 
 	if (bufev->be_ops->disable(bufev, event) < 0)
 		r = -1;
 	if (r)
-		event_debug(("%s: cannot disable 0x%hx on %p", __func__, event, bufev));
+		event_debug(("%s: cannot disable 0x%hx on %p", __func__, event, (void *)bufev));
 
 	BEV_UNLOCK(bufev);
 	return r;
 }
 
 /*
  * Sets the water marks
@@ -872,15 +872,15 @@
 	union bufferevent_ctrl_data d;
 	int res = -1;
 	d.fd = fd;
 	BEV_LOCK(bev);
 	if (bev->be_ops->ctrl)
 		res = bev->be_ops->ctrl(bev, BEV_CTRL_SET_FD, &d);
 	if (res)
-		event_debug(("%s: cannot set fd for %p to "EV_SOCK_FMT, __func__, bev, fd));
+		event_debug(("%s: cannot set fd for %p to "EV_SOCK_FMT, __func__, (void *)bev, fd));
 	BEV_UNLOCK(bev);
 	return res;
 }
 
 int
 bufferevent_replacefd(struct bufferevent *bev, evutil_socket_t fd)
 {
@@ -899,15 +899,15 @@
 		}
 		if (!err) {
 			d.fd = fd;
 			err = bev->be_ops->ctrl(bev, BEV_CTRL_SET_FD, &d);
 		}
 	}
 	if (err)
-		event_debug(("%s: cannot replace fd for %p from "EV_SOCK_FMT" to "EV_SOCK_FMT, __func__, bev, old_fd, fd));
+		event_debug(("%s: cannot replace fd for %p from "EV_SOCK_FMT" to "EV_SOCK_FMT, __func__, (void *)bev, old_fd, fd));
 	BEV_UNLOCK(bev);
 
 	return err;
 }
 
 evutil_socket_t
 bufferevent_getfd(struct bufferevent *bev)
@@ -915,15 +915,15 @@
 	union bufferevent_ctrl_data d;
 	int res = -1;
 	d.fd = -1;
 	BEV_LOCK(bev);
 	if (bev->be_ops->ctrl)
 		res = bev->be_ops->ctrl(bev, BEV_CTRL_GET_FD, &d);
 	if (res)
-		event_debug(("%s: cannot get fd for %p", __func__, bev));
+		event_debug(("%s: cannot get fd for %p", __func__, (void *)bev));
 	BEV_UNLOCK(bev);
 	return (res<0) ? -1 : d.fd;
 }
 
 enum bufferevent_options
 bufferevent_get_options_(struct bufferevent *bev)
 {
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/bufferevent_async.c` & `pvxslibs-1.2.0a1/bundle/libevent/bufferevent_async.c`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/bufferevent_filter.c` & `pvxslibs-1.2.0a1/bundle/libevent/bufferevent_filter.c`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/bufferevent_mbedtls.c` & `pvxslibs-1.2.0a1/bundle/libevent/bufferevent_mbedtls.c`

 * *Files 8% similar despite different names*

```diff
@@ -20,31 +20,38 @@
  * NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
  * DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
  * THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF
  * THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
+
+/* Mbed-TLS 3.x does not currently expose a function to retrieve
+   the bio parameters from the SSL object. When the above issue has been
+   fixed, remove the MBEDTLS_ALLOW_PRIVATE_ACCESS define and use the
+   appropriate getter function in bufferevent_mbedtls_socket_new rather than
+   accessing the struct fields directly. */
+#define MBEDTLS_ALLOW_PRIVATE_ACCESS
 #include "mbedtls-compat.h"
-#include <mbedtls/config.h>
+#include <mbedtls/version.h>
 #include <mbedtls/ssl.h>
 #include <mbedtls/error.h>
 
 #include "event2/util.h"
 #include "util-internal.h"
 #include "event2/buffer.h"
 #include "event2/bufferevent.h"
 #include "event2/bufferevent_struct.h"
 #include "event2/bufferevent_ssl.h"
 
 #include "ssl-compat.h"
 #include "mm-internal.h"
 
 struct mbedtls_context {
-	mbedtls_ssl_context *ssl;
+	mbedtls_dyncontext *ssl;
 	mbedtls_net_context net;
 };
 static void *
 mbedtls_context_init(void *ssl)
 {
 	struct mbedtls_context *ctx = mm_malloc(sizeof(*ctx));
 	if (ctx) {
@@ -54,15 +61,15 @@
 	return ctx;
 }
 static void
 mbedtls_context_free(void *ssl, int flags)
 {
 	struct mbedtls_context *ctx = ssl;
 	if (flags & BEV_OPT_CLOSE_ON_FREE)
-		mbedtls_ssl_free(ctx->ssl);
+		bufferevent_mbedtls_dyncontext_free(ctx->ssl);
 	mm_free(ctx);
 }
 static int
 mbedtls_context_renegotiate(void *ssl)
 {
 #ifdef MBEDTLS_SSL_RENEGOTIATION
 	struct mbedtls_context *ctx = ssl;
@@ -298,15 +305,15 @@
 		return 0;
 	return bufferevent_get_ssl_error(bufev);
 }
 
 static struct le_ssl_ops le_mbedtls_ops = {
 	mbedtls_context_init,
 	mbedtls_context_free,
-	(void (*)(void *))mbedtls_ssl_free,
+	(void (*)(void *))bufferevent_mbedtls_dyncontext_free,
 	mbedtls_context_renegotiate,
 	mbedtls_context_write,
 	mbedtls_context_read,
 	mbedtls_context_pending,
 	mbedtls_context_handshake,
 	mbedtls_get_error,
 	mbedtls_clear_error,
@@ -341,15 +348,15 @@
 		be_mbedtls_bio_set_fd(bufferevent_ssl_upcast(bev), -1);
 	}
 
 	return bev;
 
 err:
 	if (options & BEV_OPT_CLOSE_ON_FREE)
-		mbedtls_ssl_free(ssl);
+		bufferevent_mbedtls_dyncontext_free(ssl);
 	return NULL;
 }
 
 struct bufferevent *
 bufferevent_mbedtls_socket_new(struct event_base *base, evutil_socket_t fd,
 	mbedtls_ssl_context *ssl, enum bufferevent_ssl_state state, int options)
 {
@@ -396,7 +403,23 @@
 		be_mbedtls_bio_set_fd(bufferevent_ssl_upcast(bev), fd);
 	}
 
 	return bev;
 err:
 	return NULL;
 }
+
+mbedtls_dyncontext *
+bufferevent_mbedtls_dyncontext_new(struct mbedtls_ssl_config *conf)
+{
+	mbedtls_dyncontext *ctx = mm_calloc(1, sizeof(*ctx));
+	mbedtls_ssl_init(ctx);
+	mbedtls_ssl_setup(ctx, conf);
+	return ctx;
+}
+
+void
+bufferevent_mbedtls_dyncontext_free(mbedtls_dyncontext *ctx)
+{
+	mbedtls_ssl_free(ctx);
+	mm_free(ctx);
+}
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/bufferevent_openssl.c` & `pvxslibs-1.2.0a1/bundle/libevent/bufferevent_openssl.c`

 * *Files 2% similar despite different names*

```diff
@@ -255,15 +255,17 @@
 	case SSL_ERROR_SYSCALL:
 		/* IO error; possibly a dirty shutdown. */
 		if ((ret == 0 || ret == -1) && ERR_peek_error() == 0)
 			dirty_shutdown = 1;
 		bufferevent_ssl_put_error(bev_ssl, errcode);
 		break;
 	case SSL_ERROR_SSL:
-		/* Protocol error. */
+		/* Protocol error; possibly a dirty shutdown. */
+		if (ret == 0 && SSL_is_init_finished(bev_ssl->ssl) == 0)
+			dirty_shutdown = 1;
 		bufferevent_ssl_put_error(bev_ssl, errcode);
 		break;
 	case SSL_ERROR_WANT_X509_LOOKUP:
 		/* XXXX handle this. */
 		bufferevent_ssl_put_error(bev_ssl, errcode);
 		break;
 	case SSL_ERROR_NONE:
@@ -471,15 +473,15 @@
 		} else if (have_fd == (long)fd) {
 			/* We already know the fd from the SSL; do nothing */
 		} else {
 			/* We specified an fd different from that of the SSL.
 			   This is probably an error on our part.  Fail. */
 			goto err;
 		}
-		BIO_set_close(bio, 0);
+		(void)BIO_set_close(bio, 0);
 	} else {
 		/* The SSL isn't configured with a BIO with an fd. */
 		if (fd >= 0) {
 			/* ... and we have an fd we want to use. */
 			bio = BIO_new_socket((int)fd, 0);
 			SSL_set_bio(ssl, bio, bio);
 		} else {
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/bufferevent_pair.c` & `pvxslibs-1.2.0a1/bundle/libevent/bufferevent_pair.c`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/bufferevent_ratelim.c` & `pvxslibs-1.2.0a1/bundle/libevent/bufferevent_ratelim.c`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 int
 ev_token_bucket_update_(struct ev_token_bucket *bucket,
     const struct ev_token_bucket_cfg *cfg,
     ev_uint32_t current_tick)
 {
 	/* It's okay if the tick number overflows, since we'll just
-	 * wrap around when we do the unsigned substraction. */
+	 * wrap around when we do the unsigned subtraction. */
 	unsigned n_ticks = current_tick - bucket->last_updated;
 
 	/* Make sure some ticks actually happened, and that time didn't
 	 * roll back. */
 	if (n_ticks == 0 || n_ticks > INT_MAX)
 		return 0;
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/bufferevent_sock.c` & `pvxslibs-1.2.0a1/bundle/libevent/bufferevent_sock.c`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/bufferevent_ssl.c` & `pvxslibs-1.2.0a1/bundle/libevent/bufferevent_ssl.c`

 * *Files 1% similar despite different names*

```diff
@@ -381,15 +381,17 @@
 				bev_ssl->last_write = -1;
 			}
 			result |= OP_BLOCKED;
 			break;
 		}
 	}
 	if (n_written) {
-		evbuffer_drain(output, n_written);
+		if (evbuffer_drain(output, n_written))
+			return OP_ERR | result;
+
 		if (bev_ssl->underlying)
 			BEV_RESET_GENERIC_WRITE_TIMEOUT(bev);
 
 		bufferevent_trigger_nolock_(bev, EV_WRITE, BEV_OPT_DEFER_CALLBACKS);
 	}
 	return result;
 }
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/changelist-internal.h` & `pvxslibs-1.2.0a1/bundle/libevent/changelist-internal.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/cmake/VersionViaGit.cmake` & `pvxslibs-1.2.0a1/bundle/libevent/cmake/VersionViaGit.cmake`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/compat/sys/queue.h` & `pvxslibs-1.2.0a1/bundle/libevent/compat/sys/queue.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/defer-internal.h` & `pvxslibs-1.2.0a1/bundle/libevent/defer-internal.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/devpoll.c` & `pvxslibs-1.2.0a1/bundle/libevent/devpoll.c`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/epoll.c` & `pvxslibs-1.2.0a1/bundle/libevent/epoll.c`

 * *Files 3% similar despite different names*

```diff
@@ -77,19 +77,21 @@
 #endif
 
 #include "epolltable-internal.h"
 
 #if defined(EVENT__HAVE_SYS_TIMERFD_H) &&			  \
 	defined(EVENT__HAVE_TIMERFD_CREATE) &&			  \
 	defined(HAVE_POSIX_MONOTONIC) && defined(TFD_NONBLOCK) && \
-	defined(TFD_CLOEXEC)
+	defined(TFD_CLOEXEC) && !defined(EVENT__HAVE_EPOLL_PWAIT2)
 /* Note that we only use timerfd if TFD_NONBLOCK and TFD_CLOEXEC are available
    and working.  This means that we can't support it on 2.6.25 (where timerfd
-   was introduced) or 2.6.26, since 2.6.27 introduced those flags.
- */
+   was introduced) or 2.6.26, since 2.6.27 introduced those flags. On recent
+   enough systems (with 5.11 and never) and so epoll_pwait2() with nanosecond
+   precision for timeouts, timerfd is not needed at all.
+*/
 #define USING_TIMERFD
 #endif
 
 #ifdef EVENT__HAVE_WEPOLL
 typedef HANDLE epoll_handle;
 #define INVALID_EPOLL_HANDLE NULL
 static void close_epoll_handle(HANDLE h) { epoll_close(h); }
@@ -249,15 +251,16 @@
 			epollop->timerfd = -1;
 		}
 	} else {
 		epollop->timerfd = -1;
 	}
 #endif
 
-	evsig_init_(base);
+	if (sigfd_init_(base) < 0)
+		evsig_init_(base);
 
 	return (epollop);
 }
 
 static const char *
 change_to_string(int change)
 {
@@ -455,15 +458,19 @@
 
 static int
 epoll_dispatch(struct event_base *base, struct timeval *tv)
 {
 	struct epollop *epollop = base->evbase;
 	struct epoll_event *events = epollop->events;
 	int i, res;
+#if defined(EVENT__HAVE_EPOLL_PWAIT2)
+	struct timespec ts = { 0, 0 };
+#else /* no epoll_pwait2() */
 	long timeout = -1;
+#endif /* EVENT__HAVE_EPOLL_PWAIT2 */
 
 #ifdef USING_TIMERFD
 	if (epollop->timerfd >= 0) {
 		struct itimerspec is;
 		is.it_interval.tv_sec = 0;
 		is.it_interval.tv_nsec = 0;
 		if (tv == NULL) {
@@ -485,28 +492,36 @@
 		*/
 		if (timerfd_settime(epollop->timerfd, 0, &is, NULL) < 0) {
 			event_warn("timerfd_settime");
 		}
 	} else
 #endif
 	if (tv != NULL) {
+#if defined(EVENT__HAVE_EPOLL_PWAIT2)
+		TIMEVAL_TO_TIMESPEC(tv, &ts);
+#else /* no epoll_pwait2() */
 		timeout = evutil_tv_to_msec_(tv);
 		if (timeout < 0 || timeout > MAX_EPOLL_TIMEOUT_MSEC) {
 			/* Linux kernels can wait forever if the timeout is
 			 * too big; see comment on MAX_EPOLL_TIMEOUT_MSEC. */
 			timeout = MAX_EPOLL_TIMEOUT_MSEC;
 		}
+#endif /* EVENT__HAVE_EPOLL_PWAIT2 */
 	}
 
 	epoll_apply_changes(base);
 	event_changelist_remove_all_(&base->changelist, base);
 
 	EVBASE_RELEASE_LOCK(base, th_base_lock);
 
+#if defined(EVENT__HAVE_EPOLL_PWAIT2)
+	res = epoll_pwait2(epollop->epfd, events, epollop->nevents, tv ? &ts : NULL, NULL);
+#else /* no epoll_pwait2() */
 	res = epoll_wait(epollop->epfd, events, epollop->nevents, timeout);
+#endif /* EVENT__HAVE_EPOLL_PWAIT2 */
 
 	EVBASE_ACQUIRE_LOCK(base, th_base_lock);
 
 	if (res == -1) {
 		if (errno != EINTR) {
 			event_warn("epoll_wait");
 			return (-1);
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/epoll_sub.c` & `pvxslibs-1.2.0a1/bundle/libevent/epoll_sub.c`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/epolltable-internal.h` & `pvxslibs-1.2.0a1/bundle/libevent/epolltable-internal.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/evbuffer-internal.h` & `pvxslibs-1.2.0a1/bundle/libevent/evbuffer-internal.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/evconfig-private.h.cmake` & `pvxslibs-1.2.0a1/bundle/libevent/evconfig-private.h.cmake`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/evdns.c` & `pvxslibs-1.2.0a1/bundle/libevent/evdns.c`

 * *Files 2% similar despite different names*

```diff
@@ -118,16 +118,16 @@
 #include <netinet/in6.h>
 #endif
 
 #define EVDNS_LOG_DEBUG EVENT_LOG_DEBUG
 #define EVDNS_LOG_WARN EVENT_LOG_WARN
 #define EVDNS_LOG_MSG EVENT_LOG_MSG
 
-#ifndef HOST_NAME_MAX
-#define HOST_NAME_MAX 255
+#ifndef EVDNS_NAME_MAX
+#define EVDNS_NAME_MAX 255
 #endif
 
 #include <stdio.h>
 
 #undef MIN
 #undef MAX
 #define MIN(a,b) ((a)<(b)?(a):(b))
@@ -166,25 +166,49 @@
 /* Timeout in seconds for idle TCP connections that server keeps alive. */
 #define SERVER_IDLE_CONN_TIMEOUT 10
 /* Timeout in seconds for idle TCP connections that client keeps alive. */
 #define CLIENT_IDLE_CONN_TIMEOUT 5
 /* Default maximum number of simultaneous TCP client connections that DNS server can hold. */
 #define MAX_CLIENT_CONNECTIONS 10
 
+struct reply {
+	unsigned int type;
+	unsigned int have_answer : 1;
+	u32 rr_count;
+	union {
+		u32 *a;
+		struct in6_addr *aaaa;
+		char *ptr_name;
+		void *raw;
+	} data;
+	char *cname;
+};
+
+
 /* Persistent handle.  We keep this separate from 'struct request' since we
  * need some object to last for as long as an evdns_request is outstanding so
  * that it can be canceled, whereas a search request can lead to multiple
  * 'struct request' instances being created over its lifetime. */
 struct evdns_request {
 	struct request *current_req;
 	struct evdns_base *base;
 
 	int pending_cb; /* Waiting for its callback to be invoked; not
 			 * owned by event base any more. */
 
+	/* data used when fulfilling the callback */
+	struct event_callback deferred;
+	evdns_callback_type user_callback;
+	void *user_pointer;
+	u8 request_type;
+	u8 have_reply;
+	u32 ttl;
+	u32 err;
+	struct reply reply;
+
 	/* elements used by the searching code */
 	int search_index;
 	struct search_state *search_state;
 	char *search_origname;	/* needs to be free()ed */
 	int search_flags;
 	u16 tcp_flags;
 };
@@ -192,16 +216,14 @@
 struct request {
 	u8 *request;  /* the dns packet data */
 	u16 request_size; /* size of memory block stored in request field */
 	u8 request_type; /* TYPE_PTR or TYPE_A or TYPE_AAAA */
 	unsigned int request_len;
 	int reissue_count;
 	int tx_count;  /* the number of times that this packet has been sent */
-	void *user_pointer;  /* the pointer given to us for this request */
-	evdns_callback_type user_callback;
 	struct nameserver *ns;	/* the server which we last sent it */
 
 	/* these objects are kept in a circular list */
 	/* XXX We could turn this into a CIRCLEQ. */
 	struct request *next, *prev;
 
 	struct event timeout_event;
@@ -215,27 +237,14 @@
 	char **put_cname_in_ptr; /* store the cname here if we get one. */
 
 	struct evdns_base *base;
 
 	struct evdns_request *handle;
 };
 
-struct reply {
-	unsigned int type;
-	unsigned int have_answer : 1;
-	u32 rr_count;
-	union {
-		u32 *a;
-		struct in6_addr *aaaa;
-		char *ptr_name;
-		void *raw;
-	} data;
-	char *cname;
-};
-
 enum tcp_state {
 	TS_DISCONNECTED,
 	TS_CONNECTING,
 	TS_CONNECTED
 };
 
 struct tcp_connection {
@@ -459,18 +468,18 @@
 static void evdns_request_remove(struct request *req, struct request **head);
 static void nameserver_ready_callback(evutil_socket_t fd, short events, void *arg);
 static int evdns_transmit(struct evdns_base *base);
 static int evdns_request_transmit(struct request *req);
 static void nameserver_send_probe(struct nameserver *const ns);
 static void search_request_finished(struct evdns_request *const);
 static int search_try_next(struct evdns_request *const req);
-static struct request *search_request_new(struct evdns_base *base, struct evdns_request *handle, int type, const char *const name, int flags, evdns_callback_type user_callback, void *user_arg);
+static struct request *search_request_new(struct evdns_base *base, struct evdns_request *handle, int type, const char *const name, int flags);
 static void evdns_requests_pump_waiting_queue(struct evdns_base *base);
 static u16 transaction_id_pick(struct evdns_base *base);
-static struct request *request_new(struct evdns_base *base, struct evdns_request *handle, int type, const char *name, int flags, evdns_callback_type callback, void *ptr);
+static struct request *request_new(struct evdns_base *base, struct evdns_request *handle, int type, const char *name, int flags);
 static struct request *request_clone(struct evdns_base *base, struct request* current);
 static void request_submit(struct request *const req);
 
 static int server_request_free(struct server_request *req);
 static void server_request_free_answers(struct server_request *req);
 static void server_port_free(struct evdns_server_port *port);
 static void server_port_ready_callback(evutil_socket_t fd, short events, void *arg);
@@ -850,15 +859,15 @@
 	int was_inflight = (head != &base->req_waiting_head);
 	EVDNS_LOCK(base);
 	ASSERT_VALID_REQUEST(req);
 
 	if (head)
 		evdns_request_remove(req, head);
 
-	log(EVDNS_LOG_DEBUG, "Removing timeout for request %p", req);
+	log(EVDNS_LOG_DEBUG, "Removing timeout for request %p", (void *)req);
 	if (was_inflight) {
 		evtimer_del(&req->timeout_event);
 		base->global_requests_inflight--;
 		req->ns->requests_inflight--;
 	} else {
 		base->global_requests_waiting--;
 	}
@@ -964,122 +973,96 @@
 
 		evdns_request_insert(req, &REQ_HEAD(base, req->trans_id));
 		evdns_request_transmit(req);
 		evdns_transmit(base);
 	}
 }
 
-/* TODO(nickm) document */
-struct deferred_reply_callback {
-	struct event_callback deferred;
-	struct evdns_request *handle;
-	u8 request_type;
-	u8 have_reply;
-	u32 ttl;
-	u32 err;
-	evdns_callback_type user_callback;
-	struct reply reply;
-};
-
 static void
 reply_run_callback(struct event_callback *d, void *user_pointer)
 {
-	struct deferred_reply_callback *cb =
-	    EVUTIL_UPCAST(d, struct deferred_reply_callback, deferred);
+	struct evdns_request *handle =
+	    EVUTIL_UPCAST(d, struct evdns_request, deferred);
 
-	switch (cb->request_type) {
+	switch (handle->request_type) {
 	case TYPE_A:
-		if (cb->have_reply) {
-			cb->user_callback(DNS_ERR_NONE, DNS_IPv4_A,
-			    cb->reply.rr_count, cb->ttl,
-			    cb->reply.data.a,
+		if (handle->have_reply) {
+			handle->user_callback(DNS_ERR_NONE, DNS_IPv4_A,
+			    handle->reply.rr_count, handle->ttl,
+			    handle->reply.data.a,
 			    user_pointer);
-			if (cb->reply.cname)
-				cb->user_callback(DNS_ERR_NONE, DNS_CNAME, 1,
-				    cb->ttl, cb->reply.cname, user_pointer);
+			if (handle->reply.cname)
+				handle->user_callback(DNS_ERR_NONE, DNS_CNAME, 1,
+				    handle->ttl, handle->reply.cname, user_pointer);
 		} else
-			cb->user_callback(cb->err, 0, 0, cb->ttl, NULL, user_pointer);
+			handle->user_callback(handle->err, 0, 0, handle->ttl, NULL, user_pointer);
 		break;
 	case TYPE_PTR:
-		if (cb->have_reply) {
-			char *name = cb->reply.data.ptr_name;
-			cb->user_callback(DNS_ERR_NONE, DNS_PTR, 1, cb->ttl,
+		if (handle->have_reply) {
+			char *name = handle->reply.data.ptr_name;
+			handle->user_callback(DNS_ERR_NONE, DNS_PTR, 1, handle->ttl,
 			    &name, user_pointer);
 		} else {
-			cb->user_callback(cb->err, 0, 0, cb->ttl, NULL, user_pointer);
+			handle->user_callback(handle->err, 0, 0, handle->ttl, NULL, user_pointer);
 		}
 		break;
 	case TYPE_AAAA:
-		if (cb->have_reply) {
-			cb->user_callback(DNS_ERR_NONE, DNS_IPv6_AAAA,
-			    cb->reply.rr_count, cb->ttl,
-			    cb->reply.data.aaaa,
+		if (handle->have_reply) {
+			handle->user_callback(DNS_ERR_NONE, DNS_IPv6_AAAA,
+			    handle->reply.rr_count, handle->ttl,
+			    handle->reply.data.aaaa,
 			    user_pointer);
-			if (cb->reply.cname)
-				cb->user_callback(DNS_ERR_NONE, DNS_CNAME, 1,
-				    cb->ttl, cb->reply.cname, user_pointer);
+			if (handle->reply.cname)
+				handle->user_callback(DNS_ERR_NONE, DNS_CNAME, 1,
+				    handle->ttl, handle->reply.cname, user_pointer);
 		} else
-			cb->user_callback(cb->err, 0, 0, cb->ttl, NULL, user_pointer);
+			handle->user_callback(handle->err, 0, 0, handle->ttl, NULL, user_pointer);
 		break;
 	default:
 		EVUTIL_ASSERT(0);
 	}
 
-	if (cb->handle && cb->handle->pending_cb) {
-		mm_free(cb->handle);
-	}
-
-	if (cb->reply.data.raw) {
-		mm_free(cb->reply.data.raw);
+	if (handle->reply.data.raw) {
+		mm_free(handle->reply.data.raw);
 	}
 
-	if (cb->reply.cname) {
-		mm_free(cb->reply.cname);
+	if (handle->reply.cname) {
+		mm_free(handle->reply.cname);
 	}
 
-	mm_free(cb);
+	mm_free(handle);
 }
 
 static void
 reply_schedule_callback(struct request *const req, u32 ttl, u32 err, struct reply *reply)
 {
-	struct deferred_reply_callback *d = mm_calloc(1, sizeof(*d));
-
-	if (!d) {
-		event_warn("%s: Couldn't allocate space for deferred callback.",
-		    __func__);
-		return;
-	}
+	struct evdns_request* handle = req->handle;
 
 	ASSERT_LOCKED(req->base);
 
-	d->request_type = req->request_type;
-	d->user_callback = req->user_callback;
-	d->ttl = ttl;
-	d->err = err;
+	handle->request_type = req->request_type;
+	handle->ttl = ttl;
+	handle->err = err;
 	if (reply) {
-		d->have_reply = 1;
-		memcpy(&d->reply, reply, sizeof(struct reply));
+		handle->have_reply = 1;
+		memcpy(&handle->reply, reply, sizeof(struct reply));
 		/* We've taken ownership of the data. */
 		reply->data.raw = NULL;
 	}
 
-	if (req->handle) {
-		req->handle->pending_cb = 1;
-		d->handle = req->handle;
-	}
+	handle->pending_cb = 1;
 
 	event_deferred_cb_init_(
-	    &d->deferred,
+	    &handle->deferred,
 	    event_get_priority(&req->timeout_event),
 	    reply_run_callback,
-	    req->user_pointer);
+	    handle->user_pointer);
 	event_deferred_cb_schedule_(
 		req->base->event_base,
-		&d->deferred);
+		&handle->deferred);
 }
 
 static int
 client_retransmit_through_tcp(struct evdns_request *handle)
 {
 	struct request *req = handle->current_req;
 	struct evdns_base *base = req->base;
@@ -1346,15 +1329,15 @@
 	if (!name_matches)
 		goto err;
 
 	/* We can allocate less for the reply data, but to do it we'll have
 	 * to parse the response. To simplify things let's just allocate
 	 * a little bit more to avoid complex evaluations.
 	 */
-	buf_size = MAX(length - j, HOST_NAME_MAX);
+	buf_size = MAX(length - j, EVDNS_NAME_MAX);
 	reply.data.raw = mm_malloc(buf_size);
 
 	/* now we have the answer section which looks like
 	 * <label:name><u16:type><u16:class><u32:ttl><u16:len><data...>
 	 */
 
 	for (i = 0; i < answers; ++i) {
@@ -1390,15 +1373,15 @@
 			if (name_parse(packet, length, &j, reply.data.ptr_name,
 						   buf_size)<0)
 				goto err;
 			ttl_r = MIN(ttl_r, ttl);
 			reply.have_answer = 1;
 			break;
 		} else if (type == TYPE_CNAME) {
-			char cname[HOST_NAME_MAX];
+			char cname[EVDNS_NAME_MAX];
 			if (name_parse(packet, length, &j, cname,
 				sizeof(cname))<0)
 				goto err;
 			if (req->need_cname)
 				reply.cname = mm_strdup(cname);
 			if (req->put_cname_in_ptr && !*req->put_cname_in_ptr)
 				*req->put_cname_in_ptr = mm_strdup(cname);
@@ -1588,20 +1571,22 @@
 		return -1;
 	}
 
 	port->user_callback(&(server_req->base), port->user_data);
 
 	return 0;
 err:
-	if (server_req->base.questions) {
-		for (i = 0; i < server_req->base.nquestions; ++i)
-			mm_free(server_req->base.questions[i]);
-		mm_free(server_req->base.questions);
+	if (server_req) {
+		if (server_req->base.questions) {
+			for (i = 0; i < server_req->base.nquestions; ++i)
+				mm_free(server_req->base.questions[i]);
+			mm_free(server_req->base.questions);
+		}
+		mm_free(server_req);
 	}
-	mm_free(server_req);
 	return -1;
 
 #undef SKIP_RR
 #undef SKIP_NAME
 #undef GET32
 #undef GET16
 #undef GET8
@@ -1749,15 +1734,15 @@
 	} else {
 		int r = sendto(port->socket, req->response, (int)req->response_len, 0,
 					(struct sockaddr*) &req->addr, (ev_socklen_t)req->addrlen);
 		return r;
 	}
 
 beferevent_error:
-	log(EVDNS_LOG_WARN, "Failed to send reply to request %p for client %p", req, req->client);
+	log(EVDNS_LOG_WARN, "Failed to send reply to request %p for client %p", (void *)req, (void *)req->client);
 	/* disconnect if we got bufferevent error */
 	evdns_remove_tcp_client(port, req->client);
 	return -1;
 }
 
 /* Try to write all pending replies on a given DNS server port. */
 static void
@@ -2190,15 +2175,15 @@
 	struct evdns_server_port *port = client->port;
 	struct tcp_connection *conn = &client->connection;
 	EVUTIL_ASSERT(port && bev);
 	EVDNS_LOCK(port);
 
 	while (1) {
 		if (tcp_read_message(conn, &msg, &msg_len)) {
-			log(EVDNS_LOG_MSG, "Closing client connection %p due to error", bev);
+			log(EVDNS_LOG_MSG, "Closing client connection %p due to error", (void *)bev);
 			evdns_remove_tcp_client(port, client);
 			rc = port->refcnt;
 			EVDNS_UNLOCK(port);
 			if (!rc)
 				server_port_free(port);
 			return;
 		}
@@ -2224,15 +2209,15 @@
 {
 	struct client_tcp_connection *client = (struct client_tcp_connection *)ctx;
 	struct evdns_server_port *port = client->port;
 	int rc;
 	EVUTIL_ASSERT(port && bev);
 	EVDNS_LOCK(port);
 	if (events & (BEV_EVENT_EOF | BEV_EVENT_ERROR | BEV_EVENT_TIMEOUT)) {
-		log(EVDNS_LOG_DEBUG, "Closing connection %p", bev);
+		log(EVDNS_LOG_DEBUG, "Closing connection %p", (void *)bev);
 		evdns_remove_tcp_client(port, client);
 	}
 	rc = port->refcnt;
 	EVDNS_UNLOCK(port);
 	if (!rc)
 		server_port_free(port);
 }
@@ -2244,15 +2229,15 @@
 	struct evdns_server_port *port = (struct evdns_server_port*)arg;
 	struct bufferevent *bev = bufferevent_socket_new(port->event_base, fd, BEV_OPT_CLOSE_ON_FREE);
 	struct client_tcp_connection *client = NULL;
 	struct tcp_connection *cd = NULL;
 
 	if (!bev)
 		goto error;
-	log(EVDNS_LOG_DEBUG, "New incoming client connection %p", bev);
+	log(EVDNS_LOG_DEBUG, "New incoming client connection %p", (void *)bev);
 
 	bufferevent_set_timeouts(bev, &port->tcp_idle_timeout, &port->tcp_idle_timeout);
 
 	client = evdns_add_tcp_client(port, bev);
 	if (!client)
 		goto error;
 	cd = &client->connection;
@@ -2715,15 +2700,15 @@
 		if (!req)
 			continue;
 
 		do {
 			if (req->ns == server && (req->handle->tcp_flags & DNS_QUERY_USEVC)) {
 				if (req->tx_count >= req->base->global_max_retransmits) {
 					log(EVDNS_LOG_DEBUG, "Giving up on request %p; tx_count==%d",
-						req, req->tx_count);
+						(void *)req, req->tx_count);
 					reply_schedule_callback(req, 0, DNS_ERR_TIMEOUT, NULL);
 					request_finished(req, &REQ_HEAD(req->base, req->trans_id), 1);
 				} else {
 					(void) evtimer_del(&req->timeout_event);
 					evdns_request_transmit(req);
 				}
 			}
@@ -2837,15 +2822,15 @@
 		return 1;
 
 	EVUTIL_ASSERT(conn->state == TS_DISCONNECTED);
 	if (bufferevent_socket_connect(conn->bev, (struct sockaddr *)&server->address, server->addrlen))
 		return 1;
 
 	conn->state = TS_CONNECTING;
-	log(EVDNS_LOG_DEBUG, "New tcp connection %p created", conn);
+	log(EVDNS_LOG_DEBUG, "New tcp connection %p created", (void *)conn);
 	return 0;
 }
 
 static void
 client_tcp_event_cb(struct bufferevent *bev, short events, void *ctx);
 
 
@@ -2887,15 +2872,15 @@
 client_tcp_event_cb(struct bufferevent *bev, short events, void *ctx) {
 	struct nameserver *server = (struct nameserver*)ctx;
 	struct tcp_connection *conn = server->connection;
 	EVUTIL_ASSERT(server);
 	EVDNS_LOCK(server->base);
 	EVUTIL_ASSERT(conn && conn->bev == bev && bev);
 
-	log(EVDNS_LOG_DEBUG, "Event %d on connection %p", events, conn);
+	log(EVDNS_LOG_DEBUG, "Event %d on connection %p", events, (void *)conn);
 
 	if (events & (BEV_EVENT_TIMEOUT)) {
 		disconnect_and_free_connection(server->connection);
 		server->connection = NULL;
 	} else if (events & (BEV_EVENT_EOF | BEV_EVENT_ERROR)) {
 		disconnect_and_free_connection(server->connection);
 		server->connection = NULL;
@@ -2925,28 +2910,28 @@
 
 	if ((r = evdns_tcp_connect_if_disconnected(server)))
 		return r;
 
 	conn = server->connection;
 	bufferevent_setcb(conn->bev, client_tcp_read_packet_cb, NULL, client_tcp_event_cb, server);
 
-	log(EVDNS_LOG_DEBUG, "Sending request %p via tcp connection %p", req, conn);
+	log(EVDNS_LOG_DEBUG, "Sending request %p via tcp connection %p", (void *)req, (void *)conn);
 	packet_size = htons(req->request_len);
 	if (bufferevent_write(conn->bev, &packet_size, sizeof(packet_size)) )
 		goto fail;
 	if (bufferevent_write(conn->bev, (void*)req->request, req->request_len) )
 		goto fail;
 	if (bufferevent_enable(conn->bev, EV_READ))
 		goto fail;
 	if (evtimer_add(&req->timeout_event, &req->base->global_timeout) < 0)
 		goto fail;
 
 	return 0;
 fail:
-	log(EVDNS_LOG_WARN, "Failed to send request %p via tcp connection %p", req, conn);
+	log(EVDNS_LOG_WARN, "Failed to send request %p via tcp connection %p", (void *)req, (void *)conn);
 	disconnect_and_free_connection(server->connection);
 	server->connection = NULL;
 	return 2;
 }
 
 /* try to send a request, updating the fields of the request */
 /* as needed */
@@ -3000,19 +2985,19 @@
 		 * we'll set a timeout, which will time out, and make us retransmit the
 		 * request anyway. */
 		retcode = 1;
 		EVUTIL_FALLTHROUGH;
 	default:
 		/* all ok */
 		log(EVDNS_LOG_DEBUG,
-		    "Setting timeout for request %p, sent to nameserver %p", req, req->ns);
+		    "Setting timeout for request %p, sent to nameserver %p", (void *)req, (void *)req->ns);
 		if (evtimer_add(&req->timeout_event, &req->base->global_timeout) < 0) {
 			log(EVDNS_LOG_WARN,
 		      "Error from libevent when adding timer for request %p",
-			    req);
+			    (void *)req);
 			/* ???? Do more? */
 		}
 		req->tx_count++;
 		req->transmit_me = 0;
 		return retcode;
 	}
 }
@@ -3054,15 +3039,17 @@
 	ASSERT_LOCKED(ns->base);
 	log(EVDNS_LOG_DEBUG, "Sending probe to %s",
 	    evutil_format_sockaddr_port_(
 		    (struct sockaddr *)&ns->address,
 		    addrbuf, sizeof(addrbuf)));
 	handle = mm_calloc(1, sizeof(*handle));
 	if (!handle) return;
-	req = request_new(ns->base, handle, TYPE_A, "google.com", DNS_QUERY_NO_SEARCH, nameserver_probe_callback, ns);
+	handle->user_callback = nameserver_probe_callback;
+	handle->user_pointer = ns;
+	req = request_new(ns->base, handle, TYPE_A, "google.com", DNS_QUERY_NO_SEARCH);
 	if (!req) {
 		mm_free(handle);
 		return;
 	}
 	ns->probe_request = handle;
 	/* we force this into the inflight queue no matter what */
 	request_trans_id_set(req, transaction_id_pick(ns->base));
@@ -3284,15 +3271,15 @@
 				 EV_READ | EV_PERSIST, nameserver_ready_callback, ns);
 	if (!base->disable_when_inactive && event_add(&ns->event, NULL) < 0) {
 		err = 2;
 		goto out2;
 	}
 
 	log(EVDNS_LOG_DEBUG, "Added nameserver %s as %p",
-	    evutil_format_sockaddr_port_(address, addrbuf, sizeof(addrbuf)), ns);
+	    evutil_format_sockaddr_port_(address, addrbuf, sizeof(addrbuf)), (void *)ns);
 
 	/* insert this nameserver into the list of them */
 	if (!base->server_head) {
 		ns->next = ns->prev = ns;
 		base->server_head = ns;
 	} else {
 		ns->next = base->server_head->next;
@@ -3321,14 +3308,17 @@
 {
 	struct sockaddr_in sin;
 	int res;
 	memset(&sin, 0, sizeof(sin));
 	sin.sin_addr.s_addr = address;
 	sin.sin_port = htons(53);
 	sin.sin_family = AF_INET;
+#ifdef EVENT__HAVE_STRUCT_SOCKADDR_IN_SIN_LEN
+	sin.sin_len = sizeof(sin);
+#endif
 	EVDNS_LOCK(base);
 	res = evdns_nameserver_add_impl_(base, (struct sockaddr*)&sin, sizeof(sin));
 	EVDNS_UNLOCK(base);
 	return res;
 }
 
 int
@@ -3426,14 +3416,35 @@
 	memcpy(sa, &server->address, server->addrlen);
 	result = (int) server->addrlen;
 done:
 	EVDNS_UNLOCK(base);
 	return result;
 }
 
+int
+evdns_base_get_nameserver_fd(struct evdns_base *base, int idx)
+{
+	int result = -1;
+	int i;
+	struct nameserver *server;
+	EVDNS_LOCK(base);
+	server = base->server_head;
+	for (i = 0; i < idx && server; ++i, server = server->next) {
+		if (server->next == base->server_head)
+			goto done;
+	}
+	if (! server)
+		goto done;
+	result = server->socket;
+done:
+	EVDNS_UNLOCK(base);
+	return result;
+}
+
+
 /* remove from the queue */
 static void
 evdns_request_remove(struct request *req, struct request **head)
 {
 	ASSERT_LOCKED(req->base);
 	ASSERT_VALID_REQUEST(req);
 
@@ -3493,16 +3504,15 @@
 		count++;
 	}
 	return count;
 }
 
 static struct request *
 request_new(struct evdns_base *base, struct evdns_request *handle, int type,
-	    const char *name, int flags, evdns_callback_type callback,
-	    void *user_ptr) {
+	    const char *name, int flags) {
 
 	const char issuing_now =
 	    (base->global_requests_inflight < base->global_max_requests_inflight) ? 1 : 0;
 
 	const size_t name_len = strlen(name);
 	const size_t request_max_len = evdns_request_len(base, name_len);
 	const u16 trans_id = issuing_now ? transaction_id_pick(base) : 0xffff;
@@ -3553,16 +3563,14 @@
 	if (rlen < 0)
 		goto err1;
 
 	req->request_len = rlen;
 	req->trans_id = trans_id;
 	req->tx_count = 0;
 	req->request_type = type;
-	req->user_pointer = user_ptr;
-	req->user_callback = callback;
 	req->ns = issuing_now ? nameserver_pick(base) : NULL;
 	req->next = req->prev = NULL;
 	req->handle = handle;
 	if (handle) {
 		handle->current_req = req;
 		handle->base = base;
 	}
@@ -3669,26 +3677,26 @@
     evdns_callback_type callback, void *ptr) {
 	struct evdns_request *handle;
 	struct request *req;
 	log(EVDNS_LOG_DEBUG, "Resolve requested for %s", name);
 	handle = mm_calloc(1, sizeof(*handle));
 	if (handle == NULL)
 		return NULL;
+	handle->user_callback = callback;
+	handle->user_pointer = ptr;
 	EVDNS_LOCK(base);
 	handle->tcp_flags = base->global_tcp_flags;
 	handle->tcp_flags |= flags & (DNS_QUERY_USEVC | DNS_QUERY_IGNTC);
 	if (flags & DNS_QUERY_NO_SEARCH) {
 		req =
-			request_new(base, handle, TYPE_A, name, flags,
-				    callback, ptr);
+			request_new(base, handle, TYPE_A, name, flags);
 		if (req)
 			request_submit(req);
 	} else {
-		search_request_new(base, handle, TYPE_A, name, flags,
-		    callback, ptr);
+		search_request_new(base, handle, TYPE_A, name, flags);
 	}
 	if (handle->current_req == NULL) {
 		mm_free(handle);
 		handle = NULL;
 	}
 	EVDNS_UNLOCK(base);
 	return handle;
@@ -3710,25 +3718,25 @@
 {
 	struct evdns_request *handle;
 	struct request *req;
 	log(EVDNS_LOG_DEBUG, "Resolve requested for %s", name);
 	handle = mm_calloc(1, sizeof(*handle));
 	if (handle == NULL)
 		return NULL;
+	handle->user_callback = callback;
+	handle->user_pointer = ptr;
 	EVDNS_LOCK(base);
 	handle->tcp_flags = base->global_tcp_flags;
 	handle->tcp_flags |= flags & (DNS_QUERY_USEVC | DNS_QUERY_IGNTC);
 	if (flags & DNS_QUERY_NO_SEARCH) {
-		req = request_new(base, handle, TYPE_AAAA, name, flags,
-				  callback, ptr);
+		req = request_new(base, handle, TYPE_AAAA, name, flags);
 		if (req)
 			request_submit(req);
 	} else {
-		search_request_new(base, handle, TYPE_AAAA, name, flags,
-		    callback, ptr);
+		search_request_new(base, handle, TYPE_AAAA, name, flags);
 	}
 	if (handle->current_req == NULL) {
 		mm_free(handle);
 		handle = NULL;
 	}
 	EVDNS_UNLOCK(base);
 	return handle;
@@ -3752,19 +3760,21 @@
 			(int)(u8)((a	)&0xff),
 			(int)(u8)((a>>8 )&0xff),
 			(int)(u8)((a>>16)&0xff),
 			(int)(u8)((a>>24)&0xff));
 	handle = mm_calloc(1, sizeof(*handle));
 	if (handle == NULL)
 		return NULL;
+	handle->user_callback = callback;
+	handle->user_pointer = ptr;
 	log(EVDNS_LOG_DEBUG, "Resolve requested for %s (reverse)", buf);
 	EVDNS_LOCK(base);
 	handle->tcp_flags = base->global_tcp_flags;
 	handle->tcp_flags |= flags & (DNS_QUERY_USEVC | DNS_QUERY_IGNTC);
-	req = request_new(base, handle, TYPE_PTR, buf, flags, callback, ptr);
+	req = request_new(base, handle, TYPE_PTR, buf, flags);
 	if (req)
 		request_submit(req);
 	if (handle->current_req == NULL) {
 		mm_free(handle);
 		handle = NULL;
 	}
 	EVDNS_UNLOCK(base);
@@ -3794,19 +3804,21 @@
 		*cp++ = '.';
 	}
 	EVUTIL_ASSERT(cp + strlen("ip6.arpa") < buf+sizeof(buf));
 	memcpy(cp, "ip6.arpa", strlen("ip6.arpa")+1);
 	handle = mm_calloc(1, sizeof(*handle));
 	if (handle == NULL)
 		return NULL;
+	handle->user_callback = callback;
+	handle->user_pointer = ptr;
 	log(EVDNS_LOG_DEBUG, "Resolve requested for %s (reverse)", buf);
 	EVDNS_LOCK(base);
 	handle->tcp_flags = base->global_tcp_flags;
 	handle->tcp_flags |= flags & (DNS_QUERY_USEVC | DNS_QUERY_IGNTC);
-	req = request_new(base, handle, TYPE_PTR, buf, flags, callback, ptr);
+	req = request_new(base, handle, TYPE_PTR, buf, flags);
 	if (req)
 		request_submit(req);
 	if (handle->current_req == NULL) {
 		mm_free(handle);
 		handle = NULL;
 	}
 	EVDNS_UNLOCK(base);
@@ -3952,15 +3964,15 @@
 void
 evdns_search_ndots_set(const int ndots) {
 	evdns_base_search_ndots_set(current_base, ndots);
 }
 
 static void
 search_set_from_hostname(struct evdns_base *base) {
-	char hostname[HOST_NAME_MAX + 1], *domainname;
+	char hostname[EVDNS_NAME_MAX + 1], *domainname;
 
 	ASSERT_LOCKED(base);
 	search_postfix_clear(base);
 	if (gethostname(hostname, sizeof(hostname))) return;
 	domainname = strchr(hostname, '.');
 	if (!domainname) return;
 	search_postfix_add(base, domainname);
@@ -3995,32 +4007,31 @@
 	/* we ran off the end of the list and still didn't find the requested string */
 	EVUTIL_ASSERT(0);
 	return NULL; /* unreachable; stops warnings in some compilers. */
 }
 
 static struct request *
 search_request_new(struct evdns_base *base, struct evdns_request *handle,
-		   int type, const char *const name, int flags,
-		   evdns_callback_type user_callback, void *user_arg) {
+		   int type, const char *const name, int flags) {
 	ASSERT_LOCKED(base);
 	EVUTIL_ASSERT(type == TYPE_A || type == TYPE_AAAA);
 	EVUTIL_ASSERT(handle->current_req == NULL);
 	if ( ((flags & DNS_QUERY_NO_SEARCH) == 0) &&
 	     base->global_search_state &&
 		 base->global_search_state->num_domains) {
 		/* we have some domains to search */
 		struct request *req;
 		if (string_num_dots(name) >= base->global_search_state->ndots) {
-			req = request_new(base, handle, type, name, flags, user_callback, user_arg);
+			req = request_new(base, handle, type, name, flags);
 			if (!req) return NULL;
 			handle->search_index = -1;
 		} else {
 			char *const new_name = search_make_new(base->global_search_state, 0, name);
 			if (!new_name) return NULL;
-			req = request_new(base, handle, type, new_name, flags, user_callback, user_arg);
+			req = request_new(base, handle, type, new_name, flags);
 			mm_free(new_name);
 			if (!req) return NULL;
 			handle->search_index = 0;
 		}
 		EVUTIL_ASSERT(handle->search_origname == NULL);
 		handle->search_origname = mm_strdup(name);
 		if (handle->search_origname == NULL) {
@@ -4031,15 +4042,15 @@
 		}
 		handle->search_state = base->global_search_state;
 		handle->search_flags = flags;
 		base->global_search_state->refcount++;
 		request_submit(req);
 		return req;
 	} else {
-		struct request *const req = request_new(base, handle, type, name, flags, user_callback, user_arg);
+		struct request *const req = request_new(base, handle, type, name, flags);
 		if (!req) return NULL;
 		request_submit(req);
 		return req;
 	}
 }
 
 /* this is called when a request has failed to find a name. We need to check */
@@ -4058,28 +4069,28 @@
 		char *new_name;
 		handle->search_index++;
 		if (handle->search_index >= handle->search_state->num_domains) {
 			/* no more postfixes to try, however we may need to try */
 			/* this name without a postfix */
 			if (string_num_dots(handle->search_origname) < handle->search_state->ndots) {
 				/* yep, we need to try it raw */
-				newreq = request_new(base, NULL, req->request_type, handle->search_origname, handle->search_flags, req->user_callback, req->user_pointer);
+				newreq = request_new(base, NULL, req->request_type, handle->search_origname, handle->search_flags);
 				log(EVDNS_LOG_DEBUG, "Search: trying raw query %s", handle->search_origname);
 				if (newreq) {
 					search_request_finished(handle);
 					goto submit_next;
 				}
 			}
 			return 1;
 		}
 
 		new_name = search_make_new(handle->search_state, handle->search_index, handle->search_origname);
 		if (!new_name) return 1;
 		log(EVDNS_LOG_DEBUG, "Search: now trying %s (%d)", new_name, handle->search_index);
-		newreq = request_new(base, NULL, req->request_type, new_name, handle->search_flags, req->user_callback, req->user_pointer);
+		newreq = request_new(base, NULL, req->request_type, new_name, handle->search_flags);
 		mm_free(new_name);
 		if (!newreq) return 1;
 		goto submit_next;
 	}
 	return 1;
 
 submit_next:
@@ -5417,23 +5428,29 @@
 	 * and then either queue those or return them all. */
 	EVUTIL_ASSERT(type == DNS_IPv4_A || type == DNS_IPv6_AAAA);
 
 	if (type == DNS_IPv4_A) {
 		memset(&sin, 0, sizeof(sin));
 		sin.sin_family = AF_INET;
 		sin.sin_port = htons(data->port);
+#ifdef EVENT__HAVE_STRUCT_SOCKADDR_IN_SIN_LEN
+		sin.sin_len = sizeof(sin);
+#endif
 
 		sa = (struct sockaddr *)&sin;
 		socklen = sizeof(sin);
 		addrlen = 4;
 		addrp = &sin.sin_addr.s_addr;
 	} else {
 		memset(&sin6, 0, sizeof(sin6));
 		sin6.sin6_family = AF_INET6;
 		sin6.sin6_port = htons(data->port);
+#ifdef EVENT__HAVE_STRUCT_SOCKADDR_IN6_SIN6_LEN
+		sin6.sin6_len = sizeof(sin6);
+#endif
 
 		sa = (struct sockaddr *)&sin6;
 		socklen = sizeof(sin6);
 		addrlen = 16;
 		addrp = &sin6.sin6_addr.s6_addr;
 	}
 
@@ -5634,26 +5651,26 @@
 	 * launching those requests. (XXX we don't do that yet.)
 	 */
 
 	EVDNS_LOCK(dns_base);
 
 	if (hints.ai_family != PF_INET6) {
 		log(EVDNS_LOG_DEBUG, "Sending request for %s on ipv4 as %p",
-		    nodename, &data->ipv4_request);
+		    nodename, (void *)&data->ipv4_request);
 
 		data->ipv4_request.r = evdns_base_resolve_ipv4(dns_base,
 		    nodename, 0, evdns_getaddrinfo_gotresolve,
 		    &data->ipv4_request);
 		if (want_cname && data->ipv4_request.r)
 			data->ipv4_request.r->current_req->put_cname_in_ptr =
 			    &data->cname_result;
 	}
 	if (hints.ai_family != PF_INET) {
 		log(EVDNS_LOG_DEBUG, "Sending request for %s on ipv6 as %p",
-		    nodename, &data->ipv6_request);
+		    nodename, (void *)&data->ipv6_request);
 
 		data->ipv6_request.r = evdns_base_resolve_ipv6(dns_base,
 		    nodename, 0, evdns_getaddrinfo_gotresolve,
 		    &data->ipv6_request);
 		if (want_cname && data->ipv6_request.r)
 			data->ipv6_request.r->current_req->put_cname_in_ptr =
 			    &data->cname_result;
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/event-config.h.cmake` & `pvxslibs-1.2.0a1/bundle/libevent/event-config.h.cmake`

 * *Files 0% similar despite different names*

```diff
@@ -95,14 +95,17 @@
 
 /* Define if your system supports the epoll system calls */
 #cmakedefine EVENT__HAVE_EPOLL 1
 
 /* Define to 1 if you have the `epoll_create1' function. */
 #cmakedefine EVENT__HAVE_EPOLL_CREATE1 1
 
+/* Define to 1 if you have the `epoll_pwait2' function. */
+#cmakedefine EVENT__HAVE_EPOLL_PWAIT2 1
+
 /* Define to 1 if you have the `epoll_ctl' function. */
 #cmakedefine EVENT__HAVE_EPOLL_CTL 1
 
 /* Define if your system supports the wepoll module */
 #cmakedefine EVENT__HAVE_WEPOLL 1
 
 /* Define to 1 if you have the `eventfd' function. */
@@ -186,14 +189,17 @@
 
 /* Define to 1 if you have the <memory.h> header file. */
 #cmakedefine EVENT__HAVE_MEMORY_H 1
 
 /* Define to 1 if you have the `mmap' function. */
 #cmakedefine EVENT__HAVE_MMAP 1
 
+/* Define to 1 if you have the `mmap64' function. */
+#cmakedefine EVENT__HAVE_MMAP64 1
+
 /* Define to 1 if you have the `nanosleep' function. */
 #cmakedefine EVENT__HAVE_NANOSLEEP 1
 
 /* Define to 1 if you have the `usleep' function. */
 #cmakedefine EVENT__HAVE_USLEEP 1
 
 /* Define to 1 if you have the <netinet/in6.h> header file. */
@@ -384,14 +390,17 @@
 
 /* Define to 1 if you have the <sys/sysctl.h> header file. */
 #cmakedefine EVENT__HAVE_SYS_SYSCTL_H 1
 
 /* Define to 1 if you have the <sys/timerfd.h> header file. */
 #cmakedefine EVENT__HAVE_SYS_TIMERFD_H 1
 
+/* Define to 1 if you have the <sys/signalfd.h> header file. */
+#cmakedefine EVENT__HAVE_SYS_SIGNALFD_H 1
+
 /* Define to 1 if you have the <sys/time.h> header file. */
 #cmakedefine EVENT__HAVE_SYS_TIME_H 1
 
 /* Define to 1 if you have the <sys/types.h> header file. */
 #cmakedefine EVENT__HAVE_SYS_TYPES_H 1
 
 /* Define to 1 if you have the <sys/uio.h> header file. */
@@ -475,23 +484,23 @@
 
 /* The size of a `short', as computed by sizeof. */
 #define EVENT__SIZEOF_SHORT @EVENT__SIZEOF_SHORT@
 
 /* The size of `size_t', as computed by sizeof. */
 #define EVENT__SIZEOF_SIZE_T @EVENT__SIZEOF_SIZE_T@
 
-/* Define to 1 if you can safely include both <sys/time.h> and <time.h>. */
-#cmakedefine EVENT__TIME_WITH_SYS_TIME 1
-
 /* The size of `socklen_t', as computed by sizeof. */
 #define EVENT__SIZEOF_SOCKLEN_T @EVENT__SIZEOF_SOCKLEN_T@
 
 /* The size of 'void *', as computer by sizeof */
 #define EVENT__SIZEOF_VOID_P @EVENT__SIZEOF_VOID_P@
 
+/* The size of 'time_t', as computer by sizeof */
+#define EVENT__SIZEOF_TIME_T @EVENT__SIZEOF_TIME_T@
+
 /* Define to `__inline__' or `__inline' if that's what the C compiler
    calls it, or to nothing if 'inline' is not supported under any name.  */
 #ifndef __cplusplus
 /* why not c++?
  *
  *  and are we really expected to use EVENT__inline everywhere,
  *  shouldn't we just do:
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/event-internal.h` & `pvxslibs-1.2.0a1/bundle/libevent/event-internal.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/event.c` & `pvxslibs-1.2.0a1/bundle/libevent/event.c`

 * *Files 3% similar despite different names*

```diff
@@ -298,15 +298,15 @@
 	if (dent) {
 		dent->added = 1;
 	} else {
 		event_errx(EVENT_ERR_ABORT_,
 		    "%s: noting an add on a non-setup event %p"
 		    " (events: 0x%x, fd: "EV_SOCK_FMT
 		    ", flags: 0x%x)",
-		    __func__, ev, ev->ev_events,
+		    __func__, (void *)ev, ev->ev_events,
 		    EV_SOCK_ARG(ev->ev_fd), ev->ev_flags);
 	}
 	EVLOCK_UNLOCK(event_debug_map_lock_, 0);
 
 out:
 	event_debug_mode_too_late = 1;
 }
@@ -324,15 +324,15 @@
 	if (dent) {
 		dent->added = 0;
 	} else {
 		event_errx(EVENT_ERR_ABORT_,
 		    "%s: noting a del on a non-setup event %p"
 		    " (events: 0x%x, fd: "EV_SOCK_FMT
 		    ", flags: 0x%x)",
-		    __func__, ev, ev->ev_events,
+		    __func__, (void *)ev, ev->ev_events,
 		    EV_SOCK_ARG(ev->ev_fd), ev->ev_flags);
 	}
 	EVLOCK_UNLOCK(event_debug_map_lock_, 0);
 
 out:
 	event_debug_mode_too_late = 1;
 }
@@ -348,15 +348,15 @@
 	EVLOCK_LOCK(event_debug_map_lock_, 0);
 	dent = HT_FIND(event_debug_map, &global_debug_map, &find);
 	if (!dent) {
 		event_errx(EVENT_ERR_ABORT_,
 		    "%s called on a non-initialized event %p"
 		    " (events: 0x%x, fd: "EV_SOCK_FMT
 		    ", flags: 0x%x)",
-		    __func__, ev, ev->ev_events,
+		    __func__, (void *)ev, ev->ev_events,
 		    EV_SOCK_ARG(ev->ev_fd), ev->ev_flags);
 	}
 	EVLOCK_UNLOCK(event_debug_map_lock_, 0);
 }
 /* assert that ev is not added (i.e., okay to tear down or set up again) */
 static void event_debug_assert_not_added_(const struct event *ev)
 {
@@ -369,15 +369,15 @@
 	EVLOCK_LOCK(event_debug_map_lock_, 0);
 	dent = HT_FIND(event_debug_map, &global_debug_map, &find);
 	if (dent && dent->added) {
 		event_errx(EVENT_ERR_ABORT_,
 		    "%s called on an already added event %p"
 		    " (events: 0x%x, fd: "EV_SOCK_FMT", "
 		    "flags: 0x%x)",
-		    __func__, ev, ev->ev_events,
+		    __func__, (void *)ev, ev->ev_events,
 		    EV_SOCK_ARG(ev->ev_fd), ev->ev_flags);
 	}
 	EVLOCK_UNLOCK(event_debug_map_lock_, 0);
 }
 static void event_debug_assert_socket_nonblocking_(evutil_socket_t fd)
 {
 	if (!event_debug_mode_on_)
@@ -1371,14 +1371,23 @@
 	return (base->virtual_event_count > 0 || base->event_count > 0);
 }
 
 /* "closure" function called when processing active signal events */
 static inline void
 event_signal_closure(struct event_base *base, struct event *ev)
 {
+#if defined(__clang__)
+#elif defined(__GNUC__)
+#pragma GCC diagnostic push
+/* NOTE: it is better to avoid such code all together, by using separate
+ * variable to break the loop in the event structure, but now this code is safe
+ * */
+#pragma GCC diagnostic ignored "-Wdangling-pointer"
+#endif
+
 	short ncalls;
 	int should_break;
 
 	/* Allows deletes to work */
 	ncalls = ev->ev_ncalls;
 	if (ncalls != 0)
 		ev->ev_pncalls = &ncalls;
@@ -1396,14 +1405,19 @@
 
 		if (should_break) {
 			if (ncalls != 0)
 				ev->ev_pncalls = NULL;
 			return;
 		}
 	}
+
+#if defined(__clang__)
+#elif defined(__GNUC__)
+#pragma GCC diagnostic pop
+#endif
 }
 
 /* Common timeouts are special timeouts that are handled as queues rather than
  * in the minheap.  This is more efficient than the minheap if we happen to
  * know that we're going to get several thousands of timeout events all with
  * the same timeout value.
  *
@@ -1669,24 +1683,24 @@
 
 			if (ev->ev_events & EV_PERSIST || ev->ev_flags & EVLIST_FINALIZING)
 				event_queue_remove_active(base, evcb);
 			else
 				event_del_nolock_(ev, EVENT_DEL_NOBLOCK);
 			event_debug((
 			    "event_process_active: event: %p, %s%s%scall %p",
-			    ev,
+			    (void *)ev,
 			    ev->ev_res & EV_READ ? "EV_READ " : " ",
 			    ev->ev_res & EV_WRITE ? "EV_WRITE " : " ",
 			    ev->ev_res & EV_CLOSED ? "EV_CLOSED " : " ",
-			    ev->ev_callback));
+			    (void *)ev->ev_callback));
 		} else {
 			event_queue_remove_active(base, evcb);
 			event_debug(("event_process_active: event_callback %p, "
 				"closure %d, call %p",
-				evcb, evcb->evcb_closure, evcb->evcb_cb_union.evcb_callback));
+				(void *)evcb, evcb->evcb_closure, (void *)evcb->evcb_cb_union.evcb_callback));
 		}
 
 		if (!(evcb->evcb_flags & EVLIST_INTERNAL))
 			++count;
 
 
 		base->current_event = evcb;
@@ -1842,14 +1856,21 @@
 const char *
 event_base_get_method(const struct event_base *base)
 {
 	EVUTIL_ASSERT(base);
 	return (base->evsel->name);
 }
 
+const char *
+event_base_get_signal_method(const struct event_base *base)
+{
+	EVUTIL_ASSERT(base);
+	return (base->evsigsel->name);
+}
+
 /** Callback: used to implement event_base_loopexit by telling the event_base
  * that it's time to exit its loop. */
 static void
 event_loopexit_cb(evutil_socket_t fd, short what, void *arg)
 {
 	struct event_base *base = arg;
 	base->event_gotterm = 1;
@@ -2596,20 +2617,20 @@
 event_remove_timer_nolock_(struct event *ev)
 {
 	struct event_base *base = ev->ev_base;
 
 	EVENT_BASE_ASSERT_LOCKED(base);
 	event_debug_assert_is_setup_(ev);
 
-	event_debug(("event_remove_timer_nolock: event: %p", ev));
+	event_debug(("event_remove_timer_nolock: event: %p", (void *)ev));
 
 	/* If it's not pending on a timeout, we don't need to do anything. */
 	if (ev->ev_flags & EVLIST_TIMEOUT) {
 		event_queue_remove_timeout(base, ev);
-		evutil_timerclear(&ev->ev_.ev_io.ev_timeout);
+		evutil_timerclear(&ev->ev_io_timeout);
 	}
 
 	return (0);
 }
 
 int
 event_remove_timer(struct event *ev)
@@ -2643,21 +2664,21 @@
 	int notify = 0;
 
 	EVENT_BASE_ASSERT_LOCKED(base);
 	event_debug_assert_is_setup_(ev);
 
 	event_debug((
 		 "event_add: event: %p (fd "EV_SOCK_FMT"), %s%s%s%scall %p",
-		 ev,
+		 (void *)ev,
 		 EV_SOCK_ARG(ev->ev_fd),
 		 ev->ev_events & EV_READ ? "EV_READ " : " ",
 		 ev->ev_events & EV_WRITE ? "EV_WRITE " : " ",
 		 ev->ev_events & EV_CLOSED ? "EV_CLOSED " : " ",
 		 tv ? "EV_TIMEOUT " : " ",
-		 ev->ev_callback));
+		 (void *)ev->ev_callback));
 
 	EVUTIL_ASSERT(!(ev->ev_flags & ~EVLIST_ALL));
 
 	if (ev->ev_flags & EVLIST_FINALIZING) {
 		/* XXXX debug */
 		return (-1);
 	}
@@ -2763,15 +2784,15 @@
 			    (tv->tv_usec & ~MICROSECONDS_MASK);
 		} else {
 			evutil_timeradd(&now, tv, &ev->ev_timeout);
 		}
 
 		event_debug((
 			 "event_add: event %p, timeout in %d seconds %d useconds, call %p",
-			 ev, (int)tv->tv_sec, (int)tv->tv_usec, ev->ev_callback));
+			 (void *)ev, (int)tv->tv_sec, (int)tv->tv_usec, (void *)ev->ev_callback));
 
 #ifdef USE_REINSERT_TIMEOUT
 		event_queue_reinsert_timeout(base, ev, was_common, common_timeout, old_timeout_idx);
 #else
 		event_queue_insert_timeout(base, ev);
 #endif
 
@@ -2850,15 +2871,15 @@
 int
 event_del_nolock_(struct event *ev, int blocking)
 {
 	struct event_base *base;
 	int res = 0, notify = 0;
 
 	event_debug(("event_del: %p (fd "EV_SOCK_FMT"), callback %p",
-		ev, EV_SOCK_ARG(ev->ev_fd), ev->ev_callback));
+		(void *)ev, EV_SOCK_ARG(ev->ev_fd), (void *)ev->ev_callback));
 
 	/* An event without a base has not been added */
 	if (ev->ev_base == NULL)
 		return (-1);
 
 	EVENT_BASE_ASSERT_LOCKED(ev->ev_base);
 
@@ -2958,15 +2979,15 @@
 
 void
 event_active_nolock_(struct event *ev, int res, short ncalls)
 {
 	struct event_base *base;
 
 	event_debug(("event_active: %p (fd "EV_SOCK_FMT"), res %d, callback %p",
-		ev, EV_SOCK_ARG(ev->ev_fd), (int)res, ev->ev_callback));
+		(void *)ev, EV_SOCK_ARG(ev->ev_fd), (int)res, (void *)ev->ev_callback));
 
 	base = ev->ev_base;
 	EVENT_BASE_ASSERT_LOCKED(base);
 
 	if (ev->ev_flags & EVLIST_FINALIZING) {
 		/* XXXX debug */
 		return;
@@ -3207,15 +3228,15 @@
 		goto out;
 	}
 
 	evutil_timersub(&ev->ev_timeout, &now, tv);
 
 	EVUTIL_ASSERT(tv->tv_sec >= 0);
 	EVUTIL_ASSERT(tv->tv_usec >= 0);
-	event_debug(("timeout_next: event: %p, in %d seconds, %d useconds", ev, (int)tv->tv_sec, (int)tv->tv_usec));
+	event_debug(("timeout_next: event: %p, in %d seconds, %d useconds", (void *)ev, (int)tv->tv_sec, (int)tv->tv_usec));
 
 out:
 	return (res);
 }
 
 /* Activate every event whose timeout has elapsed. */
 static void
@@ -3235,15 +3256,15 @@
 		if (evutil_timercmp(&ev->ev_timeout, &now, >))
 			break;
 
 		/* delete this event from the I/O queues */
 		event_del_nolock_(ev, EVENT_DEL_NOBLOCK);
 
 		event_debug(("timeout_process: event: %p, call %p",
-			 ev, ev->ev_callback));
+			 (void *)ev, (void *)ev->ev_callback));
 		event_active_nolock_(ev, EV_TIMEOUT, 1);
 	}
 }
 
 #ifndef MAX
 #define MAX(a,b) (((a)>(b))?(a):(b))
 #endif
@@ -3263,27 +3284,27 @@
 
 static void
 event_queue_remove_inserted(struct event_base *base, struct event *ev)
 {
 	EVENT_BASE_ASSERT_LOCKED(base);
 	if (EVUTIL_FAILURE_CHECK(!(ev->ev_flags & EVLIST_INSERTED))) {
 		event_errx(1, "%s: %p(fd "EV_SOCK_FMT") not on queue %x", __func__,
-		    ev, EV_SOCK_ARG(ev->ev_fd), EVLIST_INSERTED);
+                   (void *)ev, EV_SOCK_ARG(ev->ev_fd), EVLIST_INSERTED);
 		return;
 	}
 	DECR_EVENT_COUNT(base, ev->ev_flags);
 	ev->ev_flags &= ~EVLIST_INSERTED;
 }
 static void
 event_queue_remove_active(struct event_base *base, struct event_callback *evcb)
 {
 	EVENT_BASE_ASSERT_LOCKED(base);
 	if (EVUTIL_FAILURE_CHECK(!(evcb->evcb_flags & EVLIST_ACTIVE))) {
 		event_errx(1, "%s: %p not on queue %x", __func__,
-			   evcb, EVLIST_ACTIVE);
+                          (void *)evcb, EVLIST_ACTIVE);
 		return;
 	}
 	DECR_EVENT_COUNT(base, evcb->evcb_flags);
 	evcb->evcb_flags &= ~EVLIST_ACTIVE;
 	base->event_count_active--;
 
 	TAILQ_REMOVE(&base->activequeues[evcb->evcb_pri],
@@ -3291,30 +3312,30 @@
 }
 static void
 event_queue_remove_active_later(struct event_base *base, struct event_callback *evcb)
 {
 	EVENT_BASE_ASSERT_LOCKED(base);
 	if (EVUTIL_FAILURE_CHECK(!(evcb->evcb_flags & EVLIST_ACTIVE_LATER))) {
 		event_errx(1, "%s: %p not on queue %x", __func__,
-			   evcb, EVLIST_ACTIVE_LATER);
+                          (void *)evcb, EVLIST_ACTIVE_LATER);
 		return;
 	}
 	DECR_EVENT_COUNT(base, evcb->evcb_flags);
 	evcb->evcb_flags &= ~EVLIST_ACTIVE_LATER;
 	base->event_count_active--;
 
 	TAILQ_REMOVE(&base->active_later_queue, evcb, evcb_active_next);
 }
 static void
 event_queue_remove_timeout(struct event_base *base, struct event *ev)
 {
 	EVENT_BASE_ASSERT_LOCKED(base);
 	if (EVUTIL_FAILURE_CHECK(!(ev->ev_flags & EVLIST_TIMEOUT))) {
 		event_errx(1, "%s: %p(fd "EV_SOCK_FMT") not on queue %x", __func__,
-		    ev, EV_SOCK_ARG(ev->ev_fd), EVLIST_TIMEOUT);
+                   (void *)ev, EV_SOCK_ARG(ev->ev_fd), EVLIST_TIMEOUT);
 		return;
 	}
 	DECR_EVENT_COUNT(base, ev->ev_flags);
 	ev->ev_flags &= ~EVLIST_TIMEOUT;
 
 	if (is_common_timeout(&ev->ev_timeout, base)) {
 		struct common_timeout_list *ctl =
@@ -3372,15 +3393,15 @@
 insert_common_timeout_inorder(struct common_timeout_list *ctl,
     struct event *ev)
 {
 	struct event *e;
 	/* By all logic, we should just be able to append 'ev' to the end of
 	 * ctl->events, since the timeout on each 'ev' is set to {the common
 	 * timeout} + {the time when we add the event}, and so the events
-	 * should arrive in order of their timeeouts.  But just in case
+	 * should arrive in order of their timeouts.  But just in case
 	 * there's some wacky threading issue going on, we do a search from
 	 * the end of 'ev' to find the right insertion point.
 	 */
 	TAILQ_FOREACH_REVERSE(e, &ctl->events,
 	    event_list, ev_timeout_pos.ev_next_with_common_timeout) {
 		/* This timercmp is a little sneaky, since both ev and e have
 		 * magic values in tv_usec.  Fortunately, they ought to have
@@ -3401,15 +3422,15 @@
 static void
 event_queue_insert_inserted(struct event_base *base, struct event *ev)
 {
 	EVENT_BASE_ASSERT_LOCKED(base);
 
 	if (EVUTIL_FAILURE_CHECK(ev->ev_flags & EVLIST_INSERTED)) {
 		event_errx(1, "%s: %p(fd "EV_SOCK_FMT") already inserted", __func__,
-		    ev, EV_SOCK_ARG(ev->ev_fd));
+                   (void *)ev, EV_SOCK_ARG(ev->ev_fd));
 		return;
 	}
 
 	INCR_EVENT_COUNT(base, ev->ev_flags);
 
 	ev->ev_flags |= EVLIST_INSERTED;
 }
@@ -3455,15 +3476,15 @@
 static void
 event_queue_insert_timeout(struct event_base *base, struct event *ev)
 {
 	EVENT_BASE_ASSERT_LOCKED(base);
 
 	if (EVUTIL_FAILURE_CHECK(ev->ev_flags & EVLIST_TIMEOUT)) {
 		event_errx(1, "%s: %p(fd "EV_SOCK_FMT") already on timeout", __func__,
-		    ev, EV_SOCK_ARG(ev->ev_fd));
+                   (void *)ev, EV_SOCK_ARG(ev->ev_fd));
 		return;
 	}
 
 	INCR_EVENT_COUNT(base, ev->ev_flags);
 
 	ev->ev_flags |= EVLIST_TIMEOUT;
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/event_iocp.c` & `pvxslibs-1.2.0a1/bundle/libevent/event_iocp.c`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/event_tagging.c` & `pvxslibs-1.2.0a1/bundle/libevent/event_tagging.c`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/evmap-internal.h` & `pvxslibs-1.2.0a1/bundle/libevent/evmap-internal.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/evmap.c` & `pvxslibs-1.2.0a1/bundle/libevent/evmap.c`

 * *Files 1% similar despite different names*

```diff
@@ -461,15 +461,15 @@
 			map, sig, sizeof(struct evmap_signal *)) == -1)
 			return (-1);
 	}
 	GET_SIGNAL_SLOT_AND_CTOR(ctx, map, sig, evmap_signal, evmap_signal_init,
 	    base->evsigsel->fdinfo_len);
 
 	if (LIST_EMPTY(&ctx->events)) {
-		if (evsel->add(base, ev->ev_fd, 0, EV_SIGNAL, NULL)
+		if (evsel->add(base, ev->ev_fd, 0, EV_SIGNAL, ev)
 		    == -1)
 			return (-1);
 	}
 
 	LIST_INSERT_HEAD(&ctx->events, ev, ev_signal_next);
 
 	return (1);
@@ -639,15 +639,16 @@
 evmap_signal_reinit_iter_fn(struct event_base *base,
     int signum, struct evmap_signal *ctx, void *arg)
 {
 	const struct eventop *evsel = base->evsigsel;
 	int *result = arg;
 
 	if (!LIST_EMPTY(&ctx->events)) {
-		if (evsel->add(base, signum, 0, EV_SIGNAL, NULL) == -1)
+		if (evsel->add(base, signum, 1, EV_SIGNAL,
+			       LIST_FIRST(&ctx->events)) == -1)
 			*result = -1;
 	}
 	return 0;
 }
 
 int
 evmap_reinit_(struct event_base *base)
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/evport.c` & `pvxslibs-1.2.0a1/bundle/libevent/evport.c`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/evrpc-internal.h` & `pvxslibs-1.2.0a1/bundle/libevent/evrpc-internal.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/evrpc.c` & `pvxslibs-1.2.0a1/bundle/libevent/evrpc.c`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/evsignal-internal.h` & `pvxslibs-1.2.0a1/bundle/libevent/evsignal-internal.h`

 * *Files 19% similar despite different names*

```diff
@@ -41,25 +41,38 @@
 	struct event ev_signal;
 	/* Socketpair used to send notifications from the signal handler */
 	evutil_socket_t ev_signal_pair[2];
 	/* True iff we've added the ev_signal event yet. */
 	int ev_signal_added;
 	/* Count of the number of signals we're currently watching. */
 	int ev_n_signals_added;
+#ifdef EVENT__HAVE_SYS_SIGNALFD_H
+	/* EV_READ events used to wakeup corresponding EV_SIGNAL ones. */
+	struct event *ev_sigevent[NSIG];
+#endif /* EVENT__HAVE_SYS_SIGNALFD_H */
 
 	/* Array of previous signal handler objects before Libevent started
 	 * messing with them.  Used to restore old signal handlers. */
 #ifdef EVENT__HAVE_SIGACTION
 	struct sigaction **sh_old;
 #else
 	ev_sighandler_t **sh_old;
 #endif
 	/* Size of sh_old. */
 	int sh_old_max;
 };
+
+#ifdef EVENT__HAVE_SYS_SIGNALFD_H
+int sigfd_init_(struct event_base *);
+#else /* no signalfd() */
+static inline int
+sigfd_init_(struct event_base *base) { return -1; }
+#endif /* have signalfd() */
+
 int evsig_init_(struct event_base *);
 void evsig_dealloc_(struct event_base *);
+int evsig_ensure_saved_(struct evsig_info *, int);
 
 void evsig_set_base_(struct event_base *base);
 void evsig_free_globals_(void);
 
 #endif /* EVSIGNAL_INTERNAL_H_INCLUDED_ */
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/evthread-internal.h` & `pvxslibs-1.2.0a1/bundle/libevent/evthread-internal.h`

 * *Files 1% similar despite different names*

```diff
@@ -312,16 +312,16 @@
 #define EVLOCK_LOCK(lockvar, mode) EVUTIL_NIL_STMT_
 #define EVLOCK_UNLOCK(lockvar, mode) EVUTIL_NIL_STMT_
 #define EVLOCK_LOCK2(lock1,lock2,mode1,mode2) EVUTIL_NIL_STMT_
 #define EVLOCK_UNLOCK2(lock1,lock2,mode1,mode2) EVUTIL_NIL_STMT_
 
 #define EVBASE_IN_THREAD(base)	1
 #define EVBASE_NEED_NOTIFY(base) 0
-#define EVBASE_ACQUIRE_LOCK(base, lock) EVUTIL_NIL_STMT_
-#define EVBASE_RELEASE_LOCK(base, lock) EVUTIL_NIL_STMT_
+#define EVBASE_ACQUIRE_LOCK(base, lock) (void)(base)
+#define EVBASE_RELEASE_LOCK(base, lock) (void)(base)
 #define EVLOCK_ASSERT_LOCKED(lock) EVUTIL_NIL_STMT_
 
 #define EVLOCK_TRY_LOCK_(lock) 1
 
 #define EVTHREAD_ALLOC_COND(condvar) EVUTIL_NIL_STMT_
 #define EVTHREAD_FREE_COND(cond) EVUTIL_NIL_STMT_
 #define EVTHREAD_COND_SIGNAL(cond) EVUTIL_NIL_STMT_
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/evthread.c` & `pvxslibs-1.2.0a1/bundle/libevent/evthread.c`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/evthread_pthread.c` & `pvxslibs-1.2.0a1/bundle/libevent/evthread_pthread.c`

 * *Files 16% similar despite different names*

```diff
@@ -38,14 +38,17 @@
 #include <string.h>
 #include "mm-internal.h"
 #include "evthread-internal.h"
 
 static pthread_mutexattr_t attr_default;
 static pthread_mutexattr_t attr_recursive;
 
+static pthread_mutex_t once_init_lock = PTHREAD_MUTEX_INITIALIZER;
+static int once_init = 0;
+
 static void *
 evthread_posix_lock_alloc(unsigned locktype)
 {
 	pthread_mutexattr_t *attr = &attr_default;
 	pthread_mutex_t *lock = mm_malloc(sizeof(pthread_mutex_t));
 	if (!lock)
 		return NULL;
@@ -176,39 +179,51 @@
 		EVTHREAD_CONDITION_API_VERSION,
 		evthread_posix_cond_alloc,
 		evthread_posix_cond_free,
 		evthread_posix_cond_signal,
 		evthread_posix_cond_wait
 	};
 
-	if (pthread_mutexattr_init(&attr_default))
-		return -1;
+	pthread_mutex_lock(&once_init_lock);
+	if (once_init == 1) {
+		pthread_mutex_unlock(&once_init_lock);
+		return 0;
+	}
+
+	if (pthread_mutexattr_init(&attr_default)) 
+		goto error;
 
 	/* Set ourselves up to get recursive locks. */
 	if (pthread_mutexattr_init(&attr_recursive))
-		return -1;
+		goto error;
 	if (pthread_mutexattr_settype(&attr_recursive, PTHREAD_MUTEX_RECURSIVE))
-		return -1;
+		goto error;
 
 	if (flags & EVTHREAD_PTHREAD_PRIO_INHERIT) {
 #ifdef EVENT__HAVE_PTHREAD_MUTEXATTR_SETPROTOCOL
 		/* Set up priority inheritance */
 		if (pthread_mutexattr_setprotocol(&attr_default, PTHREAD_PRIO_INHERIT))
-			return -1;
+			goto error;
 		if (pthread_mutexattr_setprotocol(&attr_recursive, PTHREAD_PRIO_INHERIT))
-			return -1;
+			goto error;
 #else
-		return -1;
+		goto error;
 #endif
 	}
 
 	evthread_set_lock_callbacks(&cbs);
 	evthread_set_condition_callbacks(&cond_cbs);
 	evthread_set_id_callback(evthread_posix_get_id);
+	once_init = 1;
+
+	pthread_mutex_unlock(&once_init_lock);
 	return 0;
+error:
+	pthread_mutex_unlock(&once_init_lock);
+	return -1;
 }
 
 int
 evthread_use_pthreads(void)
 {
 	return evthread_use_pthreads_with_flags(0);
 }
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/evthread_win32.c` & `pvxslibs-1.2.0a1/bundle/libevent/evthread_win32.c`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/evutil.c` & `pvxslibs-1.2.0a1/bundle/libevent/evutil.c`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 #include "event2/event-config.h"
 #include "evconfig-private.h"
 
 #ifdef _WIN32
 #include <winsock2.h>
 #include <winerror.h>
 #include <ws2tcpip.h>
+#include <stringapiset.h>
 #ifdef EVENT__HAVE_AFUNIX_H
 #include <afunix.h>
 #endif
 #define WIN32_LEAN_AND_MEAN
 #include <windows.h>
 #undef WIN32_LEAN_AND_MEAN
 #include <io.h>
@@ -208,33 +209,33 @@
 	*content_out = mem;
 	return 0;
 }
 
 #ifdef _WIN32
 
 static int
-create_tmpfile(char tmpfile[MAX_PATH])
+create_tmpfile(WCHAR tmpfile[MAX_PATH])
 {
-	char short_path[MAX_PATH] = {0};
-	char long_path[MAX_PATH] = {0};
-	char prefix[4] = {0};
-	// GetTempFileNameA() uses up to the first three characters of the prefix
+	WCHAR short_path[MAX_PATH] = {0};
+	WCHAR long_path[MAX_PATH] = {0};
+	WCHAR prefix[4] = {0};
+	// GetTempFileNameW() uses up to the first three characters of the prefix
 	// and windows filesystems are case-insensitive
-	const char *base32set = "abcdefghijklmnopqrstuvwxyz012345";
+	const WCHAR *base32set = L"abcdefghijklmnopqrstuvwxyz012345";
 	ev_uint16_t rnd;
 
 	evutil_secure_rng_get_bytes(&rnd, sizeof(rnd));
 	prefix[0] = base32set[(rnd      ) & 31];
 	prefix[1] = base32set[(rnd >>  5) & 31];
 	prefix[2] = base32set[(rnd >> 10) & 31];
 	prefix[3] = '\0';
 
-	GetTempPathA(MAX_PATH, short_path);
-	GetLongPathNameA(short_path, long_path, MAX_PATH);
-	if (!GetTempFileNameA(long_path, prefix, 0, tmpfile)) {
+	GetTempPathW(MAX_PATH, short_path);
+	GetLongPathNameW(short_path, long_path, MAX_PATH);
+	if (!GetTempFileNameW(long_path, prefix, 0, tmpfile)) {
 		event_warnx("GetTempFileName failed: %d", EVUTIL_SOCKET_ERROR());
 		return -1;
 	}
 	return 0;
 }
 
 #ifdef EVENT__HAVE_AFUNIX_H
@@ -267,15 +268,16 @@
 #define ERR(e) WSA##e
 	evutil_socket_t listener = -1;
 	evutil_socket_t connector = -1;
 	evutil_socket_t acceptor = -1;
 
 	struct sockaddr_un listen_addr;
 	struct sockaddr_un connect_addr;
-	char tmp_file[MAX_PATH] = {0};
+	WCHAR tmp_file[MAX_PATH] = {0};
+	char tmp_file_utf8[MAX_PATH] = {0};
 
 	ev_socklen_t size;
 	int saved_errno = -1;
 
 	if (!fd) {
 		EVUTIL_SET_SOCKET_ERROR(ERR(EINVAL));
 		return -1;
@@ -285,17 +287,22 @@
 	if (listener < 0)
 		return -1;
 	memset(&listen_addr, 0, sizeof(listen_addr));
 
 	if (create_tmpfile(tmp_file)) {
 		goto tidy_up_and_fail;
 	}
-	DeleteFileA(tmp_file);
+	DeleteFileW(tmp_file);
+
+	/* Windows requires `sun_path` to be encoded by UTF-8 */
+	WideCharToMultiByte(
+		CP_UTF8, 0, tmp_file, MAX_PATH, tmp_file_utf8, MAX_PATH, NULL, NULL);
+
 	listen_addr.sun_family = AF_UNIX;
-	if (strlcpy(listen_addr.sun_path, tmp_file, UNIX_PATH_MAX) >=
+	if (strlcpy(listen_addr.sun_path, tmp_file_utf8, UNIX_PATH_MAX) >=
 		UNIX_PATH_MAX) {
 		event_warnx("Temp file name is too long");
 		goto tidy_up_and_fail;
 	}
 
 	if (bind(listener, (struct sockaddr *) &listen_addr, sizeof (listen_addr))
 		== -1)
@@ -348,15 +355,15 @@
 	if (listener != -1)
 		evutil_closesocket(listener);
 	if (connector != -1)
 		evutil_closesocket(connector);
 	if (acceptor != -1)
 		evutil_closesocket(acceptor);
 	if (tmp_file[0])
-		DeleteFileA(tmp_file);
+		DeleteFileW(tmp_file);
 
 	EVUTIL_SET_SOCKET_ERROR(saved_errno);
 	return -1;
 #undef ERR
 }
 #endif
 
@@ -1564,14 +1571,22 @@
 		if (!ai_new)
 			return -1;
 		memcpy(ai_new, ai, sizeof(*ai_new));
 		ai->ai_socktype = SOCK_STREAM;
 		ai->ai_protocol = IPPROTO_TCP;
 		ai_new->ai_socktype = SOCK_DGRAM;
 		ai_new->ai_protocol = IPPROTO_UDP;
+		ai_new->ai_flags = EVUTIL_AI_LIBEVENT_ALLOCATED;
+		if (ai_new->ai_canonname != NULL) {
+			ai_new->ai_canonname = mm_strdup(ai_new->ai_canonname);
+			if (ai_new->ai_canonname == NULL) {
+				mm_free(ai_new);
+				return -1;
+			}
+		}
 
 		ai_new->ai_next = ai->ai_next;
 		ai->ai_next = ai_new;
 	}
 	return 0;
 }
 #endif
@@ -1767,26 +1782,49 @@
 #endif
 }
 
 void
 evutil_freeaddrinfo(struct evutil_addrinfo *ai)
 {
 #ifdef EVENT__HAVE_GETADDRINFO
-	if (!(ai->ai_flags & EVUTIL_AI_LIBEVENT_ALLOCATED)) {
-		freeaddrinfo(ai);
-		return;
+	struct evutil_addrinfo *ai_prev = NULL;
+	struct evutil_addrinfo *ai_temp = ai;
+	/* Linked list may be the result of a native getaddrinfo() call plus
+	 * locally allocated nodes, Before releasing it using freeaddrinfo(),
+	 * these custom structs need to be freed separately.
+	 */
+	while (ai_temp) {
+		struct evutil_addrinfo *next = ai_temp->ai_next;
+		if (ai_temp->ai_flags & EVUTIL_AI_LIBEVENT_ALLOCATED) {
+			/* Remove this node from the linked list */
+			if (ai_temp->ai_canonname)
+				mm_free(ai_temp->ai_canonname);
+			mm_free(ai_temp);
+			if (ai_prev == NULL) {
+				ai = next;
+			} else {
+				ai_prev->ai_next = next;
+			}
+
+		} else {
+			ai_prev = ai_temp;
+		}
+		ai_temp = next;
 	}
-#endif
+	if (ai != NULL)
+		freeaddrinfo(ai);
+#else
 	while (ai) {
 		struct evutil_addrinfo *next = ai->ai_next;
 		if (ai->ai_canonname)
 			mm_free(ai->ai_canonname);
 		mm_free(ai);
 		ai = next;
 	}
+#endif
 }
 
 static evdns_getaddrinfo_fn evdns_getaddrinfo_impl = NULL;
 static evdns_getaddrinfo_cancel_fn evdns_getaddrinfo_cancel_impl = NULL;
 
 void
 evutil_set_evdns_getaddrinfo_fn_(evdns_getaddrinfo_fn fn)
@@ -2206,15 +2244,17 @@
 	if (if_index == 0) {
 		/* Could be numeric */
 		if_index = strtoul(cp + 1, &check, 10);
 		if (check[0] != '\0')
 			return 0;
 	}
 	*indexp = if_index;
-	tmp_src = mm_strdup(src);
+	if (!(tmp_src = mm_strdup(src))) {
+		return -1;
+	}
 	cp = strchr(tmp_src, '%');
 	*cp = '\0';
 	r = evutil_inet_pton(af, tmp_src, dst);
 	free(tmp_src);
 	return r;
 }
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/evutil_rand.c` & `pvxslibs-1.2.0a1/bundle/libevent/evutil_rand.c`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/evutil_time.c` & `pvxslibs-1.2.0a1/bundle/libevent/evutil_time.c`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/ht-internal.h` & `pvxslibs-1.2.0a1/bundle/libevent/ht-internal.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/http-internal.h` & `pvxslibs-1.2.0a1/bundle/libevent/http-internal.h`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,17 @@
 
 	char *bind_address;		/* address to use for binding the src */
 	ev_uint16_t bind_port;		/* local port for binding the src */
 
 	char *address;			/* address to connect to */
 	ev_uint16_t port;
 
+#ifndef _WIN32
+	char *unixsocket;
+#endif
 	size_t max_headers_size;
 	ev_uint64_t max_body_size;
 
 	int flags;
 #define EVHTTP_CON_INCOMING	0x0001       /* only one request on it ever */
 #define EVHTTP_CON_OUTGOING	0x0002       /* multiple requests possible */
 #define EVHTTP_CON_CLOSEDETECT	0x0004   /* detecting if persistent close */
@@ -117,18 +120,25 @@
 	void (*cb)(struct evhttp_request *req, void *);
 	void *cbarg;
 };
 
 /* both the http server as well as the rpc system need to queue connections */
 TAILQ_HEAD(evconq, evhttp_connection);
 
+/* WebSockets connections */
+TAILQ_HEAD(evwsq, evws_connection);
+
 /* each bound socket is stored in one of these */
 struct evhttp_bound_socket {
 	TAILQ_ENTRY(evhttp_bound_socket) next;
 
+	struct evhttp *http;
+	struct bufferevent* (*bevcb)(struct event_base *, void *);
+	void *bevcbarg;
+
 	struct evconnlistener *listener;
 };
 
 /* server alias list item. */
 struct evhttp_server_alias {
 	TAILQ_ENTRY(evhttp_server_alias) next;
 
@@ -140,16 +150,18 @@
 	TAILQ_ENTRY(evhttp) next_vhost;
 
 	/* All listeners for this host */
 	TAILQ_HEAD(boundq, evhttp_bound_socket) sockets;
 
 	TAILQ_HEAD(httpcbq, evhttp_cb) callbacks;
 
-	/* All live connections on this host. */
+	/* All live HTTP connections on this host. */
 	struct evconq connections;
+	/* All live WebSockets sessions on this host. */
+	struct evwsq ws_sessions;
 	int connection_max;
 	int connection_cnt;
 
 	TAILQ_HEAD(vhostsq, evhttp) virtualhosts;
 
 	TAILQ_HEAD(aliasq, evhttp_server_alias) aliases;
 
@@ -210,14 +222,16 @@
 void evhttp_start_read_(struct evhttp_connection *);
 void evhttp_start_write_(struct evhttp_connection *);
 
 /* response sending HTML the data in the buffer */
 void evhttp_response_code_(struct evhttp_request *, int, const char *);
 void evhttp_send_page_(struct evhttp_request *, struct evbuffer *);
 
+struct bufferevent * evhttp_start_ws_(struct evhttp_request *req);
+
 /* [] has been stripped */
 #define _EVHTTP_URI_HOST_HAS_BRACKETS 0x02
 
 EVENT2_EXPORT_SYMBOL
 int evhttp_decode_uri_internal(const char *uri, size_t length,
     char *ret, int decode_plus);
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/http.c` & `pvxslibs-1.2.0a1/bundle/libevent/http.c`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,16 @@
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF
  * THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 #include "event2/event-config.h"
 #include "evconfig-private.h"
 
+#define member_size(type, member) sizeof(((type *)0)->member)
+
 #ifdef EVENT__HAVE_SYS_PARAM_H
 #include <sys/param.h>
 #endif
 #ifdef EVENT__HAVE_SYS_TYPES_H
 #include <sys/types.h>
 #endif
 
@@ -101,14 +103,15 @@
 #include "event2/http.h"
 #include "event2/event.h"
 #include "event2/buffer.h"
 #include "event2/bufferevent.h"
 #include "event2/http_struct.h"
 #include "event2/http_compat.h"
 #include "event2/util.h"
+#include "event2/ws.h"
 #include "event2/listener.h"
 #include "log-internal.h"
 #include "util-internal.h"
 #include "http-internal.h"
 #include "mm-internal.h"
 #include "bufferevent-internal.h"
 
@@ -191,15 +194,15 @@
 static void evhttp_read_firstline(struct evhttp_connection *evcon,
 				  struct evhttp_request *req);
 static void evhttp_read_header(struct evhttp_connection *evcon,
     struct evhttp_request *req);
 static int evhttp_add_header_internal(struct evkeyvalq *headers,
     const char *key, const char *value);
 static const char *evhttp_response_phrase_internal(int code);
-static void evhttp_get_request(struct evhttp *, evutil_socket_t, struct sockaddr *, ev_socklen_t);
+static void evhttp_get_request(struct evhttp *, evutil_socket_t, struct sockaddr *, ev_socklen_t, struct bufferevent *bev);
 static void evhttp_write_buffer(struct evhttp_connection *,
     void (*)(struct evhttp_connection *, void *), void *);
 static void evhttp_make_header(struct evhttp_connection *, struct evhttp_request *);
 static int evhttp_method_may_have_body_(struct evhttp_connection *, enum evhttp_cmd_type);
 
 /* callbacks for bufferevent */
 static void evhttp_read_cb(struct bufferevent *, void *);
@@ -494,15 +497,16 @@
  * connection's output buffer.
  */
 static void
 evhttp_make_header_request(struct evhttp_connection *evcon,
     struct evhttp_request *req)
 {
 	const char *method;
-	ev_uint16_t flags;
+	/* NOTE: some version of GCC reports a warning that flags may be uninitialized, hence assignment */
+	ev_uint16_t flags = 0;
 
 	evhttp_remove_header(req->output_headers, "Proxy-Connection");
 
 	/* Generate request line */
 	if (!(method = evhttp_method_(evcon, req->type, &flags))) {
 		method = "NULL";
 	}
@@ -733,15 +737,15 @@
 	case EVREQ_HTTP_EOF:
 		/*
 		 * these are cases in which we probably should just
 		 * close the connection and not send a reply.  this
 		 * case may happen when a browser keeps a persistent
 		 * connection open and we timeout on the read.  when
 		 * the request is still being used for sending, we
-		 * need to disassociated it from the connection here.
+		 * need to disassociate it from the connection here.
 		 */
 		if (!req->userdone) {
 			/* remove it so that it will not be freed */
 			TAILQ_REMOVE(&req->evcon->requests, req, next);
 			/* indicate that this request no longer has a
 			 * connection object
 			 */
@@ -1350,14 +1354,19 @@
 
 	if (evcon->bind_address != NULL)
 		mm_free(evcon->bind_address);
 
 	if (evcon->address != NULL)
 		mm_free(evcon->address);
 
+#ifndef _WIN32
+	if (evcon->unixsocket != NULL)
+		mm_free(evcon->unixsocket);
+#endif
+
 	mm_free(evcon);
 }
 
 void
 evhttp_connection_free_on_completion(struct evhttp_connection *evcon) {
 	evcon->flags |= EVHTTP_CON_AUTOFREE;
 }
@@ -1730,15 +1739,15 @@
 evhttp_parse_http_version(const char *version, struct evhttp_request *req)
 {
 	int major, minor;
 	char ch;
 	int n = sscanf(version, "HTTP/%d.%d%c", &major, &minor, &ch);
 	if (n != 2 || major > 1) {
 		event_debug(("%s: bad version %s on message %p from %s",
-			__func__, version, req, req->remote_host));
+			__func__, version, (void *)req, req->remote_host));
 		return (-1);
 	}
 	req->major = major;
 	req->minor = minor;
 	return (0);
 }
 
@@ -2002,15 +2011,15 @@
 			}
 			type = ext_method.type;
 		}
 	}
 
 	if (!type) {
 		event_debug(("%s: bad method %s on request %p from %s",
-		            __func__, method, req, req->remote_host));
+		            __func__, method, (void *)req, req->remote_host));
 		/* No error yet; we'll give a better error later when
 		 * we see that req->type is unsupported. */
 	}
 
 	req->type = type;
 
 	if (evhttp_parse_http_version(version, req) < 0)
@@ -2340,15 +2349,16 @@
 
 	return (0);
 }
 
 static int
 evhttp_method_may_have_body_(struct evhttp_connection *evcon, enum evhttp_cmd_type type)
 {
-	ev_uint16_t flags;
+	/* NOTE: some version of GCC reports a warning that flags may be uninitialized, hence assignment */
+	ev_uint16_t flags = 0;
 	evhttp_method_(evcon, type, &flags);
 	return (flags & EVHTTP_METHOD_HAS_BODY) ? 1 : 0;
 }
 
 static void
 evhttp_get_body(struct evhttp_connection *evcon, struct evhttp_request *req)
 {
@@ -2509,44 +2519,34 @@
 
 struct evhttp_connection *
 evhttp_connection_new(const char *address, ev_uint16_t port)
 {
 	return (evhttp_connection_base_new(NULL, NULL, address, port));
 }
 
-struct evhttp_connection *
-evhttp_connection_base_bufferevent_new(struct event_base *base, struct evdns_base *dnsbase, struct bufferevent* bev,
-    const char *address, ev_uint16_t port)
+static struct evhttp_connection *
+evhttp_connection_new_(struct event_base *base, struct bufferevent* bev)
 {
-	struct evhttp_connection *evcon = NULL;
-
-	event_debug(("Attempting connection to %s:%d\n", address, port));
+	struct evhttp_connection *evcon;
 
 	if ((evcon = mm_calloc(1, sizeof(struct evhttp_connection))) == NULL) {
 		event_warn("%s: calloc failed", __func__);
 		goto error;
 	}
 
-	evcon->port = port;
-
 	evcon->max_headers_size = EV_SIZE_MAX;
 	evcon->max_body_size = EV_SIZE_MAX;
 
 	evcon->timeout_connect.tv_sec = HTTP_CONNECT_TIMEOUT;
 	evcon->timeout_read.tv_sec    = HTTP_READ_TIMEOUT;
 	evcon->timeout_write.tv_sec   = HTTP_WRITE_TIMEOUT;
 	evcon->initial_retry_timeout.tv_sec = HTTP_INITIAL_RETRY_TIMEOUT;
 
 	evcon->retry_cnt = evcon->retry_max = 0;
 
-	if ((evcon->address = mm_strdup(address)) == NULL) {
-		event_warn("%s: strdup failed", __func__);
-		goto error;
-	}
-
 	if (bev == NULL) {
 		if (!(bev = bufferevent_socket_new(base, -1, BEV_OPT_CLOSE_ON_FREE))) {
 			event_warn("%s: bufferevent_socket_new failed", __func__);
 			goto error;
 		}
 	}
 
@@ -2563,25 +2563,81 @@
 	}
 
 	event_deferred_cb_init_(
 	    &evcon->read_more_deferred_cb,
 	    bufferevent_get_priority(bev),
 	    evhttp_deferred_read_cb, evcon);
 
-	evcon->dns_base = dnsbase;
 	evcon->ai_family = AF_UNSPEC;
 
 	return (evcon);
 
  error:
 	if (evcon != NULL)
 		evhttp_connection_free(evcon);
 	return (NULL);
 }
 
+#ifndef _WIN32
+struct evhttp_connection *
+evhttp_connection_base_bufferevent_unix_new(struct event_base *base, struct bufferevent* bev, const char *unixsocket)
+{
+	struct evhttp_connection *evcon;
+
+	if (strlen(unixsocket) >= member_size(struct sockaddr_un, sun_path)) {
+		event_warn("%s: unix socket too long", __func__);
+		return NULL;
+	}
+
+	evcon = evhttp_connection_new_(base, bev);
+	if (evcon == NULL)
+		goto error;
+
+	if ((evcon->unixsocket = mm_strdup(unixsocket)) == NULL) {
+		event_warn("%s: strdup failed", __func__);
+		goto error;
+	}
+
+	evcon->ai_family = AF_UNIX;
+
+	return (evcon);
+ error:
+	if (evcon != NULL)
+		evhttp_connection_free(evcon);
+	return (NULL);
+}
+#endif
+
+struct evhttp_connection *
+evhttp_connection_base_bufferevent_new(struct event_base *base, struct evdns_base *dnsbase, struct bufferevent* bev,
+    const char *address, unsigned short port)
+{
+	struct evhttp_connection *evcon;
+
+	event_debug(("Attempting connection to %s:%d\n", address, port));
+
+	evcon = evhttp_connection_new_(base, bev);
+	if (evcon == NULL)
+		goto error;
+
+	if ((evcon->address = mm_strdup(address)) == NULL) {
+		event_warn("%s: strdup failed", __func__);
+		goto error;
+	}
+	evcon->port = port;
+	evcon->dns_base = dnsbase;
+
+	return (evcon);
+error:
+	if (evcon != NULL)
+		evhttp_connection_free(evcon);
+	return (NULL);
+}
+
+
 struct bufferevent* evhttp_connection_get_bufferevent(struct evhttp_connection *evcon)
 {
 	return evcon->bufev;
 }
 
 struct evhttp *
 evhttp_connection_get_server(struct evhttp_connection *evcon)
@@ -2788,15 +2844,24 @@
 		sa &&
 		(sa->sa_family == AF_INET || sa->sa_family == AF_INET6)) {
 		int socklen = sizeof(struct sockaddr_in);
 		if (sa->sa_family == AF_INET6) {
 			socklen = sizeof(struct sockaddr_in6);
 		}
 		ret = bufferevent_socket_connect(evcon->bufev, sa, socklen);
-	} else {
+	}
+#ifndef _WIN32
+	else if (evcon->unixsocket) {
+		struct sockaddr_un sockaddr;
+		sockaddr.sun_family = AF_UNIX;
+		strcpy(sockaddr.sun_path, evcon->unixsocket);
+		ret = bufferevent_socket_connect(evcon->bufev, (const struct sockaddr*)&sockaddr, sizeof(sockaddr));
+	}
+#endif
+	else {
 		ret = bufferevent_socket_connect_hostname(evcon->bufev,
 				evcon->dns_base, evcon->ai_family, address, evcon->port);
 	}
 
 	if (ret < 0) {
 		evcon->state = old_state;
 		event_sock_warn(bufferevent_getfd(evcon->bufev), "%s: connection to \"%s\" failed",
@@ -3123,14 +3188,39 @@
 	evbuffer_add_buffer(output, databuf);
 	if (req->chunked) {
 		evbuffer_add(output, "\r\n", 2);
 	}
 	evhttp_write_buffer(evcon, cb, arg);
 }
 
+struct bufferevent *
+evhttp_start_ws_(struct evhttp_request *req)
+{
+	struct evhttp_connection *evcon = req->evcon;
+	struct bufferevent *bufev;
+
+	evhttp_response_code_(req, HTTP_SWITCH_PROTOCOLS, "Switching Protocols");
+
+	if (req->evcon == NULL)
+		return NULL;
+
+	evhttp_make_header(req->evcon, req);
+	evhttp_write_buffer(req->evcon, NULL, NULL);
+
+	TAILQ_REMOVE(&evcon->requests, req, next);
+
+	bufev = evcon->bufev;
+	evcon->bufev = NULL;
+	evcon->closecb = NULL;
+
+	evhttp_request_free(req);
+	evhttp_connection_free(evcon);
+	return bufev;
+}
+
 void
 evhttp_send_reply_chunk(struct evhttp_request *req, struct evbuffer *databuf)
 {
 	evhttp_send_reply_chunk_with_cb(req, databuf, NULL, NULL);
 }
 void
 evhttp_send_reply_end(struct evhttp_request *req)
@@ -3727,17 +3817,23 @@
 		evhttp_send_notfound(req, NULL);
 }
 
 /* Listener callback when a connection arrives at a server. */
 static void
 accept_socket_cb(struct evconnlistener *listener, evutil_socket_t nfd, struct sockaddr *peer_sa, int peer_socklen, void *arg)
 {
-	struct evhttp *http = arg;
+	struct evhttp_bound_socket *bound = arg;
 
-	evhttp_get_request(http, nfd, peer_sa, peer_socklen);
+	struct evhttp *http = bound->http;
+
+	struct bufferevent *bev = NULL;
+	if (bound->bevcb)
+		bev = bound->bevcb(http->base, bound->bevcbarg);
+
+	evhttp_get_request(http, nfd, peer_sa, peer_socklen, bev);
 }
 
 int
 evhttp_bind_socket(struct evhttp *http, const char *address, ev_uint16_t port)
 {
 	struct evhttp_bound_socket *bound =
 		evhttp_bind_socket_with_handle(http, address, port);
@@ -3825,17 +3921,19 @@
 	struct evhttp_bound_socket *bound;
 
 	bound = mm_malloc(sizeof(struct evhttp_bound_socket));
 	if (bound == NULL)
 		return (NULL);
 
 	bound->listener = listener;
+	bound->bevcb = NULL;
+	bound->http = http;
 	TAILQ_INSERT_TAIL(&http->sockets, bound, next);
 
-	evconnlistener_set_cb(listener, accept_socket_cb, http);
+	evconnlistener_set_cb(listener, accept_socket_cb, bound);
 	return bound;
 }
 
 evutil_socket_t
 evhttp_bound_socket_get_fd(struct evhttp_bound_socket *bound)
 {
 	return evconnlistener_get_fd(bound->listener);
@@ -3844,14 +3942,22 @@
 struct evconnlistener *
 evhttp_bound_socket_get_listener(struct evhttp_bound_socket *bound)
 {
 	return bound->listener;
 }
 
 void
+evhttp_bound_set_bevcb(struct evhttp_bound_socket *bound,
+    struct bufferevent* (*cb)(struct event_base *, void *), void *cbarg)
+{
+	bound->bevcb = cb;
+	bound->bevcbarg = cbarg;
+}
+
+void
 evhttp_del_accept_socket(struct evhttp *http, struct evhttp_bound_socket *bound)
 {
 	TAILQ_REMOVE(&http->sockets, bound, next);
 	evconnlistener_free(bound->listener);
 	mm_free(bound);
 }
 
@@ -3877,14 +3983,15 @@
 	    EVHTTP_REQ_HEAD |
 	    EVHTTP_REQ_PUT |
 	    EVHTTP_REQ_DELETE);
 
 	TAILQ_INIT(&http->sockets);
 	TAILQ_INIT(&http->callbacks);
 	TAILQ_INIT(&http->connections);
+	TAILQ_INIT(&http->ws_sessions);
 	TAILQ_INIT(&http->virtualhosts);
 	TAILQ_INIT(&http->aliases);
 
 	return (http);
 }
 
 struct evhttp *
@@ -3921,14 +4028,15 @@
 }
 
 void
 evhttp_free(struct evhttp* http)
 {
 	struct evhttp_cb *http_cb;
 	struct evhttp_connection *evcon;
+	struct evws_connection *evws;
 	struct evhttp_bound_socket *bound;
 	struct evhttp* vhost;
 	struct evhttp_server_alias *alias;
 
 	/* Remove the accepting part */
 	while ((bound = TAILQ_FIRST(&http->sockets)) != NULL) {
 		TAILQ_REMOVE(&http->sockets, bound, next);
@@ -3939,14 +4047,18 @@
 	}
 
 	while ((evcon = TAILQ_FIRST(&http->connections)) != NULL) {
 		/* evhttp_connection_free removes the connection */
 		evhttp_connection_free(evcon);
 	}
 
+	while ((evws = TAILQ_FIRST(&http->ws_sessions)) != NULL) {
+		evws_connection_free(evws);
+	}
+
 	while ((http_cb = TAILQ_FIRST(&http->callbacks)) != NULL) {
 		TAILQ_REMOVE(&http->callbacks, http_cb, next);
 		mm_free(http_cb->what);
 		mm_free(http_cb);
 	}
 
 	while ((vhost = TAILQ_FIRST(&http->virtualhosts)) != NULL) {
@@ -4349,23 +4461,23 @@
 /*
  * Allows for inspection of the request URI
  */
 
 const char *
 evhttp_request_get_uri(const struct evhttp_request *req) {
 	if (req->uri == NULL)
-		event_debug(("%s: request %p has no uri\n", __func__, req));
+		event_debug(("%s: request %p has no uri\n", __func__, (void *)req));
 	return (req->uri);
 }
 
 const struct evhttp_uri *
 evhttp_request_get_evhttp_uri(const struct evhttp_request *req) {
 	if (req->uri_elems == NULL)
 		event_debug(("%s: request %p has no uri elems\n",
-			    __func__, req));
+			    __func__, (void *)req));
 	return (req->uri_elems);
 }
 
 const char *
 evhttp_request_get_host(struct evhttp_request *req)
 {
 	const char *host = NULL;
@@ -4449,45 +4561,65 @@
  * Takes a file descriptor to read a request from.
  * The callback is executed once the whole request has been read.
  */
 
 static struct evhttp_connection*
 evhttp_get_request_connection(
 	struct evhttp* http,
-	evutil_socket_t fd, struct sockaddr *sa, ev_socklen_t salen)
+	evutil_socket_t fd, struct sockaddr *sa, ev_socklen_t salen,
+	struct bufferevent* bev)
 {
 	struct evhttp_connection *evcon;
-	char *hostname = NULL, *portname = NULL;
-	struct bufferevent* bev = NULL;
 
 #ifdef EVENT__HAVE_STRUCT_SOCKADDR_UN
 	if (sa->sa_family == AF_UNIX) {
 		struct sockaddr_un *sa_un = (struct sockaddr_un *)sa;
 		sa_un->sun_path[0] = '\0';
 	}
 #endif
 
-	name_from_addr(sa, salen, &hostname, &portname);
-	if (hostname == NULL || portname == NULL) {
-		if (hostname) mm_free(hostname);
-		if (portname) mm_free(portname);
-		return (NULL);
+#ifndef _WIN32
+	if (sa->sa_family == AF_UNIX) {
+		struct sockaddr_un *sockaddr = (struct sockaddr_un *)sa;
+
+		event_debug(("%s: new request from unix socket on "
+			EV_SOCK_FMT"\n", __func__, EV_SOCK_ARG(fd)));
+
+		/* we need a connection object to put the http request on */
+		if (!bev && http->bevcb != NULL) {
+			bev = (*http->bevcb)(http->base, http->bevcbarg);
+		}
+
+		evcon = evhttp_connection_base_bufferevent_unix_new(http->base,
+			bev, sockaddr->sun_path);
 	}
+	else
+#endif
+	{
+		char *hostname = NULL, *portname = NULL;
+
+		name_from_addr(sa, salen, &hostname, &portname);
+		if (hostname == NULL || portname == NULL) {
+			if (hostname) mm_free(hostname);
+			if (portname) mm_free(portname);
+			return (NULL);
+		}
 
-	event_debug(("%s: new request from %s:%s on "EV_SOCK_FMT"\n",
-		__func__, hostname, portname, EV_SOCK_ARG(fd)));
+		event_debug(("%s: new request from %s:%s on "EV_SOCK_FMT"\n",
+			__func__, hostname, portname, EV_SOCK_ARG(fd)));
 
-	/* we need a connection object to put the http request on */
-	if (http->bevcb != NULL) {
-		bev = (*http->bevcb)(http->base, http->bevcbarg);
-	}
-	evcon = evhttp_connection_base_bufferevent_new(
-		http->base, NULL, bev, hostname, atoi(portname));
-	mm_free(hostname);
-	mm_free(portname);
+		/* we need a connection object to put the http request on */
+		if (!bev && http->bevcb != NULL) {
+			bev = (*http->bevcb)(http->base, http->bevcbarg);
+		}
+		evcon = evhttp_connection_base_bufferevent_new(
+			http->base, NULL, bev, hostname, atoi(portname));
+		mm_free(hostname);
+		mm_free(portname);
+	}
 	if (evcon == NULL)
 		return (NULL);
 
 	evcon->max_headers_size = http->default_max_headers_size;
 	evcon->max_body_size = http->default_max_body_size;
 	if (http->flags & EVHTTP_SERVER_LINGERING_CLOSE)
 		evcon->flags |= EVHTTP_CON_LINGERING_CLOSE;
@@ -4514,18 +4646,20 @@
 evhttp_associate_new_request_with_connection(struct evhttp_connection *evcon)
 {
 	struct evhttp *http = evcon->http_server;
 	struct evhttp_request *req;
 	if ((req = evhttp_request_new(evhttp_handle_request, http)) == NULL)
 		return (-1);
 
-	if ((req->remote_host = mm_strdup(evcon->address)) == NULL) {
-		event_warn("%s: strdup", __func__);
-		evhttp_request_free(req);
-		return (-1);
+	if (evcon->address != NULL) {
+		if ((req->remote_host = mm_strdup(evcon->address)) == NULL) {
+			event_warn("%s: strdup", __func__);
+			evhttp_request_free(req);
+			return (-1);
+		}
 	}
 	req->remote_port = evcon->port;
 
 	req->evcon = evcon;	/* the request ends up owning the connection */
 	req->flags |= EVHTTP_REQ_OWN_CONNECTION;
 
 	/* We did not present the request to the user yet, so treat it
@@ -4546,19 +4680,20 @@
 	evhttp_start_read_(evcon);
 
 	return (0);
 }
 
 static void
 evhttp_get_request(struct evhttp *http, evutil_socket_t fd,
-    struct sockaddr *sa, ev_socklen_t salen)
+    struct sockaddr *sa, ev_socklen_t salen,
+    struct bufferevent *bev)
 {
 	struct evhttp_connection *evcon;
 
-	evcon = evhttp_get_request_connection(http, fd, sa, salen);
+	evcon = evhttp_get_request_connection(http, fd, sa, salen, bev);
 	if (evcon == NULL) {
 		event_sock_warn(fd, "%s: cannot get connection on "EV_SOCK_FMT,
 		    __func__, EV_SOCK_ARG(fd));
 		evutil_closesocket(fd);
 		return;
 	}
 
@@ -4735,14 +4870,17 @@
 
 struct evhttp_uri {
 	unsigned flags;
 	char *scheme; /* scheme; e.g http, ftp etc */
 	char *userinfo; /* userinfo (typically username:pass), or NULL */
 	char *host; /* hostname, IP address, or NULL */
 	int port; /* port, or zero */
+#ifndef _WIN32
+	char *unixsocket; /* unix domain socket or NULL */
+#endif
 	char *path; /* path, or "". */
 	char *query; /* query, or NULL */
 	char *fragment; /* fragment or NULL */
 };
 
 struct evhttp_uri *
 evhttp_uri_new(void)
@@ -4906,14 +5044,28 @@
 		if (uri->userinfo == NULL) {
 			event_warn("%s: strdup", __func__);
 			return -1;
 		}
 	} else {
 		cp = s;
 	}
+
+#ifndef _WIN32
+	if (*flags & EVHTTP_URI_UNIX_SOCKET && !strncmp(cp, "unix:", 5)) {
+		char *e = strchr(cp + 5, ':');
+		if (e) {
+			*e = '\0';
+			uri->unixsocket = mm_strdup(cp + 5);
+			return 0;
+		} else {
+			return -1;
+		}
+	}
+#endif
+
 	/* Optionally, we end with ":port" */
 	for (port=eos-1; port >= cp && EVUTIL_ISDIGIT_(*port); --port)
 		;
 	if (port >= cp && *port == ':') {
 		if (port+1 == eos) /* Leave port unspecified; the RFC allows a
 				    * nil port */
 			uri->port = -1;
@@ -5199,14 +5351,17 @@
 	if (uri->f) {			\
 		mm_free(uri->f);		\
 	}
 
 	URI_FREE_STR_(scheme);
 	URI_FREE_STR_(userinfo);
 	URI_FREE_STR_(host);
+#ifndef _WIN32
+	URI_FREE_STR_(unixsocket);
+#endif
 	URI_FREE_STR_(path);
 	URI_FREE_STR_(query);
 	URI_FREE_STR_(fragment);
 
 	mm_free(uri);
 #undef URI_FREE_STR_
 }
@@ -5227,14 +5382,23 @@
 	if (!tmp)
 		return NULL;
 
 	if (uri->scheme) {
 		URI_ADD_(scheme);
 		evbuffer_add(tmp, ":", 1);
 	}
+#ifndef _WIN32
+	if (uri->unixsocket) {
+		evbuffer_add(tmp, "//", 2);
+		if (uri->userinfo)
+			evbuffer_add_printf(tmp, "%s@", uri->userinfo);
+		evbuffer_add_printf(tmp, "unix:%s:", uri->unixsocket);
+	}
+	else
+#endif
 	if (uri->host) {
 		evbuffer_add(tmp, "//", 2);
 		if (uri->userinfo)
 			evbuffer_add_printf(tmp,"%s@", uri->userinfo);
 		if (uri->flags & _EVHTTP_URI_HOST_HAS_BRACKETS) {
 			evbuffer_add(tmp, "[", 1);
 			URI_ADD_(host);
@@ -5292,14 +5456,21 @@
 	return uri->userinfo;
 }
 const char *
 evhttp_uri_get_host(const struct evhttp_uri *uri)
 {
 	return uri->host;
 }
+#ifndef _WIN32
+const char *
+evhttp_uri_get_unixsocket(const struct evhttp_uri *uri)
+{
+	return uri->unixsocket;
+}
+#endif
 int
 evhttp_uri_get_port(const struct evhttp_uri *uri)
 {
 	return uri->port;
 }
 const char *
 evhttp_uri_get_path(const struct evhttp_uri *uri)
@@ -5381,14 +5552,22 @@
 	} else {
 		URI_SET_STR_(host);
 		uri->flags &= ~_EVHTTP_URI_HOST_HAS_BRACKETS;
 	}
 
 	return 0;
 }
+#ifndef _WIN32
+int
+evhttp_uri_set_unixsocket(struct evhttp_uri *uri, const char *unixsocket)
+{
+	URI_SET_STR_(unixsocket);
+	return 0;
+}
+#endif
 int
 evhttp_uri_set_port(struct evhttp_uri *uri, int port)
 {
 	if (port < -1)
 		return -1;
 	uri->port = port;
 	return 0;
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/evdns.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/evdns.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event.h`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 #endif
 #ifdef EVENT__HAVE_STDINT_H
 #include <stdint.h>
 #endif
 #include <stdarg.h>
 
 /* For int types. */
-#include <evutil.h>
+#include <event2/util.h>
 
 #ifdef _WIN32
 #ifndef WIN32_LEAN_AND_MEAN
 #define WIN32_LEAN_AND_MEAN
 #endif
 #include <winsock2.h>
 #include <windows.h>
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event2/buffer.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event2/buffer.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event2/buffer_compat.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event2/buffer_compat.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event2/bufferevent.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event2/bufferevent.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event2/bufferevent_compat.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event2/bufferevent_compat.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event2/bufferevent_ssl.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event2/bufferevent_ssl.h`

 * *Files 11% similar despite different names*

```diff
@@ -179,14 +179,17 @@
 /** Return the most recent OpenSSL error reported on an SSL bufferevent. */
 EVENT2_EXPORT_SYMBOL
 unsigned long bufferevent_get_openssl_error(struct bufferevent *bev);
 
 #endif
 #if defined(EVENT__HAVE_MBEDTLS) || defined(EVENT_IN_DOXYGEN_)
 struct mbedtls_ssl_context;
+struct mbedtls_ssl_config;
+typedef struct mbedtls_ssl_context mbedtls_dyncontext;
+
 /**
    Create a new SSL bufferevent to send its data over another bufferevent.
 
    @param base An event_base to use to detect reading and writing.  It
       must also be the base for the underlying bufferevent.
    @param underlying A socket to use for this SSL
    @param ssl A SSL* object from openssl.
@@ -194,15 +197,15 @@
    @param options One or more bufferevent_options
    @return A new bufferevent on success, or NULL on failure
 */
 EVENT2_EXPORT_SYMBOL
 struct bufferevent *
 bufferevent_mbedtls_filter_new(struct event_base *base,
     struct bufferevent *underlying,
-    struct mbedtls_ssl_context *ssl,
+    mbedtls_dyncontext *ssl,
     enum bufferevent_ssl_state state,
     int options);
 
 /**
    Create a new SSL bufferevent to send its data over an SSL * on a socket.
 
    @param base An event_base to use to detect reading and writing
@@ -212,15 +215,15 @@
    @param options One or more bufferevent_options
    @return A new bufferevent on success, or NULL on failure.
 */
 EVENT2_EXPORT_SYMBOL
 struct bufferevent *
 bufferevent_mbedtls_socket_new(struct event_base *base,
     evutil_socket_t fd,
-    struct mbedtls_ssl_context *ssl,
+    mbedtls_dyncontext *ssl,
     enum bufferevent_ssl_state state,
     int options);
 
 /**
  * Get value of the BUFFEREVENT_SSL_DIRTY_SHUTDOWN flag.
  *
  * @see BUFFEREVENT_SSL_DIRTY_SHUTDOWN
@@ -245,18 +248,28 @@
 struct mbedtls_ssl_context *
 bufferevent_mbedtls_get_ssl(struct bufferevent *bufev);
 
 /** Tells a bufferevent to begin SSL renegotiation. */
 EVENT2_EXPORT_SYMBOL
 int bufferevent_mbedtls_renegotiate(struct bufferevent *bev);
 
-/** Return the most recent OpenSSL error reported on an SSL bufferevent. */
+/** Return the most recent MbedTLS error reported on an SSL bufferevent. */
 EVENT2_EXPORT_SYMBOL
 unsigned long bufferevent_get_mbedtls_error(struct bufferevent *bev);
 
+/** Create a new heap-based MbedTLS context for use it in bufferevent_mbedtls_* functions */
+EVENT2_EXPORT_SYMBOL
+mbedtls_dyncontext *
+bufferevent_mbedtls_dyncontext_new(struct mbedtls_ssl_config *conf);
+
+/** Deallocate heap-based MbedTLS context */
+EVENT2_EXPORT_SYMBOL
+void
+bufferevent_mbedtls_dyncontext_free(mbedtls_dyncontext *ctx);
+
 #endif
 
 #ifdef __cplusplus
 }
 #endif
 
 #endif /* EVENT2_BUFFEREVENT_SSL_H_INCLUDED_ */
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event2/bufferevent_struct.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event2/bufferevent_struct.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event2/dns.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event2/dns.h`

 * *Files 1% similar despite different names*

```diff
@@ -265,21 +265,21 @@
   Initialize the asynchronous DNS library.
 
   This function initializes support for non-blocking name resolution by
   calling evdns_resolv_conf_parse() on UNIX and
   evdns_config_windows_nameservers() on Windows.
 
   @param event_base the event base to associate the dns client with
-  @param initialize_nameservers any of EVDNS_BASE_INITIALIZE_NAMESERVERS|
+  @param flags any of EVDNS_BASE_INITIALIZE_NAMESERVERS|
     EVDNS_BASE_DISABLE_WHEN_INACTIVE|EVDNS_BASE_NAMESERVERS_NO_DEFAULT
   @return evdns_base object if successful, or NULL if an error occurred.
   @see evdns_base_free()
  */
 EVENT2_EXPORT_SYMBOL
-struct evdns_base * evdns_base_new(struct event_base *event_base, int initialize_nameservers);
+struct evdns_base * evdns_base_new(struct event_base *event_base, int flags);
 
 
 /**
   Shut down the asynchronous DNS resolver and terminate all active requests.
 
   If the 'fail_requests' option is enabled, all active requests will return
   an empty result with the error flag set to DNS_ERR_SHUTDOWN. Otherwise,
@@ -796,12 +796,24 @@
      -1 if idx is greater than the number of configured nameservers, or a
      value greater than 'len' if len was not high enough.
  */
 EVENT2_EXPORT_SYMBOL
 int evdns_base_get_nameserver_addr(struct evdns_base *base, int idx,
     struct sockaddr *sa, ev_socklen_t len);
 
+/**
+   Retrieve the fd of the 'idx'th configured nameserver.
+
+   @param base The evdns_base to examine.
+   @param idx The index of the nameserver to get the address of.
+
+   @return the fd value.  On failure, returns
+     -1 if idx is greater than the number of configured nameservers
+ */
+EVENT2_EXPORT_SYMBOL
+int evdns_base_get_nameserver_fd(struct evdns_base *base, int idx);
+
 #ifdef __cplusplus
 }
 #endif
 
 #endif  /* !EVENT2_DNS_H_INCLUDED_ */
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event2/dns_compat.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event2/dns_compat.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event2/dns_struct.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event2/dns_struct.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event2/event.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event2/event.h`

 * *Files 1% similar despite different names*

```diff
@@ -378,29 +378,41 @@
  @param eb the event_base structure returned by event_base_new()
  @return a string identifying the kernel event mechanism (kqueue, epoll, etc.)
  */
 EVENT2_EXPORT_SYMBOL
 const char *event_base_get_method(const struct event_base *eb);
 
 /**
+ Get the kernel signal handling mechanism used by Libevent.
+
+ @param eb the event_base structure returned by event_base_new()
+ @return a string identifying the kernel signal handling mechanism,
+   which is "signal" for traditional UNIX signal handlers,
+   "kqueue_signal" for kqueue(2)-based method on *BSD and macOS,
+   and "signalfd_signal" for Linux-only signalfd(2)-based method.
+ */
+EVENT2_EXPORT_SYMBOL
+const char *event_base_get_signal_method(const struct event_base *eb);
+
+/**
    Gets all event notification mechanisms supported by Libevent.
 
    This functions returns the event mechanism in order preferred by
    Libevent.  Note that this list will include all backends that
    Libevent has compiled-in support for, and will not necessarily check
    your OS to see whether it has the required resources.
 
    @return an array with pointers to the names of support methods.
      The end of the array is indicated by a NULL pointer.  If an
      error is encountered NULL is returned.
 */
 EVENT2_EXPORT_SYMBOL
 const char **event_get_supported_methods(void);
 
-/** Query the current monotonic time from a the timer for a struct
+/** Query the current monotonic time from the timer for a struct
  * event_base.
  */
 EVENT2_EXPORT_SYMBOL
 int event_gettime_monotonic(struct event_base *base, struct timeval *tp);
 
 /**
    @name event type flag
@@ -538,14 +550,16 @@
 	    an event_base  */
 	EVENT_BASE_FLAG_IGNORE_ENV = 0x02,
 	/** Windows only: enable the IOCP dispatcher at startup
 
 	    If this flag is set then bufferevent_socket_new() and
 	    evconn_listener_new() will use IOCP-backed implementations
 	    instead of the usual select-based one on Windows.
+
+	    Note: it is experimental feature, and has some bugs.
 	 */
 	EVENT_BASE_FLAG_STARTUP_IOCP = 0x04,
 	/** Instead of checking the current time every time the event loop is
 	    ready to run timeout callbacks, check after each timeout callback.
 	 */
 	EVENT_BASE_FLAG_NO_CACHE_TIME = 0x08,
 
@@ -580,14 +594,18 @@
 	    (CLOCK_MONOTONIC_COARSE) and enabled EVENT_BASE_FLAG_PRECISE_TIMER
 	    (CLOCK_MONOTONIC + timerfd).
 
 	    This flag has no effect if you wind up using a backend other than
 	    epoll and if you do not have EVENT_BASE_FLAG_PRECISE_TIMER enabled.
 	 */
 	EVENT_BASE_FLAG_EPOLL_DISALLOW_TIMERFD = 0x40,
+
+	/** Do not use signalfd(2) to handle signals even if supported.
+	 */
+	EVENT_BASE_FLAG_DISALLOW_SIGNALFD = 0x80,
 };
 
 /**
    Return a bitmask of the features implemented by an event base.  This
    will be a bitwise OR of one or more of the values of
    event_method_feature
 
@@ -825,15 +843,16 @@
   By default, this loop will run the event base until either there are no more
   pending or active events, or until something calls event_base_loopbreak() or
   event_base_loopexit().  You can override this behavior with the 'flags'
   argument.
 
   @param eb the event_base structure returned by event_base_new() or
      event_base_new_with_config()
-  @param flags any combination of EVLOOP_ONCE | EVLOOP_NONBLOCK
+  @param flags any combination of EVLOOP_ONCE | EVLOOP_NONBLOCK |
+     EVLOOP_NO_EXIT_ON_EMPTY
   @return 0 if successful, -1 if an error occurred, or 1 if we exited because
      no events were pending or active.
   @see event_base_loopexit(), event_base_dispatch(), EVLOOP_ONCE,
      EVLOOP_NONBLOCK
   */
 EVENT2_EXPORT_SYMBOL
 int event_base_loop(struct event_base *eb, int flags);
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event2/event_compat.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event2/event_compat.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event2/event_struct.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event2/event_struct.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event2/http.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event2/http.h`

 * *Files 2% similar despite different names*

```diff
@@ -49,26 +49,37 @@
  * interesting applications are networked today, I have often found the
  * need to write HTTP code.  The following prototypes and definitions provide
  * an application with a minimal interface for making HTTP requests and for
  * creating a very simple HTTP server.
  */
 
 /* Response codes */
+#define HTTP_CONTINUE		100	/**< client should proceed to send */
+#define HTTP_SWITCH_PROTOCOLS	101	/**< switching to another protocol */
+#define HTTP_PROCESSING		102	/**< processing the request, but no response is available yet */
+#define HTTP_EARLYHINTS		103	/**< return some response headers */
 #define HTTP_OK			200	/**< request completed ok */
+#define HTTP_CREATED		201	/**< new resource is created */
+#define HTTP_ACCEPTED		202	/**< accepted for processing */
+#define HTTP_NONAUTHORITATIVE	203	/**< returning a modified version of the origin's response */
 #define HTTP_NOCONTENT		204	/**< request does not have content */
 #define HTTP_MOVEPERM		301	/**< the uri moved permanently */
 #define HTTP_MOVETEMP		302	/**< the uri moved temporarily */
 #define HTTP_NOTMODIFIED	304	/**< page was not modified from last */
 #define HTTP_BADREQUEST		400	/**< invalid http request was made */
+#define HTTP_UNAUTHORIZED	401	/**< authentication is required */
+#define HTTP_PAYMENTREQUIRED	402	/**< user exceeded limit on requests */
+#define HTTP_FORBIDDEN		403	/**< user not having the necessary permissions */
 #define HTTP_NOTFOUND		404	/**< could not find content for uri */
 #define HTTP_BADMETHOD		405 	/**< method not allowed for this uri */
-#define HTTP_ENTITYTOOLARGE	413	/**<  */
+#define HTTP_ENTITYTOOLARGE	413	/**< request is larger than the server is able to process */
 #define HTTP_EXPECTATIONFAILED	417	/**< we can't handle this expectation */
 #define HTTP_INTERNAL           500     /**< internal error */
 #define HTTP_NOTIMPLEMENTED     501     /**< not implemented */
+#define HTTP_BADGATEWAY		502	/**< received an invalid response from the upstream */
 #define HTTP_SERVUNAVAIL	503	/**< the server is not available */
 
 struct evhttp;
 struct evhttp_request;
 struct evkeyvalq;
 struct evhttp_bound_socket;
 struct evconnlistener;
@@ -157,14 +168,22 @@
 
 /**
  * Return the listener used to implement a bound socket.
  */
 EVENT2_EXPORT_SYMBOL
 struct evconnlistener *evhttp_bound_socket_get_listener(struct evhttp_bound_socket *bound);
 
+/*
+ * Like evhttp_set_bevcb.
+ * If cb returns a non-NULL bufferevent, * the callback supplied through
+ * evhttp_set_bevcb isn't used.
+ */
+EVENT2_EXPORT_SYMBOL
+void evhttp_bound_set_bevcb(struct evhttp_bound_socket *bound, struct bufferevent* (*cb)(struct event_base *, void *), void *cbarg);
+
 typedef void evhttp_bound_socket_foreach_fn(struct evhttp_bound_socket *, void *);
 /**
  * Applies the function specified in the first argument to all
  * evhttp_bound_sockets associated with "http". The user must not
  * attempt to free or remove any connections, sockets or listeners
  * in the callback "function".
  *
@@ -318,14 +337,16 @@
 EVENT2_EXPORT_SYMBOL
 void evhttp_set_gencb(struct evhttp *http,
     void (*cb)(struct evhttp_request *, void *), void *arg);
 
 /**
    Set a callback used to create new bufferevents for connections
    to a given evhttp object.
+   cb is not called if a non-NULL bufferevent was supplied by
+   evhttp_bound_set_bevcb.
 
    You can use this to override the default bufferevent type -- for example,
    to make this evhttp object use SSL bufferevents rather than unencrypted
    ones.
 
    New bufferevents must be allocated with no fd set on them.
 
@@ -648,26 +669,41 @@
  * - read    HTTP_READ_TIMEOUT which is 50 seconds
  * - write   HTTP_WRITE_TIMEOUT, which is 50 seconds
  *
  * @param base the event_base to use for handling the connection
  * @param dnsbase the dns_base to use for resolving host names; if not
  *     specified host name resolution will block.
  * @param bev a bufferevent to use for connecting to the server; if NULL, a
- *     socket-based bufferevent will be created.  This buffrevent will be freed
+ *     socket-based bufferevent will be created.  This bufferevent will be freed
  *     when the connection closes.  It must have no fd set on it.
  * @param address the address to which to connect
  * @param port the port to connect to
  * @return an evhttp_connection object that can be used for making requests or
  *   NULL on error
  */
 EVENT2_EXPORT_SYMBOL
 struct evhttp_connection *evhttp_connection_base_bufferevent_new(
 	struct event_base *base, struct evdns_base *dnsbase, struct bufferevent* bev, const char *address, ev_uint16_t port);
 
 /**
+ * Create and return a connection object that can be used to for making HTTP
+ * requests over an unix domain socket.
+ *
+ * @param base the event_base to use for handling the connection
+ * @param bev a bufferevent to use for connecting to the server; if NULL, a
+ *     socket-based bufferevent will be created.  This bufferevent will be freed
+ *     when the connection closes.  It must have no fd set on it.
+ * @param path path of unix domain socket
+ * @return an evhttp_connection object that can be used for making requests
+ */
+EVENT2_EXPORT_SYMBOL
+struct evhttp_connection *evhttp_connection_base_bufferevent_unix_new(
+	struct event_base *base, struct bufferevent* bev, const char *path);
+
+/**
  * Return the bufferevent that an evhttp_connection is using.
  */
 EVENT2_EXPORT_SYMBOL
 struct bufferevent* evhttp_connection_get_bufferevent(struct evhttp_connection *evcon);
 
 /**
  * Return the HTTP server associated with this connection, or NULL.
@@ -1281,14 +1317,18 @@
  * section, but having an empty-string host means that the URI has an
  * authority section with no host part.  For example,
  * "mailto:user@example.com" has a host of NULL, but "file:///etc/motd"
  * has a host of "".
  */
 EVENT2_EXPORT_SYMBOL
 const char *evhttp_uri_get_host(const struct evhttp_uri *uri);
+/** Return the unix socket part of an evhttp_uri, or NULL if there is no unix
+ * socket set */
+EVENT2_EXPORT_SYMBOL
+const char *evhttp_uri_get_unixsocket(const struct evhttp_uri *uri);
 /** Return the port part of an evhttp_uri, or -1 if there is no port set. */
 EVENT2_EXPORT_SYMBOL
 int evhttp_uri_get_port(const struct evhttp_uri *uri);
 /** Return the path part of an evhttp_uri, or NULL if it has no path set */
 EVENT2_EXPORT_SYMBOL
 const char *evhttp_uri_get_path(const struct evhttp_uri *uri);
 /** Return the query part of an evhttp_uri (excluding the leading "?"), or
@@ -1308,14 +1348,19 @@
  * Returns 0 on success, -1 if userinfo is not well-formed. */
 EVENT2_EXPORT_SYMBOL
 int evhttp_uri_set_userinfo(struct evhttp_uri *uri, const char *userinfo);
 /** Set the host of an evhttp_uri, or clear the host if host==NULL.
  * Returns 0 on success, -1 if host is not well-formed. */
 EVENT2_EXPORT_SYMBOL
 int evhttp_uri_set_host(struct evhttp_uri *uri, const char *host);
+/** Set the unix socket of an evhttp_uri, or clear the unix socket if unixsocket==NULL.
+ * Returns 0 on success, -1 if unixsocket is not well-formed */
+EVENT2_EXPORT_SYMBOL
+int evhttp_uri_set_unixsocket(struct evhttp_uri *uri, const char *unixsocket);
+
 /** Set the port of an evhttp_uri, or clear the port if port==-1.
  * Returns 0 on success, -1 if port is not well-formed. */
 EVENT2_EXPORT_SYMBOL
 int evhttp_uri_set_port(struct evhttp_uri *uri, int port);
 /** Set the path of an evhttp_uri, or clear the path if path==NULL.
  * Returns 0 on success, -1 if path is not well-formed. */
 EVENT2_EXPORT_SYMBOL
@@ -1378,24 +1423,32 @@
  * Currently, these changes are:
  * <ul>
  *   <li> Nonconformant URIs are allowed to contain otherwise unreasonable
  *        characters in their path, query, and fragment components.
  * </ul>
  */
 #define EVHTTP_URI_NONCONFORMANT 0x01
+
 /**
  * Strip brackets from the IPv6 address and only for evhttp_uri_get_host(),
  * evhttp_uri_join() returns the host with brackets.
  *
  * Thus you can use host part of the evhttp_uri for getaddrinfo().
  *
  * @see also _EVHTTP_URI_HOST_HAS_BRACKETS
  */
 #define EVHTTP_URI_HOST_STRIP_BRACKETS 0x04
 
+/**
+ * Parse unix domain socket URIs, for example:
+ *
+ * http://unix:/run/control.sock:/controller
+ */
+#define EVHTTP_URI_UNIX_SOCKET 0x08
+
 /** Alias for evhttp_uri_parse_with_flags(source_uri, 0) */
 EVENT2_EXPORT_SYMBOL
 struct evhttp_uri *evhttp_uri_parse(const char *source_uri);
 
 /**
  * Free all memory allocated for a parsed uri.  Only use this for URIs
  * generated by evhttp_uri_parse.
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event2/http_compat.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event2/http_compat.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event2/http_struct.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event2/http_struct.h`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 	 * Callback added for forked-daapd so they can collect ICY
 	 * (shoutcast) metadata from the http header. If return
 	 * int is negative the connection will be closed.
 	 */
 	int (*header_cb)(struct evhttp_request *, void *);
 
 	/*
-	 * Error callback - called when error is occured.
+	 * Error callback - called when error is occurred.
 	 * @see evhttp_request_error for error types.
 	 *
 	 * @see evhttp_request_set_error_cb()
 	 */
 	void (*error_cb)(enum evhttp_request_error, void *);
 
 	/*
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event2/keyvalq_struct.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event2/keyvalq_struct.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event2/listener.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event2/listener.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event2/rpc.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event2/rpc.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event2/rpc_compat.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event2/rpc_compat.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event2/rpc_struct.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event2/rpc_struct.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event2/tag.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event2/tag.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event2/tag_compat.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event2/tag_compat.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event2/thread.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event2/thread.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event2/util.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event2/util.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event2/visibility.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event2/visibility.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/event2/watch.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/event2/watch.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/evhttp.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/evhttp.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/evrpc.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/evrpc.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/include/evutil.h` & `pvxslibs-1.2.0a1/bundle/libevent/include/evutil.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/iocp-internal.h` & `pvxslibs-1.2.0a1/bundle/libevent/iocp-internal.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/ipv6-internal.h` & `pvxslibs-1.2.0a1/bundle/libevent/ipv6-internal.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/kqueue-internal.h` & `pvxslibs-1.2.0a1/bundle/libevent/kqueue-internal.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/kqueue.c` & `pvxslibs-1.2.0a1/bundle/libevent/kqueue.c`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/listener.c` & `pvxslibs-1.2.0a1/bundle/libevent/listener.c`

 * *Files 1% similar despite different names*

```diff
@@ -271,16 +271,21 @@
 
 	listener = evconnlistener_new(base, cb, ptr, flags, backlog, fd);
 	if (!listener)
 		goto err;
 
 	return listener;
 err:
-	evutil_closesocket(fd);
-	return NULL;
+	{
+		int saved_errno = EVUTIL_SOCKET_ERROR();
+		evutil_closesocket(fd);
+		if (saved_errno)
+			EVUTIL_SET_SOCKET_ERROR(saved_errno);
+		return NULL;
+	}
 }
 
 void
 evconnlistener_free(struct evconnlistener *lev)
 {
 	LOCK(lev);
 	lev->cb = NULL;
@@ -429,18 +434,16 @@
 			evutil_closesocket(new_fd);
 			UNLOCK(lev);
 			return;
 		}
 		++lev->refcnt;
 		cb = lev->cb;
 		user_data = lev->user_data;
-		UNLOCK(lev);
 		cb(lev, new_fd, (struct sockaddr*)&ss, (int)socklen,
 		    user_data);
-		LOCK(lev);
 		if (lev->refcnt == 1) {
 			int freed = listener_decref_and_unlock(lev);
 			EVUTIL_ASSERT(freed);
 			return;
 		}
 		--lev->refcnt;
 		if (!lev->enabled) {
@@ -454,17 +457,15 @@
 		UNLOCK(lev);
 		return;
 	}
 	if (lev->errorcb != NULL) {
 		++lev->refcnt;
 		errorcb = lev->errorcb;
 		user_data = lev->user_data;
-		UNLOCK(lev);
 		errorcb(lev, user_data);
-		LOCK(lev);
 		listener_decref_and_unlock(lev);
 	} else {
 		event_sock_warn(fd, "Error from accept() call");
 		UNLOCK(lev);
 	}
 }
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/log-internal.h` & `pvxslibs-1.2.0a1/bundle/libevent/log-internal.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/log.c` & `pvxslibs-1.2.0a1/bundle/libevent/log.c`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/minheap-internal.h` & `pvxslibs-1.2.0a1/bundle/libevent/minheap-internal.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/mm-internal.h` & `pvxslibs-1.2.0a1/bundle/libevent/mm-internal.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/openssl-compat.h` & `pvxslibs-1.2.0a1/bundle/libevent/openssl-compat.h`

 * *Files 9% similar despite different names*

```diff
@@ -36,12 +36,13 @@
 
 #define X509_getm_notBefore X509_get_notBefore
 #define X509_getm_notAfter X509_get_notAfter
 
 #endif /* (OPENSSL_VERSION_NUMBER < 0x10100000L) || \
 	(defined(LIBRESSL_VERSION_NUMBER) && LIBRESSL_VERSION_NUMBER < 0x20700000L) */
 
-#if defined(LIBRESSL_VERSION_NUMBER) && LIBRESSL_VERSION_NUMBER >= 0x20700000L
+#if defined(LIBRESSL_VERSION_NUMBER) && LIBRESSL_VERSION_NUMBER >= 0x20700000L && \
+	LIBRESSL_VERSION_NUMBER < 0x30500000L
 #define BIO_get_init(b) (b)->init
 #endif
 
 #endif /* OPENSSL_COMPAT_H */
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/poll.c` & `pvxslibs-1.2.0a1/bundle/libevent/poll.c`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,16 @@
 poll_init(struct event_base *base)
 {
 	struct pollop *pollop;
 
 	if (!(pollop = mm_calloc(1, sizeof(struct pollop))))
 		return (NULL);
 
-	evsig_init_(base);
+	if (sigfd_init_(base) < 0)
+		evsig_init_(base);
 
 	evutil_weakrand_seed_(&base->weakrand_seed, 0);
 
 	return (pollop);
 }
 
 #ifdef CHECK_INVARIANTS
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/ratelim-internal.h` & `pvxslibs-1.2.0a1/bundle/libevent/ratelim-internal.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/select.c` & `pvxslibs-1.2.0a1/bundle/libevent/select.c`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,16 @@
 		return (NULL);
 
 	if (select_resize(sop, SELECT_ALLOC_SIZE(32 + 1))) {
 		select_free_selectop(sop);
 		return (NULL);
 	}
 
-	evsig_init_(base);
+	if (sigfd_init_(base) < 0)
+		evsig_init_(base);
 
 	evutil_weakrand_seed_(&base->weakrand_seed, 0);
 
 	return (sop);
 }
 
 #ifdef CHECK_INVARIANTS
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/signal.c` & `pvxslibs-1.2.0a1/bundle/libevent/signal.c`

 * *Files 3% similar despite different names*

```diff
@@ -204,33 +204,21 @@
 	event_priority_set(&base->sig.ev_signal, 0);
 
 	base->evsigsel = &evsigops;
 
 	return 0;
 }
 
-/* Helper: set the signal handler for evsignal to handler in base, so that
- * we can restore the original handler when we clear the current one. */
+/* Helper: resize saved signal handler array up to the highest signal
+   number. A dynamic array is used to keep footprint on the low side. */
 int
-evsig_set_handler_(struct event_base *base,
-    int evsignal, void (__cdecl *handler)(int))
+evsig_ensure_saved_(struct evsig_info *sig, int evsignal)
 {
-#ifdef EVENT__HAVE_SIGACTION
-	struct sigaction sa;
-#else
-	ev_sighandler_t sh;
-#endif
-	struct evsig_info *sig = &base->sig;
-	void *p;
-
-	/*
-	 * resize saved signal handler array up to the highest signal number.
-	 * a dynamic array is used to keep footprint on the low side.
-	 */
 	if (evsignal >= sig->sh_old_max) {
+		void *p;
 		int new_max = evsignal + 1;
 		event_debug(("%s: evsignal (%d) >= sh_old_max (%d), resizing",
 			    __func__, evsignal, sig->sh_old_max));
 		p = mm_realloc(sig->sh_old, new_max * sizeof(*sig->sh_old));
 		if (p == NULL) {
 			event_warn("realloc");
 			return (-1);
@@ -238,14 +226,33 @@
 
 		memset((char *)p + sig->sh_old_max * sizeof(*sig->sh_old),
 		    0, (new_max - sig->sh_old_max) * sizeof(*sig->sh_old));
 
 		sig->sh_old_max = new_max;
 		sig->sh_old = p;
 	}
+	return 0;
+}
+
+/* Helper: set the signal handler for evsignal to handler in base, so that
+ * we can restore the original handler when we clear the current one. */
+int
+evsig_set_handler_(struct event_base *base,
+    int evsignal, void (__cdecl *handler)(int))
+{
+#ifdef EVENT__HAVE_SIGACTION
+	struct sigaction sa;
+#else
+	ev_sighandler_t sh;
+#endif
+	struct evsig_info *sig = &base->sig;
+
+	/* ensure saved array is large enough */
+	if (evsig_ensure_saved_(sig, evsignal) < 0)
+		return (-1);
 
 	/* allocate space for previous handler out of dynamic array */
 	sig->sh_old[evsignal] = mm_malloc(sizeof *sig->sh_old[evsignal]);
 	if (sig->sh_old[evsignal] == NULL) {
 		event_warn("malloc");
 		return (-1);
 	}
@@ -291,15 +298,15 @@
 	if (evsig_base != base && evsig_base_n_signals_added) {
 		event_warnx("Added a signal to event base %p with signals "
 		    "already added to event_base %p.  Only one can have "
 		    "signals at a time with the %s backend.  The base with "
 		    "the most recently added signal or the most recent "
 		    "event_base_loop() call gets preference; do "
 		    "not rely on this behavior in future Libevent versions.",
-		    base, evsig_base, base->evsel->name);
+                   (void *)base, (void *)evsig_base, base->evsel->name);
 	}
 	evsig_base = base;
 	evsig_base_n_signals_added = ++sig->ev_n_signals_added;
 	evsig_base_fd = base->sig.ev_signal_pair[1];
 	EVSIGBASE_UNLOCK();
 
 	event_debug(("%s: %d: changing signal handler", __func__, (int)evsignal));
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/ssl-compat.h` & `pvxslibs-1.2.0a1/bundle/libevent/ssl-compat.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/strlcpy.c` & `pvxslibs-1.2.0a1/bundle/libevent/strlcpy.c`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/time-internal.h` & `pvxslibs-1.2.0a1/bundle/libevent/time-internal.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/util-internal.h` & `pvxslibs-1.2.0a1/bundle/libevent/util-internal.h`

 * *Files 1% similar despite different names*

```diff
@@ -457,16 +457,22 @@
 void evutil_free_globals_(void);
 
 #ifdef _WIN32
 EVENT2_EXPORT_SYMBOL
 HMODULE evutil_load_windows_system_library_(const TCHAR *library_name);
 #endif
 
-#ifndef EV_SIZE_FMT
 #if defined(_MSC_VER) || defined(__MINGW32__) || defined(__MINGW64__)
+#define EV_WINDOWS 1
+#else
+#define EV_WINDOWS 0
+#endif
+
+#ifndef EV_SIZE_FMT
+#if EV_WINDOWS
 #define EV_U64_FMT "%I64u"
 #define EV_I64_FMT "%I64d"
 #define EV_I64_ARG(x) ((__int64)(x))
 #define EV_U64_ARG(x) ((unsigned __int64)(x))
 #else
 #define EV_U64_FMT "%llu"
 #define EV_I64_FMT "%lld"
```

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/watch.c` & `pvxslibs-1.2.0a1/bundle/libevent/watch.c`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/wepoll.c` & `pvxslibs-1.2.0a1/bundle/libevent/wepoll.c`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/wepoll.h` & `pvxslibs-1.2.0a1/bundle/libevent/wepoll.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/bundle/libevent/win32select.c` & `pvxslibs-1.2.0a1/bundle/libevent/win32select.c`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/configure/CONFIG_PVXS_VERSION` & `pvxslibs-1.2.0a1/configure/CONFIG_PVXS_VERSION`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 PVXS_MAJOR_VERSION = 1
-PVXS_MINOR_VERSION = 1
-PVXS_MAINTENANCE_VERSION = 4
+PVXS_MINOR_VERSION = 2
+PVXS_MAINTENANCE_VERSION = 0
 
 # Version range conditions in Makefiles
 #
 # ifdef PVXS_X_Y_Z   # PVXS >= X.Y.Z
 #
 # ifndef PVXS_X_Y_Z  # PVXS < X.Y.Z
 #
 # ifeq ($(PVXS_X_Y_Z),YES)   # PVXS == X.Y.Z
 #
 # ifneq ($(PVXS_X_Y_Z),YES)   # PVXS != X.Y.Z
 #
-PVXS_1_1_4 = YES
+PVXS_1_2_0 = YES
+PVXS_1_1_4 = NO
 PVXS_1_1_3 = NO
 PVXS_1_1_2 = NO
 PVXS_1_1_1 = NO
 PVXS_1_1_0 = NO
 PVXS_1_0_1 = NO
 PVXS_1_0_0 = NO
 PVXS_0_3_1 = NO
```

### Comparing `pvxslibs-1.1.4a1/python/pvxslibs/version.py` & `pvxslibs-1.2.0a1/python/pvxslibs/version.py`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/python/pvxslibs.egg-info/PKG-INFO` & `pvxslibs-1.2.0a1/python/pvxslibs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvxslibs
-Version: 1.1.4a1
+Version: 1.2.0a1
 Summary: PVXS libraries packaged for python
 Home-page: https://mdavidsaver.github.io/pvxs
 Author: Michael Davidsaver
 Author-email: mdavidsaver@gmail.com
 License: BSD
 Keywords: epics scada
 Platform: UNKNOWN
```

### Comparing `pvxslibs-1.1.4a1/setup.py` & `pvxslibs-1.2.0a1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -216,14 +216,15 @@
                             ('mach/mach_time.h', False),
                             ('mach/mach.h', False),
                             ('netinet/tcp.h', False),
                             ('sys/wait.h', False),
                             ('sys/resource.h', False),
                             ('sys/sysctl.h', False), # TODO !linux
                             ('sys/timerfd.h', False),
+                            ('sys/signalfd.h', False),
                             ('errno.h', False)]:
             if probe.check_include(hfile):
                 DEFS['EVENT__HAVE_'+hfile.upper().replace('/','_').replace('.','_')] = '1'
                 probe.headers.append(hfile)
             else:
                 DEFS['EVENT__HAVE_'+hfile.upper().replace('/','_').replace('.','_')] = None
 
@@ -231,14 +232,15 @@
                 'epoll_ctl',
                 'eventfd',
                 'clock_gettime',
                 'fcntl',
                 'gettimeofday',
                 'kqueue',
                 'mmap',
+                'mmap64',
                 'pipe',
                 'pipe2',
                 'poll',
                 'port_create',
                 'sendfile',
                 'sigaction',
                 'signal',
@@ -250,14 +252,15 @@
                 'vasprintf',
                 'sysctl',
                 'accept4',
                 'arc4random',
                 'arc4random_buf',
                 'arc4random_addrandom',
                 'epoll_create1',
+                'epoll_pwait2',
                 'getegid',
                 'geteuid',
                 'getifaddrs',
                 'issetugid',
                 'mach_absolute_time',
                 'nanosleep',
                 'usleep',
@@ -287,14 +290,15 @@
                 'timerisset',
                 'putenv']:
             DEFS['EVENT__HAVE_'+sym.upper().replace('/','_').replace('.','_')] = '1' if probe.check_symbol(sym) else None
 
         DEFS['EVENT__HAVE___func__'] = '1' if probe.check_symbol('__func__') else None
 
         DEFS['EVENT__HAVE_EPOLL'] = DEFS['EVENT__HAVE_EPOLL_CREATE']
+        DEFS['EVENT__HAVE_SIGNALFD'] = DEFS['EVENT__HAVE_SYS_SIGNALFD_H']
         DEFS['EVENT__HAVE_DEVPOLL'] = DEFS['EVENT__HAVE_SYS_DEVPOLL_H']
 
         DEFS['EVENT__HAVE_TAILQFOREACH'] = '1' if probe.check_symbol('TAILQ_FOREACH', ['sys/queue.h']) else None
         DEFS['EVENT__HAVE_DECL_CTL_KERN'] = '1' if probe.check_symbol('CTL_KERN', ['sys/sysctl.h']) else '0'
         DEFS['EVENT__HAVE_DECL_KERN_ARND'] = '1' if probe.check_symbol('KERN_ARND', ['sys/sysctl.h']) else '0'
         DEFS['EVENT__HAVE_FD_MASK'] = '1' if probe.check_symbol('FD_MASK') else '0'
         DEFS['EVENT__HAVE_SETFD'] = '1' if probe.check_symbol('F_SETFD') else '0'
@@ -450,14 +454,18 @@
         log.info("In InstallHeaders")
         self.mkpath(os.path.join(self.build_lib, 'pvxs'))
 
         for header in glob('src/pvxs/*.h'):
             self.copy_file(header,
                            os.path.join(self.build_lib, 'pvxslibs', 'include', os.path.relpath(header, 'src')))
 
+        for header in glob('ioc/pvxs/*.h'):
+            self.copy_file(header,
+                           os.path.join(self.build_lib, 'pvxslibs', 'include', os.path.relpath(header, 'ioc')))
+
 
 @logexc
 def define_DSOS(self):
     DEFS = self.distribution.DEFS
     OS_CLASS = get_config_var('OS_CLASS')
 
     src_core = [
@@ -493,14 +501,17 @@
         src_core += ['wepoll.c', 'epoll.c']
     elif DEFS['EVENT__HAVE_EPOLL']=='1':
         src_core += ['epoll.c']
 
     if DEFS['EVENT__HAVE_EVENT_PORTS']=='1':
         src_core += ['evport.c']
 
+    if DEFS['EVENT__HAVE_SIGNALFD']=='1':
+        src_core += ['signalfd.c']
+
     if OS_CLASS=='WIN32':
         src_core += [
             'buffer_iocp.c',
             'bufferevent_async.c',
             'event_iocp.c',
             'win32select.c',
             'evthread_win32.c',
@@ -552,14 +563,38 @@
     else:
         src_pvxs += ['src/os/default/osdSockExt.cpp']
 
     event_libs = []
     if OS_CLASS=='WIN32':
         event_libs = ['ws2_32','shell32','advapi32','bcrypt','iphlpapi']
 
+    src_pvxsIoc = [
+        "ioc/channel.cpp",
+        "ioc/credentials.cpp",
+        "ioc/dberrormessage.cpp",
+        "ioc/demo.cpp",
+        "ioc/field.cpp",
+        "ioc/fielddefinition.cpp",
+        "ioc/fieldname.cpp",
+        "ioc/fieldsubscriptionctx.cpp",
+        "ioc/groupconfigprocessor.cpp",
+        "ioc/group.cpp",
+        "ioc/groupprocessorcontext.cpp",
+        "ioc/groupsource.cpp",
+        "ioc/groupsourcehooks.cpp",
+        "ioc/iochooks.cpp",
+        "ioc/iocsource.cpp",
+        "ioc/localfieldlog.cpp",
+        "ioc/securityclient.cpp",
+        "ioc/singlesource.cpp",
+        "ioc/singlesourcehooks.cpp",
+        "ioc/singlesrcsubscriptionctx.cpp",
+        "ioc/typeutils.cpp",
+    ]
+
     probe = ProbeToolchain()
 
     cxx11_flags = []
     if probe.try_compile('int probefn() { auto x=1; return x; }',
                          language='c++',
                          extra_preargs=['-std=c++11']):
         cxx11_flags += ['-std=c++11']
@@ -608,14 +643,37 @@
                 epicscorelibs.path.include_path
                 ],
             extra_compile_args = cxx11_flags + get_config_var('CXXFLAGS'),
             extra_link_args = cxx11_flags + get_config_var('LDFLAGS'),
             soversion = pvxs_abi,
             dsos = dsos_pvxs,
             libraries = get_config_var('LDADD') + event_libs,
+        ),
+        DSO('pvxslibs.lib.pvxsIoc', src_pvxsIoc,
+            define_macros = [('PVXS_IOC_API_BUILDING', None), ('PVXS_ENABLE_EXPERT_API', None)] + get_config_var('CPPFLAGS'),
+            include_dirs=[
+                'bundle/libevent/include',
+                'src',
+                'ioc',
+                '.', # generated headers under build/tmp
+                'pvxslibs/include', # generated headers under build/lib
+                epicscorelibs.path.include_path
+                ],
+            extra_compile_args = cxx11_flags + get_config_var('CXXFLAGS'),
+            extra_link_args = cxx11_flags + get_config_var('LDFLAGS'),
+            soversion = pvxs_abi,
+            dsos = [
+                'pvxslibs.lib.pvxs',
+                'pvxslibs.lib.event_core',
+                'epicscorelibs.lib.dbRecStd',
+                'epicscorelibs.lib.dbCore',
+                #'epicscorelibs.lib.ca',
+                'epicscorelibs.lib.Com',
+            ],
+            libraries = get_config_var('LDADD') + event_libs,
         )
     ]
 
     return DSOS
 
 build_dso.sub_commands.extend([
     ('build_expand', lambda self:True),
```

### Comparing `pvxslibs-1.1.4a1/src/bitmask.cpp` & `pvxslibs-1.2.0a1/src/bitmask.cpp`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/bitmask.h` & `pvxslibs-1.2.0a1/src/bitmask.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/client.cpp` & `pvxslibs-1.2.0a1/src/client.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -23,32 +23,58 @@
 
 typedef epicsGuard<epicsMutex> Guard;
 typedef epicsGuardRelease<epicsMutex> UnGuard;
 
 namespace pvxs {
 namespace client {
 
+DEFINE_INST_COUNTER(Connection);
+DEFINE_INST_COUNTER(Channel);
+DEFINE_INST_COUNTER2(ContextImpl, ClientContextImpl);
+DEFINE_INST_COUNTER2(Context::Pvt, ClientPvt);
+
+namespace {
+/* "normal" tick interval for the search bucket ring, and "fast" interval
+ * used for one revolution after a successful poke().
+ */
 constexpr timeval bucketInterval{1,0};
+constexpr timeval bucketIntervalFast{0,200000};
+// coalescence time for first search for a batch of newly created Channels
+constexpr timeval initialSearchDelay{0, 10000}; // 10 ms
+// number of buckets in the search ring
 constexpr size_t nBuckets = 30u;
 
-// try not to fragment with usual MTU==1500
+/* our limit for UDP packet payload.
+ * try not to fragment with usual MTU==1500 allowing for some overhead
+ * by transport protocols.  Ethernet+ip+udp headers add >= 42 bytes.
+ * May be more with eg. IP header options, VLAN tag, etc.
+ */
 constexpr size_t maxSearchPayload = 1400;
 
+/* Interval between checks for Channels which are no longer used by any operation.
+ * Channels will be discarded if found to be unused by two consecutive checks.
+ */
 constexpr timeval channelCacheCleanInterval{10,0};
 
+// time to wait before allowing another hurryUp().
+constexpr double pokeHoldoff = 30.0;
+
 // limit on the number of GUIDs * protocols * addresses we will track
 constexpr size_t beaconTrackLimit{20000};
 
+// interval between checks to discard servers which have stopped sending beacons
 constexpr timeval beaconCleanInterval{180, 0};
 
+// special interval to attempt to reconnect to disconnected name servers
 constexpr timeval tcpNSCheckInterval{10, 0};
 
 // searchSequenceID in CMD_SEARCH is redundant.
 // So we use a static value and instead rely on IDs for individual PVs
 constexpr uint32_t search_seq{0x66696e64}; // "find"
+} // namespace
 
 Disconnect::Disconnect()
     :std::runtime_error("Disconnected")
     ,time(epicsTime::getCurrent())
 {}
 
 Disconnect::~Disconnect() {}
@@ -177,15 +203,15 @@
 
         context->searchBuckets[context->currentBucket].push_back(self);
 
         log_debug_printf(io, "Server %s detach channel '%s' to re-search\n",
                          current ? current->peerName.c_str() : "<disconnected>",
                          name.c_str());
 
-    } else { // reconnect to specific server
+    } else if(context->state==ContextImpl::Running) { // reconnect to specific server
         conn = Connection::build(context, forcedServer, true);
 
         conn->pending[cid] = self;
         state = Connecting;
 
         conn->createChannels();
 
@@ -336,17 +362,17 @@
 
         chan = std::make_shared<Channel>(context, name, context->nextCID);
 
         context->chanByCID[chan->cid] = chan;
         context->chanByName[namekey] = chan;
 
         if(server.empty()) {
-            context->searchBuckets[context->currentBucket].push_back(chan);
+            context->initialSearchBucket.push_back(chan);
 
-            context->poke(true);
+            context->scheduleInitialSearch();
 
         } else { // bypass search and connect so a specific server
             chan->forcedServer = forceServer;
             chan->conn = Connection::build(context, forceServer);
 
             chan->conn->pending[chan->cid] = chan;
             chan->state = Connecting;
@@ -394,15 +420,15 @@
 
 void Context::hurryUp()
 {
     if(!pvt)
         throw std::logic_error("NULL Context");
 
     pvt->impl->manager.loop().call([this](){
-        pvt->impl->poke(true);
+        pvt->impl->poke();
     });
 }
 
 void Context::cacheClear(const std::string& name, cacheAction action)
 {
     if(!pvt)
         throw std::logic_error("NULL Context");
@@ -479,35 +505,39 @@
                        String("user"),
                        String("host"),
                    }).create();
 }
 
 ContextImpl::ContextImpl(const Config& conf, const evbase& tcp_loop)
     :ifmap(IfaceMap::instance())
-    ,effective(conf)
+    ,effective([conf]() -> Config{
+        Config eff(conf);
+        eff.expand();
+        return eff;
+    }())
     ,caMethod(buildCAMethod())
     ,searchTx4(AF_INET, SOCK_DGRAM, 0)
     ,searchTx6(AF_INET6, SOCK_DGRAM, 0)
     ,tcp_loop(tcp_loop)
     ,searchRx4(__FILE__, __LINE__,
                event_new(tcp_loop.base, searchTx4.sock, EV_READ|EV_PERSIST, &ContextImpl::onSearchS, this))
     ,searchRx6(__FILE__, __LINE__,
                event_new(tcp_loop.base, searchTx6.sock, EV_READ|EV_PERSIST, &ContextImpl::onSearchS, this))
     ,searchTimer(__FILE__, __LINE__,
                  event_new(tcp_loop.base, -1, EV_TIMEOUT, &ContextImpl::tickSearchS, this))
-    ,manager(UDPManager::instance())
+    ,initialSearcher(__FILE__, __LINE__,
+                     event_new(tcp_loop.base, -1, EV_TIMEOUT, &ContextImpl::initialSearchS, this))
+    ,manager(UDPManager::instance(effective.shareUDP()))
     ,beaconCleaner(__FILE__, __LINE__,
                    event_new(manager.loop().base, -1, EV_TIMEOUT|EV_PERSIST, &ContextImpl::tickBeaconCleanS, this))
     ,cacheCleaner(__FILE__, __LINE__,
                   event_new(tcp_loop.base, -1, EV_TIMEOUT|EV_PERSIST, &ContextImpl::cacheCleanS, this))
     ,nsChecker(__FILE__, __LINE__,
                event_new(tcp_loop.base, -1, EV_TIMEOUT|EV_PERSIST, &ContextImpl::onNSCheckS, this))
 {
-    effective.expand();
-
     searchBuckets.resize(nBuckets);
 
     std::set<SockAddr, SockAddrOnlyLess> bcasts;
     for(auto& addr : searchTx4.broadcasts()) {
         addr.setPort(0u);
         bcasts.insert(addr);
     }
@@ -652,50 +682,64 @@
                 continue;
 
             conn->cleanup();
         }
 
         conns.clear();
         chans.clear();
+        // breaks a ref. loop between Connection and ClientContextImpl
+        nameServers.clear();
 
         // internal_self.use_count() may be >1 if
         // we are orphaning some Operations
     });
 
     tcp_loop.sync();
 
     // ensure any in-progress callbacks have completed
     manager.sync();
 }
 
-void ContextImpl::poke(bool force)
+void ContextImpl::poke()
 {
     {
         Guard G(pokeLock);
-        if(poked)
+        if(nPoked)
             return;
 
         epicsTimeStamp now{};
 
         double age = -1.0;
-        if(!force && (epicsTimeGetCurrent(&now) || (age=epicsTimeDiffInSeconds(&now, &lastPoke))<30.0)) {
+        if(epicsTimeGetCurrent(&now) || (age=epicsTimeDiffInSeconds(&now, &lastPoke))<pokeHoldoff) {
             log_debug_printf(setup, "Ignoring hurryUp() age=%.1f sec\n", age);
             return;
         }
         lastPoke = now;
-        poked = true;
+        nPoked = nBuckets;
     }
 
     log_debug_printf(setup, "hurryUp()%s\n", "");
 
     timeval immediate{0,0};
     if(event_add(searchTimer.get(), &immediate))
         throw std::runtime_error("Unable to schedule searchTimer");
 }
 
+void ContextImpl::scheduleInitialSearch()
+{
+    if (!initialSearchScheduled)
+    {
+        log_debug_printf(setup, "%s()\n", __func__);
+
+        initialSearchScheduled = true;
+        if (event_add(initialSearcher.get(), &initialSearchDelay))
+            throw std::runtime_error("Unable to schedule initialSearcher");
+    }
+}
+
 void ContextImpl::onBeacon(const UDPManager::Beacon& msg)
 {
     epicsTimeStamp now;
     epicsTimeGetCurrent(&now);
 
     Guard G(pokeLock);
 
@@ -761,15 +805,15 @@
                                msg.src.tostring(),
                                msg.proto,
                                msg.server.tostring(),
                                msg.guid,
                                now
                     });
 
-        poke(false);
+        poke();
     }
 }
 
 static
 void procSearchReply(ContextImpl& self, const SockAddr& src, uint8_t peerVersion, Buffer& M, bool istcp)
 {
     ServerGUID guid;
@@ -952,76 +996,80 @@
         log_debug_printf(io, "UDP search processed %u/%u\n", i, limit);
 
     }catch(std::exception& e){
         log_exc_printf(io, "Unhandled error in search Rx callback: %s\n", e.what());
     }
 }
 
-void ContextImpl::tickSearch(bool discover)
+void ContextImpl::tickSearch(SearchKind kind, bool poked)
 {
-    // If !discover, then this is a discovery ping.
+    // If kind == SearchKind::discover, then this is a discovery ping.
     // these are really empty searches with must-reply set.
     // So if !discover, then we should not be modifying any internal state
-    {
-        Guard G(pokeLock);
-        poked = false;
-    }
+    //
+    // If kind == SearchKind::initial we are sending the first search request
+    // for the channels in initalSearchBucket, and not resending requests for
+    // channels in the searchBuckets.
 
     auto idx = currentBucket;
-    if(!discover)
+    if(kind == SearchKind::check)
         currentBucket = (currentBucket+1u)%searchBuckets.size();
 
     log_debug_printf(io, "Search tick %zu\n", idx);
 
     decltype (searchBuckets)::value_type bucket;
-    if(!discover)
+    if (kind == SearchKind::initial) {
+        initialSearchBucket.swap(bucket);
+    } else if(kind == SearchKind::check) {
         searchBuckets[idx].swap(bucket);
+    }
 
-    while(!bucket.empty() || discover) {
+    while(!bucket.empty() || kind == SearchKind::discover) {
         // when 'discover' we only loop once
 
         searchMsg.resize(0x10000);
         FixedBuf M(true, searchMsg.data(), searchMsg.size());
         M.skip(8, __FILE__, __LINE__); // fill in header after body length known
 
         // searchSequenceID
         to_wire(M, search_seq);
 
         // flags and reserved.
         // initially flags[7] is cleared (bcast)
         auto pflags = M.save();
-        to_wire(M, uint8_t(discover ? pva_search_flags::MustReply : 0u)); // must-reply to discovery, ignore regular negative search
+        to_wire(M, uint8_t(kind == SearchKind::discover ?
+                           pva_search_flags::MustReply : 0u)); // must-reply to discovery, ignore regular negative search
         to_wire(M, uint8_t(0u));
         to_wire(M, uint16_t(0u));
 
         // IN6ADDR_ANY_INIT
         to_wire(M, uint32_t(0u));
         to_wire(M, uint32_t(0u));
         to_wire(M, uint32_t(0u));
         to_wire(M, uint32_t(0u));
 
         auto pport = M.save();
         to_wire(M, uint16_t(searchRxPort));
 
-        if(discover) {
+        if(kind == SearchKind::discover) {
             to_wire(M, uint8_t(0u));
 
         } else {
             to_wire(M, uint8_t(1u));
             to_wire(M, "tcp");
         }
 
         // placeholder for channel count;
         auto pcount = M.save();
         uint16_t count = 0u;
         M.skip(2u, __FILE__, __LINE__);
 
         bool payload = false;
         while(!bucket.empty()) {
-            assert(!discover);
+            assert(kind != SearchKind::discover);
 
             auto chan = bucket.front().lock();
             if(!chan || chan->state!=Channel::Searching) {
                 bucket.pop_front();
                 continue;
             }
 
@@ -1048,15 +1096,17 @@
                     // than typical MTU.  Try to send, probably
                     // no choice but to fragment.
                 }
             }
 
             count++;
 
-            auto ninc = chan->nSearch = std::min(searchBuckets.size(), chan->nSearch+1u);
+            size_t ninc = 0u;
+            if(kind==SearchKind::check && !poked)
+                ninc = chan->nSearch = std::min(searchBuckets.size(), chan->nSearch+1u);
             auto next = (idx + ninc)%searchBuckets.size();
             auto nextnext = (next + 1u)%searchBuckets.size();
 
             // try to smooth out UDP bcast load by waiting one extra tick
             {
                 auto nextN = searchBuckets[next].size();
                 auto nextnextN = searchBuckets[nextnext].size();
@@ -1070,15 +1120,15 @@
             nextBucket.splice(nextBucket.end(),
                               bucket,
                               bucket.begin());
             payload = true;
         }
         assert(M.good());
 
-        if(!payload && !discover)
+        if(!payload && kind != SearchKind::discover)
             break;
 
         {
             FixedBuf C(true, pcount, 2u);
             to_wire(C, count);
         }
         size_t consumed = M.save() - searchMsg.data();
@@ -1138,31 +1188,53 @@
             if(evbuffer_get_length(tx) > 64*1024u)
                 continue;
 
             (void)evbuffer_add(tx, (char*)searchMsg.data(), consumed);
             // fail silently, will retry
         }
 
-        if(discover)
+        if(kind == SearchKind::discover)
             break;
     }
-
-    if(event_add(searchTimer.get(), &bucketInterval))
-        log_err_printf(setup, "Error re-enabling search timer on\n%s", "");
 }
 
 void ContextImpl::tickSearchS(evutil_socket_t fd, short evt, void *raw)
 {
+    auto self(static_cast<ContextImpl*>(raw));
     try {
-        static_cast<ContextImpl*>(raw)->tickSearch(false);
+        bool poke = false;
+        {
+            Guard G(self->pokeLock);
+            if(self->nPoked) {
+                poke = true;
+                self->nPoked--;
+            }
+        }
+
+        self->tickSearch(SearchKind::check, poke);
+
+        if(event_add(self->searchTimer.get(), poke ? &bucketIntervalFast : &bucketInterval))
+            log_err_printf(setup, "Error re-enabling search timer on\n%s", "");
+
     }catch(std::exception& e){
         log_exc_printf(io, "Unhandled error in search timer callback: %s\n", e.what());
     }
 }
 
+void ContextImpl::initialSearchS(evutil_socket_t fd, short evt, void *raw)
+{
+    auto self(static_cast<ContextImpl*>(raw));
+    try {
+        self->initialSearchScheduled = false;
+        self->tickSearch(SearchKind::initial, false);
+    }catch(std::exception& e){
+        log_exc_printf(io, "Unhandled error in initial search callback: %s\n", e.what());
+    }
+}
+
 void ContextImpl::tickBeaconClean()
 {
     epicsTimeStamp now;
     epicsTimeGetCurrent(&now);
 
     Guard G(pokeLock);
```

### Comparing `pvxslibs-1.1.4a1/src/clientconn.cpp` & `pvxslibs-1.2.0a1/src/clientconn.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -306,15 +306,15 @@
 
     ready = true;
 
     createChannels();
 
     if(nameserver) {
         log_info_printf(io, "(re)connected to nameserver %s\n", peerName.c_str());
-        context->poke(true);
+        context->poke();
     }
 }
 
 void Connection::handle_CREATE_CHANNEL()
 {
     auto rxlen = 8u + evbuffer_get_length(segBuf.get());
     EvInBuf M(peerBE, segBuf.get(), 16);
```

### Comparing `pvxslibs-1.1.4a1/src/clientdiscover.cpp` & `pvxslibs-1.2.0a1/src/clientdiscover.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
         context->discoverers[op.get()] = op;
         op->running = true;
 
         if(first && ping) {
             log_debug_printf(setup, "Starting Discover%s", "\n");
 
-            context->tickSearch(true);
+            context->tickSearch(ContextImpl::SearchKind::discover, false);
         }
     });
 
     return external;
 }
 
 void ContextImpl::serverEvent(const Discovered &evt)
```

### Comparing `pvxslibs-1.1.4a1/src/clientget.cpp` & `pvxslibs-1.2.0a1/src/clientget.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -379,14 +379,15 @@
             state = Done;
             result = Result(std::make_exception_ptr(std::logic_error("GPR Disconnect in unexpected state")));
 
             notify();
         }
     }
 };
+DEFINE_INST_COUNTER(GPROp);
 
 } // namespace
 
 void Connection::handle_GPR(pva_app_msg_t cmd)
 {
     auto rxlen = 8u + evbuffer_get_length(segBuf.get());
     EvInBuf M(peerBE, segBuf.get(), 16);
```

### Comparing `pvxslibs-1.1.4a1/src/clientimpl.h` & `pvxslibs-1.2.0a1/src/clientimpl.h`

 * *Files 8% similar despite different names*

```diff
@@ -250,31 +250,34 @@
 
     enum state_t {
         Init,
         Running,
         Stopped,
     } state = Init;
 
-    // "const" after ctor
-    Config effective;
+    const Config effective;
 
     const Value caMethod;
 
     uint32_t nextCID=0x12345678;
     uint32_t prevndrop = 0u;
 
     evsocket searchTx4, searchTx6;
     uint16_t searchRxPort;
 
     std::vector<ServerGUID> ignoreServerGUIDs;
 
     // poked and beaconSenders from both TCP and UDP workers
     epicsMutex pokeLock;
     epicsTimeStamp lastPoke{};
-    bool poked = false;
+    size_t nPoked = 0u;
+
+    // unlike `poke`, `scheduleInitialSearch` is only ever called from the
+    // tcp_loop so this does not need to be guarded by a mutex
+    bool initialSearchScheduled = false;
 
     // map: endpoint+proto -> Beaconer
     typedef std::pair<SockAddr, std::string> BeaconServer;
     struct BeaconInfo {
         SockAddr sender;
         ServerGUID guid{};
         uint8_t peerVersion{};
@@ -284,14 +287,17 @@
 
     std::vector<uint8_t> searchMsg;
 
     // search destination address and whether to set the unicast flag
     std::vector<std::pair<SockEndpoint, bool>> searchDest;
 
     size_t currentBucket = 0u;
+    // Channels where we have yet to send out an initial search request
+    std::list<std::weak_ptr<Channel>> initialSearchBucket;
+    // Channels where we are waiting for a search response
     std::vector<std::list<std::weak_ptr<Channel>>> searchBuckets;
 
     std::list<std::unique_ptr<UDPListener> > beaconRx;
 
     std::map<uint32_t, std::weak_ptr<Channel>> chanByCID;
     // strong ref. loop through Channel::context
     // explicitly broken by Context::close(), Context::cacheClear(), or ContextImpl::cacheClean()
@@ -301,14 +307,15 @@
     std::map<SockAddr, std::weak_ptr<Connection>> connByAddr;
 
     std::vector<std::pair<SockAddr, std::shared_ptr<Connection>>> nameServers;
 
     evbase tcp_loop;
     const evevent searchRx4, searchRx6;
     const evevent searchTimer;
+    const evevent initialSearcher;
 
     // beacon handling done on UDP worker.
     // we keep a ref here as long as beaconCleaner is in use
     UDPManager manager;
 
     std::map<Discovery*, std::weak_ptr<Discovery>> discoverers;
 
@@ -321,24 +328,28 @@
     ContextImpl(const Config& conf, const evbase &tcp_loop);
     ~ContextImpl();
 
     void startNS();
 
     void close();
 
-    void poke(bool force);
+    void poke();
 
     void serverEvent(const Discovered &evt);
 
     void onBeacon(const UDPManager::Beacon& msg);
 
+    void scheduleInitialSearch();
+
     bool onSearch(evutil_socket_t fd);
     static void onSearchS(evutil_socket_t fd, short evt, void *raw);
-    void tickSearch(bool discover);
+    enum class SearchKind { discover, initial, check };
+    void tickSearch(SearchKind kind, bool poked);
     static void tickSearchS(evutil_socket_t fd, short evt, void *raw);
+    static void initialSearchS(evutil_socket_t fd, short evt, void *raw);
     void tickBeaconClean();
     static void tickBeaconCleanS(evutil_socket_t fd, short evt, void *raw);
     void cacheClean(const std::string &name, Context::cacheAction force);
     static void cacheCleanS(evutil_socket_t fd, short evt, void *raw);
     void onNSCheck();
     static void onNSCheckS(evutil_socket_t fd, short evt, void *raw);
 };
```

### Comparing `pvxslibs-1.1.4a1/src/clientintrospect.cpp` & `pvxslibs-1.2.0a1/src/clientintrospect.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,15 @@
             // return to pending
 
             chan->pending.push_back(self);
             state = Connecting;
         }
     }
 };
+DEFINE_INST_COUNTER(InfoOp);
 
 } // namespace
 
 void Connection::handle_GET_FIELD()
 {
     auto rxlen = 8u + evbuffer_get_length(segBuf.get());
     EvInBuf M(peerBE, segBuf.get(), 16);
```

### Comparing `pvxslibs-1.1.4a1/src/clientmon.cpp` & `pvxslibs-1.2.0a1/src/clientmon.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -156,45 +156,41 @@
         }
     }
 
     void _pop(Value& ret, bool canthrow)
     {
         {
             if(!queue.empty()) {
-                auto ent(std::move(queue.front()));
 
-                if(!canthrow && ent.exc)
+                if(!canthrow && queue.front().exc)
                     return;
 
+                auto ent(std::move(queue.front()));
                 queue.pop_front();
 
                 if(pipeline) {
                     timeval tick{}; // immediate ACK
 
-                    // schedule delayed ack while below threshold.
-                    // avoid overhead of re-scheduling when unack in range [1, ackAt)
-                    if(unack==0u && ackAt!=1u)
-                        tick = timeval{1,0};
+                    unack++;
 
                     if(!ackPending && unack>=ackAt) {
                         if(event_add(ackTick.get(), &tick)) {
                             log_err_printf(io, "Monitor '%s' unable to schedule ack\n", channelName.c_str());
                         } else {
                             log_debug_printf(io, "Monitor '%s' sched ack %u/%u\n",
                                              channelName.c_str(), unsigned(unack), unsigned(ackAt));
                             ackPending = true;
                         }
                     }
-
-                    unack++;
                 }
-                log_info_printf(monevt, "channel '%s' monitor pop() %s %u,%u\n",
-                                channelName.c_str(),
-                                ent.exc ? "exception" : ent.val ? "data" : "null!",
-                                unsigned(window), unsigned(unack));
+                log_printf(monevt, ent.exc || ent.val ? Level::Info : Level::Err,
+                           "channel '%s' monitor pop() %s %u,%u\n",
+                           channelName.c_str(),
+                           ent.exc ? "exception" : ent.val ? "data" : "null!",
+                           unsigned(window), unsigned(unack));
 
                 if(ent.exc)
                     std::rethrow_exception(ent.exc);
                 else
                     ret = std::move(ent.val);
 
             } else {
@@ -459,14 +455,15 @@
             static_cast<SubscriptionImpl*>(raw)->tickAck();
         }catch(std::exception& e) {
             log_exc_printf(io, "Unhandled exception in %s %s : %s\n",
                            __func__, typeid (e).name(), e.what());
         }
     }
 };
+DEFINE_INST_COUNTER(SubscriptionImpl);
 
 void Connection::handle_MONITOR()
 {
     auto rxlen = 8u + evbuffer_get_length(segBuf.get());
     EvInBuf M(peerBE, segBuf.get(), 16);
 
     uint32_t ioid=0;
@@ -717,28 +714,30 @@
                     log_err_printf(io, "Server %s channel '%s' MONITOR exceeds window size\n",
                                     peerName.c_str(), mon->chan->name.c_str());
                 }
             }
 
             notify = mon->queue.empty();
 
-            if(update.exc || (mon->queue.size() < mon->queueSize) || mon->queue.back().exc) {
+            assert(mon->queueSize >= 1u);
+            if(update.val && mon->queue.size() >= mon->queueSize && mon->queue.back().val && !mon->pipeline) {
+                log_debug_printf(io, "Server %s channel %s monitor Squash\n",
+                                 peerName.c_str(),
+                                 mon->chan->name.c_str());
+
+                mon->queue.back().val.assign(update.val);
+                mon->nCliSquash++;
+
+            } else if(update.exc || update.val) {
                 log_debug_printf(io, "Server %s channel %s monitor PUSH\n",
                                 peerName.c_str(),
                                 mon->chan->name.c_str());
 
                 mon->queue.emplace_back(std::move(update));
 
-            } else if(update.val) {
-                log_debug_printf(io, "Server %s channel %s monitor Squash\n",
-                                peerName.c_str(),
-                                mon->chan->name.c_str());
-
-                mon->queue.back().val.assign(update.val);
-                mon->nCliSquash++;
             }
 
             if(final && !update.exc) {
                 log_debug_printf(io, "Server %s channel %s monitor FINISH\n",
                                 peerName.c_str(),
                                 mon->chan->name.c_str());
 
@@ -807,15 +806,15 @@
 
     auto ackAny = options["ackAny"];
 
     if(ackAny.type()==TypeCode::String) {
         auto sval = ackAny.as<std::string>();
         if(sval.size()>1 && sval.back()=='%') {
             try {
-                auto percent = parseTo<double>(sval);
+                auto percent = parseTo<double>(sval.substr(0, sval.size()-1u));
                 if(percent>0.0 && percent<=100.0) {
                     op->ackAt = uint32_t(percent * op->queueSize);
                 } else {
                     throw std::invalid_argument("not in range (0%, 100%]");
                 }
             }catch(std::exception&){
                 log_warn_printf(monevt, "Error parsing as percent ackAny: \"%s\"\n", sval.c_str());
```

### Comparing `pvxslibs-1.1.4a1/src/clientreq.cpp` & `pvxslibs-1.2.0a1/src/clientreq.cpp`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/config.cpp` & `pvxslibs-1.2.0a1/src/config.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -479,54 +479,29 @@
     defs["EPICS_PVA_INTF_ADDR_LIST"] = defs["EPICS_PVAS_INTF_ADDR_LIST"]   = join_addr(interfaces);
     defs["EPICS_PVAS_IGNORE_ADDR_LIST"]   = join_addr(ignoreAddrs);
     defs["EPICS_PVA_CONN_TMO"] = SB()<<tcpTimeout/tmoScale;
 }
 
 void Config::expand()
 {
-    if(tcp_port==0)
-        tcp_port = 5075;
-
     auto ifaces(parseAddresses(interfaces));
     auto bdest(parseAddresses(beaconDestinations));
 
     // empty interface address list implies the wildcard
     // (because no addresses isn't interesting...)
     if(ifaces.empty()) {
         ifaces.emplace_back(SockAddr::any(AF_INET));
     }
 
     auto& ifmap = IfaceMap::instance();
 
     for(size_t i=0; i<ifaces.size(); i++) {
         auto& ep = ifaces[i];
 
-        if(evsocket::canIPv6 && ep.addr.isAny()) {
-            // special handling for IP4/6 wildcard addresses
-
-            if(evsocket::ipstack==evsocket::Linsock && ep.addr.family()==AF_INET) {
-                // Linux IP stack disallows binding both 0.0.0.0 and [::] for the same port.
-                // so promote to IPv6 when possible
-                ep.addr = SockAddr::any(AF_INET6, ep.addr.port());
-                log_debug_printf(serversetup, "Promote 0.0.0.0 -> [::]%s", "\n");
-
-            } else if(evsocket::ipstack!=evsocket::Linsock) {
-                /* Other IP stacks allow binding different sockets.
-                 * OSX has the added oddity of ordering dependence.
-                 * 0.0.0.0 and then :: is allowed, but not the reverse.
-                 *
-                 * So when possible, we always bind both in the allowed order.
-                 */
-                ep.addr = SockAddr::any(AF_INET, ep.addr.port());
-                ifaces.emplace(ifaces.begin()+i+1u,
-                               SockAddr::any(AF_INET6, ep.addr.port()));
-                i++; // continue after newly inserted EP
-            }
-
-        } else if(!ep.addr.isMCast()) {
+        if(!ep.addr.isMCast()) {
             // no-op
 
         } else if(!ep.iface.empty()) {
             ifaces.emplace_back(ifmap.address_of(ep.iface));
         } else {
             ifaces.emplace_back(SockAddr::any(ep.addr.family()));
         }
@@ -550,39 +525,25 @@
 
     enforceTimeout(tcpTimeout);
 
 }
 
 std::ostream& operator<<(std::ostream& strm, const Config& conf)
 {
-    auto showAddrs = [&strm](const char* var, const std::vector<std::string>& addrs) {
-        strm<<indent{}<<var<<"=\"";
-        bool first = true;
-        for(auto& iface : addrs) {
-            if(first)
-                first = false;
-            else
-                strm<<' ';
-            strm<<iface;
-        }
-        strm<<"\"\n";
-    };
-
-    showAddrs("EPICS_PVAS_INTF_ADDR_LIST", conf.interfaces);
-    showAddrs("EPICS_PVAS_BEACON_ADDR_LIST", conf.beaconDestinations);
-    showAddrs("EPICS_PVAS_IGNORE_ADDR_LIST", conf.ignoreAddrs);
-
-    strm<<indent{}<<"EPICS_PVAS_AUTO_BEACON_ADDR_LIST="<<(conf.auto_beacon?"YES":"NO")<<'\n';
-
-    strm<<indent{}<<"EPICS_PVAS_SERVER_PORT="<<conf.tcp_port<<'\n';
-
-    strm<<indent{}<<"EPICS_PVAS_BROADCAST_PORT="<<conf.udp_port<<'\n';
-
-    strm<<indent{}<<"EPICS_PVA_CONN_TMO="<<conf.tcpTimeout/tmoScale<<'\n';
+    Config::defs_t defs;
+    conf.updateDefs(defs);
 
+    for(const auto& pair : defs) {
+        // only print the server variant
+        static const char prefix[] = "EPICS_PVAS_";
+        if(pair.first.size() >= sizeof(prefix)-1u && strncmp(pair.first.c_str(),
+                                                             prefix,
+                                                             sizeof(prefix)-1u)==0)
+            strm<<indent{}<<pair.first<<'='<<pair.second<<'\n';
+    }
     return strm;
 }
 
 } // namespace server
 
 namespace client {
 
@@ -652,14 +613,15 @@
 {
     defs["EPICS_PVA_BROADCAST_PORT"] = SB()<<udp_port;
     defs["EPICS_PVA_SERVER_PORT"] = SB()<<tcp_port;
     defs["EPICS_PVA_AUTO_ADDR_LIST"] = autoAddrList ? "YES" : "NO";
     defs["EPICS_PVA_ADDR_LIST"] = join_addr(addressList);
     defs["EPICS_PVA_INTF_ADDR_LIST"] = join_addr(interfaces);
     defs["EPICS_PVA_CONN_TMO"] = SB()<<tcpTimeout/tmoScale;
+    defs["EPICS_PVA_NAME_SERVERS"] = join_addr(nameServers);
 }
 
 void Config::expand()
 {
     if(udp_port==0)
         throw std::runtime_error("Client can't use UDP random port");
 
@@ -683,34 +645,20 @@
     printAddresses(addressList, addrs);
 
     enforceTimeout(tcpTimeout);
 }
 
 std::ostream& operator<<(std::ostream& strm, const Config& conf)
 {
-    bool first;
+    Config::defs_t defs;
+    conf.updateDefs(defs);
 
-    strm<<indent{}<<"EPICS_PVA_ADDR_LIST=\"";
-    first = true;
-    for(auto& iface : conf.addressList) {
-        if(first)
-            first = false;
-        else
-            strm<<' ';
-        strm<<iface;
+    for(const auto& pair : defs) {
+        strm<<indent{}<<pair.first<<'='<<pair.second<<'\n';
     }
-    strm<<"\"\n";
-
-    strm<<indent{}<<"EPICS_PVA_AUTO_ADDR_LIST="<<(conf.autoAddrList?"YES":"NO")<<'\n';
-
-    strm<<indent{}<<"EPICS_PVA_BROADCAST_PORT="<<conf.udp_port<<'\n';
-
-    strm<<indent{}<<"EPICS_PVA_SERVER_PORT="<<conf.tcp_port<<'\n';
-
-    strm<<indent{}<<"EPICS_PVA_CONN_TMO="<<conf.tcpTimeout/tmoScale<<'\n';
 
     return strm;
 }
 
 } // namespace client
 
 } // namespace pvxs
```

### Comparing `pvxslibs-1.1.4a1/src/conn.cpp` & `pvxslibs-1.2.0a1/src/conn.cpp`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/conn.h` & `pvxslibs-1.2.0a1/src/conn.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/data.cpp` & `pvxslibs-1.2.0a1/src/data.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 #include <epicsAssert.h>
 
 #include "dataimpl.h"
 #include "utilpvt.h"
 
 namespace pvxs {
 
+DEFINE_INST_COUNTER(StructTop);
+
 NoField::NoField()
     :std::runtime_error ("No such field")
 {}
 
 NoField::~NoField() {}
 
 NoConvert::~NoConvert() {}
@@ -629,16 +631,19 @@
                 }
                 dest = src;
 
             } else if(src.original_type()!=ArrayType::Value && uint8_t(desc->code.code)==uint8_t(src.original_type())) {
                 // assign array of scalar w/o convert
                 dest = src;
 
+            } else if(src.original_type()!=ArrayType::Value) {
+                // assign array of scalar w/ implicit conversion
+                dest = detail::copyAs(desc->code.arrayType(), src.original_type(), src.data(), src.size()).freeze();
+
             } else {
-                // TODO: alloc and convert
                 throw NoConvert(SB()<<"Unable to assign "<<desc->code<<" with "<<type);
             }
             break;
         }
         default:
             throw NoConvert(SB()<<"Unable to assign "<<desc->code<<" with "<<type);
         }
@@ -649,15 +654,18 @@
             store->as<Value>() = Value(); // unselect Union or Any
             break;
 
         } else if(desc->code==TypeCode::Any) {
             // assigning variant union.
             auto& val = store->as<Value>();
             if(type==StoreType::Compound) {
-                val = *reinterpret_cast<const Value*>(ptr);
+                auto& newval = *reinterpret_cast<const Value*>(ptr);
+                if(store == newval.store)
+                    throw std::logic_error("Any self-assignment would recurse.  Not allowed.");
+                val = newval;
                 break;
 
             } else {
                 val = Value::Helper::build(ptr, type);
                 break;
             }
```

### Comparing `pvxslibs-1.1.4a1/src/dataencode.cpp` & `pvxslibs-1.2.0a1/src/dataencode.cpp`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/datafmt.cpp` & `pvxslibs-1.2.0a1/src/datafmt.cpp`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/dataimpl.h` & `pvxslibs-1.2.0a1/src/dataimpl.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/describe.cpp` & `pvxslibs-1.2.0a1/src/describe.cpp`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/evhelper.cpp` & `pvxslibs-1.2.0a1/src/evhelper.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,21 @@
 
         return evt;
     }
 
     inline epicsEvent* operator->() { return get(); }
 };
 
+namespace {
+struct evbaseRunning {
+    INST_COUNTER(evbaseRunning);
+};
+DEFINE_INST_COUNTER(evbaseRunning);
+}
+
 struct evbase::Pvt final : public epicsThreadRunable
 {
     SockAttach attach;
 
     std::weak_ptr<Pvt> internal_self;
 
     struct Work {
@@ -161,15 +168,15 @@
         if(event_base_loopexit(base.get(), nullptr))
             log_crit_printf(logerr, "evbase error while interrupting loop for %p\n", base.get());
         worker.exitWait();
     }
 
     virtual void run() override final
     {
-        INST_COUNTER(evbaseRunning);
+        evbaseRunning track;
         try {
             evconfig conf(__FILE__, __LINE__, event_config_new());
 #ifdef __rtems__
             /* with libbsd circa RTEMS 5.1
              * TCP peer close/reset notifications appear to be lost.
              * Maybe due to absence of NOTE_EOF?
              * poll() seems to work though.
@@ -249,14 +256,15 @@
     void evkeepalive(evutil_socket_t sock, short evt, void *raw)
     {
         auto self = static_cast<Pvt*>(raw);
         log_debug_printf(logerr, "Look keepalive %p\n", self);
     }
 
 };
+DEFINE_INST_COUNTER2(evbase::Pvt, evbase);
 
 evbase::evbase(const std::string &name, unsigned prio)
 {
     auto internal(std::make_shared<Pvt>(name, prio));
     internal->internal_self = internal;
 
     pvt.reset(internal.get(), [internal](Pvt*) mutable {
@@ -366,15 +374,15 @@
                    name, epicsThread::getNameSelf());
     throw std::logic_error("Not in running evbase worker");
 }
 
 bool evsocket::canIPv6;
 evsocket::ipstack_t evsocket::ipstack;
 
-evsocket::evsocket(int af, evutil_socket_t sock)
+evsocket::evsocket(int af, evutil_socket_t sock, bool blocking)
     :sock(sock)
     ,af(af)
 {
     if(sock==evutil_socket_t(-1)) {
         int err = evutil_socket_geterror(sock);
 #ifdef _WIN32
         if(err==WSANOTINITIALISED) {
@@ -386,27 +394,27 @@
     if(af!=AF_INET && af!=AF_INET6) {
         evutil_closesocket(sock);
         throw std::logic_error("Unsupported address family");
     }
 
     evutil_make_socket_closeonexec(sock);
 
-    if(evutil_make_socket_nonblocking(sock)) {
+    if(!blocking && evutil_make_socket_nonblocking(sock)) {
         evutil_closesocket(sock);
         throw std::runtime_error("Unable to make non-blocking socket");
     }
 }
 
 // Linux specific way to atomically create a socket with O_CLOEXEC
 #ifndef SOCK_CLOEXEC
 #  define SOCK_CLOEXEC 0
 #endif
 
-evsocket::evsocket(int af, int type, int proto)
-    :evsocket(af, socket(af, type | SOCK_CLOEXEC, proto))
+evsocket::evsocket(int af, int type, int proto, bool blocking)
+    :evsocket(af, socket(af, type | SOCK_CLOEXEC, proto), blocking)
 {
 #ifdef __linux__
 #  ifndef IP_MULTICAST_ALL
 #    define IP_MULTICAST_ALL		49
 #  endif
     // Disable non-compliant legacy behavior of Linux IP stack
     if(af==AF_INET && type==SOCK_DGRAM){
@@ -818,20 +826,21 @@
         if(hit)
             ret = it->second->index;
         return hit;
     });
     return ret;
 }
 
-bool IfaceMap::is_address(const SockAddr& addr)
+bool IfaceMap::is_iface(const SockAddr& addr)
 {
     Guard G(lock);
 
     return try_cache(*this, [this, addr]() {
-        return byAddr.find(addr)!=byAddr.end();
+        auto it(byAddr.find(addr));
+        return it!=byAddr.end() && !it->second.second;
     });
 }
 
 bool IfaceMap::is_broadcast(const SockAddr& addr)
 {
     Guard G(lock);
 
@@ -1019,14 +1028,16 @@
     to_wire(M, H);
     if(!M.good())
         throw BAD_ALLOC();
 }
 
 } // namespace impl
 
+std::atomic<size_t> Timer::Pvt::cnt_Timer {0u};
+
 Timer::~Timer() {}
 
 bool Timer::cancel()
 {
     if(!pvt)
         throw std::logic_error("NULL Timer");
```

### Comparing `pvxslibs-1.1.4a1/src/evhelper.h` & `pvxslibs-1.2.0a1/src/evhelper.h`

 * *Files 2% similar despite different names*

```diff
@@ -195,18 +195,18 @@
     evutil_socket_t sock;
     int af;
 
     // default construct an invalid socket
     constexpr evsocket() noexcept :sock(-1), af(AF_UNSPEC) {}
 
     // construct from a valid (not -1) socket
-    explicit evsocket(int af, evutil_socket_t sock);
+    explicit evsocket(int af, evutil_socket_t sock, bool blocking=false);
 
     // create a new socket
-    evsocket(int, int, int);
+    evsocket(int af, int type, int proto, bool blocking=false);
 
     // movable
     evsocket(evsocket&& o) noexcept;
     evsocket& operator=(evsocket&&) noexcept;
 
     // not copyable
     evsocket(const evsocket&) = delete;
@@ -276,15 +276,15 @@
     // lookup interface name by index
     std::string name_of(uint64_t index);
     // find (an) interface name with this address.  useful for IPv4.  returns empty string if not found.
     std::string name_of(const SockAddr& addr);
     // returns 0 if not found
     uint64_t index_of(const std::string& name);
     // is this a valid interface or broadcast address?
-    bool is_address(const SockAddr& addr);
+    bool is_iface(const SockAddr& addr);
     // is this a valid interface or broadcast address?
     bool is_broadcast(const SockAddr& addr);
     // look up interface address.  useful for IPV4.  returns AF_UNSPEC if not found
     SockAddr address_of(const std::string& name);
     // all interface names except LO
     std::set<std::string> all_external();
```

### Comparing `pvxslibs-1.1.4a1/src/log.cpp` & `pvxslibs-1.2.0a1/src/log.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,18 @@
     std::list<std::pair<std::string, Level>> config;
     std::multimap<std::string, logger*> loggers;
 
     logger_gbl_t()
     {
         event_set_log_callback(&evlog_handler);
     }
+    ~logger_gbl_t()
+    {
+        event_set_log_callback(nullptr);
+    }
 
     Level init(logger *logger)
     {
         std::string name(logger->name);
 
         auto lvl = Level::Warn;
```

### Comparing `pvxslibs-1.1.4a1/src/nt.cpp` & `pvxslibs-1.2.0a1/src/nt.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -56,23 +56,32 @@
 
     if(display && isnumeric) {
         def += {
                 Struct("display", {
                            Member(scalar, "limitLow"),
                            Member(scalar, "limitHigh"),
                            String("description"),
-                           //String("format"),
                            String("units"),
                        }),
         };
+        if(form) {
+            def += {
+                    Struct("display", {
+                           Int32("precision"),
+                           Struct("form", "enum_t", {
+                               Int32("index"),
+                               StringA("choices"),
+                           }),
+                    }),
+            };
+        }
     } else if(display && !isnumeric) {
             def += {
                     Struct("display", {
                                String("description"),
-                               //String("format"),
                                String("units"),
                            }),
             };
     }
 
     if(control && isnumeric) {
         def += {
@@ -111,14 +120,17 @@
     TypeDef def(TypeCode::Struct, "epics:nt/NTEnum:1.0", {
                     Struct("value", "enum_t", {
                         Int32("index"),
                         StringA("choices"),
                     }),
                     Alarm{}.build().as("alarm"),
                     TimeStamp{}.build().as("timeStamp"),
+                    Struct("display", {
+                        String("description"),
+                    }),
                 });
 
     return def;
 }
 
 TypeDef NTNDArray::build() const
 {
```

### Comparing `pvxslibs-1.1.4a1/src/os/WIN32/osdSockExt.cpp` & `pvxslibs-1.2.0a1/src/os/WIN32/osdSockExt.cpp`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/os/default/osdSockExt.cpp` & `pvxslibs-1.2.0a1/src/os/default/osdSockExt.cpp`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/osgroups.cpp` & `pvxslibs-1.2.0a1/src/osgroups.cpp`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/osiSockExt.h` & `pvxslibs-1.2.0a1/src/osiSockExt.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/pvaproto.h` & `pvxslibs-1.2.0a1/src/pvaproto.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/pvrequest.cpp` & `pvxslibs-1.2.0a1/src/pvrequest.cpp`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/pvrequest.h` & `pvxslibs-1.2.0a1/src/pvrequest.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/pvxs/client.h` & `pvxslibs-1.2.0a1/src/pvxs/client.h`

 * *Files 1% similar despite different names*

```diff
@@ -1029,14 +1029,15 @@
 
     //! Inactivity timeout interval for TCP connections.  (seconds)
     //! @since 0.2.0
     double tcpTimeout = 40.0;
 
 private:
     bool BE = EPICS_BYTE_ORDER==EPICS_ENDIAN_BIG;
+    bool UDP = true;
 public:
 
     // compat
     static inline Config from_env() { return Config{}.applyEnv(); }
 
     //! Default configuration using process environment
     static inline Config fromEnv()  { return Config{}.applyEnv(); }
@@ -1069,14 +1070,16 @@
         return Context(*this);
     }
 
 #ifdef PVXS_EXPERT_API_ENABLED
     // for protocol compatibility testing
     inline Config& overrideSendBE(bool be) { BE = be; return *this; }
     inline bool sendBE() const { return BE; }
+    inline Config& overrideShareUDP(bool share) { UDP = share; return *this; }
+    inline bool shareUDP() const { return UDP; }
 #endif
 };
 
 PVXS_API
 std::ostream& operator<<(std::ostream& strm, const Config& conf);
 
 } // namespace client
```

### Comparing `pvxslibs-1.1.4a1/src/pvxs/data.h` & `pvxslibs-1.2.0a1/src/pvxs/data.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/pvxs/log.h` & `pvxslibs-1.2.0a1/src/pvxs/log.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/pvxs/netcommon.h` & `pvxslibs-1.2.0a1/src/pvxs/netcommon.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/pvxs/nt.h` & `pvxslibs-1.2.0a1/src/pvxs/nt.h`

 * *Files 10% similar despite different names*

```diff
@@ -63,21 +63,27 @@
     TypeCode value;
     //! Include display (range) meta-data
     bool display;
     //! Include control (range) meta-data
     bool control;
     //! Include alarm (range) meta-data
     bool valueAlarm;
+    /** Include 'display.form' and 'display.precision' when 'value' is a numeric type
+     *  @pre requires display=true
+     *  @since UNRELEASED
+     */
+    bool form;
 
     constexpr
     NTScalar(TypeCode value = TypeCode::Float64,
              bool display = false,
              bool control = false,
-             bool valueAlarm = false)
-        :value(value), display(display), control(control), valueAlarm(valueAlarm)
+             bool valueAlarm = false,
+             bool form = false)
+        :value(value), display(display), control(control), valueAlarm(valueAlarm), form(form)
     {}
 
     //! A TypeDef which can be appended
     PVXS_API
     TypeDef build() const;
     //! Instantiate
     inline Value create() const {
```

### Comparing `pvxslibs-1.1.4a1/src/pvxs/server.h` & `pvxslibs-1.2.0a1/src/pvxs/server.h`

 * *Files 4% similar despite different names*

```diff
@@ -172,14 +172,15 @@
     double tcpTimeout = 40.0;
 
     //! Server unique ID.  Only meaningful in readback via Server::config()
     ServerGUID guid{};
 
 private:
     bool BE = EPICS_BYTE_ORDER==EPICS_ENDIAN_BIG;
+    bool UDP = true;
 public:
 
     // compat
     static inline Config from_env() { return Config{}.applyEnv(); }
 
     //! Default configuration using process environment
     static inline Config fromEnv()  { return Config{}.applyEnv(); }
@@ -216,14 +217,16 @@
         return Server(*this);
     }
 
 #ifdef PVXS_EXPERT_API_ENABLED
     // for protocol compatibility testing
     inline Config& overrideSendBE(bool be) { BE = be; return *this; }
     inline bool sendBE() const { return BE; }
+    inline Config& overrideShareUDP(bool share) { UDP = share; return *this; }
+    inline bool shareUDP() const { return UDP; }
 #endif
 };
 
 PVXS_API
 std::ostream& operator<<(std::ostream& strm, const Config& conf);
 
 }} // namespace pvxs::server
```

### Comparing `pvxslibs-1.1.4a1/src/pvxs/sharedArray.h` & `pvxslibs-1.2.0a1/src/pvxs/sharedArray.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/pvxs/sharedpv.h` & `pvxslibs-1.2.0a1/src/pvxs/sharedpv.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/pvxs/source.h` & `pvxslibs-1.2.0a1/src/pvxs/source.h`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,17 @@
     //! serialized and in the TX buffer.
     size_t nQueue=0;
     //! Highest value of nQueue seen
     //! @since 1.1.0
     size_t maxQueue=0;
     //! Negotiated limit on nQueue
     size_t limitQueue=0;
+    //! Number of updates squashed during post() calss
+    //! @since UNRELEASED
+    size_t nSquash=0;
 
     bool running=false;
     bool finished=false;
     bool pipeline=false;
 };
 
 //! Handle for active subscription
@@ -102,15 +105,15 @@
     bool tryPost(const Value& val) {
         return doPost(val, true, false);
     }
 
     //! Signal to subscriber that this subscription will not yield any further events.
     //! This is not an error.  Client should not retry.
     void finish() {
-        doPost(Value(), false, false);
+        doPost(Value(), false, true);
     }
 
     //! Poll information and statistics for this subscription.
     //! @since 1.1.0 Added 'reset' argument.
     virtual void stats(MonitorStat&, bool reset=false) const =0;
 
     /** Set flow control levels.
```

### Comparing `pvxslibs-1.1.4a1/src/pvxs/srvcommon.h` & `pvxslibs-1.2.0a1/src/pvxs/srvcommon.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/pvxs/unittest.h` & `pvxslibs-1.2.0a1/src/pvxs/unittest.h`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 #include <pvxs/version.h>
 #include <pvxs/util.h>
 
 namespace pvxs {
 
 /** Prepare for testing.  Call after testPlan()
+ * @since UNRELEASED If linked with pvxsIoc library, PVA server started
+ *                   by ``iocInit()`` will use "isolated" configuration.
  */
 PVXS_API
 void testSetup();
 
 /** Free some internal global allocations to avoid false positives in
  *  valgrind (or similar) tools looking for memory leaks.
  *
```

### Comparing `pvxslibs-1.1.4a1/src/pvxs/util.h` & `pvxslibs-1.2.0a1/src/pvxs/util.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/pvxs/version.h` & `pvxslibs-1.2.0a1/src/pvxs/version.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/server.cpp` & `pvxslibs-1.2.0a1/src/server.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -386,39 +386,58 @@
     ,builtinsrc(StaticSource::build())
     ,state(Stopped)
 {
     effective.expand();
 
     beaconSender4.set_broadcast(true);
 
-    auto manager = UDPManager::instance();
+    auto manager = UDPManager::instance(effective.shareUDP());
 
     evsocket dummy(AF_INET, SOCK_DGRAM, 0);
 
     const auto cb(std::bind(&Pvt::onSearch, this, std::placeholders::_1));
 
+    bool bindAny = false;
     std::vector<SockAddr> tcpifaces; // may have port zero
     for(const auto& iface : effective.interfaces) {
         SockEndpoint addr(iface.c_str());
-        if(!addr.addr.isMCast())
+
+        if(addr.addr.isAny()) {
+            bindAny = true;
+
+        } else if(!addr.addr.isMCast()) {
             tcpifaces.push_back(addr.addr);
 
+        }
+
         addr.addr.setPort(effective.udp_port);
 
         listeners.push_back(manager.onSearch(addr, cb));
 
         // update to allow udp_port==0
         effective.udp_port = addr.addr.port();
 
+
+        if(addr.addr.isAny()) {
+            continue; // special case handling below
+        }
+
         if(addr.addr.family()==AF_INET && addr.addr.isAny()) {
             // if listening on 0.0.0.0, also listen on [::]
             auto any6(addr);
             any6.addr = SockAddr::any(AF_INET6);
 
             listeners.push_back(manager.onSearch(any6, cb));
+
+        } else if(addr.addr.family()==AF_INET6 && addr.addr.isAny()) {
+            // if listening on [::], also listen on 0.0.0.0
+            auto any4(addr);
+            any4.addr = SockAddr::any(AF_INET);
+
+            listeners.push_back(manager.onSearch(any4, cb));
         }
 
         if(evsocket::ipstack!=evsocket::Winsock
                 && addr.addr.family()==AF_INET && !addr.addr.isAny() && !addr.addr.isMCast()) {
             /* An oddness of BSD sockets (not winsock) is that binding to
              * INADDR_ANY will receive unicast and broadcast, but binding to
              * a specific interface address receives only unicast.  The trick
@@ -428,14 +447,36 @@
             for(auto bcast : dummy.broadcasts(&addr.addr)) {
                 bcast.setPort(addr.addr.port());
                 listeners.push_back(manager.onSearch(bcast, cb));
             }
         }
     }
 
+    if(bindAny) {
+        if(evsocket::canIPv6) {
+            if(evsocket::ipstack==evsocket::Linsock) {
+                /* Linux IP stack disallows binding both 0.0.0.0 and [::] for the same port.
+                 * so we must always bind [::]
+                 */
+                tcpifaces.emplace_back(AF_INET6);
+            } else {
+                /* Other IP stacks allow binding different sockets.
+                 * OSX has the added oddity of ordering dependence.
+                 * 0.0.0.0 and then :: is allowed, but not the reverse.
+                 *
+                 * Always bind both in the OSX allowed order.
+                 */
+                tcpifaces.emplace_back(AF_INET);
+                tcpifaces.emplace_back(AF_INET6);
+            }
+        } else {
+            tcpifaces.emplace_back(AF_INET);
+        }
+    }
+
     if(tcpifaces.empty()) {
         log_err_printf(serversetup, "Server Unreachable.  Interface address list includes not TCP interfaces.%s", "\n");
     }
 
     for(const auto& addr : effective.ignoreAddrs) {
         SockAddr temp(addr.c_str());
         ignoreList.push_back(temp);
@@ -608,14 +649,20 @@
         for(auto& pair : conns) {
             pair.second->disconnect();
             pair.second->cleanup();
         }
 
         state = Stopped;
     });
+
+    /* Cycle through once more to ensure any callbacks queue during the previous call have completed.
+     * TODO: this is partly a crutch as eg. SharedPV::attach() binds strong self references
+     *       into on*() lambdas, which indirectly hold references keeping acceptor_loop alive.
+     */
+    acceptor_loop.sync();
 }
 
 void Server::Pvt::onSearch(const UDPManager::Search& msg)
 {
     // on UDPManager worker
 
     for(const auto& addr : ignoreList) { // expected to be a short list
```

### Comparing `pvxslibs-1.1.4a1/src/serverchan.cpp` & `pvxslibs-1.2.0a1/src/serverchan.cpp`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/serverconn.cpp` & `pvxslibs-1.2.0a1/src/serverconn.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,24 @@
 #include "serverconn.h"
 
 // limit on size of TX buffer above which we suspend RX.
 // defined as multiple of OS socket TX buffer size
 static constexpr size_t tcp_tx_limit_mult = 2u;
 
 namespace pvxs {
+namespace impl {
+DEFINE_INST_COUNTER(ServerChannelControl);
+DEFINE_INST_COUNTER(ServerChan);
+DEFINE_INST_COUNTER(ServerConn);
+DEFINE_INST_COUNTER(ServerSource);
+}
 namespace server {
+
+DEFINE_INST_COUNTER2(Server::Pvt, ServerPvt);
+
 std::set<std::string> ClientCredentials::roles() const
 {
     std::set<std::string> ret;
     osdGetRoles(account, ret);
     return ret;
 }
```

### Comparing `pvxslibs-1.1.4a1/src/serverconn.h` & `pvxslibs-1.2.0a1/src/serverconn.h`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/serverget.cpp` & `pvxslibs-1.2.0a1/src/serverget.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,15 @@
 
     std::function<void(std::unique_ptr<server::ExecOp>&&, Value&&)> onPut;
 
     std::function<void(std::unique_ptr<server::ExecOp>&&)> onGet;
 
     INST_COUNTER(ServerGPR);
 };
+DEFINE_INST_COUNTER(ServerGPR);
 
 
 struct ServerGPRConnect : public server::ConnectOp
 {
     ServerGPRConnect(ServerConn* conn,
                      pva_app_msg_t cmd,
                      const std::weak_ptr<server::Server::Pvt>& server,
@@ -242,14 +243,15 @@
     }
 
     const std::weak_ptr<server::Server::Pvt> server;
     const std::weak_ptr<ServerGPR> op;
 
     INST_COUNTER(ServerGPRConnect);
 };
+DEFINE_INST_COUNTER(ServerGPRConnect);
 
 struct ServerGPRExec : public server::ExecOp
 {
     ServerGPRExec(ServerConn* conn,
                   pva_app_msg_t cmd,
                   const std::weak_ptr<server::Server::Pvt>& server,
                   const std::string& name,
@@ -313,14 +315,15 @@
     }
 
     const std::weak_ptr<server::Server::Pvt> server;
     const std::weak_ptr<ServerGPR> op;
 
     INST_COUNTER(ServerGPRExec);
 };
+DEFINE_INST_COUNTER(ServerGPRExec);
 
 } // namespace
 
 void ServerConn::handle_GPR(pva_app_msg_t cmd)
 {
     auto rxlen = 8u + evbuffer_get_length(segBuf.get());
     EvInBuf M(peerBE, segBuf.get(), 16);
```

### Comparing `pvxslibs-1.1.4a1/src/serverintrospect.cpp` & `pvxslibs-1.2.0a1/src/serverintrospect.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     void show(std::ostream& strm) const override final
     {
         strm<<"INFO\n";
     }
 
     INST_COUNTER(ServerIntrospect);
 };
+DEFINE_INST_COUNTER(ServerIntrospect);
 
 struct ServerIntrospectControl : public server::ConnectOp
 {
     ServerIntrospectControl(ServerConn *conn, ServerChan *chan,
                             const std::weak_ptr<server::Server::Pvt>& server,
                             const std::weak_ptr<ServerIntrospect>& op)
         :server::ConnectOp(chan->name, conn->cred, Info, Value()) // TODO: pvRequest?
@@ -113,14 +114,15 @@
     virtual void onPut(std::function<void(std::unique_ptr<server::ExecOp>&& fn, Value&&)>&& fn) override final {}
 
     const std::weak_ptr<server::Server::Pvt> server;
     const std::weak_ptr<ServerIntrospect> op;
 
     INST_COUNTER(ServerIntrospectControl);
 };
+DEFINE_INST_COUNTER(ServerIntrospectControl);
 } // namespace
 
 void ServerConn::handle_GET_FIELD()
 {
     // aka. GetField
 
     auto rxlen = 8u + evbuffer_get_length(segBuf.get());
```

### Comparing `pvxslibs-1.1.4a1/src/servermon.cpp` & `pvxslibs-1.2.0a1/src/servermon.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -57,18 +57,21 @@
     // Further members can only be changed from the accepter worker thread with this lock held.
     // They may be read from the worker, or if this lock is held.
     mutable epicsMutex lock;
 
     // is doReply() scheduled to run
     bool scheduled=false;
     bool pipeline=false;
+    // finish() called
     bool finished=false;
-    size_t window=0u, limit=1u;
+    size_t window=0u, limit=4u;
     size_t low=0u, high=0u;
+    size_t ackAt=1u;
     size_t maxQueue=0u;
+    size_t nSquash=0u;
 
     std::deque<Value> queue;
 
     INST_COUNTER(MonitorOp);
 
     // caller must hold lock.
     // only used after State==Idle
@@ -92,14 +95,16 @@
                 } else {
                     // connection TX queue is too full
                     conn->backlog.push_back(std::bind(&MonitorOp::doReply, op));
                 }
             });
 
             op->scheduled = true;
+        } else {
+            log_debug_printf(connio, "Skip reply%s", "\n");
         }
     }
 
     void doReply()
     {
         auto ch = chan.lock();
         if(!ch)
@@ -107,30 +112,35 @@
         auto conn = ch->conn.lock();
         if(!conn || !conn->connection())
             return;
 
         Guard G(lock);
         scheduled = false;
 
+        log_debug_printf(connio, "%s state=%d\n", __func__, state);
+
         if(state==Dead)
             return;
 
         uint8_t subcmd = 0u;
         if(state==Creating) {
             subcmd = 0x08;
             state = type ? Idle : Dead;
 
         } else if(state==Executing) {
-            if(queue.empty() || (pipeline && !window)) {
+            if(queue.empty() || (pipeline && !window && !finished)) {
+                log_debug_printf(connio, "Client %s IOID %u done reply\n",
+                                 conn->peerName.c_str(), unsigned(ioid));
                 return; // nothing to do
 
             } else if(!queue.front()) {
-                finished = true;
                 subcmd = 0x10;
                 state = Dead;
+                log_debug_printf(connio, "Client %s IOID %u finishes\n",
+                                 conn->peerName.c_str(), unsigned(ioid));
             }
         }
 
         {
             (void)evbuffer_drain(conn->txBody.get(), evbuffer_get_length(conn->txBody.get()));
 
             EvOutBuf R(conn->sendBE, conn->txBody.get());
@@ -165,30 +175,34 @@
         if(state == ServerOp::Dead) {
             cleanup();
             return;
         }
 
         auto self(shared_from_this());
 
-        if(state==Executing && pipeline) {
-            assert(window); // previously tested
+        if(state==Executing && pipeline && window) {
 
             window--;
 
             if(!lowMarkPending && window <= low && onLowMark) {
                 lowMarkPending = true;
                 conn->iface->server->acceptor_loop.dispatch([self]() {
-                    self->lowMarkPending = false;
-                    if(self->onLowMark)
-                        self->onLowMark();
+                    decltype (self->onLowMark) fn;
+                    {
+                        Guard G(self->lock);
+                        self->lowMarkPending = false;
+                        fn = self->onLowMark;
+                    }
+                    if(fn)
+                        fn();
                 });
             }
         }
 
-        if(state==Executing && !queue.empty() && (!pipeline || window)) {
+        if(state==Executing && !queue.empty() && (!pipeline || window || finished)) {
             // reschedule myself
             assert(!scheduled); // we've been holding the lock, so this should not have changed
 
             conn->iface->server->acceptor_loop.dispatch([self]() {
                 self->doReply();
             });
             scheduled = true;
@@ -196,14 +210,15 @@
     }
 
     void show(std::ostream& strm) const override final
     {
         strm<<"MONITOR\n";
     }
 };
+DEFINE_INST_COUNTER(MonitorOp);
 
 struct ServerMonitorSetup;
 
 struct ServerMonitorControl : public server::MonitorControlOp
 {
     ServerMonitorControl(ServerMonitorSetup* setup,
                      const std::weak_ptr<server::Server::Pvt>& server,
@@ -222,28 +237,33 @@
         if(val && mon->type && mon->type.get()!=Value::Helper::desc(val))
             throw std::logic_error("Type change not allowed in post().  Recommend pvxs::Value::cloneEmpty()");
 
         // pvMask is const at this point, so no need to lock
         bool real = testmask(val, mon->pvMask);
 
         Guard G(mon->lock);
-        if(real) {
+        if(mon->finished)
+            throw std::logic_error("Already finish()'d"); // TODO fail soft
+
+        if(real || !val) {
 
             if((mon->queue.size() < mon->limit) || force || !val) {
+
+                mon->finished = !val;
                 mon->queue.push_back(val);
 
                 if(mon->maxQueue < mon->queue.size())
                     mon->maxQueue = mon->queue.size();
 
             } else if(!maybe) {
                 // squash
                 assert(mon->limit>0 && !mon->queue.empty());
 
                 mon->queue.back().assign(val);
-                // TODO track overrun
+                mon->nSquash++;
 
             } else {
                 // nope
             }
 
             if(auto serv = server.lock())
                 MonitorOp::maybeReply(serv.get(), mon);
@@ -264,32 +284,34 @@
         stat.finished = mon->finished;
         stat.pipeline = mon->pipeline;
 
         stat.nQueue = mon->queue.size();
         stat.maxQueue = mon->maxQueue;
         stat.limitQueue = mon->limit;
         stat.window = mon->window;
+        stat.nQueue = mon->nSquash;
 
         if(reset)
-            stat.maxQueue = 0u;
+            mon->maxQueue = mon->nSquash = 0u;
     }
 
     virtual void setWatermarks(size_t low, size_t high) override final
     {
         if(low > high)
             throw std::logic_error("low must be <= high");
 
         auto serv = server.lock();
         if(!serv)
             return;
         serv->acceptor_loop.call([this, low, high](){
             if(auto oper = op.lock()) {
                 Guard G(oper->lock);
-                oper->low = low;
-                oper->high = high;
+                oper->low = std::min(low, oper->ackAt-1u);
+                oper->high = std::min(high, oper->ackAt-1u);
+                log_debug_printf(connsetup, "setWatermarks(%zu, %zu)", oper->low, oper->high);
                 // TODO handle change of levels after start
             }
         });
     }
     virtual void onStart(std::function<void (bool)> &&fn) override final
     {
         auto serv = server.lock();
@@ -322,14 +344,15 @@
     }
 
     const std::weak_ptr<server::Server::Pvt> server;
     const std::weak_ptr<MonitorOp> op;
 
     INST_COUNTER(ServerMonitorControl);
 };
+DEFINE_INST_COUNTER(ServerMonitorControl);
 
 struct ServerMonitorSetup : public server::MonitorSetupOp
 {
     ServerMonitorSetup(ServerConn* conn,
                      const std::weak_ptr<server::Server::Pvt>& server,
                      const std::string& name,
                      const Value& request,
@@ -397,14 +420,15 @@
     }
 
     const std::weak_ptr<server::Server::Pvt> server;
     const std::weak_ptr<MonitorOp> op;
 
     INST_COUNTER(ServerMonitorSetup);
 };
+DEFINE_INST_COUNTER(ServerMonitorSetup);
 
 
 ServerMonitorControl::ServerMonitorControl(ServerMonitorSetup* setup,
                                            const std::weak_ptr<server::Server::Pvt>& server,
                                            const std::string& name,
                                            const std::weak_ptr<MonitorOp>& op)
     :server::MonitorControlOp(name, setup->credentials(), Info)
@@ -453,22 +477,52 @@
         }
         chan->statRx += rxlen;
 
         auto op(std::make_shared<MonitorOp>(chan, ioid));
         op->window = nack;
         (void)pvRequest["record._options.pipeline"].as(op->pipeline);
 
-        pvRequest["record._options.queueSize"].as<size_t>([&op](size_t qSize){
-            if(qSize>1)
-                op->limit = qSize;
+        pvRequest["record._options.queueSize"].as<uint32_t>([&op](size_t qSize){
+            op->limit = qSize;
         });
 
         if(op->limit < op->window)
             op->limit = op->window;
 
+        if(!op->limit)
+            op->limit = 1u;
+
+        auto ackAny = pvRequest["record._options.ackAny"];
+        if(ackAny.type()==TypeCode::String) {
+            auto sval = ackAny.as<std::string>();
+            if(sval.size()>1 && sval.back()=='%') {
+                try {
+                    auto percent = parseTo<double>(sval.substr(0, sval.size()-1u));
+                    op->ackAt = std::max(0.0, std::min(percent, 100.0)) * op->limit;
+                }catch(std::exception&){
+                    log_warn_printf(connio, "Error parsing as percent ackAny: \"%s\"\n", sval.c_str());
+                }
+            }
+
+        }
+
+        if(op->ackAt==0u){
+            uint32_t count=0u;
+
+            if(ackAny.as(count)) {
+                op->ackAt = count;
+            }
+        }
+
+        if(op->ackAt==0u){
+            op->ackAt = op->limit/2u;
+        }
+
+        op->ackAt = std::max<size_t>(1u, std::min(op->ackAt, op->limit));
+
         std::unique_ptr<ServerMonitorSetup> ctrl(new ServerMonitorSetup(this, iface->server->internal_self, chan->name, pvRequest, op));
 
         op->state = ServerOp::Creating;
 
         opByIOID[ioid] = op;
         chan->opByIOID[ioid] = op;
 
@@ -524,30 +578,38 @@
             return;
         }
         chan->statRx += rxlen;
 
         // pvAccessCPP won't accept ack and start/stop in the same message,
         // although it will accept destroy in any !INIT message.
         // We do accept ack+start/stop as there is no reason not to.
-        if(subcmd&0x80 && op->pipeline) { // ack
+        if((subcmd&0x80) && op->pipeline) { // ack
 
             Guard G(op->lock);
 
-            log_debug_printf(connio, "Client %s IOID %u acks %u, %u/%u\n",
+            log_debug_printf(connio, "Client %s IOID %u acks %u, %u/%u%s%s\n",
                        peerName.c_str(), unsigned(ioid), unsigned(nack),
-                             unsigned(op->window), unsigned(op->high));
+                             unsigned(op->window), unsigned(op->high),
+                             op->highMarkPending ? " pend" : "",
+                             op->finished ? " fin" : "");
 
             op->window += nack;
 
-            if(!op->highMarkPending && op->window > op->high && op->onHighMark) {
+            if(!op->highMarkPending && op->window > op->high && op->onHighMark && !op->finished) {
                 op->highMarkPending = true;
                 iface->server->acceptor_loop.dispatch([op](){
-                    op->highMarkPending = false;
-                    if(op->onHighMark)
-                        op->onHighMark();
+                    decltype(op->onHighMark) fn;
+                    {
+                        Guard G(op->lock);
+                        op->highMarkPending = false;
+                        if(!op->finished)
+                            fn = op->onHighMark;
+                    }
+                    if(fn)
+                        fn();
                 });
             }
         }
 
         if(subcmd&0x04) {
             bool start = subcmd&0x40;
```

### Comparing `pvxslibs-1.1.4a1/src/serversource.cpp` & `pvxslibs-1.2.0a1/src/serversource.cpp`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/sharedarray.cpp` & `pvxslibs-1.2.0a1/src/sharedarray.cpp`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/sharedpv.cpp` & `pvxslibs-1.2.0a1/src/sharedpv.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,15 @@
                             conn->name().c_str(), conn->peerName().c_str(), e.what());
             // not re-throwing for consistency
             // we couldn't deliver an error after pending
             conn->error(e.what());
         }
     }
 };
+DEFINE_INST_COUNTER2(SharedPV::Impl, SharedPVImpl);
 
 SharedPV SharedPV::buildMailbox()
 {
     SharedPV ret;
     ret.impl = std::make_shared<Impl>();
 
     ret.onPut([](SharedPV& pv, std::unique_ptr<ExecOp>&& op, Value&& val) {
```

### Comparing `pvxslibs-1.1.4a1/src/type.cpp` & `pvxslibs-1.2.0a1/src/type.cpp`

 * *Files identical despite different names*

### Comparing `pvxslibs-1.1.4a1/src/udp_collector.cpp` & `pvxslibs-1.2.0a1/src/udp_collector.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 
 
 namespace pvxs {namespace impl {
 
 DEFINE_LOGGER(logio, "pvxs.udp.io");
 DEFINE_LOGGER(logsetup, "pvxs.udp.setup");
 
+DEFINE_INST_COUNTER(UDPListener);
+
 struct UDPCollector final : public UDPManager::Search,
                             public std::enable_shared_from_this<UDPCollector>
 {
     UDPManager::Pvt* const manager;
     SockAddr bind_addr; // address our socket is bound to
     SockEndpoint lo_mcast_addr; // destination endpoint for local mcast forwarding
     SockAddr lo_addr;
@@ -55,16 +57,16 @@
 
     void addListener(UDPListener *l);
     void delListener(UDPListener *l);
 
     bool handle_one();
 
     enum origin_t {
-        Remote,    // received from interface other than loopback
-        Loopback,  // received through loopback
+        Remote,    // non-local sender
+        Local,     // sent from a local interface, including loopback
         OriginTag, // payload of CMD_ORIGIN_TAG
     };
 
     void process_one(const SockAddr& dest, const uint8_t* buf, size_t nrx, origin_t origin);
     static void handle_static(evutil_socket_t fd, short ev, void *raw)
     {
         (void)fd;
@@ -257,15 +259,15 @@
         log_debug_printf(logio, "Ignoring UDP with mcast source %s.\n", src.tostring().c_str());
         return true;
     }
 
     log_hex_printf(logio, Level::Debug, rxbuf, nrx, "UDP Rx %d, %s -> %s @%u (%s)\n",
             nrx, src.tostring().c_str(), dest.tostring().c_str(), unsigned(rx.dstif), bind_addr.tostring().c_str());
 
-    origin_t origin = manager->ifmap.has_address(rx.dstif, lo_addr) ? Loopback : Remote;
+    origin_t origin = manager->ifmap.is_iface(src) ? Local : Remote;
 
     process_one(dest, rxbuf, nrx, origin);
     return true;
 }
 
 void UDPCollector::process_one(const SockAddr &dest, const uint8_t *buf, size_t nrx, origin_t origin)
 {
@@ -312,26 +314,36 @@
             if(origin==OriginTag) {
                 log_err_printf(logio, "CMD_ORIGIN_TAG search with reply to sender never works%s", "\n");
                 return;
             }
         }
         server.setPort(port);
 
-        if(M.good() && origin==Loopback && (flags&pva_search_flags::Unicast) && dest.family()==AF_INET) {
+        if(!M.good() || !(flags&pva_search_flags::Unicast) || dest.family()!=AF_INET) {
+            // invalid, bcast, or not ipv4
+
+        } else if(dest.compare(lo_mcast_addr.addr,false)!=0) {
             assert(buf==&this->buf[cmd_origin_tag_size]);
             // clear unicast flag in forwarded message
             *save_flags &= ~pva_search_flags::Unicast;
             // recipient of forwarded message must use, and trust, replyAddr in body :(
             {
                 FixedBuf R(M.be, save_replyAddr, 16u);
                 to_wire(R, server);
                 assert(R.good());
             }
             forwardM(dest, buf, nrx);
             return;
+
+        } else {
+            /* refuse to re-forward.  Also, if received via. localhost as
+             * some PVA implementations don't prefix forwarded messages with CMD_ORIGIN_TAG
+             */
+            log_debug_printf(logio, "Ignore as originated for %s\n",
+                             dest.tostring().c_str());
         }
 
         // so far, only "tcp" transport has ever been seen.
         // however, we will pass through others which might appear
         otherproto.clear();
         Size nproto{0};
         from_wire(M, nproto);
@@ -418,30 +430,29 @@
 
     case CMD_ORIGIN_TAG: {
         SockAddr originaddr; // aka. original destination
         from_wire(M, originaddr);
         M.skip(head.len-16u, __FILE__, __LINE__);
 
         // only allow one CMD_ORIGIN_TAG message per packet
-        // only accept when sent to the mcast address from the loopback address
+        // only accept when sent to the mcast address through the loopback address
         //   since we only join the mcast group on loopback this will hopefully
         //   frustrate attempts to inject CMD_ORIGIN_TAG externally.
-        if(M.good() && origin==Loopback && dest.compare(lo_mcast_addr.addr,false)==0 && src.isLO()) {
+        if(M.good() && origin==Local && dest.compare(lo_mcast_addr.addr,false)==0) {
             originaddr.setPort(bind_addr.port());
 
             process_one(originaddr, M.save(), M.size(), OriginTag);
 
             return;
         }
-        log_debug_printf(logio, "Ignore originated from %s %c%c%c%c\n",
+        log_debug_printf(logio, "Ignore originated from %s %c%c%c\n",
                          originaddr.tostring().c_str(),
                          M.good() ? 'T' : 'F',
-                         origin==Loopback ? 'T' : 'F',
-                         dest.compare(lo_mcast_addr.addr,false)==0 ? 'T' : 'F',
-                         src.isLO() ? 'T' : 'F');
+                         origin==Local ? 'T' : 'F',
+                         dest.compare(lo_mcast_addr.addr,false)==0 ? 'T' : 'F');
 
         break;
     }
 
     default:
         break; // ignore unknown
     }
@@ -511,26 +522,30 @@
 void collector_init(void *unused)
 {
     (void)unused;
     udp_gbl = new udp_gbl_t;
 }
 } // namespace
 
-UDPManager UDPManager::instance()
+UDPManager UDPManager::instance(bool share)
 {
     threadOnce(&collector_once, &collector_init, nullptr);
     assert(udp_gbl);
 
     Guard G(udp_gbl->lock);
 
-    auto ret = udp_gbl->inst.lock();
+    std::shared_ptr<UDPManager::Pvt> ret;
+
+    if(share)
+        ret = udp_gbl->inst.lock();
 
     if(!ret) {
         ret.reset(new UDPManager::Pvt);
-        udp_gbl->inst = ret;
+        if(share)
+            udp_gbl->inst = ret;
     }
 
     return UDPManager(ret);
 }
 
 void UDPManager::cleanup()
 {
```

### Comparing `pvxslibs-1.1.4a1/src/udp_collector.h` & `pvxslibs-1.2.0a1/src/udp_collector.h`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 //! Manage reception, fanout, and reply of UDP PVA on the well known port.
 struct PVXS_API UDPManager
 {
     SockAttach attach;
 
     //! get process-wide singleton.
-    static UDPManager instance();
+    static UDPManager instance(bool share=true);
     static void cleanup();
     ~UDPManager();
 
     evbase& loop();
 
     struct Beacon {
         const SockAddr& src;
@@ -77,15 +77,15 @@
     std::unique_ptr<UDPListener> onSearch(SockAddr& dest,
                                           std::function<void(const Search&)>&& cb);
 
     void sync();
 
     explicit operator bool() const { return !!pvt; }
 
-    UDPManager();
+    UDPManager() = default;
 
     struct Pvt;
 private:
     explicit inline UDPManager(const std::shared_ptr<Pvt>& pvt) :pvt(pvt) {}
     std::shared_ptr<Pvt> pvt;
     friend class UDPListener;
     friend struct UDPCollector;
```

### Comparing `pvxslibs-1.1.4a1/src/unittest.cpp` & `pvxslibs-1.2.0a1/src/unittest.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 /**
  * Copyright - See the COPYRIGHT that is included with this distribution.
  * pvxs is distributed subject to a Software License Agreement found
  * in file LICENSE that is included with this distribution.
  */
 
+#include <atomic>
+
 #include "pvxs/version.h"
 
 #if !defined(GCC_VERSION) || GCC_VERSION>VERSION_INT(4,9,0,0)
 #  include <regex>
 
 #else
 // GCC 4.8 provides the regex header and symbols, but with a no-op implementation
@@ -25,27 +27,35 @@
 
 #include "pvxs/unittest.h"
 #include "utilpvt.h"
 #include "udp_collector.h"
 
 namespace pvxs {
 
+static std::atomic<bool> thisIsATest{false};
+
 void testSetup()
 {
 #ifdef _WIN32
     // One of the SEM_* options, either SEM_FAILCRITICALERRORS or SEM_NOGPFAULTERRORBOX,
     // depending on who you ask, acts to disable Windows Error Reporting entirely.
     // This also prevents the AeDebug facility from triggering.
     UINT prev = SetErrorMode(0);
     if(prev)
         testDiag("SetErrorMode() disables 0x%x\n", (unsigned)prev);
 #endif
+    thisIsATest = true;
 }
 
 namespace impl {
+bool inUnitTest()
+{
+    return thisIsATest;
+}
+
 loc_bad_alloc::loc_bad_alloc(const char *file, int line)
 {
     if(auto sep = strrchr(file, '/')) {
         file = sep+1;
     }
 #ifdef _WIN32
     if(auto sep = strrchr(file, '\\')) {
```

### Comparing `pvxslibs-1.1.4a1/src/util.cpp` & `pvxslibs-1.2.0a1/src/util.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -74,26 +74,56 @@
 }
 
 unsigned long version_abi_int()
 {
     return PVXS_ABI_VERSION;
 }
 
+namespace {
+epicsThreadOnceId ICountOnce = EPICS_THREAD_ONCE_INIT;
+struct ICountGbl_t {
+    RWLock lock;
+    std::map<std::string, std::atomic<size_t>*> counters;
+} *ICountGbl;
 
-#define CASE(KLASS) std::atomic<size_t> cnt_ ## KLASS{}
-#include "instcounters.h"
-#undef CASE
+void ICountInit(void*)
+{
+    ICountGbl = new ICountGbl_t;
+}
+
+} // namespace
+
+void registerICount(const char *name, std::atomic<size_t>& Cnt)
+{
+    epicsThreadOnce(&ICountOnce, &ICountInit, nullptr);
+    auto& gbl = *ICountGbl;
+    try {
+        auto L(gbl.lock.lockWriter());
+        if(!gbl.counters.emplace(name, &Cnt).second) { // duplicate name
+            return;
+        }
+    } catch(std::exception& e) { // bad_alloc
+        return;
+    }
+    Cnt++; // bias by +1 to indicate initialization
+}
 
 std::map<std::string, size_t> instanceSnapshot()
 {
     std::map<std::string, size_t> ret;
 
-#define CASE(KLASS) ret[#KLASS] = cnt_ ## KLASS .load(std::memory_order_relaxed)
-#include "instcounters.h"
-#undef CASE
+    {
+        epicsThreadOnce(&ICountOnce, &ICountInit, nullptr);
+        auto& gbl = *ICountGbl;
+        auto L(gbl.lock.lockReader());
+        for(auto& pair : gbl.counters) {
+            // remove -1 bias for initialized counter
+            ret.emplace(pair.first, pair.second->load(std::memory_order_relaxed)-1u);
+        }
+    }
 
     return ret;
 }
 
 // _assume_ only positive indices will be used
 static
 std::atomic<int> indentIndex{INT_MIN};
```

### Comparing `pvxslibs-1.1.4a1/src/utilpvt.h` & `pvxslibs-1.2.0a1/src/utilpvt.h`

 * *Files 11% similar despite different names*

```diff
@@ -52,14 +52,17 @@
 template<typename T>
 struct promote_print { static T op(const T& v) { return v; }};
 template<>
 struct promote_print<int8_t> { static int op(const char& v) { return v; }};
 template<>
 struct promote_print<uint8_t> { static unsigned op(const char& v) { return v; }};
 
+PVXS_API
+bool inUnitTest();
+
 /* specialization of bad_alloc which notes the location from which
  * the exception originates.
  */
 struct PVXS_API loc_bad_alloc final : public std::bad_alloc
 {
     loc_bad_alloc(const char *file, int line);
     virtual ~loc_bad_alloc();
@@ -237,14 +240,18 @@
 {
     timeval ret;
     ret.tv_sec = t;
     ret.tv_usec = (t - ret.tv_sec)*1e6;
     return ret;
 }
 
+namespace ioc {
+void IOCGroupConfigCleanup();
+}
+
 //! Scoped restore of std::ostream state (format flags, fill char, and field width)
 struct Restore {
     std::ostream& strm;
     std::ios_base::fmtflags pflags;
     std::ostream::char_type pfill;
     std::streamsize pwidth;
     Restore(std::ostream& strm)
@@ -256,23 +263,32 @@
     ~Restore() {
         strm.flags(pflags);
         strm.fill(pfill);
         strm.width(pwidth);
     }
 };
 
-template<std::atomic<size_t>* Cnt>
-struct InstCounter
-{
-    InstCounter() {(*Cnt).fetch_add(1, std::memory_order_relaxed);}
-    ~InstCounter() {(*Cnt).fetch_sub(1, std::memory_order_relaxed);}
-};
+PVXS_API
+void registerICount(const char* name, std::atomic<size_t>& Cnt);
 
-#define INST_COUNTER(KLASS) InstCounter<&cnt_ ## KLASS> instances
+// Name and Cnt must have global lifetime
+template<std::atomic<size_t>& Cnt>
+struct InstCounter {
+    explicit InstCounter(const char* Name) {
+        if(0u==Cnt.fetch_add(1u, std::memory_order_relaxed)) { // first
+            registerICount(Name, Cnt);
+        }
+    }
+    ~InstCounter() {
+        Cnt.fetch_sub(1u, std::memory_order_relaxed);
+    }
+};
 
-#define CASE(KLASS) PVXS_API extern std::atomic<size_t> cnt_ ## KLASS
-#include "instcounters.h"
-#undef CASE
+#define INST_COUNTER(KLASS) \
+                    static std::atomic<size_t> cnt_ ## KLASS; \
+                    InstCounter<cnt_ ## KLASS> instances{#KLASS}
+#define DEFINE_INST_COUNTER2(KLASS, NAME) std::atomic<size_t> KLASS::cnt_ ## NAME {0u}
+#define DEFINE_INST_COUNTER(KLASS) DEFINE_INST_COUNTER2(KLASS, KLASS)
 
 } // namespace pvxs
 
 #endif // UTILPVT_H
```

