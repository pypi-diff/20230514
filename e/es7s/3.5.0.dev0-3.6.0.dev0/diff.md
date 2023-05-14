# Comparing `tmp/es7s-3.5.0.dev0.tar.gz` & `tmp/es7s-3.6.0.dev0.tar.gz`

## Comparing `es7s-3.5.0.dev0.tar` & `es7s-3.6.0.dev0.tar`

### file list

```diff
@@ -1,129 +1,140 @@
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/_version.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/__init__.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/__main__.py
--rw-r--r--   0        0        0    24503 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/_base.py
--rw-r--r--   0        0        0    31588 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/_base_monitor.py
--rw-r--r--   0        0        0     9993 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/_entrypoint.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/exec_get_socket.py
--rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/exec_hilight_num.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/exec_list_commands.py
--rw-r--r--   0        0        0    14484 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/exec_list_dir.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/exec_notify.py
--rw-r--r--   0        0        0     5914 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/exec_sun.py
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/exec_wrap.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/group_config.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/group_exec.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/group_manage.py
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/group_monitor.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/group_print.py
--rw-r--r--   0        0        0    10289 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/monitor_battery.py
--rw-r--r--   0        0        0     6990 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/monitor_combined.py
--rw-r--r--   0        0        0     5580 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/monitor_cpu_freq.py
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/monitor_cpu_load.py
--rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/monitor_cpu_load_avg.py
--rw-r--r--   0        0        0     4111 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/monitor_datetime.py
--rw-r--r--   0        0        0     6156 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/monitor_disk_usage.py
--rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/monitor_docker.py
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/monitor_fan_speed.py
--rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/monitor_memory.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/monitor_network_country.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/monitor_network_latency.py
--rw-r--r--   0        0        0     6210 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/monitor_temperature.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/monitor_timestamp.py
--rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/monitor_weather.py
--rw-r--r--   0        0        0     9803 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/options.py
--rwxr-xr-x   0        0        0    29644 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/print-tmux-keys.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/print_printscr.txt
--rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/print_regex.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/print_static.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/cli/print_weather_icons.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/d/__init__.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/d/__main__.py
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/d/_base.py
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/d/_entrypoint.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/d/factory.py
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/d/provider_battery.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/d/provider_cpu.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/d/provider_datetime.py
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/d/provider_disk_usage.py
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/d/provider_docker.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/d/provider_fan_speed.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/d/provider_memory.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/d/provider_network_country.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/d/provider_network_latency.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/d/provider_temperature.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/d/provider_timestamp.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/d/provider_weather.py
--rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/control-codes.yml
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/demo-text.txt
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/es7s.conf.d
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/external-apps.yml
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/cpuload-0.svg
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/cpuload-12.svg
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/cpuload-25.svg
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/cpuload-37.svg
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/cpuload-50.svg
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/cpuload-62.svg
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/cpuload-75.svg
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/cpuload-87.svg
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/cpuload-95.svg
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/memory-0.svg
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/memory-10.svg
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/memory-20.svg
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/memory-30.svg
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/memory-40.svg
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/memory-50.svg
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/memory-60.svg
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/memory-70.svg
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/memory-80.svg
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/memory-90.svg
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/memory-95.svg
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/temperature-0.svg
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/temperature-10.svg
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/temperature-30.svg
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/temperature-50.svg
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/temperature-70.svg
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/temperature-80.svg
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-v7/temperature-90.svg
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-vitals/battery-symbolic.svg
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-vitals/cpu-symbolic.svg
--rw-r--r--   0        0        0     5486 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-vitals/fan-symbolic.svg
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-vitals/memory-symbolic.svg
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-vitals/network-download-symbolic.svg
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-vitals/network-symbolic.svg
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-vitals/network-upload-symbolic.svg
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-vitals/storage-symbolic.svg
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-vitals/system-symbolic.svg
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-vitals/temperature-symbolic.svg
--rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/data/icons-vitals/voltage-symbolic.svg
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/gtk/__init__.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/gtk/__main__.py
--rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/gtk/_base.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/gtk/_entrypoint.py
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/gtk/indicator_cpu_load.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/gtk/indicator_datetime.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/gtk/indicator_memory.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/gtk/indicator_temperature.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/shared/__init__.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/shared/color.py
--rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/shared/config.py
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/shared/dto.py
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/shared/io.py
--rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/shared/ipc.py
--rw-r--r--   0        0        0    13148 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/shared/log.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/shared/prefixed_unit.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/shared/separator.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/shared/spinner.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/shared/styles.py
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/shared/sub.py
--rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/shared/sun_calc.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/shared/system.py
--rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/shared/threads.py
--rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/es7s/shared/weather_icons.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/tests/__init__.py
--rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/tests/test_cli.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/.gitignore
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/README.md
--rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 es7s-3.5.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/_version.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/__init__.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/__main__.py
+-rw-r--r--   0        0        0    24503 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/_base.py
+-rw-r--r--   0        0        0    31588 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/_base_monitor.py
+-rw-r--r--   0        0        0     9993 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/_entrypoint.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/exec_get_socket.py
+-rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/exec_hilight_num.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/exec_list_commands.py
+-rw-r--r--   0        0        0    14484 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/exec_list_dir.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/exec_notify.py
+-rw-r--r--   0        0        0     5914 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/exec_sun.py
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/exec_wrap.py
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/group_config.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/group_exec.py
+-rw-r--r--   0        0        0     5312 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/group_manage.py
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/group_monitor.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/group_print.py
+-rw-r--r--   0        0        0    10289 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/monitor_battery.py
+-rw-r--r--   0        0        0     6990 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/monitor_combined.py
+-rw-r--r--   0        0        0     5580 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/monitor_cpu_freq.py
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/monitor_cpu_load.py
+-rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/monitor_cpu_load_avg.py
+-rw-r--r--   0        0        0     4111 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/monitor_datetime.py
+-rw-r--r--   0        0        0     6156 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/monitor_disk_usage.py
+-rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/monitor_docker.py
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/monitor_fan_speed.py
+-rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/monitor_memory.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/monitor_network_country.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/monitor_network_latency.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/monitor_network_tunnel.py
+-rw-r--r--   0        0        0     6210 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/monitor_temperature.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/monitor_timestamp.py
+-rw-r--r--   0        0        0     8877 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/monitor_weather.py
+-rw-r--r--   0        0        0     9803 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/options.py
+-rwxr-xr-x   0        0        0    29644 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/print-tmux-keys.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/print_printscr.txt
+-rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/print_regex.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/print_static.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/cli/print_weather_icons.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/d/__init__.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/d/__main__.py
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/d/_base.py
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/d/_entrypoint.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/d/factory.py
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/d/provider_battery.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/d/provider_cpu.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/d/provider_datetime.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/d/provider_disk_usage.py
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/d/provider_docker.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/d/provider_fan_speed.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/d/provider_memory.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/d/provider_network_country.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/d/provider_network_latency.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/d/provider_network_tunnel.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/d/provider_shocks.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/d/provider_temperature.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/d/provider_timestamp.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/d/provider_weather.py
+-rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/control-codes.yml
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/demo-text.txt
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/es7s.conf.d
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/external-apps.yml
+-rwxr-xr-x   0        0        0     1742 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/bin/shocks
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/cpuload-0.svg
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/cpuload-12.svg
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/cpuload-25.svg
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/cpuload-37.svg
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/cpuload-50.svg
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/cpuload-62.svg
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/cpuload-75.svg
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/cpuload-87.svg
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/cpuload-95.svg
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/memory-0.svg
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/memory-10.svg
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/memory-20.svg
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/memory-30.svg
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/memory-40.svg
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/memory-50.svg
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/memory-60.svg
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/memory-70.svg
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/memory-80.svg
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/memory-90.svg
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/memory-95.svg
+-rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/shocks-down.svg
+-rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/shocks-failure.orig.svg
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/shocks-failure.svg
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/shocks-up.svg
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/shocks.svg
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/temperature-0.svg
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/temperature-10.svg
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/temperature-30.svg
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/temperature-50.svg
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/temperature-70.svg
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/temperature-80.svg
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-v7/temperature-90.svg
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-vitals/battery-symbolic.svg
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-vitals/cpu-symbolic.svg
+-rw-r--r--   0        0        0     5486 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-vitals/fan-symbolic.svg
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-vitals/memory-symbolic.svg
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-vitals/network-download-symbolic.svg
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-vitals/network-symbolic.svg
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-vitals/network-upload-symbolic.svg
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-vitals/storage-symbolic.svg
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-vitals/system-symbolic.svg
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-vitals/temperature-symbolic.svg
+-rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/icons-vitals/voltage-symbolic.svg
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/data/systemd/es7s-shocks.service
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/gtk/__init__.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/gtk/__main__.py
+-rw-r--r--   0        0        0     8500 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/gtk/_base.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/gtk/_entrypoint.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/gtk/indicator_cpu_load.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/gtk/indicator_datetime.py
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/gtk/indicator_memory.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/gtk/indicator_shocks.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/gtk/indicator_temperature.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/shared/__init__.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/shared/color.py
+-rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/shared/config.py
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/shared/dto.py
+-rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/shared/io.py
+-rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/shared/ipc.py
+-rw-r--r--   0        0        0    13174 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/shared/log.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/shared/prefixed_unit.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/shared/separator.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/shared/spinner.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/shared/styles.py
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/shared/sub.py
+-rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/shared/sun_calc.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/shared/system.py
+-rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/shared/threads.py
+-rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/es7s/shared/weather_icons.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/tests/__init__.py
+-rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/tests/test_cli.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/.gitignore
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/README.md
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 es7s-3.6.0.dev0/PKG-INFO
```

### Comparing `es7s-3.5.0.dev0/es7s/cli/_base.py` & `es7s-3.6.0.dev0/es7s/cli/_base.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/_base_monitor.py` & `es7s-3.6.0.dev0/es7s/cli/_base_monitor.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/_entrypoint.py` & `es7s-3.6.0.dev0/es7s/cli/_entrypoint.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/exec_get_socket.py` & `es7s-3.6.0.dev0/es7s/cli/exec_get_socket.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/exec_hilight_num.py` & `es7s-3.6.0.dev0/es7s/cli/exec_hilight_num.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/exec_list_commands.py` & `es7s-3.6.0.dev0/es7s/cli/exec_list_commands.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/exec_list_dir.py` & `es7s-3.6.0.dev0/es7s/cli/exec_list_dir.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/exec_notify.py` & `es7s-3.6.0.dev0/es7s/cli/exec_notify.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/exec_sun.py` & `es7s-3.6.0.dev0/es7s/cli/exec_sun.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/exec_wrap.py` & `es7s-3.6.0.dev0/es7s/cli/exec_wrap.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/group_config.py` & `es7s-3.6.0.dev0/es7s/cli/group_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,15 @@
                 stdout.echo()
             stdout.echo_rendered(f"[{section}]", self.HEADER_STYLE)
             for option in config.options(section):
                 option_fmtd = stdout.render(option, self.OPT_NAME_STYLE)
                 value_fmtd = stdout.render(config.get(section, option), self.OPT_VALUE_STYLE)
                 stdout.echo_rendered(option_fmtd + " = " + value_fmtd)
 
+
 @click.option(
     "-p",
     "--prune",
     is_flag=True,
     default=False,
     cls=CommandOption,
     help="Silently overwrite original config, do not make a backup."
@@ -80,27 +81,36 @@
     def __init__(self, prune: bool):
         self._run(prune)
 
     def _run(self, prune: bool):
         reset_config(backup=not prune)
         get_stdout().echo("Config was reset to default")
 
-
+@click.option(
+    "--boolean",
+    is_flag=True,
+    default=False,
+    cls=CommandOption,
+    help='Cast the value to boolean "True" or "False".'
+)
 @group.command("get", cls=CliCommand)
 @click.argument("name")
 @_catch_and_log_and_exit
 class GetCommand:
     """Display config variable value."""
 
-    def __init__(self, name: str):
-        self._run(name)
+    def __init__(self, name: str, boolean: bool):
+        self._run(name, boolean)
 
-    def _run(self, name: str):
+    def _run(self, name: str, boolean: bool):
         section, option = split_name(name)
-        value = get_config().get(section, option)
+        if boolean:
+            value = get_config().getboolean(section, option)
+        else:
+            value = get_config().get(section, option)
         get_stdout().echo(value)
 
 
 @group.command("set", cls=CliCommand)
 @click.argument("name")
 @click.argument("value")
 @_catch_and_log_and_exit
```

### Comparing `es7s-3.5.0.dev0/es7s/cli/group_exec.py` & `es7s-3.6.0.dev0/es7s/cli/group_exec.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/group_monitor.py` & `es7s-3.6.0.dev0/es7s/cli/group_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     monitor_memory,
     monitor_temperature,
     monitor_timestamp,
     monitor_weather,
     monitor_fan_speed,
     monitor_disk_usage,
     monitor_network_country,
-    monitor_network_latency,
+    monitor_network_latency, monitor_network_tunnel,
 )
 from ._base import CliGroup, _catch_and_log_and_exit
 
 
 @click.group(
     name=__file__,
     cls=CliGroup,
@@ -49,13 +49,14 @@
     monitor_cpu_load_avg.invoker,
     monitor_cpu_freq.invoker,
     monitor_disk_usage.invoker,
     monitor_fan_speed.invoker,
     monitor_memory.invoker,
     monitor_network_country.invoker,
     monitor_network_latency.invoker,
+    monitor_network_tunnel.invoker,
     monitor_timestamp.invoker,
     monitor_temperature.invoker,
     monitor_weather.invoker,
 ]
 for command in commands:
     group.add_command(command)
```

### Comparing `es7s-3.5.0.dev0/es7s/cli/group_print.py` & `es7s-3.6.0.dev0/es7s/cli/group_print.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/monitor_battery.py` & `es7s-3.6.0.dev0/es7s/cli/monitor_battery.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/monitor_combined.py` & `es7s-3.6.0.dev0/es7s/cli/monitor_combined.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/monitor_cpu_freq.py` & `es7s-3.6.0.dev0/es7s/cli/monitor_cpu_freq.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/monitor_cpu_load.py` & `es7s-3.6.0.dev0/es7s/cli/monitor_cpu_load.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/monitor_cpu_load_avg.py` & `es7s-3.6.0.dev0/es7s/cli/monitor_cpu_load_avg.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/monitor_datetime.py` & `es7s-3.6.0.dev0/es7s/cli/monitor_datetime.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/monitor_disk_usage.py` & `es7s-3.6.0.dev0/es7s/cli/monitor_disk_usage.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/monitor_docker.py` & `es7s-3.6.0.dev0/es7s/cli/monitor_docker.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/monitor_fan_speed.py` & `es7s-3.6.0.dev0/es7s/cli/monitor_fan_speed.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/monitor_memory.py` & `es7s-3.6.0.dev0/es7s/cli/monitor_memory.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/monitor_network_country.py` & `es7s-3.6.0.dev0/es7s/cli/monitor_network_country.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/monitor_network_latency.py` & `es7s-3.6.0.dev0/es7s/cli/monitor_network_latency.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/monitor_temperature.py` & `es7s-3.6.0.dev0/es7s/cli/monitor_temperature.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/monitor_timestamp.py` & `es7s-3.6.0.dev0/es7s/cli/monitor_timestamp.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/monitor_weather.py` & `es7s-3.6.0.dev0/es7s/cli/monitor_weather.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
     def get_output_width(self) -> int:
         return OUTPUT_WIDTH
 
     def _format_data_impl(self, msg: SocketMessage[WeatherInfo]) -> pt.Text:
         logger = get_logger()
         fields = msg.data.fields
-        logger.trace(fields, "Message data")
+        logger.trace(str(fields), "Message data")
         if len(fields) != 3:
             raise ValueError(f"Malformed response: {fields!s}")
 
         wicon_max_width = self._setup.config.weather_icon_max_width
         wicon_origin = fields[0].strip().removesuffix("\ufe0f")  # U+FE0F VARIATION SELECTOR-16
         wicon, w_term, wicon_st = get_wicon(wicon_origin, self._setup.config.weather_icon_set_id)
         temp_origin = fields[1]
```

### Comparing `es7s-3.5.0.dev0/es7s/cli/options.py` & `es7s-3.6.0.dev0/es7s/cli/options.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/print-tmux-keys.py` & `es7s-3.6.0.dev0/es7s/cli/print-tmux-keys.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/print_printscr.txt` & `es7s-3.6.0.dev0/es7s/cli/print_printscr.txt`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/print_regex.py` & `es7s-3.6.0.dev0/es7s/cli/print_regex.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/print_static.py` & `es7s-3.6.0.dev0/es7s/cli/print_static.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/cli/print_weather_icons.py` & `es7s-3.6.0.dev0/es7s/cli/print_weather_icons.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/d/_base.py` & `es7s-3.6.0.dev0/es7s/d/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,24 +84,29 @@
 
     def _collect(self) -> T:
         raise NotImplementedError()
 
     def _get_request_timeout(self) -> float:
         return max(1.0, self._poll_interval_sec / 2)
 
-    def _make_request(self, url: str, request_fn: t.Callable = None):
+    def _make_request(
+        self,
+        url: str,
+        request_fn: t.Callable[[], requests.Response] = None,
+        log_response_body: bool = True,
+    ) -> requests.Response:
         logger = get_logger()
         try:
             request_id = self._network_request_id.next()
             self._network_req_event.set()
             logger.log_http_request(request_id, url)
             if not request_fn:
                 request_fn = lambda: requests.get(url, timeout=self._get_request_timeout())
             response = request_fn()
-            logger.log_http_response(request_id, response, with_body=True)
+            logger.log_http_response(request_id, response, with_body=log_response_body)
         except requests.exceptions.ConnectionError as e:
             logger.error(e)
             raise DataCollectionError()
         except requests.RequestException as e:
             logger.exception(e)
             raise DataCollectionError()
         finally:
```

### Comparing `es7s-3.5.0.dev0/es7s/d/_entrypoint.py` & `es7s-3.6.0.dev0/es7s/d/_entrypoint.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/d/factory.py` & `es7s-3.6.0.dev0/es7s/d/factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from .provider_datetime import DatetimeProvider
 from .provider_disk_usage import DiskUsageProvider
 from .provider_docker import DockerStatusProvider
 from .provider_fan_speed import FanSpeedProvider
 from .provider_memory import MemoryProvider
 from .provider_network_country import NetworkCountryProvider
 from .provider_network_latency import NetworkLatencyProvider
+from .provider_network_tunnel import NetworkTunnelProvider
+from .provider_shocks import ShocksProvider
 from .provider_temperature import TemperatureProvider
 from .provider_timestamp import TimestampProvider
 from .provider_weather import WeatherProvider
 
 
 class DataProviderFactory:
     @classmethod
@@ -25,12 +27,14 @@
             CpuProvider(),
             DiskUsageProvider(),
             DockerStatusProvider(),
             FanSpeedProvider(),
             MemoryProvider(),
             NetworkCountryProvider(),
             NetworkLatencyProvider(),
+            NetworkTunnelProvider(),
+            ShocksProvider(),
             DatetimeProvider(),
             TemperatureProvider(),
             TimestampProvider(),
             WeatherProvider(),
         ]
```

### Comparing `es7s-3.5.0.dev0/es7s/d/provider_battery.py` & `es7s-3.6.0.dev0/es7s/d/provider_battery.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/d/provider_cpu.py` & `es7s-3.6.0.dev0/es7s/d/provider_cpu.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/d/provider_disk_usage.py` & `es7s-3.6.0.dev0/es7s/d/provider_disk_usage.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/d/provider_docker.py` & `es7s-3.6.0.dev0/es7s/d/provider_docker.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/d/provider_fan_speed.py` & `es7s-3.6.0.dev0/es7s/d/provider_fan_speed.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/d/provider_memory.py` & `es7s-3.6.0.dev0/es7s/d/provider_memory.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/d/provider_network_country.py` & `es7s-3.6.0.dev0/es7s/d/provider_network_country.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/d/provider_network_latency.py` & `es7s-3.6.0.dev0/es7s/d/provider_network_latency.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self._timer = _Timer()
         self._last_results = deque[bool](maxlen=50)
         super().__init__("network-latency", "network-latency", 13.0)
 
     def _reset(self):
         return NetworkLatencyInfo()
 
-    def _collect(self) ->   NetworkLatencyInfo:
+    def _collect(self) -> NetworkLatencyInfo:
         attempts = 4
         timeout = 5
         host = get_config().get('provider.'+self._config_var, 'host')
         port = get_config().getint('provider.'+self._config_var, 'port')
 
         conn_times_s = []
```

### Comparing `es7s-3.5.0.dev0/es7s/d/provider_temperature.py` & `es7s-3.6.0.dev0/es7s/d/provider_temperature.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/d/provider_timestamp.py` & `es7s-3.6.0.dev0/es7s/d/provider_timestamp.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/d/provider_weather.py` & `es7s-3.6.0.dev0/es7s/d/provider_weather.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/control-codes.yml` & `es7s-3.6.0.dev0/es7s/data/control-codes.yml`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/demo-text.txt` & `es7s-3.6.0.dev0/es7s/data/demo-text.txt`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/es7s.conf.d` & `es7s-3.6.0.dev0/es7s/data/es7s.conf.d`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 ######################################
 #  DEFAULT es7s configuration file   #
 #  DO NOT EDIT                       #
 #  Run 'es7s config edit' to set up  #
 ######################################
 
 [general]
-syntax-version = 2.0
+syntax-version = 2.2
 theme-color = blue
 
 [provider]
 battery = on
 cpu = on
 disk = on
 datetime = on
 docker = on
 fan = on
 memory = on
 network-country = on
 network-latency = on
+network-tunnel = on
+shocks = on
 temperature = on
 timestamp = on
 weather = on
 
 [provider.network-latency]
 host = 1.1.1.1
 port = 53
 
+[provider.shocks]
+socks_protocol = socks5
+socks_host = 127.0.0.1
+socks_port = 1080
+check_url = http://1.1.1.1
+
 [provider.timestamp]
 url = https://dlup.link/temp/nalog.mtime
 
 [provider.weather]
 location = MSK
 
 [monitor]
@@ -49,14 +57,16 @@
     es7s.cli.monitor_combined.SPACE
     es7s.cli.monitor_docker.DockerMonitor
 
     es7s.cli.monitor_combined.SPACE
     es7s.cli.monitor_network_latency.NetworkLatencyMonitor
     es7s.cli.monitor_combined.SPACE
     es7s.cli.monitor_network_country.NetworkCountryMonitor
+    es7s.cli.monitor_combined.SPACE_2
+    es7s.cli.monitor_network_tunnel.NetworkTunnelMonitor
     es7s.cli.monitor_combined.SPACE
     es7s.cli.monitor_timestamp.TimestampMonitor
     es7s.cli.monitor_combined.SPACE
     es7s.cli.monitor_weather.WeatherMonitor
 
     es7s.cli.monitor_combined.SPACE_2
     es7s.cli.monitor_datetime.DatetimeMonitor
```

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/cpuload-0.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/cpuload-0.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/cpuload-12.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/cpuload-12.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/cpuload-25.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/cpuload-25.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/cpuload-37.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/cpuload-37.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/cpuload-50.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/cpuload-50.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/cpuload-62.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/cpuload-62.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/cpuload-75.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/cpuload-75.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/cpuload-87.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/cpuload-87.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/cpuload-95.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/cpuload-95.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/memory-0.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/memory-0.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/memory-10.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/memory-10.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/memory-20.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/memory-20.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/memory-30.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/memory-30.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/memory-40.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/memory-40.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/memory-50.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/memory-50.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/memory-60.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/memory-60.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/memory-70.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/memory-70.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/memory-80.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/memory-80.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/memory-90.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/memory-90.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/memory-95.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/memory-95.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/temperature-0.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/temperature-0.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/temperature-10.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/temperature-10.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/temperature-30.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/temperature-30.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/temperature-50.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/temperature-50.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/temperature-70.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/temperature-70.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/temperature-80.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/temperature-80.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-v7/temperature-90.svg` & `es7s-3.6.0.dev0/es7s/data/icons-v7/temperature-90.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-vitals/battery-symbolic.svg` & `es7s-3.6.0.dev0/es7s/data/icons-vitals/battery-symbolic.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-vitals/cpu-symbolic.svg` & `es7s-3.6.0.dev0/es7s/data/icons-vitals/cpu-symbolic.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-vitals/fan-symbolic.svg` & `es7s-3.6.0.dev0/es7s/data/icons-vitals/fan-symbolic.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-vitals/memory-symbolic.svg` & `es7s-3.6.0.dev0/es7s/data/icons-vitals/memory-symbolic.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-vitals/network-download-symbolic.svg` & `es7s-3.6.0.dev0/es7s/data/icons-vitals/network-download-symbolic.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-vitals/network-symbolic.svg` & `es7s-3.6.0.dev0/es7s/data/icons-vitals/network-symbolic.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-vitals/network-upload-symbolic.svg` & `es7s-3.6.0.dev0/es7s/data/icons-vitals/network-upload-symbolic.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-vitals/temperature-symbolic.svg` & `es7s-3.6.0.dev0/es7s/data/icons-vitals/temperature-symbolic.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/data/icons-vitals/voltage-symbolic.svg` & `es7s-3.6.0.dev0/es7s/data/icons-vitals/voltage-symbolic.svg`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/gtk/__init__.py` & `es7s-3.6.0.dev0/es7s/gtk/__init__.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/gtk/_base.py` & `es7s-3.6.0.dev0/es7s/gtk/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,74 +1,89 @@
 # ------------------------------------------------------------------------------
 #  es7s/core
 #  (c) 2023 A. Shavykin <0.delameter@gmail.com>
 # ------------------------------------------------------------------------------
 import os
 import pickle
-import random
+import threading as th
 import time
 import typing as t
-import threading as th
 from abc import ABC, abstractmethod
 from collections import deque, OrderedDict
 from dataclasses import dataclass
 
 import pkg_resources
 
 from . import AppIndicator, Gtk
-from .. import APP_NAME
-from ..shared import ShutdownableThread, SocketClient, get_logger, SocketMessage
+from ..shared import ShutdownableThread, SocketClient, get_logger, SocketMessage, get_config
 
 DT = t.TypeVar("DT")
 
 
 @dataclass(frozen=True)
 class _MenuItemConfig:
     label: str
     sensitive: bool = True
     separator_before: bool = False
 
 
 @dataclass
 class _State:
     active = False
+    gobject: Gtk.MenuItem = None
 
     @abstractmethod
     def click(self):
         ...
 
 
 @dataclass
 class _StaticState(_State):
-    callback: t.Callable = None
+    callback: t.Callable[[_State], None] = None
 
     def click(self):
         if self.callback:
-            self.callback()
+            self.callback(self)
 
 
 @dataclass
 class _BoolState(_StaticState):
     value: bool = True
+    gobject: Gtk.CheckMenuItem = None
 
     def __bool__(self):
         return self.value
 
     @property
     def active(self) -> bool:
         return self.value
 
     def click(self):
         self.value = not self.value
         super().click()
 
+    def update_title(self, title: str):
+        if not self.gobject:
+            return
+        self.gobject.set_title(title)
+
+    def activate(self):
+        if self.value:
+            return
+        self.gobject.set_active(True)
+
+    def deactivate(self):
+        if not self.value:
+            return
+        self.gobject.set_active(False)
+
 
 class _BaseIndicator(ShutdownableThread, t.Generic[DT], ABC):
     SOCKRCV_INTERVAL_SEC = 1.0
-    RENDER_INTERVAL_SEC = 1.0
+    RENDER_INTERVAL_SEC = 2.0
     RENDER_ERROR_TIMEOUT_SEC = 5.0
 
     def __init__(
         self,
         indicator_name: str,
         socket_topic: str = None,
         icon_name_default: str = None,
@@ -137,22 +152,23 @@
 
         item = Gtk.CheckMenuItem.new_with_label(config.label)
         item.set_active(state.active)
         item.set_sensitive(config.sensitive)
         item.connect("activate", lambda c=config: self._click_menu_item(config))
         item.show()
         self._menu.append(item)
+        state.gobject = item
 
         return item
 
     def _click_menu_item(self, config: _MenuItemConfig):
         if (state := self._state_map.get(config)) is not None:
             state.click()
 
-    def _update_visibility(self):
+    def _update_visibility(self, _: _State = None):
         if self._hidden:
             self._indicator.set_status(AppIndicator.IndicatorStatus.PASSIVE)
         else:
             self._indicator.set_status(AppIndicator.IndicatorStatus.ACTIVE)
 
     def run(self):
         super().run()
@@ -246,9 +262,12 @@
 
     def _render_error(self):
         self._set("ERR", None, AppIndicator.IndicatorStatus.ATTENTION)
 
     def _set(self, label: str, guide: str | None, status: AppIndicator.IndicatorStatus):
         if self._hidden:
             return
+        get_logger().trace(label, "Output", out_ucp=True)
+        if get_config().get_monitor_debug_mode():
+            label = label.replace(" ", "␣")
         self._indicator.set_label(label, guide or label)
         self._indicator.set_status(status)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `es7s-3.5.0.dev0/es7s/gtk/_entrypoint.py` & `es7s-3.6.0.dev0/es7s/gtk/_entrypoint.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os
 import signal
 import sys
 
 from . import Gtk
 from .indicator_cpu_load import IndicatorCpuLoad
 from .indicator_memory import IndicatorMemory
+from .indicator_shocks import IndicatorShocks
 from .indicator_temperature import IndicatorTemperature
 from .. import APP_TRACE
 from ..shared import (
     get_stdout,
     init_logger,
     LoggerParams,
     init_io,
@@ -61,14 +62,15 @@
 class IndicatorController:
     def __init__(self):
         signal.signal(signal.SIGINT, self._exit)
         signal.signal(signal.SIGTERM, self._exit)
 
         self._indicators = [
             # IndicatorDatetime(),
+            IndicatorShocks(),
             IndicatorTemperature(),
             IndicatorCpuLoad(),
             IndicatorMemory(),
         ]
 
     def run(self):
         Gtk.main()
```

### Comparing `es7s-3.5.0.dev0/es7s/gtk/indicator_cpu_load.py` & `es7s-3.6.0.dev0/es7s/gtk/indicator_cpu_load.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 from ._base import _BaseIndicator, _MenuItemConfig, _BoolState, _State
 from ..shared import SocketMessage
 from ..shared.dto import CpuInfo
 
 
 class IndicatorCpuLoad(_BaseIndicator[CpuInfo]):
     def __init__(self):
-        self._show_perc = _BoolState(value=True)
+        self._show_perc = _BoolState(value=False)
         self._show_avg = _BoolState(value=False)
 
         super().__init__(
             "cpu-load",
             "cpu",
             icon_name_default="cpuload-0.svg",
             icon_path_dynamic_tpl="cpuload-%d.svg",
             icon_thresholds=[
-                85,
+                95,
                 87,
                 75,
                 62,
                 50,
                 37,
                 25,
                 12,
@@ -51,8 +51,8 @@
 
     def _format_result(self, perc: float, *avg: float) -> str:
         parts = []
         if self._show_perc.active:
             parts += [f"{perc:3.0f}% "]
         if self._show_avg.active:
             parts += (format_auto_float(a, 4) for a in avg)
-        return " ".join(parts)
+        return " ".join(parts).rstrip()
```

### Comparing `es7s-3.5.0.dev0/es7s/gtk/indicator_datetime.py` & `es7s-3.6.0.dev0/es7s/gtk/indicator_datetime.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/gtk/indicator_memory.py` & `es7s-3.6.0.dev0/es7s/gtk/indicator_memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from ..shared import SocketMessage
 from ..shared.dto import MemoryInfo
 
 
 class IndicatorMemory(_BaseIndicator[MemoryInfo]):
     def __init__(self):
         self._show_perc = _BoolState(value=False)
-        self._show_bytes = _BoolState(value=True)
+        self._show_bytes = _BoolState(value=False)
 
         super().__init__(
             "memory",
             icon_name_default="memory-0",
             icon_path_dynamic_tpl="memory-%d.svg",
             icon_thresholds=[
                 95,
@@ -45,15 +45,15 @@
 
     def _format_result(self, used: float, total: float) -> str:
         parts = []
         if self._show_perc:
             parts += [f"{100 * used / total:3.0f}% "]
         if self._show_bytes:
             parts += ["".join(self._format_used_value(round(used)))]
-        return " ".join(parts)
+        return " ".join(parts).rstrip()
 
     def _format_used_value(self, used: int) -> tuple[str, str]:
         used_kb = used / 1024
         used_mb = used / 1024**2
         used_gb = used / 1024**3
         if used_kb < 1000:
             return format_auto_float(used_kb, 4, False), "k"
```

### Comparing `es7s-3.5.0.dev0/es7s/gtk/indicator_temperature.py` & `es7s-3.6.0.dev0/es7s/gtk/indicator_temperature.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,60 @@
 # ------------------------------------------------------------------------------
 #  es7s/core
 #  (c) 2023 A. Shavykin <0.delameter@gmail.com>
 # ------------------------------------------------------------------------------
-from ._base import _BaseIndicator
+from ._base import _BaseIndicator, _BoolState, _MenuItemConfig, _State
 from ..shared import SocketMessage
 from ..shared.dto import TemperatureInfo
 
 
 class IndicatorTemperature(_BaseIndicator[TemperatureInfo]):
     def __init__(self):
+        self._show_one = _BoolState(value=False, callback=self._update_state)
+        self._show_three = _BoolState(value=False, callback=self._update_state)
+
         super().__init__(
             "temperature",
             icon_name_default="temperature-0.svg",
             icon_path_dynamic_tpl="temperature-%d.svg",
             icon_thresholds=[
                 90,
                 80,
                 70,
                 50,
                 30,
                 10,
                 0,
             ],
+            label="Thermal sensors",
         )
 
+    def _init_state(self):
+        self._state_map.update({
+            _MenuItemConfig("Current (°C)"): self._show_one,
+            _MenuItemConfig("Extra (°C)"): self._show_three,
+        })
+
+    def _update_state(self, _: _State = None):
+        self._show_three.gobject.set_sensitive(True)
+        if not self._show_one:
+            self._show_three.deactivate()
+            self._show_three.gobject.set_sensitive(False)
+        elif self._show_three:
+            self._show_one.activate()
+
     def _render(self, msg: SocketMessage[TemperatureInfo]):
         orig_values = msg.data.values_c
         sorted_values = sorted(orig_values, key=lambda v: v[1], reverse=True)
 
         max_value = 0
         if len(sorted_values) > 0:
             max_value = sorted_values[0][1]
 
-        values_limit = 1  # @TODO to config
+        values_limit = 3 if self._show_three else 1
         top_values_origin_indexes = []
         for (k, v) in sorted_values[:values_limit]:
             top_values_origin_indexes.append(orig_values.index((k, v)))
 
         values_str = []
         guide = []
         warning = False
@@ -52,12 +70,15 @@
             self._format_result(*values_str),
             self._format_result(*guide),
             warning,
             icon=self._select_icon(max_value),
         )
 
     def _format_result(self, *result: str) -> str:
-        parts = [
-            #*result,
-            #"°C",
-        ]
+        parts = []
+        if self._show_three:
+            parts += result[:3]
+        elif self._show_one:
+            parts += result[:1]
+        if len(parts):
+            parts += ["°C"]
         return " ".join(parts)
```

### Comparing `es7s-3.5.0.dev0/es7s/shared/__init__.py` & `es7s-3.6.0.dev0/es7s/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/shared/color.py` & `es7s-3.6.0.dev0/es7s/shared/color.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/shared/config.py` & `es7s-3.6.0.dev0/es7s/shared/config.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/shared/dto.py` & `es7s-3.6.0.dev0/es7s/shared/dto.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,24 +105,36 @@
 class DiskUsageInfo:
     free: int
     total: int
     used_perc: float
 
 
 @dataclass(frozen=True)
-class NetworkLatencyInfo:
-    failed_ratio: float = None
-    latency_s: float = None
-
-
-@dataclass(frozen=True)
 class NetworkCountryInfo:
     country: str = None
     ip: str = None
     mobile: bool = None
     proxy: bool = None
     hosting: bool = None
 
 
 @dataclass(frozen=True)
+class NetworkLatencyInfo:
+    failed_ratio: float = None
+    latency_s: float = None
+
+
+@dataclass(frozen=True)
+class NetworkTunnelInfo:
+    amount: int = None
+
+
+@dataclass(frozen=True)
+class ShocksInfo:
+    running: bool = None
+    healthy: bool = None
+    latency_s: float = None
+
+
+@dataclass(frozen=True)
 class TimestampInfo:
     ts: int = None
```

### Comparing `es7s-3.5.0.dev0/es7s/shared/io.py` & `es7s-3.6.0.dev0/es7s/shared/io.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/shared/ipc.py` & `es7s-3.6.0.dev0/es7s/shared/ipc.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/shared/log.py` & `es7s-3.6.0.dev0/es7s/shared/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,29 +201,32 @@
         out_sanitized: bool = True,
         out_ucp: bool = True,
         out_utf8: bool = False,
         out_hex: bool = True,
     ):
         if not data:
             return
-        label = (f":: {label} " if label else "") + "::\n"
+        label = (f"{label.upper()} " if label else "") + "::"
+        dump = ""
 
         if not isinstance(data, (str, bytes)):
             data = str(data)
 
         if isinstance(data, str):
             if out_sanitized:
-                self.log(TRACE, label + pt.apply_filters(data, *self.TRACE_EXTRA_FILTERS))
+                dump += "\n" + pt.apply_filters(data, *self.TRACE_EXTRA_FILTERS)
             if out_ucp:
-                self.log(TRACE, label + pt.utilstr.dump(data, "", 32))
+                dump += "\n" + pt.utilstr.dump(data, "", 32)
             if out_utf8:
-                self.log(TRACE, pt.StringTracer().apply(data))
+                dump += "\n" + pt.StringTracer().apply(data)
         else:
             if out_hex:
-                self.log(TRACE,  "::\n" + pt.BytesTracer().apply(data))
+                dump += "\n" + pt.BytesTracer().apply(data)
+
+        self.log(TRACE, label + dump)
 
     def makeRecord(
         self,
         name: str,
         level: int,
         fn: str,
         lno: int,
```

### Comparing `es7s-3.5.0.dev0/es7s/shared/separator.py` & `es7s-3.6.0.dev0/es7s/shared/separator.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/shared/spinner.py` & `es7s-3.6.0.dev0/es7s/shared/spinner.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/shared/styles.py` & `es7s-3.6.0.dev0/es7s/shared/styles.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/shared/sub.py` & `es7s-3.6.0.dev0/es7s/shared/sub.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/shared/sun_calc.py` & `es7s-3.6.0.dev0/es7s/shared/sun_calc.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/shared/system.py` & `es7s-3.6.0.dev0/es7s/shared/system.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/shared/threads.py` & `es7s-3.6.0.dev0/es7s/shared/threads.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/es7s/shared/weather_icons.py` & `es7s-3.6.0.dev0/es7s/shared/weather_icons.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/tests/test_cli.py` & `es7s-3.6.0.dev0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/README.md` & `es7s-3.6.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `es7s-3.5.0.dev0/pyproject.toml` & `es7s-3.6.0.dev0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,20 +27,19 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Topic :: Terminals",
 ]
 dependencies = [
     "click~=8.1",
-    "invoke~=2.0",
     "psutil~=5.9",
     "pytermor",
     "python-daemon~=2.3",
     "PyYAML==6.0",
-    "requests==2.28.1",
+    "requests[socks]==2.28.1",
 ]
 
 # pip install pygobject-stubs --no-cache-dir --config-settings=config=Gtk3,Gdk3,Soup2
 [project.optional-dependencies]
 dev = [
     "PyGObject-stubs==2.4.0",
 ]
```

### Comparing `es7s-3.5.0.dev0/PKG-INFO` & `es7s-3.6.0.dev0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: es7s
-Version: 3.5.0.dev0
+Version: 3.6.0.dev0
 Summary: es7s system (un-)installer, shared code, settings manager
 Project-URL: Homepage, https://github.com/es7s/core
 Author-email: Aleksandr Shavykin <0.delameter@gmail.com>
 License: MIT
 Keywords: cli,console,daemon,es7s,monitor,prmopt,shell,system,terminal
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -15,20 +15,19 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Terminals
 Requires-Python: >=3.10
 Requires-Dist: click~=8.1
-Requires-Dist: invoke~=2.0
 Requires-Dist: psutil~=5.9
 Requires-Dist: pytermor
 Requires-Dist: python-daemon~=2.3
 Requires-Dist: pyyaml==6.0
-Requires-Dist: requests==2.28.1
+Requires-Dist: requests[socks]==2.28.1
 Provides-Extra: dev
 Requires-Dist: pygobject-stubs==2.4.0; extra == 'dev'
 Provides-Extra: gtk
 Requires-Dist: pycairo~=1.23; extra == 'gtk'
 Requires-Dist: pygobject~=3.42; extra == 'gtk'
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: es7s Version: 3.5.0.dev0 Summary: es7s system (un-
+Metadata-Version: 2.1 Name: es7s Version: 3.6.0.dev0 Summary: es7s system (un-
 )installer, shared code, settings manager Project-URL: Homepage, https://
 github.com/es7s/core Author-email: Aleksandr Shavykin <0.delameter@gmail.com>
 License: MIT Keywords:
 cli,console,daemon,es7s,monitor,prmopt,shell,system,terminal Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Console Classifier:
 Environment :: No Input/Output (Daemon) Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Terminals Requires-Python: >=3.10 Requires-Dist:
-click~=8.1 Requires-Dist: invoke~=2.0 Requires-Dist: psutil~=5.9 Requires-Dist:
-pytermor Requires-Dist: python-daemon~=2.3 Requires-Dist: pyyaml==6.0 Requires-
-Dist: requests==2.28.1 Provides-Extra: dev Requires-Dist: pygobject-
-stubs==2.4.0; extra == 'dev' Provides-Extra: gtk Requires-Dist: pycairo~=1.23;
-extra == 'gtk' Requires-Dist: pygobject~=3.42; extra == 'gtk' Description-
-Content-Type: text/markdown
+click~=8.1 Requires-Dist: psutil~=5.9 Requires-Dist: pytermor Requires-Dist:
+python-daemon~=2.3 Requires-Dist: pyyaml==6.0 Requires-Dist: requests
+[socks]==2.28.1 Provides-Extra: dev Requires-Dist: pygobject-stubs==2.4.0;
+extra == 'dev' Provides-Extra: gtk Requires-Dist: pycairo~=1.23; extra == 'gtk'
+Requires-Dist: pygobject~=3.42; extra == 'gtk' Description-Content-Type: text/
+markdown
  [https://user-images.githubusercontent.com/50381946/219891285-172659e0-8315-
                           459a-a2b4-9d6f3a0cf4f0.png]
  [https://user-images.githubusercontent.com/50381946/219889704-f3fe7b8f-ce50-
                           4acf-8615-810b0729118c.png]
                   [https://img.shields.io/badge/python-3.10-
   3776AB?logo=python&logoColor=white&labelColor=333333] [Hatch_project] [Code
                                 style:_black]
```

