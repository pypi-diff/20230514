# Comparing `tmp/aioqui-1.0.8.tar.gz` & `tmp/aioqui-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioqui-1.0.8.tar", last modified: Sun May 14 04:56:31 2023, max compression
+gzip compressed data, was "aioqui-1.0.9.tar", last modified: Sun May 14 05:12:45 2023, max compression
```

## Comparing `aioqui-1.0.8.tar` & `aioqui-1.0.9.tar`

### file list

```diff
@@ -1,367 +1,367 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 04:56:31.881430 aioqui-1.0.8/
--rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 aioqui-1.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0     2755 2023-05-14 04:56:31.881430 aioqui-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      515 2023-05-13 21:14:57.000000 aioqui-1.0.8/README.md
--rw-rw-rw-   0        0        0     1551 2023-05-14 04:56:04.000000 aioqui-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-14 04:56:31.881430 aioqui-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-14 04:56:31.597430 aioqui-1.0.8/src/
--rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 aioqui-1.0.8/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:56:31.600430 aioqui-1.0.8/src/aioqui/
-drwxrwxrwx   0        0        0        0 2023-05-14 04:56:31.592430 aioqui-1.0.8/src/aioqui/.assets/
-drwxrwxrwx   0        0        0        0 2023-05-14 04:56:31.840430 aioqui-1.0.8/src/aioqui/.assets/icons/
--rw-rw-rw-   0        0        0      277 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/activity.svg
--rw-rw-rw-   0        0        0      357 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/airplay.svg
--rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/alert-circle.svg
--rw-rw-rw-   0        0        0      411 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/alert-octagon.svg
--rw-rw-rw-   0        0        0      419 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/alert-triangle.svg
--rw-rw-rw-   0        0        0      393 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/align-center.svg
--rw-rw-rw-   0        0        0      394 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/align-justify.svg
--rw-rw-rw-   0        0        0      391 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/align-left.svg
--rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/align-right.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/anchor.svg
--rw-rw-rw-   0        0        0      563 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/aperture.svg
--rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/archive.svg
--rw-rw-rw-   0        0        0      355 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/arrow-down-circle.svg
--rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/arrow-down-left.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/arrow-down-right.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/arrow-down.svg
--rw-rw-rw-   0        0        0      354 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/arrow-left-circle.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/arrow-left.svg
--rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/arrow-right-circle.svg
--rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/arrow-right.svg
--rw-rw-rw-   0        0        0      352 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/arrow-up-circle.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/arrow-up-left.svg
--rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/arrow-up-right.svg
--rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/arrow-up.svg
--rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/at-sign.svg
--rw-rw-rw-   0        0        0      320 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/award.svg
--rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/bar-chart-2.svg
--rw-rw-rw-   0        0        0      348 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/bar-chart.svg
--rw-rw-rw-   0        0        0      422 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/battery-charging.svg
--rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/battery.svg
--rw-rw-rw-   0        0        0      455 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/bell-off.svg
--rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/bell.svg
--rw-rw-rw-   0        0        0      293 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/bluetooth.svg
--rw-rw-rw-   0        0        0      322 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/bold.svg
--rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/book-open.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/book.svg
--rw-rw-rw-   0        0        0      282 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/bookmark.svg
--rw-rw-rw-   0        0        0      457 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/box.svg
--rw-rw-rw-   0        0        0      338 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/briefcase.svg
--rw-rw-rw-   0        0        0      405 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/calendar.svg
--rw-rw-rw-   0        0        0      380 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/camera-off.svg
--rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/camera.svg
--rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/cast.svg
--rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/check-circle.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/check-square.svg
--rw-rw-rw-   0        0        0      257 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/check.svg
--rw-rw-rw-   0        0        0      264 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/chevron-down.svg
--rw-rw-rw-   0        0        0      265 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/chevron-left.svg
--rw-rw-rw-   0        0        0      265 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/chevron-right.svg
--rw-rw-rw-   0        0        0      263 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/chevron-up.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/chevrons-down.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/chevrons-left.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/chevrons-right.svg
--rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/chevrons-up.svg
--rw-rw-rw-   0        0        0      443 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/chrome.svg
--rw-rw-rw-   0        0        0      253 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/circle.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/clipboard.svg
--rw-rw-rw-   0        0        0      299 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/clock.svg
--rw-rw-rw-   0        0        0      552 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/cloud-drizzle.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/cloud-lightning.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/cloud-off.svg
--rw-rw-rw-   0        0        0      416 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/cloud-rain.svg
--rw-rw-rw-   0        0        0      567 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/cloud-snow.svg
--rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/cloud.svg
--rw-rw-rw-   0        0        0      302 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/code.svg
--rw-rw-rw-   0        0        0      481 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/codepen.svg
--rw-rw-rw-   0        0        0      633 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/codesandbox.svg
--rw-rw-rw-   0        0        0      442 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/coffee.svg
--rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/columns.svg
--rw-rw-rw-   0        0        0      416 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/command.svg
--rw-rw-rw-   0        0        0      337 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/compass.svg
--rw-rw-rw-   0        0        0      346 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/copy.svg
--rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/corner-down-left.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/corner-down-right.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/corner-left-down.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/corner-left-up.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/corner-right-down.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/corner-right-up.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/corner-up-left.svg
--rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/corner-up-right.svg
--rw-rw-rw-   0        0        0      662 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/cpu.svg
--rw-rw-rw-   0        0        0      324 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/credit-card.svg
--rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/crop.svg
--rw-rw-rw-   0        0        0      432 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/crosshair.svg
--rw-rw-rw-   0        0        0      367 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/database.svg
--rw-rw-rw-   0        0        0      369 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/delete.svg
--rw-rw-rw-   0        0        0      290 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/disc.svg
--rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/divide-circle.svg
--rw-rw-rw-   0        0        0      414 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/divide-square.svg
--rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/divide.svg
--rw-rw-rw-   0        0        0      329 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/dollar-sign.svg
--rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/download-cloud.svg
--rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/download.svg
--rw-rw-rw-   0        0        0      419 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/dribbble.svg
--rw-rw-rw-   0        0        0      269 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/droplet.svg
--rw-rw-rw-   0        0        0      286 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/edit-2.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/edit-3.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/edit.svg
--rw-rw-rw-   0        0        0      383 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/external-link.svg
--rw-rw-rw-   0        0        0      455 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/eye-off.svg
--rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/eye.svg
--rw-rw-rw-   0        0        0      298 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/facebook.svg
--rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/fast-forward.svg
--rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/feather.svg
--rw-rw-rw-   0        0        0      548 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/figma.svg
--rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/file-minus.svg
--rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/file-plus.svg
--rw-rw-rw-   0        0        0      468 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/file-text.svg
--rw-rw-rw-   0        0        0      332 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/file.svg
--rw-rw-rw-   0        0        0      581 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/film.svg
--rw-rw-rw-   0        0        0      285 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/filter.svg
--rw-rw-rw-   0        0        0      329 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/flag.svg
--rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/folder-minus.svg
--rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/folder-plus.svg
--rw-rw-rw-   0        0        0      306 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/folder.svg
--rw-rw-rw-   0        0        0      273 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/framer.svg
--rw-rw-rw-   0        0        0      385 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/frown.svg
--rw-rw-rw-   0        0        0      476 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/gift.svg
--rw-rw-rw-   0        0        0      372 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/git-branch.svg
--rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/git-commit.svg
--rw-rw-rw-   0        0        0      331 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/git-merge.svg
--rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/git-pull-request.svg
--rw-rw-rw-   0        0        0      522 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/github.svg
--rw-rw-rw-   0        0        0      485 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/gitlab.svg
--rw-rw-rw-   0        0        0      404 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/globe.svg
--rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/grid.svg
--rw-rw-rw-   0        0        0      479 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/hard-drive.svg
--rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/hash.svg
--rw-rw-rw-   0        0        0      390 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/headphones.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/heart.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/help-circle.svg
--rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/hexagon.svg
--rw-rw-rw-   0        0        0      327 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/home.svg
--rw-rw-rw-   0        0        0      364 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/image.svg
--rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/inbox.svg
--rw-rw-rw-   0        0        0      342 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/info.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/instagram.svg
--rw-rw-rw-   0        0        0      343 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/italic.svg
--rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/key.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/layers.svg
--rw-rw-rw-   0        0        0      359 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/layout.svg
--rw-rw-rw-   0        0        0      570 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/life-buoy.svg
--rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/link-2.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/link.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/linkedin.svg
--rw-rw-rw-   0        0        0      477 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/list.svg
--rw-rw-rw-   0        0        0      609 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/loader.svg
--rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/lock.svg
--rw-rw-rw-   0        0        0      363 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/log-in.svg
--rw-rw-rw-   0        0        0      362 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/log-out.svg
--rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/mail.svg
--rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/map-pin.svg
--rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/map.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/maximize-2.svg
--rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/maximize.svg
--rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/meh.svg
--rw-rw-rw-   0        0        0      341 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/menu.svg
--rw-rw-rw-   0        0        0      423 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/message-circle.svg
--rw-rw-rw-   0        0        0      300 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/message-square.svg
--rw-rw-rw-   0        0        0      489 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/mic-off.svg
--rw-rw-rw-   0        0        0      413 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/mic.svg
--rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/minimize-2.svg
--rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/minimize.svg
--rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/minus-circle.svg
--rw-rw-rw-   0        0        0      325 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/minus-square.svg
--rw-rw-rw-   0        0        0      256 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/minus.svg
--rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/monitor.svg
--rw-rw-rw-   0        0        0      276 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/moon.svg
--rw-rw-rw-   0        0        0      338 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/more-horizontal.svg
--rw-rw-rw-   0        0        0      336 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/more-vertical.svg
--rw-rw-rw-   0        0        0      306 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/mouse-pointer.svg
--rw-rw-rw-   0        0        0      481 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/move.svg
--rw-rw-rw-   0        0        0      322 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/music.svg
--rw-rw-rw-   0        0        0      274 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/navigation-2.svg
--rw-rw-rw-   0        0        0      272 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/navigation.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/octagon.svg
--rw-rw-rw-   0        0        0      512 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/package.svg
--rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/paperclip.svg
--rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/pause-circle.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/pause.svg
--rw-rw-rw-   0        0        0      386 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/pen-tool.svg
--rw-rw-rw-   0        0        0      345 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/percent.svg
--rw-rw-rw-   0        0        0      571 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/phone-call.svg
--rw-rw-rw-   0        0        0      613 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/phone-forwarded.svg
--rw-rw-rw-   0        0        0      612 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/phone-incoming.svg
--rw-rw-rw-   0        0        0      608 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/phone-missed.svg
--rw-rw-rw-   0        0        0      586 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/phone-off.svg
--rw-rw-rw-   0        0        0      612 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/phone-outgoing.svg
--rw-rw-rw-   0        0        0      515 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/phone.svg
--rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/pie-chart.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/play-circle.svg
--rw-rw-rw-   0        0        0      258 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/play.svg
--rw-rw-rw-   0        0        0      345 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/plus-circle-gray.svg
--rw-rw-rw-   0        0        0      346 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/plus-circle.svg
--rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/plus-square.svg
--rw-rw-rw-   0        0        0      299 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/plus.svg
--rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/pocket.svg
--rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/power.svg
--rw-rw-rw-   0        0        0      402 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/printer.svg
--rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/radio.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/refresh-ccw.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/refresh-cw.svg
--rw-rw-rw-   0        0        0      387 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/repeat.svg
--rw-rw-rw-   0        0        0      314 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/rewind.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/rotate-ccw.svg
--rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/rotate-cw.svg
--rw-rw-rw-   0        0        0      325 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/rss.svg
--rw-rw-rw-   0        0        0      387 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/save.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/schedule.svg
--rw-rw-rw-   0        0        0      439 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/scissors.svg
--rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/search.svg
--rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/send.svg
--rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/server.svg
--rw-rw-rw-   0        0        0     1006 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/settings.svg
--rw-rw-rw-   0        0        0      440 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/share-2.svg
--rw-rw-rw-   0        0        0      359 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/share.svg
--rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/shield-off.svg
--rw-rw-rw-   0        0        0      274 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/shield.svg
--rw-rw-rw-   0        0        0      367 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/shopping-bag.svg
--rw-rw-rw-   0        0        0      378 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/shopping-cart.svg
--rw-rw-rw-   0        0        0      436 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/shuffle.svg
--rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/sidebar.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/skip-back.svg
--rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/skip-forward.svg
--rw-rw-rw-   0        0        0      994 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/slack.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/slash.svg
--rw-rw-rw-   0        0        0      606 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/sliders.svg
--rw-rw-rw-   0        0        0      327 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/smartphone.svg
--rw-rw-rw-   0        0        0      383 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/smile.svg
--rw-rw-rw-   0        0        0      361 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/speaker.svg
--rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/square.svg
--rw-rw-rw-   0        0        0      391 2023-04-06 21:10:35.000000 aioqui-1.0.8/src/aioqui/.assets/icons/star-fill.svg
--rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/star.svg
--rw-rw-rw-   0        0        0      304 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/stop-circle.svg
--rw-rw-rw-   0        0        0      645 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/sun.svg
--rw-rw-rw-   0        0        0      584 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/sunrise.svg
--rw-rw-rw-   0        0        0      583 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/sunset.svg
--rw-rw-rw-   0        0        0      335 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/table.svg
--rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/tablet.svg
--rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/tag.svg
--rw-rw-rw-   0        0        0      331 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/target.svg
--rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/terminal.svg
--rw-rw-rw-   0        0        0      292 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/thermometer.svg
--rw-rw-rw-   0        0        0      369 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/thumbs-down.svg
--rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/thumbs-up.svg
--rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/toggle-left.svg
--rw-rw-rw-   0        0        0      320 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/toggle-right.svg
--rw-rw-rw-   0        0        0      381 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/tool.svg
--rw-rw-rw-   0        0        0      443 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/trash-2.svg
--rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/trash.svg
--rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/trello.svg
--rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/trending-down.svg
--rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/trending-up.svg
--rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/triangle.svg
--rw-rw-rw-   0        0        0      410 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/truck.svg
--rw-rw-rw-   0        0        0      315 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/tv.svg
--rw-rw-rw-   0        0        0      272 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/twitch.svg
--rw-rw-rw-   0        0        0      403 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/twitter.svg
--rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/type.svg
--rw-rw-rw-   0        0        0      285 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/umbrella.svg
--rw-rw-rw-   0        0        0      314 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/underline.svg
--rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/unlock.svg
--rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/upload-cloud.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/upload.svg
--rw-rw-rw-   0        0        0      362 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/user-check.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/user-minus.svg
--rw-rw-rw-   0        0        0      403 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/user-plus.svg
--rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/user-x.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/user.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/users.svg
--rw-rw-rw-   0        0        0      374 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/video-off.svg
--rw-rw-rw-   0        0        0      324 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/video.svg
--rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/voicemail.svg
--rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/volume-1.svg
--rw-rw-rw-   0        0        0      354 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/volume-2.svg
--rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/volume-x.svg
--rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/volume.svg
--rw-rw-rw-   0        0        0      457 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/watch.svg
--rw-rw-rw-   0        0        0      564 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/wifi-off.svg
--rw-rw-rw-   0        0        0      396 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/wifi.svg
--rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/wind.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/x-circle-gray.svg
--rw-rw-rw-   0        0        0      341 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/x-circle.svg
--rw-rw-rw-   0        0        0      401 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/x-octagon.svg
--rw-rw-rw-   0        0        0      363 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/x-square.svg
--rw-rw-rw-   0        0        0      294 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/x.svg
--rw-rw-rw-   0        0        0      560 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/youtube.svg
--rw-rw-rw-   0        0        0      428 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/zap-off.svg
--rw-rw-rw-   0        0        0      277 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/zap.svg
--rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/zoom-in.svg
--rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-1.0.8/src/aioqui/.assets/icons/zoom-out.svg
--rw-rw-rw-   0        0        0      161 2023-05-14 00:40:20.000000 aioqui-1.0.8/src/aioqui/__init__.py
--rw-rw-rw-   0        0        0      443 2023-05-14 00:18:53.000000 aioqui-1.0.8/src/aioqui/contextapi.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:56:31.846431 aioqui-1.0.8/src/aioqui/enums/
--rw-rw-rw-   0        0        0      222 2023-05-14 01:09:08.000000 aioqui-1.0.8/src/aioqui/enums/__init__.py
--rw-rw-rw-   0        0        0      687 2023-05-13 23:00:29.000000 aioqui-1.0.8/src/aioqui/enums/alignment.py
--rw-rw-rw-   0        0        0      249 2023-05-14 01:16:18.000000 aioqui-1.0.8/src/aioqui/enums/elide_mode.py
--rw-rw-rw-   0        0        0      151 2023-05-13 23:00:29.000000 aioqui-1.0.8/src/aioqui/enums/orientation.py
--rw-rw-rw-   0        0        0      264 2023-05-14 00:48:52.000000 aioqui-1.0.8/src/aioqui/enums/scroll_policy.py
--rw-rw-rw-   0        0        0      270 2023-05-14 04:55:20.000000 aioqui-1.0.8/src/aioqui/enums/size_policy.py
--rw-rw-rw-   0        0        0      105 2023-05-13 23:00:29.000000 aioqui-1.0.8/src/aioqui/enums/window_hint.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:56:31.851430 aioqui-1.0.8/src/aioqui/misc/
--rw-rw-rw-   0        0        0      137 2023-05-14 03:02:34.000000 aioqui-1.0.8/src/aioqui/misc/__init__.py
--rw-rw-rw-   0        0        0     1931 2023-05-12 16:41:32.000000 aioqui-1.0.8/src/aioqui/misc/aiorequest.py
--rw-rw-rw-   0        0        0     1062 2023-05-02 22:09:01.000000 aioqui-1.0.8/src/aioqui/misc/ctq.py
--rw-rw-rw-   0        0        0     2181 2023-05-14 00:12:50.000000 aioqui-1.0.8/src/aioqui/misc/parser.py
--rw-rw-rw-   0        0        0      701 2023-05-14 00:40:28.000000 aioqui-1.0.8/src/aioqui/misc/server.py
--rw-rw-rw-   0        0        0      679 2023-05-14 00:09:55.000000 aioqui-1.0.8/src/aioqui/misc/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:56:31.854430 aioqui-1.0.8/src/aioqui/objects/
--rw-rw-rw-   0        0        0      107 2023-05-14 01:38:47.000000 aioqui-1.0.8/src/aioqui/objects/__init__.py
--rw-rw-rw-   0        0        0     2407 2023-05-14 02:31:01.000000 aioqui-1.0.8/src/aioqui/objects/context_obj.py
--rw-rw-rw-   0        0        0     2526 2023-05-14 04:46:03.000000 aioqui-1.0.8/src/aioqui/objects/evented_obj.py
--rw-rw-rw-   0        0        0     3083 2023-05-14 04:30:01.000000 aioqui-1.0.8/src/aioqui/objects/sized_obj.py
--rw-rw-rw-   0        0        0     1135 2023-05-14 00:38:47.000000 aioqui-1.0.8/src/aioqui/qasyncio.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:56:31.857430 aioqui-1.0.8/src/aioqui/types/
--rw-rw-rw-   0        0        0       71 2023-05-14 03:02:21.000000 aioqui-1.0.8/src/aioqui/types/__init__.py
--rw-rw-rw-   0        0        0      167 2023-05-14 04:46:50.000000 aioqui-1.0.8/src/aioqui/types/common.py
--rw-rw-rw-   0        0        0     3539 2023-05-14 00:07:05.000000 aioqui-1.0.8/src/aioqui/types/icon.py
--rw-rw-rw-   0        0        0      274 2023-04-20 15:54:13.000000 aioqui-1.0.8/src/aioqui/types/size.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:56:31.871430 aioqui-1.0.8/src/aioqui/widgets/
--rw-rw-rw-   0        0        0      589 2023-05-13 22:32:44.000000 aioqui-1.0.8/src/aioqui/widgets/__init__.py
--rw-rw-rw-   0        0        0      846 2023-05-14 03:24:34.000000 aioqui-1.0.8/src/aioqui/widgets/button.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:56:31.876430 aioqui-1.0.8/src/aioqui/widgets/custom/
--rw-rw-rw-   0        0        0      236 2023-05-14 04:54:16.000000 aioqui-1.0.8/src/aioqui/widgets/custom/__init__.py
--rw-rw-rw-   0        0        0     5557 2023-05-13 22:43:13.000000 aioqui-1.0.8/src/aioqui/widgets/custom/date_picker.py
--rw-rw-rw-   0        0        0     1830 2023-05-14 03:19:49.000000 aioqui-1.0.8/src/aioqui/widgets/custom/error_label.py
--rw-rw-rw-   0        0        0     2028 2023-05-14 03:17:33.000000 aioqui-1.0.8/src/aioqui/widgets/custom/favourite_button.py
--rw-rw-rw-   0        0        0     2732 2023-05-14 03:24:34.000000 aioqui-1.0.8/src/aioqui/widgets/custom/image_button.py
--rw-rw-rw-   0        0        0     1437 2023-05-14 03:18:51.000000 aioqui-1.0.8/src/aioqui/widgets/custom/menu_button.py
--rw-rw-rw-   0        0        0     1011 2023-05-13 22:50:44.000000 aioqui-1.0.8/src/aioqui/widgets/custom/search_bar.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:56:31.880430 aioqui-1.0.8/src/aioqui/widgets/extensions/
--rw-rw-rw-   0        0        0      127 2023-05-14 01:36:51.000000 aioqui-1.0.8/src/aioqui/widgets/extensions/__init__.py
--rw-rw-rw-   0        0        0     1899 2023-05-13 21:23:34.000000 aioqui-1.0.8/src/aioqui/widgets/extensions/layout_ext.py
--rw-rw-rw-   0        0        0      676 2023-05-13 21:23:34.000000 aioqui-1.0.8/src/aioqui/widgets/extensions/side_menu_ext.py
--rw-rw-rw-   0        0        0     1954 2023-05-14 04:55:20.000000 aioqui-1.0.8/src/aioqui/widgets/extensions/splitter_widget_ext.py
--rw-rw-rw-   0        0        0      822 2023-05-14 03:24:34.000000 aioqui-1.0.8/src/aioqui/widgets/frame.py
--rw-rw-rw-   0        0        0     1504 2023-05-14 03:32:01.000000 aioqui-1.0.8/src/aioqui/widgets/label.py
--rw-rw-rw-   0        0        0     1311 2023-05-14 01:40:16.000000 aioqui-1.0.8/src/aioqui/widgets/layout.py
--rw-rw-rw-   0        0        0     1056 2023-05-14 03:24:34.000000 aioqui-1.0.8/src/aioqui/widgets/line_input.py
--rw-rw-rw-   0        0        0     4132 2023-05-14 04:47:48.000000 aioqui-1.0.8/src/aioqui/widgets/popup.py
--rw-rw-rw-   0        0        0     1788 2023-05-14 03:49:48.000000 aioqui-1.0.8/src/aioqui/widgets/scroll_area.py
--rw-rw-rw-   0        0        0     1235 2023-05-14 03:24:34.000000 aioqui-1.0.8/src/aioqui/widgets/selector.py
--rw-rw-rw-   0        0        0      921 2023-05-14 01:40:16.000000 aioqui-1.0.8/src/aioqui/widgets/slider.py
--rw-rw-rw-   0        0        0      384 2023-05-14 00:57:08.000000 aioqui-1.0.8/src/aioqui/widgets/spacer.py
--rw-rw-rw-   0        0        0     1800 2023-05-14 01:40:16.000000 aioqui-1.0.8/src/aioqui/widgets/splitter.py
--rw-rw-rw-   0        0        0     1317 2023-05-14 04:13:29.000000 aioqui-1.0.8/src/aioqui/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0      374 2023-05-14 01:40:16.000000 aioqui-1.0.8/src/aioqui/widgets/statusbar.py
--rw-rw-rw-   0        0        0      694 2023-05-14 04:49:44.000000 aioqui-1.0.8/src/aioqui/widgets/text_input.py
--rw-rw-rw-   0        0        0      833 2023-05-14 03:24:34.000000 aioqui-1.0.8/src/aioqui/widgets/widget.py
--rw-rw-rw-   0        0        0      600 2023-05-14 04:22:11.000000 aioqui-1.0.8/src/aioqui/widgets/window.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:56:31.605430 aioqui-1.0.8/src/aioqui.egg-info/
--rw-rw-rw-   0        0        0     2755 2023-05-14 04:56:31.000000 aioqui-1.0.8/src/aioqui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    13043 2023-05-14 04:56:31.000000 aioqui-1.0.8/src/aioqui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 04:56:31.000000 aioqui-1.0.8/src/aioqui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-14 04:56:31.000000 aioqui-1.0.8/src/aioqui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-14 04:56:31.000000 aioqui-1.0.8/src/aioqui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 05:12:45.714921 aioqui-1.0.9/
+-rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 aioqui-1.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     2641 2023-05-14 05:12:45.713921 aioqui-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2023-05-14 05:04:46.000000 aioqui-1.0.9/README.md
+-rw-rw-rw-   0        0        0     1551 2023-05-14 05:12:23.000000 aioqui-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-14 05:12:45.714921 aioqui-1.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-14 05:12:45.418921 aioqui-1.0.9/src/
+-rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 aioqui-1.0.9/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:12:45.421921 aioqui-1.0.9/src/aioqui/
+drwxrwxrwx   0        0        0        0 2023-05-14 05:12:45.413921 aioqui-1.0.9/src/aioqui/.assets/
+drwxrwxrwx   0        0        0        0 2023-05-14 05:12:45.672922 aioqui-1.0.9/src/aioqui/.assets/icons/
+-rw-rw-rw-   0        0        0      277 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/activity.svg
+-rw-rw-rw-   0        0        0      357 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/airplay.svg
+-rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/alert-circle.svg
+-rw-rw-rw-   0        0        0      411 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/alert-octagon.svg
+-rw-rw-rw-   0        0        0      419 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/alert-triangle.svg
+-rw-rw-rw-   0        0        0      393 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/align-center.svg
+-rw-rw-rw-   0        0        0      394 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/align-justify.svg
+-rw-rw-rw-   0        0        0      391 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/align-left.svg
+-rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/align-right.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/anchor.svg
+-rw-rw-rw-   0        0        0      563 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/aperture.svg
+-rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/archive.svg
+-rw-rw-rw-   0        0        0      355 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/arrow-down-circle.svg
+-rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/arrow-down-left.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/arrow-down-right.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/arrow-down.svg
+-rw-rw-rw-   0        0        0      354 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/arrow-left-circle.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/arrow-left.svg
+-rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/arrow-right-circle.svg
+-rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/arrow-right.svg
+-rw-rw-rw-   0        0        0      352 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/arrow-up-circle.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/arrow-up-left.svg
+-rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/arrow-up-right.svg
+-rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/arrow-up.svg
+-rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/at-sign.svg
+-rw-rw-rw-   0        0        0      320 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/award.svg
+-rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/bar-chart-2.svg
+-rw-rw-rw-   0        0        0      348 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/bar-chart.svg
+-rw-rw-rw-   0        0        0      422 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/battery-charging.svg
+-rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/battery.svg
+-rw-rw-rw-   0        0        0      455 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/bell-off.svg
+-rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/bell.svg
+-rw-rw-rw-   0        0        0      293 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/bluetooth.svg
+-rw-rw-rw-   0        0        0      322 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/bold.svg
+-rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/book-open.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/book.svg
+-rw-rw-rw-   0        0        0      282 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/bookmark.svg
+-rw-rw-rw-   0        0        0      457 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/box.svg
+-rw-rw-rw-   0        0        0      338 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/briefcase.svg
+-rw-rw-rw-   0        0        0      405 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/calendar.svg
+-rw-rw-rw-   0        0        0      380 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/camera-off.svg
+-rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/camera.svg
+-rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/cast.svg
+-rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/check-circle.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/check-square.svg
+-rw-rw-rw-   0        0        0      257 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/check.svg
+-rw-rw-rw-   0        0        0      264 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/chevron-down.svg
+-rw-rw-rw-   0        0        0      265 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/chevron-left.svg
+-rw-rw-rw-   0        0        0      265 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/chevron-right.svg
+-rw-rw-rw-   0        0        0      263 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/chevron-up.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/chevrons-down.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/chevrons-left.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/chevrons-right.svg
+-rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/chevrons-up.svg
+-rw-rw-rw-   0        0        0      443 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/chrome.svg
+-rw-rw-rw-   0        0        0      253 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/circle.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/clipboard.svg
+-rw-rw-rw-   0        0        0      299 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/clock.svg
+-rw-rw-rw-   0        0        0      552 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/cloud-drizzle.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/cloud-lightning.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/cloud-off.svg
+-rw-rw-rw-   0        0        0      416 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/cloud-rain.svg
+-rw-rw-rw-   0        0        0      567 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/cloud-snow.svg
+-rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/cloud.svg
+-rw-rw-rw-   0        0        0      302 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/code.svg
+-rw-rw-rw-   0        0        0      481 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/codepen.svg
+-rw-rw-rw-   0        0        0      633 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/codesandbox.svg
+-rw-rw-rw-   0        0        0      442 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/coffee.svg
+-rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/columns.svg
+-rw-rw-rw-   0        0        0      416 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/command.svg
+-rw-rw-rw-   0        0        0      337 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/compass.svg
+-rw-rw-rw-   0        0        0      346 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/copy.svg
+-rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/corner-down-left.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/corner-down-right.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/corner-left-down.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/corner-left-up.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/corner-right-down.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/corner-right-up.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/corner-up-left.svg
+-rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/corner-up-right.svg
+-rw-rw-rw-   0        0        0      662 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/cpu.svg
+-rw-rw-rw-   0        0        0      324 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/credit-card.svg
+-rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/crop.svg
+-rw-rw-rw-   0        0        0      432 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/crosshair.svg
+-rw-rw-rw-   0        0        0      367 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/database.svg
+-rw-rw-rw-   0        0        0      369 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/delete.svg
+-rw-rw-rw-   0        0        0      290 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/disc.svg
+-rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/divide-circle.svg
+-rw-rw-rw-   0        0        0      414 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/divide-square.svg
+-rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/divide.svg
+-rw-rw-rw-   0        0        0      329 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/dollar-sign.svg
+-rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/download-cloud.svg
+-rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/download.svg
+-rw-rw-rw-   0        0        0      419 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/dribbble.svg
+-rw-rw-rw-   0        0        0      269 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/droplet.svg
+-rw-rw-rw-   0        0        0      286 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/edit-2.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/edit-3.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/edit.svg
+-rw-rw-rw-   0        0        0      383 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/external-link.svg
+-rw-rw-rw-   0        0        0      455 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/eye-off.svg
+-rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/eye.svg
+-rw-rw-rw-   0        0        0      298 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/facebook.svg
+-rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/fast-forward.svg
+-rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/feather.svg
+-rw-rw-rw-   0        0        0      548 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/figma.svg
+-rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/file-minus.svg
+-rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/file-plus.svg
+-rw-rw-rw-   0        0        0      468 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/file-text.svg
+-rw-rw-rw-   0        0        0      332 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/file.svg
+-rw-rw-rw-   0        0        0      581 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/film.svg
+-rw-rw-rw-   0        0        0      285 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/filter.svg
+-rw-rw-rw-   0        0        0      329 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/flag.svg
+-rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/folder-minus.svg
+-rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/folder-plus.svg
+-rw-rw-rw-   0        0        0      306 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/folder.svg
+-rw-rw-rw-   0        0        0      273 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/framer.svg
+-rw-rw-rw-   0        0        0      385 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/frown.svg
+-rw-rw-rw-   0        0        0      476 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/gift.svg
+-rw-rw-rw-   0        0        0      372 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/git-branch.svg
+-rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/git-commit.svg
+-rw-rw-rw-   0        0        0      331 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/git-merge.svg
+-rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/git-pull-request.svg
+-rw-rw-rw-   0        0        0      522 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/github.svg
+-rw-rw-rw-   0        0        0      485 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/gitlab.svg
+-rw-rw-rw-   0        0        0      404 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/globe.svg
+-rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/grid.svg
+-rw-rw-rw-   0        0        0      479 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/hard-drive.svg
+-rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/hash.svg
+-rw-rw-rw-   0        0        0      390 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/headphones.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/heart.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/help-circle.svg
+-rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/hexagon.svg
+-rw-rw-rw-   0        0        0      327 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/home.svg
+-rw-rw-rw-   0        0        0      364 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/image.svg
+-rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/inbox.svg
+-rw-rw-rw-   0        0        0      342 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/info.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/instagram.svg
+-rw-rw-rw-   0        0        0      343 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/italic.svg
+-rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/key.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/layers.svg
+-rw-rw-rw-   0        0        0      359 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/layout.svg
+-rw-rw-rw-   0        0        0      570 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/life-buoy.svg
+-rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/link-2.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/link.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/linkedin.svg
+-rw-rw-rw-   0        0        0      477 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/list.svg
+-rw-rw-rw-   0        0        0      609 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/loader.svg
+-rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/lock.svg
+-rw-rw-rw-   0        0        0      363 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/log-in.svg
+-rw-rw-rw-   0        0        0      362 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/log-out.svg
+-rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/mail.svg
+-rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/map-pin.svg
+-rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/map.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/maximize-2.svg
+-rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/maximize.svg
+-rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/meh.svg
+-rw-rw-rw-   0        0        0      341 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/menu.svg
+-rw-rw-rw-   0        0        0      423 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/message-circle.svg
+-rw-rw-rw-   0        0        0      300 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/message-square.svg
+-rw-rw-rw-   0        0        0      489 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/mic-off.svg
+-rw-rw-rw-   0        0        0      413 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/mic.svg
+-rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/minimize-2.svg
+-rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/minimize.svg
+-rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/minus-circle.svg
+-rw-rw-rw-   0        0        0      325 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/minus-square.svg
+-rw-rw-rw-   0        0        0      256 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/minus.svg
+-rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/monitor.svg
+-rw-rw-rw-   0        0        0      276 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/moon.svg
+-rw-rw-rw-   0        0        0      338 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/more-horizontal.svg
+-rw-rw-rw-   0        0        0      336 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/more-vertical.svg
+-rw-rw-rw-   0        0        0      306 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/mouse-pointer.svg
+-rw-rw-rw-   0        0        0      481 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/move.svg
+-rw-rw-rw-   0        0        0      322 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/music.svg
+-rw-rw-rw-   0        0        0      274 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/navigation-2.svg
+-rw-rw-rw-   0        0        0      272 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/navigation.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/octagon.svg
+-rw-rw-rw-   0        0        0      512 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/package.svg
+-rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/paperclip.svg
+-rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/pause-circle.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/pause.svg
+-rw-rw-rw-   0        0        0      386 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/pen-tool.svg
+-rw-rw-rw-   0        0        0      345 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/percent.svg
+-rw-rw-rw-   0        0        0      571 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/phone-call.svg
+-rw-rw-rw-   0        0        0      613 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/phone-forwarded.svg
+-rw-rw-rw-   0        0        0      612 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/phone-incoming.svg
+-rw-rw-rw-   0        0        0      608 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/phone-missed.svg
+-rw-rw-rw-   0        0        0      586 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/phone-off.svg
+-rw-rw-rw-   0        0        0      612 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/phone-outgoing.svg
+-rw-rw-rw-   0        0        0      515 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/phone.svg
+-rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/pie-chart.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/play-circle.svg
+-rw-rw-rw-   0        0        0      258 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/play.svg
+-rw-rw-rw-   0        0        0      345 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/plus-circle-gray.svg
+-rw-rw-rw-   0        0        0      346 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/plus-circle.svg
+-rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/plus-square.svg
+-rw-rw-rw-   0        0        0      299 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/plus.svg
+-rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/pocket.svg
+-rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/power.svg
+-rw-rw-rw-   0        0        0      402 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/printer.svg
+-rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/radio.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/refresh-ccw.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/refresh-cw.svg
+-rw-rw-rw-   0        0        0      387 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/repeat.svg
+-rw-rw-rw-   0        0        0      314 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/rewind.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/rotate-ccw.svg
+-rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/rotate-cw.svg
+-rw-rw-rw-   0        0        0      325 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/rss.svg
+-rw-rw-rw-   0        0        0      387 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/save.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/schedule.svg
+-rw-rw-rw-   0        0        0      439 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/scissors.svg
+-rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/search.svg
+-rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/send.svg
+-rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/server.svg
+-rw-rw-rw-   0        0        0     1006 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/settings.svg
+-rw-rw-rw-   0        0        0      440 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/share-2.svg
+-rw-rw-rw-   0        0        0      359 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/share.svg
+-rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/shield-off.svg
+-rw-rw-rw-   0        0        0      274 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/shield.svg
+-rw-rw-rw-   0        0        0      367 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/shopping-bag.svg
+-rw-rw-rw-   0        0        0      378 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/shopping-cart.svg
+-rw-rw-rw-   0        0        0      436 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/shuffle.svg
+-rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/sidebar.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/skip-back.svg
+-rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/skip-forward.svg
+-rw-rw-rw-   0        0        0      994 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/slack.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/slash.svg
+-rw-rw-rw-   0        0        0      606 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/sliders.svg
+-rw-rw-rw-   0        0        0      327 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/smartphone.svg
+-rw-rw-rw-   0        0        0      383 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/smile.svg
+-rw-rw-rw-   0        0        0      361 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/speaker.svg
+-rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/square.svg
+-rw-rw-rw-   0        0        0      391 2023-04-06 21:10:35.000000 aioqui-1.0.9/src/aioqui/.assets/icons/star-fill.svg
+-rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/star.svg
+-rw-rw-rw-   0        0        0      304 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/stop-circle.svg
+-rw-rw-rw-   0        0        0      645 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/sun.svg
+-rw-rw-rw-   0        0        0      584 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/sunrise.svg
+-rw-rw-rw-   0        0        0      583 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/sunset.svg
+-rw-rw-rw-   0        0        0      335 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/table.svg
+-rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/tablet.svg
+-rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/tag.svg
+-rw-rw-rw-   0        0        0      331 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/target.svg
+-rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/terminal.svg
+-rw-rw-rw-   0        0        0      292 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/thermometer.svg
+-rw-rw-rw-   0        0        0      369 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/thumbs-down.svg
+-rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/thumbs-up.svg
+-rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/toggle-left.svg
+-rw-rw-rw-   0        0        0      320 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/toggle-right.svg
+-rw-rw-rw-   0        0        0      381 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/tool.svg
+-rw-rw-rw-   0        0        0      443 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/trash-2.svg
+-rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/trash.svg
+-rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/trello.svg
+-rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/trending-down.svg
+-rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/trending-up.svg
+-rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/triangle.svg
+-rw-rw-rw-   0        0        0      410 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/truck.svg
+-rw-rw-rw-   0        0        0      315 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/tv.svg
+-rw-rw-rw-   0        0        0      272 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/twitch.svg
+-rw-rw-rw-   0        0        0      403 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/twitter.svg
+-rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/type.svg
+-rw-rw-rw-   0        0        0      285 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/umbrella.svg
+-rw-rw-rw-   0        0        0      314 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/underline.svg
+-rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/unlock.svg
+-rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/upload-cloud.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/upload.svg
+-rw-rw-rw-   0        0        0      362 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/user-check.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/user-minus.svg
+-rw-rw-rw-   0        0        0      403 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/user-plus.svg
+-rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/user-x.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/user.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/users.svg
+-rw-rw-rw-   0        0        0      374 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/video-off.svg
+-rw-rw-rw-   0        0        0      324 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/video.svg
+-rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/voicemail.svg
+-rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/volume-1.svg
+-rw-rw-rw-   0        0        0      354 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/volume-2.svg
+-rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/volume-x.svg
+-rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/volume.svg
+-rw-rw-rw-   0        0        0      457 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/watch.svg
+-rw-rw-rw-   0        0        0      564 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/wifi-off.svg
+-rw-rw-rw-   0        0        0      396 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/wifi.svg
+-rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/wind.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/x-circle-gray.svg
+-rw-rw-rw-   0        0        0      341 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/x-circle.svg
+-rw-rw-rw-   0        0        0      401 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/x-octagon.svg
+-rw-rw-rw-   0        0        0      363 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/x-square.svg
+-rw-rw-rw-   0        0        0      294 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/x.svg
+-rw-rw-rw-   0        0        0      560 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/youtube.svg
+-rw-rw-rw-   0        0        0      428 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/zap-off.svg
+-rw-rw-rw-   0        0        0      277 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/zap.svg
+-rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/zoom-in.svg
+-rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-1.0.9/src/aioqui/.assets/icons/zoom-out.svg
+-rw-rw-rw-   0        0        0      161 2023-05-14 00:40:20.000000 aioqui-1.0.9/src/aioqui/__init__.py
+-rw-rw-rw-   0        0        0      443 2023-05-14 00:18:53.000000 aioqui-1.0.9/src/aioqui/contextapi.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:12:45.677922 aioqui-1.0.9/src/aioqui/enums/
+-rw-rw-rw-   0        0        0      222 2023-05-14 01:09:08.000000 aioqui-1.0.9/src/aioqui/enums/__init__.py
+-rw-rw-rw-   0        0        0      687 2023-05-13 23:00:29.000000 aioqui-1.0.9/src/aioqui/enums/alignment.py
+-rw-rw-rw-   0        0        0      249 2023-05-14 01:16:18.000000 aioqui-1.0.9/src/aioqui/enums/elide_mode.py
+-rw-rw-rw-   0        0        0      151 2023-05-13 23:00:29.000000 aioqui-1.0.9/src/aioqui/enums/orientation.py
+-rw-rw-rw-   0        0        0      264 2023-05-14 00:48:52.000000 aioqui-1.0.9/src/aioqui/enums/scroll_policy.py
+-rw-rw-rw-   0        0        0      270 2023-05-14 04:55:20.000000 aioqui-1.0.9/src/aioqui/enums/size_policy.py
+-rw-rw-rw-   0        0        0      105 2023-05-13 23:00:29.000000 aioqui-1.0.9/src/aioqui/enums/window_hint.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:12:45.682922 aioqui-1.0.9/src/aioqui/misc/
+-rw-rw-rw-   0        0        0      137 2023-05-14 03:02:34.000000 aioqui-1.0.9/src/aioqui/misc/__init__.py
+-rw-rw-rw-   0        0        0     1931 2023-05-12 16:41:32.000000 aioqui-1.0.9/src/aioqui/misc/aiorequest.py
+-rw-rw-rw-   0        0        0     1062 2023-05-02 22:09:01.000000 aioqui-1.0.9/src/aioqui/misc/ctq.py
+-rw-rw-rw-   0        0        0     2181 2023-05-14 00:12:50.000000 aioqui-1.0.9/src/aioqui/misc/parser.py
+-rw-rw-rw-   0        0        0      701 2023-05-14 00:40:28.000000 aioqui-1.0.9/src/aioqui/misc/server.py
+-rw-rw-rw-   0        0        0      679 2023-05-14 00:09:55.000000 aioqui-1.0.9/src/aioqui/misc/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:12:45.686921 aioqui-1.0.9/src/aioqui/objects/
+-rw-rw-rw-   0        0        0      107 2023-05-14 01:38:47.000000 aioqui-1.0.9/src/aioqui/objects/__init__.py
+-rw-rw-rw-   0        0        0     2407 2023-05-14 02:31:01.000000 aioqui-1.0.9/src/aioqui/objects/context_obj.py
+-rw-rw-rw-   0        0        0     2526 2023-05-14 04:46:03.000000 aioqui-1.0.9/src/aioqui/objects/evented_obj.py
+-rw-rw-rw-   0        0        0     3083 2023-05-14 04:30:01.000000 aioqui-1.0.9/src/aioqui/objects/sized_obj.py
+-rw-rw-rw-   0        0        0     1135 2023-05-14 00:38:47.000000 aioqui-1.0.9/src/aioqui/qasyncio.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:12:45.689922 aioqui-1.0.9/src/aioqui/types/
+-rw-rw-rw-   0        0        0       71 2023-05-14 03:02:21.000000 aioqui-1.0.9/src/aioqui/types/__init__.py
+-rw-rw-rw-   0        0        0      167 2023-05-14 04:46:50.000000 aioqui-1.0.9/src/aioqui/types/common.py
+-rw-rw-rw-   0        0        0     3539 2023-05-14 00:07:05.000000 aioqui-1.0.9/src/aioqui/types/icon.py
+-rw-rw-rw-   0        0        0      274 2023-04-20 15:54:13.000000 aioqui-1.0.9/src/aioqui/types/size.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:12:45.703922 aioqui-1.0.9/src/aioqui/widgets/
+-rw-rw-rw-   0        0        0      589 2023-05-13 22:32:44.000000 aioqui-1.0.9/src/aioqui/widgets/__init__.py
+-rw-rw-rw-   0        0        0      846 2023-05-14 03:24:34.000000 aioqui-1.0.9/src/aioqui/widgets/button.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:12:45.709921 aioqui-1.0.9/src/aioqui/widgets/custom/
+-rw-rw-rw-   0        0        0      236 2023-05-14 04:54:16.000000 aioqui-1.0.9/src/aioqui/widgets/custom/__init__.py
+-rw-rw-rw-   0        0        0     5557 2023-05-13 22:43:13.000000 aioqui-1.0.9/src/aioqui/widgets/custom/date_picker.py
+-rw-rw-rw-   0        0        0     1935 2023-05-14 05:02:31.000000 aioqui-1.0.9/src/aioqui/widgets/custom/error_label.py
+-rw-rw-rw-   0        0        0     2029 2023-05-14 05:11:48.000000 aioqui-1.0.9/src/aioqui/widgets/custom/favourite_button.py
+-rw-rw-rw-   0        0        0     2720 2023-05-14 05:11:48.000000 aioqui-1.0.9/src/aioqui/widgets/custom/image_button.py
+-rw-rw-rw-   0        0        0     1472 2023-05-14 05:00:58.000000 aioqui-1.0.9/src/aioqui/widgets/custom/menu_button.py
+-rw-rw-rw-   0        0        0     1182 2023-05-14 05:09:33.000000 aioqui-1.0.9/src/aioqui/widgets/custom/search_bar.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:12:45.712921 aioqui-1.0.9/src/aioqui/widgets/extensions/
+-rw-rw-rw-   0        0        0      127 2023-05-14 01:36:51.000000 aioqui-1.0.9/src/aioqui/widgets/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1899 2023-05-13 21:23:34.000000 aioqui-1.0.9/src/aioqui/widgets/extensions/layout_ext.py
+-rw-rw-rw-   0        0        0      676 2023-05-13 21:23:34.000000 aioqui-1.0.9/src/aioqui/widgets/extensions/side_menu_ext.py
+-rw-rw-rw-   0        0        0     1954 2023-05-14 04:55:20.000000 aioqui-1.0.9/src/aioqui/widgets/extensions/splitter_widget_ext.py
+-rw-rw-rw-   0        0        0      792 2023-05-14 05:09:16.000000 aioqui-1.0.9/src/aioqui/widgets/frame.py
+-rw-rw-rw-   0        0        0     1504 2023-05-14 03:32:01.000000 aioqui-1.0.9/src/aioqui/widgets/label.py
+-rw-rw-rw-   0        0        0     1311 2023-05-14 01:40:16.000000 aioqui-1.0.9/src/aioqui/widgets/layout.py
+-rw-rw-rw-   0        0        0     1056 2023-05-14 03:24:34.000000 aioqui-1.0.9/src/aioqui/widgets/line_input.py
+-rw-rw-rw-   0        0        0     4132 2023-05-14 04:47:48.000000 aioqui-1.0.9/src/aioqui/widgets/popup.py
+-rw-rw-rw-   0        0        0     1788 2023-05-14 03:49:48.000000 aioqui-1.0.9/src/aioqui/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0     1235 2023-05-14 03:24:34.000000 aioqui-1.0.9/src/aioqui/widgets/selector.py
+-rw-rw-rw-   0        0        0      921 2023-05-14 01:40:16.000000 aioqui-1.0.9/src/aioqui/widgets/slider.py
+-rw-rw-rw-   0        0        0      384 2023-05-14 00:57:08.000000 aioqui-1.0.9/src/aioqui/widgets/spacer.py
+-rw-rw-rw-   0        0        0     1800 2023-05-14 01:40:16.000000 aioqui-1.0.9/src/aioqui/widgets/splitter.py
+-rw-rw-rw-   0        0        0     1283 2023-05-14 05:08:46.000000 aioqui-1.0.9/src/aioqui/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0      374 2023-05-14 01:40:16.000000 aioqui-1.0.9/src/aioqui/widgets/statusbar.py
+-rw-rw-rw-   0        0        0      694 2023-05-14 04:49:44.000000 aioqui-1.0.9/src/aioqui/widgets/text_input.py
+-rw-rw-rw-   0        0        0      799 2023-05-14 05:08:45.000000 aioqui-1.0.9/src/aioqui/widgets/widget.py
+-rw-rw-rw-   0        0        0      570 2023-05-14 05:08:34.000000 aioqui-1.0.9/src/aioqui/widgets/window.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:12:45.427931 aioqui-1.0.9/src/aioqui.egg-info/
+-rw-rw-rw-   0        0        0     2641 2023-05-14 05:12:45.000000 aioqui-1.0.9/src/aioqui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13043 2023-05-14 05:12:45.000000 aioqui-1.0.9/src/aioqui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 05:12:45.000000 aioqui-1.0.9/src/aioqui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-14 05:12:45.000000 aioqui-1.0.9/src/aioqui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-14 05:12:45.000000 aioqui-1.0.9/src/aioqui.egg-info/top_level.txt
```

### Comparing `aioqui-1.0.8/LICENSE.txt` & `aioqui-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/PKG-INFO` & `aioqui-1.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioqui
-Version: 1.0.8
+Version: 1.0.9
 Summary: Asynchronous GUI framework based on PySide6
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
         
@@ -37,23 +37,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # ToDo:
-- move to pyside6
-- favourite_label is actually a TwoStateIconLabel
-- error_label is actually a PopupTextLabel
+- favourite_button is actually a StateButton ? IconButton
+- error_label is actually a PopupTextLabel ? DelayLabel
 - make all widgets to have:
-    - min_height
-    - min_width
-    - min_size
-    - max_height
-    - max_width
-    - max_size
-    - policy
     - margins (in abstract frame)
     - padding (in abstract frame)
     - alignment (in abstract frame)
 - make popup to be generic (configure different buttons (ok, cancel, no, yes)
 - crete generic animation class to create simple animations
```

### Comparing `aioqui-1.0.8/pyproject.toml` & `aioqui-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aioqui"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
     { name="cxllmerichie", email="cxllmerichie@gmail.com" },
 ]
 maintainers = [
     { name="cxllmerichie", email="cxllmerichie@gmail.com" },
 ]
 description = "Asynchronous GUI framework based on PySide6"
```

### Comparing `aioqui-1.0.8/src/aioqui/.assets/icons/aperture.svg` & `aioqui-1.0.9/src/aioqui/.assets/icons/aperture.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/.assets/icons/cloud-drizzle.svg` & `aioqui-1.0.9/src/aioqui/.assets/icons/cloud-drizzle.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/.assets/icons/cloud-snow.svg` & `aioqui-1.0.9/src/aioqui/.assets/icons/cloud-snow.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/.assets/icons/codesandbox.svg` & `aioqui-1.0.9/src/aioqui/.assets/icons/codesandbox.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/.assets/icons/cpu.svg` & `aioqui-1.0.9/src/aioqui/.assets/icons/cpu.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/.assets/icons/figma.svg` & `aioqui-1.0.9/src/aioqui/.assets/icons/figma.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/.assets/icons/film.svg` & `aioqui-1.0.9/src/aioqui/.assets/icons/film.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/.assets/icons/github.svg` & `aioqui-1.0.9/src/aioqui/.assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/.assets/icons/life-buoy.svg` & `aioqui-1.0.9/src/aioqui/.assets/icons/life-buoy.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/.assets/icons/loader.svg` & `aioqui-1.0.9/src/aioqui/.assets/icons/loader.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/.assets/icons/package.svg` & `aioqui-1.0.9/src/aioqui/.assets/icons/package.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/.assets/icons/phone-call.svg` & `aioqui-1.0.9/src/aioqui/.assets/icons/phone-call.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/.assets/icons/phone-forwarded.svg` & `aioqui-1.0.9/src/aioqui/.assets/icons/phone-forwarded.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/.assets/icons/phone-incoming.svg` & `aioqui-1.0.9/src/aioqui/.assets/icons/phone-incoming.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/.assets/icons/phone-missed.svg` & `aioqui-1.0.9/src/aioqui/.assets/icons/phone-missed.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/.assets/icons/phone-off.svg` & `aioqui-1.0.9/src/aioqui/.assets/icons/phone-off.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/.assets/icons/phone-outgoing.svg` & `aioqui-1.0.9/src/aioqui/.assets/icons/phone-outgoing.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/.assets/icons/phone.svg` & `aioqui-1.0.9/src/aioqui/.assets/icons/phone.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/.assets/icons/settings.svg` & `aioqui-1.0.9/src/aioqui/.assets/icons/settings.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/.assets/icons/slack.svg` & `aioqui-1.0.9/src/aioqui/.assets/icons/slack.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/.assets/icons/sliders.svg` & `aioqui-1.0.9/src/aioqui/.assets/icons/sliders.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/.assets/icons/sun.svg` & `aioqui-1.0.9/src/aioqui/.assets/icons/sun.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/.assets/icons/sunrise.svg` & `aioqui-1.0.9/src/aioqui/.assets/icons/sunrise.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/.assets/icons/sunset.svg` & `aioqui-1.0.9/src/aioqui/.assets/icons/sunset.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/.assets/icons/wifi-off.svg` & `aioqui-1.0.9/src/aioqui/.assets/icons/wifi-off.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/.assets/icons/youtube.svg` & `aioqui-1.0.9/src/aioqui/.assets/icons/youtube.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/enums/alignment.py` & `aioqui-1.0.9/src/aioqui/enums/alignment.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/misc/aiorequest.py` & `aioqui-1.0.9/src/aioqui/misc/aiorequest.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/misc/ctq.py` & `aioqui-1.0.9/src/aioqui/misc/ctq.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/misc/parser.py` & `aioqui-1.0.9/src/aioqui/misc/parser.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/misc/server.py` & `aioqui-1.0.9/src/aioqui/misc/server.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/misc/utils.py` & `aioqui-1.0.9/src/aioqui/misc/utils.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/objects/context_obj.py` & `aioqui-1.0.9/src/aioqui/objects/context_obj.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/objects/evented_obj.py` & `aioqui-1.0.9/src/aioqui/objects/evented_obj.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/objects/sized_obj.py` & `aioqui-1.0.9/src/aioqui/objects/sized_obj.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/qasyncio.py` & `aioqui-1.0.9/src/aioqui/qasyncio.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/types/icon.py` & `aioqui-1.0.9/src/aioqui/types/icon.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/widgets/__init__.py` & `aioqui-1.0.9/src/aioqui/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/widgets/button.py` & `aioqui-1.0.9/src/aioqui/widgets/button.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/widgets/custom/date_picker.py` & `aioqui-1.0.9/src/aioqui/widgets/custom/date_picker.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/widgets/custom/error_label.py` & `aioqui-1.0.9/src/aioqui/widgets/custom/error_label.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,17 @@
         self.__duration: float = 0.5
 
     async def init(self, *args, **kwargs) -> 'ErrorLabel':
         await super().init(*args, **kwargs)
         return self
 
     def setText(self, text: str, delay: float = 2, duration: int = 0.5) -> None:
+        if not delay:  # if delay is 0, just set the text
+            return Label.setText(self, '')
+
         if not text:  # text == '' means instantly clear the text and hide label without `post` action
             self.setVisible(False)
             return Label.setText(self, '')
 
         def pre():
             self._set_opacity(1)
             Label.setText(self, text)
```

### Comparing `aioqui-1.0.8/src/aioqui/widgets/custom/favourite_button.py` & `aioqui-1.0.9/src/aioqui/widgets/custom/favourite_button.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,16 +15,15 @@
         self.if_unset_icon: Icon = Icon('star.svg', (30, 30))
 
     async def init(
             self, *,
             if_set_icon: Icon = None, if_unset_icon: Icon = None, pre_slot: Callable[..., bool],
             **kwargs
     ) -> 'Button':
-        await super().init(**kwargs)
-        self.clicked.connect(lambda: self.slot(pre_slot))
+        await super().init(events=Button.Events(on_click=lambda: self.slot(pre_slot)), **kwargs)
         if if_unset_icon:
             self.setIcon(QIcon(if_unset_icon.icon))
             self.setIconSize(if_unset_icon.size)
         if if_set_icon:
             self.if_set_icon = if_set_icon
         if if_unset_icon:
             self.if_unset_icon = if_unset_icon
```

### Comparing `aioqui-1.0.8/src/aioqui/widgets/custom/image_button.py` & `aioqui-1.0.9/src/aioqui/widgets/custom/image_button.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,17 @@
         super().__init__(parent, name if name else self.__class__.__name__, visible)
         self.image_bytes = None
 
     async def init(
             self, *,
             icon: Icon, slot: callable = lambda: None, directory: str = ''
     ) -> 'ImageButton':
-        await super().init(icon=icon)
-        self.clicked.connect(lambda: self.choose_image(slot, directory))
+        await super().init(icon=icon, events=Button.Events(on_click=lambda: self.choose_image(slot, directory)))
         self.RemoveImageBtn = await Button(self, f'{self.objectName()}RemoveImageBtn').init(
-            icon=Icon('x-circle.svg', (30, 30)),
-            sizes=Button.Sizes(fixed_size=Size(30, 30)),
+            icon=Icon('x-circle.svg', (30, 30)), sizes=Button.Sizes(fixed_size=Size(30, 30)),
             events=Button.Events(
                 on_click=lambda: Popup(self.core).display(message=f'Remove icon?', on_success=self.remove_icon)
             )
         )
         self.RemoveImageBtn.move(self.width() - 30, 0)
         self.RemoveImageBtn.setStyleSheet(f'''
             #{self.objectName()}RemoveImageBtn {{background-color: transparent; border-radius: 14px;}}
```

### Comparing `aioqui-1.0.8/src/aioqui/widgets/custom/menu_button.py` & `aioqui-1.0.9/src/aioqui/widgets/label.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-from PySide6.QtWidgets import QWidget, QSizePolicy
+from PySide6.QtGui import QFontMetrics, QPaintEvent
+from PySide6.QtWidgets import QLabel, QWidget
 
-from ..button import Button
-from ..label import Label
-from ..layout import Layout
-from ...types import Icon
+from ..objects import ContextObj, SizedObj, EventedObj
+from ..enums import Alignment, ElideMode
+from ..types import Applicable, Icon
 
 
-class MenuButton(Button):
-    def __init__(self, parent: QWidget, name: str = None, visible: bool = True):
-        super().__init__(parent, name if name else self.__class__.__name__, visible)
+class Label(ContextObj, Alignment, ElideMode, QLabel):
+    __elide = ElideMode.ElideNone
+    __elide_text = ''
+
+    def __init__(self, parent: QWidget, name: str, visible: bool = True):
+        QLabel.__init__(self, parent)
+        ContextObj.__init__(self, parent, name, visible)
 
     async def init(
             self, *,
-            icon: Icon, text: str, total: int = 0, alignment: Label.Alignment = None, slot: callable = None
-    ) -> 'MenuButton':
-        self.setLayout(await Layout.horizontal().init(
-            margins=(10, 5, 10, 5), spacing=10,
-            items=[
-                icon_btn := await Button(self, f'{self.objectName()}IconBtn').init(
-                    size=icon.size, icon=icon, disabled=True
-                ), Layout.Left,
-                text_lbl := await Label(self, f'{self.objectName()}TextLbl').init(
-                    text=text, alignment=alignment, elided=True, policy=(QSizePolicy.Expanding, QSizePolicy.Minimum)
-                ),
-                total_lbl := await Label(self, f'{self.objectName()}TotalLbl').init(
-                    text=str(total)
-                ), Layout.Right
-            ]
-        ))
-        self.icon_btn = icon_btn
-        self.text_lbl = text_lbl
-        self.total_lbl = total_lbl
-        if slot:
-            self.clicked.connect(slot)
-        return self
+            text: str = '', wrap: bool = False, icon: Icon = None, elide: ElideMode.ElideMode = ElideMode.ElideNone,
+            sizes: Applicable = SizedObj.Sizes(), events: Applicable = EventedObj.Events()
+    ) -> 'Label':
+        self.__elide, self.__elide_text = elide, text
+        self.setText(text)
+        self.setWordWrap(wrap)
+        if icon:
+            self.setPixmap(icon.icon.pixmap(icon.size))
+        return await sizes(await events(self))
+
+    def paintEvent(self, event: QPaintEvent):
+        if elide_mode := self.__elide:
+            elided_text = self.__elide_text
+            self.setText(QFontMetrics(self.font()).elidedText(elided_text, elide_mode, self.width() - 10))
+            self.__elide_text = elided_text
+        super().paintEvent(event)
+
+    def setText(self, text: str) -> None:
+        if self.__elide:
+            self.__elide_text = text
+        super().setText(text)
```

### Comparing `aioqui-1.0.8/src/aioqui/widgets/custom/search_bar.py` & `aioqui-1.0.9/src/aioqui/widgets/custom/search_bar.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from PySide6.QtWidgets import QWidget, QCompleter, QStyledItemDelegate
 from PySide6.QtCore import Qt
 from typing import Iterable
 
 from ..line_input import LineInput
+from ...types import Applicable
+from ...objects import SizedObj, EventedObj
 
 
 class SearchBar(LineInput):
     def __init__(self, parent: QWidget, name: str = None, visible: bool = True):
         LineInput.__init__(self, parent, name if name else self.__class__.__name__, visible)
 
     async def init(
             self, *,
-            items: Iterable[str] = (), textchanged: callable = None, placeholder: str = '',
-            stylesheet: str = ''
+            items: Iterable[str] = (), placeholder: str = '', stylesheet: str = '',
+            sizes: Applicable = SizedObj.Sizes(), events: Applicable = EventedObj.Events()
     ) -> 'SearchBar':
         completer = QCompleter(set(items))
         completer.setCaseSensitivity(Qt.CaseInsensitive)
         completer.popup().setObjectName(f'{self.objectName()}Popup')
         completer.popup().setItemDelegate(QStyledItemDelegate(completer))
         completer.popup().setStyleSheet(stylesheet)
+        self.setStyleSheet(stylesheet)
         self.setCompleter(completer)
-        await super().init(textchanged=textchanged, placeholder=placeholder)
+        await super().init(placeholder=placeholder, events=events, sizes=sizes)
         return self
```

### Comparing `aioqui-1.0.8/src/aioqui/widgets/extensions/layout_ext.py` & `aioqui-1.0.9/src/aioqui/widgets/extensions/layout_ext.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/widgets/extensions/side_menu_ext.py` & `aioqui-1.0.9/src/aioqui/widgets/extensions/side_menu_ext.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/widgets/extensions/splitter_widget_ext.py` & `aioqui-1.0.9/src/aioqui/widgets/extensions/splitter_widget_ext.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/widgets/frame.py` & `aioqui-1.0.9/src/aioqui/widgets/frame.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from PySide6.QtWidgets import QFrame, QWidget, QLayout
 
 from ..objects import ContextObj, SizedObj, EventedObj
 from ..types import Applicable
 
 
 class Frame(ContextObj, QFrame):
-    def __init__(self, parent: QWidget, name: str, visible: bool = True, stylesheet: str = None):
+    def __init__(self, parent: QWidget, name: str, visible: bool = True, stylesheet: str = ''):
         QFrame.__init__(self, parent)
         ContextObj.__init__(self, parent, name, visible)
-        if stylesheet:
-            self.setStyleSheet(stylesheet)
+        self.setStyleSheet(stylesheet)
 
     async def init(
             self, *,
             style: ... = None, layout: QLayout = None,
             sizes: Applicable = SizedObj.Sizes(), events: Applicable = EventedObj.Events()
     ) -> 'Frame':
         if style:
```

### Comparing `aioqui-1.0.8/src/aioqui/widgets/layout.py` & `aioqui-1.0.9/src/aioqui/widgets/layout.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/widgets/line_input.py` & `aioqui-1.0.9/src/aioqui/widgets/line_input.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/widgets/popup.py` & `aioqui-1.0.9/src/aioqui/widgets/popup.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/widgets/scroll_area.py` & `aioqui-1.0.9/src/aioqui/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/widgets/selector.py` & `aioqui-1.0.9/src/aioqui/widgets/selector.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/widgets/slider.py` & `aioqui-1.0.9/src/aioqui/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/widgets/splitter.py` & `aioqui-1.0.9/src/aioqui/widgets/splitter.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/widgets/stacked_widget.py` & `aioqui-1.0.9/src/aioqui/widgets/stacked_widget.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,19 @@
 
 from ..objects import ContextObj, SizedObj, EventedObj
 from ..enums import Alignment, Orientation
 from ..types import Applicable
 
 
 class StackedWidget(ContextObj, Orientation, QStackedWidget):
-    def __init__(self, parent: QWidget, name: str, visible: bool = True, stylesheet: str = None):
+    def __init__(self, parent: QWidget, name: str, visible: bool = True, stylesheet: str = ''):
         QStackedWidget.__init__(self, parent)
         ContextObj.__init__(self, parent, name, visible)
-        if stylesheet:
-            self.setStyleSheet(stylesheet)
-            self.setAttribute(Qt.WA_StyledBackground, True)
+        self.setStyleSheet(stylesheet)
+        self.setAttribute(Qt.WA_StyledBackground, True)
 
         # workaround which includes override of `setCurrentIndex`, otherwise problems with `parent()`
         self.addWidget(QWidget(self))
 
     async def init(
             self, *,
             alignment: Alignment.Alignment = Alignment.HCenter, items: Iterable[QObject] = (),
```

### Comparing `aioqui-1.0.8/src/aioqui/widgets/text_input.py` & `aioqui-1.0.9/src/aioqui/widgets/text_input.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.0.8/src/aioqui/widgets/widget.py` & `aioqui-1.0.9/src/aioqui/widgets/widget.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 from PySide6.QtCore import Qt
 
 from ..objects import ContextObj, SizedObj, EventedObj
 from ..types import Applicable
 
 
 class Widget(ContextObj, QWidget):
-    def __init__(self, parent: QWidget, name: str, visible: bool = True, stylesheet: str = None):
+    def __init__(self, parent: QWidget, name: str, visible: bool = True, stylesheet: str = ''):
         QWidget.__init__(self, parent)
         ContextObj.__init__(self, parent, name, visible)
-        if stylesheet:
-            self.setAttribute(Qt.WA_StyledBackground, True)
-            self.setStyleSheet(stylesheet)
+        self.setAttribute(Qt.WA_StyledBackground, True)
+        self.setStyleSheet(stylesheet)
 
     async def init(
             self, *,
             layout: QLayout = None,
             sizes: Applicable = SizedObj.Sizes(), events: Applicable = EventedObj.Events()
     ) -> 'Widget':
         if layout:
```

### Comparing `aioqui-1.0.8/src/aioqui/widgets/window.py` & `aioqui-1.0.9/src/aioqui/widgets/window.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 
 from ..objects import SizedObj, EventedObj
 from ..enums import WindowHint
 from ..types import Applicable
 
 
 class Window(WindowHint, QMainWindow):
-    def __init__(self, name: str, stylesheet: str = None):
+    def __init__(self, name: str, stylesheet: str = ''):
         QMainWindow.__init__(self)
         self.setObjectName(name)
-        if stylesheet:
-            self.setStyleSheet(stylesheet)
+        self.setStyleSheet(stylesheet)
 
     async def init(
             self, *,
             sizes: Applicable = SizedObj.Sizes(), events: Applicable = EventedObj.Events()
     ) -> 'Window':
         return await sizes(await events(self))
```

### Comparing `aioqui-1.0.8/src/aioqui.egg-info/PKG-INFO` & `aioqui-1.0.9/src/aioqui.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioqui
-Version: 1.0.8
+Version: 1.0.9
 Summary: Asynchronous GUI framework based on PySide6
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
         
@@ -37,23 +37,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # ToDo:
-- move to pyside6
-- favourite_label is actually a TwoStateIconLabel
-- error_label is actually a PopupTextLabel
+- favourite_button is actually a StateButton ? IconButton
+- error_label is actually a PopupTextLabel ? DelayLabel
 - make all widgets to have:
-    - min_height
-    - min_width
-    - min_size
-    - max_height
-    - max_width
-    - max_size
-    - policy
     - margins (in abstract frame)
     - padding (in abstract frame)
     - alignment (in abstract frame)
 - make popup to be generic (configure different buttons (ok, cancel, no, yes)
 - crete generic animation class to create simple animations
```

### Comparing `aioqui-1.0.8/src/aioqui.egg-info/SOURCES.txt` & `aioqui-1.0.9/src/aioqui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

