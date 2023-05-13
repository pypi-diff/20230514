# Comparing `tmp/qcontext-1.0.9.tar.gz` & `tmp/qcontext-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcontext-1.0.9.tar", last modified: Sat May 13 20:06:38 2023, max compression
+gzip compressed data, was "qcontext-1.1.0.tar", last modified: Sat May 13 22:11:01 2023, max compression
```

## Comparing `qcontext-1.0.9.tar` & `qcontext-1.1.0.tar`

### file list

```diff
@@ -1,355 +1,356 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 20:06:38.208105 qcontext-1.0.9/
--rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 qcontext-1.0.9/LICENSE.txt
--rw-rw-rw-   0        0        0     2788 2023-05-13 20:06:38.208105 qcontext-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      545 2023-05-11 02:27:47.000000 qcontext-1.0.9/README.md
--rw-rw-rw-   0        0        0     1577 2023-05-13 20:06:21.000000 qcontext-1.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-13 20:06:38.208105 qcontext-1.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-13 20:06:37.893005 qcontext-1.0.9/src/
--rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 qcontext-1.0.9/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 20:06:37.896994 qcontext-1.0.9/src/qcontext/
-drwxrwxrwx   0        0        0        0 2023-05-13 20:06:38.171792 qcontext-1.0.9/src/qcontext/.assets/
--rw-rw-rw-   0        0        0      277 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/activity.svg
--rw-rw-rw-   0        0        0      357 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/airplay.svg
--rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/alert-circle.svg
--rw-rw-rw-   0        0        0      411 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/alert-octagon.svg
--rw-rw-rw-   0        0        0      419 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/alert-triangle.svg
--rw-rw-rw-   0        0        0      393 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/align-center.svg
--rw-rw-rw-   0        0        0      394 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/align-justify.svg
--rw-rw-rw-   0        0        0      391 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/align-left.svg
--rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/align-right.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/anchor.svg
--rw-rw-rw-   0        0        0      563 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/aperture.svg
--rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/archive.svg
--rw-rw-rw-   0        0        0      355 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/arrow-down-circle.svg
--rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/arrow-down-left.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/arrow-down-right.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/arrow-down.svg
--rw-rw-rw-   0        0        0      354 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/arrow-left-circle.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/arrow-left.svg
--rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/arrow-right-circle.svg
--rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/arrow-right.svg
--rw-rw-rw-   0        0        0      352 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/arrow-up-circle.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/arrow-up-left.svg
--rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/arrow-up-right.svg
--rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/arrow-up.svg
--rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/at-sign.svg
--rw-rw-rw-   0        0        0      320 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/award.svg
--rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/bar-chart-2.svg
--rw-rw-rw-   0        0        0      348 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/bar-chart.svg
--rw-rw-rw-   0        0        0      422 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/battery-charging.svg
--rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/battery.svg
--rw-rw-rw-   0        0        0      455 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/bell-off.svg
--rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/bell.svg
--rw-rw-rw-   0        0        0      293 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/bluetooth.svg
--rw-rw-rw-   0        0        0      322 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/bold.svg
--rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/book-open.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/book.svg
--rw-rw-rw-   0        0        0      282 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/bookmark.svg
--rw-rw-rw-   0        0        0      457 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/box.svg
--rw-rw-rw-   0        0        0      338 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/briefcase.svg
--rw-rw-rw-   0        0        0      405 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/calendar.svg
--rw-rw-rw-   0        0        0      380 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/camera-off.svg
--rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/camera.svg
--rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/cast.svg
--rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/check-circle.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/check-square.svg
--rw-rw-rw-   0        0        0      257 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/check.svg
--rw-rw-rw-   0        0        0      264 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/chevron-down.svg
--rw-rw-rw-   0        0        0      265 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/chevron-left.svg
--rw-rw-rw-   0        0        0      265 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/chevron-right.svg
--rw-rw-rw-   0        0        0      263 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/chevron-up.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/chevrons-down.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/chevrons-left.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/chevrons-right.svg
--rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/chevrons-up.svg
--rw-rw-rw-   0        0        0      443 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/chrome.svg
--rw-rw-rw-   0        0        0      253 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/circle.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/clipboard.svg
--rw-rw-rw-   0        0        0      299 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/clock.svg
--rw-rw-rw-   0        0        0      552 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/cloud-drizzle.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/cloud-lightning.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/cloud-off.svg
--rw-rw-rw-   0        0        0      416 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/cloud-rain.svg
--rw-rw-rw-   0        0        0      567 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/cloud-snow.svg
--rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/cloud.svg
--rw-rw-rw-   0        0        0      302 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/code.svg
--rw-rw-rw-   0        0        0      481 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/codepen.svg
--rw-rw-rw-   0        0        0      633 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/codesandbox.svg
--rw-rw-rw-   0        0        0      442 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/coffee.svg
--rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/columns.svg
--rw-rw-rw-   0        0        0      416 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/command.svg
--rw-rw-rw-   0        0        0      337 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/compass.svg
--rw-rw-rw-   0        0        0      346 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/copy.svg
--rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/corner-down-left.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/corner-down-right.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/corner-left-down.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/corner-left-up.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/corner-right-down.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/corner-right-up.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/corner-up-left.svg
--rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/corner-up-right.svg
--rw-rw-rw-   0        0        0      662 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/cpu.svg
--rw-rw-rw-   0        0        0      324 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/credit-card.svg
--rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/crop.svg
--rw-rw-rw-   0        0        0      432 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/crosshair.svg
--rw-rw-rw-   0        0        0      367 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/database.svg
--rw-rw-rw-   0        0        0      369 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/delete.svg
--rw-rw-rw-   0        0        0      290 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/disc.svg
--rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/divide-circle.svg
--rw-rw-rw-   0        0        0      414 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/divide-square.svg
--rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/divide.svg
--rw-rw-rw-   0        0        0      329 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/dollar-sign.svg
--rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/download-cloud.svg
--rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/download.svg
--rw-rw-rw-   0        0        0      419 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/dribbble.svg
--rw-rw-rw-   0        0        0      269 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/droplet.svg
--rw-rw-rw-   0        0        0      286 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/edit-2.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/edit-3.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/edit.svg
--rw-rw-rw-   0        0        0      383 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/external-link.svg
--rw-rw-rw-   0        0        0      455 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/eye-off.svg
--rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/eye.svg
--rw-rw-rw-   0        0        0      298 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/facebook.svg
--rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/fast-forward.svg
--rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/feather.svg
--rw-rw-rw-   0        0        0      548 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/figma.svg
--rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/file-minus.svg
--rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/file-plus.svg
--rw-rw-rw-   0        0        0      468 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/file-text.svg
--rw-rw-rw-   0        0        0      332 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/file.svg
--rw-rw-rw-   0        0        0      581 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/film.svg
--rw-rw-rw-   0        0        0      285 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/filter.svg
--rw-rw-rw-   0        0        0      329 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/flag.svg
--rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/folder-minus.svg
--rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/folder-plus.svg
--rw-rw-rw-   0        0        0      306 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/folder.svg
--rw-rw-rw-   0        0        0      273 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/framer.svg
--rw-rw-rw-   0        0        0      385 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/frown.svg
--rw-rw-rw-   0        0        0      476 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/gift.svg
--rw-rw-rw-   0        0        0      372 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/git-branch.svg
--rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/git-commit.svg
--rw-rw-rw-   0        0        0      331 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/git-merge.svg
--rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/git-pull-request.svg
--rw-rw-rw-   0        0        0      522 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/github.svg
--rw-rw-rw-   0        0        0      485 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/gitlab.svg
--rw-rw-rw-   0        0        0      404 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/globe.svg
--rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/grid.svg
--rw-rw-rw-   0        0        0      479 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/hard-drive.svg
--rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/hash.svg
--rw-rw-rw-   0        0        0      390 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/headphones.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/heart.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/help-circle.svg
--rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/hexagon.svg
--rw-rw-rw-   0        0        0      327 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/home.svg
--rw-rw-rw-   0        0        0      364 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/image.svg
--rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/inbox.svg
--rw-rw-rw-   0        0        0      342 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/info.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/instagram.svg
--rw-rw-rw-   0        0        0      343 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/italic.svg
--rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/key.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/layers.svg
--rw-rw-rw-   0        0        0      359 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/layout.svg
--rw-rw-rw-   0        0        0      570 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/life-buoy.svg
--rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/link-2.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/link.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/linkedin.svg
--rw-rw-rw-   0        0        0      477 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/list.svg
--rw-rw-rw-   0        0        0      609 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/loader.svg
--rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/lock.svg
--rw-rw-rw-   0        0        0      363 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/log-in.svg
--rw-rw-rw-   0        0        0      362 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/log-out.svg
--rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/mail.svg
--rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/map-pin.svg
--rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/map.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/maximize-2.svg
--rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/maximize.svg
--rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/meh.svg
--rw-rw-rw-   0        0        0      341 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/menu.svg
--rw-rw-rw-   0        0        0      423 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/message-circle.svg
--rw-rw-rw-   0        0        0      300 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/message-square.svg
--rw-rw-rw-   0        0        0      489 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/mic-off.svg
--rw-rw-rw-   0        0        0      413 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/mic.svg
--rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/minimize-2.svg
--rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/minimize.svg
--rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/minus-circle.svg
--rw-rw-rw-   0        0        0      325 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/minus-square.svg
--rw-rw-rw-   0        0        0      256 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/minus.svg
--rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/monitor.svg
--rw-rw-rw-   0        0        0      276 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/moon.svg
--rw-rw-rw-   0        0        0      338 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/more-horizontal.svg
--rw-rw-rw-   0        0        0      336 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/more-vertical.svg
--rw-rw-rw-   0        0        0      306 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/mouse-pointer.svg
--rw-rw-rw-   0        0        0      481 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/move.svg
--rw-rw-rw-   0        0        0      322 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/music.svg
--rw-rw-rw-   0        0        0      274 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/navigation-2.svg
--rw-rw-rw-   0        0        0      272 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/navigation.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/octagon.svg
--rw-rw-rw-   0        0        0      512 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/package.svg
--rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/paperclip.svg
--rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/pause-circle.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/pause.svg
--rw-rw-rw-   0        0        0      386 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/pen-tool.svg
--rw-rw-rw-   0        0        0      345 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/percent.svg
--rw-rw-rw-   0        0        0      571 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/phone-call.svg
--rw-rw-rw-   0        0        0      613 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/phone-forwarded.svg
--rw-rw-rw-   0        0        0      612 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/phone-incoming.svg
--rw-rw-rw-   0        0        0      608 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/phone-missed.svg
--rw-rw-rw-   0        0        0      586 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/phone-off.svg
--rw-rw-rw-   0        0        0      612 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/phone-outgoing.svg
--rw-rw-rw-   0        0        0      515 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/phone.svg
--rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/pie-chart.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/play-circle.svg
--rw-rw-rw-   0        0        0      258 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/play.svg
--rw-rw-rw-   0        0        0      345 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/plus-circle-gray.svg
--rw-rw-rw-   0        0        0      346 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/plus-circle.svg
--rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/plus-square.svg
--rw-rw-rw-   0        0        0      299 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/plus.svg
--rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/pocket.svg
--rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/power.svg
--rw-rw-rw-   0        0        0      402 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/printer.svg
--rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/radio.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/refresh-ccw.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/refresh-cw.svg
--rw-rw-rw-   0        0        0      387 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/repeat.svg
--rw-rw-rw-   0        0        0      314 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/rewind.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/rotate-ccw.svg
--rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/rotate-cw.svg
--rw-rw-rw-   0        0        0      325 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/rss.svg
--rw-rw-rw-   0        0        0      387 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/save.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/schedule.svg
--rw-rw-rw-   0        0        0      439 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/scissors.svg
--rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/search.svg
--rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/send.svg
--rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/server.svg
--rw-rw-rw-   0        0        0     1006 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/settings.svg
--rw-rw-rw-   0        0        0      440 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/share-2.svg
--rw-rw-rw-   0        0        0      359 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/share.svg
--rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/shield-off.svg
--rw-rw-rw-   0        0        0      274 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/shield.svg
--rw-rw-rw-   0        0        0      367 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/shopping-bag.svg
--rw-rw-rw-   0        0        0      378 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/shopping-cart.svg
--rw-rw-rw-   0        0        0      436 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/shuffle.svg
--rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/sidebar.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/skip-back.svg
--rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/skip-forward.svg
--rw-rw-rw-   0        0        0      994 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/slack.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/slash.svg
--rw-rw-rw-   0        0        0      606 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/sliders.svg
--rw-rw-rw-   0        0        0      327 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/smartphone.svg
--rw-rw-rw-   0        0        0      383 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/smile.svg
--rw-rw-rw-   0        0        0      361 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/speaker.svg
--rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/square.svg
--rw-rw-rw-   0        0        0      391 2023-04-06 21:10:35.000000 qcontext-1.0.9/src/qcontext/.assets/star-fill.svg
--rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/star.svg
--rw-rw-rw-   0        0        0      304 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/stop-circle.svg
--rw-rw-rw-   0        0        0      645 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/sun.svg
--rw-rw-rw-   0        0        0      584 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/sunrise.svg
--rw-rw-rw-   0        0        0      583 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/sunset.svg
--rw-rw-rw-   0        0        0      335 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/table.svg
--rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/tablet.svg
--rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/tag.svg
--rw-rw-rw-   0        0        0      331 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/target.svg
--rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/terminal.svg
--rw-rw-rw-   0        0        0      292 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/thermometer.svg
--rw-rw-rw-   0        0        0      369 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/thumbs-down.svg
--rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/thumbs-up.svg
--rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/toggle-left.svg
--rw-rw-rw-   0        0        0      320 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/toggle-right.svg
--rw-rw-rw-   0        0        0      381 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/tool.svg
--rw-rw-rw-   0        0        0      443 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/trash-2.svg
--rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/trash.svg
--rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/trello.svg
--rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/trending-down.svg
--rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/trending-up.svg
--rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/triangle.svg
--rw-rw-rw-   0        0        0      410 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/truck.svg
--rw-rw-rw-   0        0        0      315 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/tv.svg
--rw-rw-rw-   0        0        0      272 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/twitch.svg
--rw-rw-rw-   0        0        0      403 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/twitter.svg
--rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/type.svg
--rw-rw-rw-   0        0        0      285 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/umbrella.svg
--rw-rw-rw-   0        0        0      314 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/underline.svg
--rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/unlock.svg
--rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/upload-cloud.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/upload.svg
--rw-rw-rw-   0        0        0      362 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/user-check.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/user-minus.svg
--rw-rw-rw-   0        0        0      403 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/user-plus.svg
--rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/user-x.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/user.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/users.svg
--rw-rw-rw-   0        0        0      374 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/video-off.svg
--rw-rw-rw-   0        0        0      324 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/video.svg
--rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/voicemail.svg
--rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/volume-1.svg
--rw-rw-rw-   0        0        0      354 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/volume-2.svg
--rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/volume-x.svg
--rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/volume.svg
--rw-rw-rw-   0        0        0      457 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/watch.svg
--rw-rw-rw-   0        0        0      564 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/wifi-off.svg
--rw-rw-rw-   0        0        0      396 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/wifi.svg
--rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/wind.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/x-circle-gray.svg
--rw-rw-rw-   0        0        0      341 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/x-circle.svg
--rw-rw-rw-   0        0        0      401 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/x-octagon.svg
--rw-rw-rw-   0        0        0      363 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/x-square.svg
--rw-rw-rw-   0        0        0      294 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/x.svg
--rw-rw-rw-   0        0        0      560 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/youtube.svg
--rw-rw-rw-   0        0        0      428 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/zap-off.svg
--rw-rw-rw-   0        0        0      277 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/zap.svg
--rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/zoom-in.svg
--rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 qcontext-1.0.9/src/qcontext/.assets/zoom-out.svg
--rw-rw-rw-   0        0        0       62 2023-05-11 03:03:55.000000 qcontext-1.0.9/src/qcontext/__init__.py
--rw-rw-rw-   0        0        0      426 2023-05-09 13:48:36.000000 qcontext-1.0.9/src/qcontext/contextapi.py
-drwxrwxrwx   0        0        0        0 2023-05-13 20:06:38.178864 qcontext-1.0.9/src/qcontext/misc/
--rw-rw-rw-   0        0        0      217 2023-05-02 22:09:11.000000 qcontext-1.0.9/src/qcontext/misc/__init__.py
--rw-rw-rw-   0        0        0     1931 2023-05-12 16:41:32.000000 qcontext-1.0.9/src/qcontext/misc/aiorequest.py
--rw-rw-rw-   0        0        0     1062 2023-05-02 22:09:01.000000 qcontext-1.0.9/src/qcontext/misc/conditional_thread_queue.py
--rw-rw-rw-   0        0        0     3533 2023-05-11 07:05:58.000000 qcontext-1.0.9/src/qcontext/misc/icon.py
--rw-rw-rw-   0        0        0      274 2023-04-20 15:54:13.000000 qcontext-1.0.9/src/qcontext/misc/size.py
--rw-rw-rw-   0        0        0     2181 2023-05-09 19:37:01.000000 qcontext-1.0.9/src/qcontext/misc/stylesheet_parser.py
--rw-rw-rw-   0        0        0      959 2023-05-11 02:43:57.000000 qcontext-1.0.9/src/qcontext/misc/utils.py
--rw-rw-rw-   0        0        0      642 2023-05-13 19:40:41.000000 qcontext-1.0.9/src/qcontext/misc/uvicorn_threaded_server.py
--rw-rw-rw-   0        0        0      821 2023-05-13 20:06:12.000000 qcontext-1.0.9/src/qcontext/qasyncio.py
-drwxrwxrwx   0        0        0        0 2023-05-13 20:06:38.191956 qcontext-1.0.9/src/qcontext/widgets/
--rw-rw-rw-   0        0        0      569 2023-05-13 19:40:41.000000 qcontext-1.0.9/src/qcontext/widgets/__init__.py
--rw-rw-rw-   0        0        0     1141 2023-05-11 02:59:52.000000 qcontext-1.0.9/src/qcontext/widgets/button.py
-drwxrwxrwx   0        0        0        0 2023-05-13 20:06:38.199050 qcontext-1.0.9/src/qcontext/widgets/custom/
--rw-rw-rw-   0        0        0      279 2023-05-02 20:21:51.000000 qcontext-1.0.9/src/qcontext/widgets/custom/__init__.py
--rw-rw-rw-   0        0        0     5580 2023-05-11 03:01:38.000000 qcontext-1.0.9/src/qcontext/widgets/custom/date_picker.py
--rw-rw-rw-   0        0        0     1930 2023-05-11 03:02:05.000000 qcontext-1.0.9/src/qcontext/widgets/custom/error_label.py
--rw-rw-rw-   0        0        0     2018 2023-05-11 04:47:21.000000 qcontext-1.0.9/src/qcontext/widgets/custom/favourite_button.py
--rw-rw-rw-   0        0        0     2676 2023-05-11 03:02:25.000000 qcontext-1.0.9/src/qcontext/widgets/custom/image_button.py
--rw-rw-rw-   0        0        0     1319 2023-05-11 03:03:19.000000 qcontext-1.0.9/src/qcontext/widgets/custom/label_extended.py
--rw-rw-rw-   0        0        0     1460 2023-05-11 03:03:19.000000 qcontext-1.0.9/src/qcontext/widgets/custom/menu_button.py
--rw-rw-rw-   0        0        0     1004 2023-05-11 03:03:19.000000 qcontext-1.0.9/src/qcontext/widgets/custom/search_bar.py
-drwxrwxrwx   0        0        0        0 2023-05-13 20:06:38.207105 qcontext-1.0.9/src/qcontext/widgets/extensions/
--rw-rw-rw-   0        0        0      298 2023-05-11 03:10:19.000000 qcontext-1.0.9/src/qcontext/widgets/extensions/__init__.py
--rw-rw-rw-   0        0        0      652 2023-05-11 03:08:55.000000 qcontext-1.0.9/src/qcontext/widgets/extensions/alignment_ext.py
--rw-rw-rw-   0        0        0     2130 2023-05-11 03:01:38.000000 qcontext-1.0.9/src/qcontext/widgets/extensions/context_object_ext.py
--rw-rw-rw-   0        0        0     1895 2023-05-10 02:24:48.000000 qcontext-1.0.9/src/qcontext/widgets/extensions/layout_ext.py
--rw-rw-rw-   0        0        0      150 2023-05-13 09:08:57.000000 qcontext-1.0.9/src/qcontext/widgets/extensions/orientation_ext.py
--rw-rw-rw-   0        0        0      225 2023-05-11 03:09:33.000000 qcontext-1.0.9/src/qcontext/widgets/extensions/policy_ext.py
--rw-rw-rw-   0        0        0      674 2023-04-20 15:21:35.000000 qcontext-1.0.9/src/qcontext/widgets/extensions/side_menu_ext.py
--rw-rw-rw-   0        0        0     1897 2023-04-27 03:54:17.000000 qcontext-1.0.9/src/qcontext/widgets/extensions/splitter_widget_ext.py
--rw-rw-rw-   0        0        0      778 2023-05-11 03:00:02.000000 qcontext-1.0.9/src/qcontext/widgets/frame.py
--rw-rw-rw-   0        0        0     1701 2023-05-11 03:11:47.000000 qcontext-1.0.9/src/qcontext/widgets/label.py
--rw-rw-rw-   0        0        0     1305 2023-05-11 03:10:28.000000 qcontext-1.0.9/src/qcontext/widgets/layout.py
--rw-rw-rw-   0        0        0     1118 2023-05-11 03:01:38.000000 qcontext-1.0.9/src/qcontext/widgets/line_input.py
--rw-rw-rw-   0        0        0     3945 2023-05-10 23:37:34.000000 qcontext-1.0.9/src/qcontext/widgets/popup.py
--rw-rw-rw-   0        0        0     1687 2023-05-11 03:01:38.000000 qcontext-1.0.9/src/qcontext/widgets/scroll_area.py
--rw-rw-rw-   0        0        0     1328 2023-05-11 03:01:38.000000 qcontext-1.0.9/src/qcontext/widgets/selector.py
--rw-rw-rw-   0        0        0      925 2023-05-13 19:40:16.000000 qcontext-1.0.9/src/qcontext/widgets/slider.py
--rw-rw-rw-   0        0        0      369 2023-04-08 19:53:22.000000 qcontext-1.0.9/src/qcontext/widgets/spacer.py
--rw-rw-rw-   0        0        0     1741 2023-05-11 03:01:38.000000 qcontext-1.0.9/src/qcontext/widgets/splitter.py
--rw-rw-rw-   0        0        0     1062 2023-05-11 03:01:38.000000 qcontext-1.0.9/src/qcontext/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0      392 2023-05-11 03:01:38.000000 qcontext-1.0.9/src/qcontext/widgets/statusbar.py
--rw-rw-rw-   0        0        0      779 2023-05-11 03:01:38.000000 qcontext-1.0.9/src/qcontext/widgets/text_input.py
--rw-rw-rw-   0        0        0      675 2023-05-11 02:59:52.000000 qcontext-1.0.9/src/qcontext/widgets/widget.py
--rw-rw-rw-   0        0        0      335 2023-05-10 00:56:17.000000 qcontext-1.0.9/src/qcontext/widgets/window.py
-drwxrwxrwx   0        0        0        0 2023-05-13 20:06:37.918258 qcontext-1.0.9/src/qcontext.egg-info/
--rw-rw-rw-   0        0        0     2788 2023-05-13 20:06:37.000000 qcontext-1.0.9/src/qcontext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11853 2023-05-13 20:06:37.000000 qcontext-1.0.9/src/qcontext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 20:06:37.000000 qcontext-1.0.9/src/qcontext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-05-13 20:06:37.000000 qcontext-1.0.9/src/qcontext.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-13 20:06:37.000000 qcontext-1.0.9/src/qcontext.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-13 22:11:01.748459 qcontext-1.1.0/
+-rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 qcontext-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2758 2023-05-13 22:11:01.747465 qcontext-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      515 2023-05-13 21:14:57.000000 qcontext-1.1.0/README.md
+-rw-rw-rw-   0        0        0     1577 2023-05-13 22:10:21.000000 qcontext-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-13 22:11:01.749461 qcontext-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-13 22:10:59.396275 qcontext-1.1.0/src/
+-rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 qcontext-1.1.0/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-13 22:10:59.399254 qcontext-1.1.0/src/qcontext/
+drwxrwxrwx   0        0        0        0 2023-05-13 22:11:01.531462 qcontext-1.1.0/src/qcontext/.assets/
+-rw-rw-rw-   0        0        0      277 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/activity.svg
+-rw-rw-rw-   0        0        0      357 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/airplay.svg
+-rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/alert-circle.svg
+-rw-rw-rw-   0        0        0      411 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/alert-octagon.svg
+-rw-rw-rw-   0        0        0      419 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/alert-triangle.svg
+-rw-rw-rw-   0        0        0      393 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/align-center.svg
+-rw-rw-rw-   0        0        0      394 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/align-justify.svg
+-rw-rw-rw-   0        0        0      391 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/align-left.svg
+-rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/align-right.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/anchor.svg
+-rw-rw-rw-   0        0        0      563 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/aperture.svg
+-rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/archive.svg
+-rw-rw-rw-   0        0        0      355 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/arrow-down-circle.svg
+-rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/arrow-down-left.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/arrow-down-right.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/arrow-down.svg
+-rw-rw-rw-   0        0        0      354 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/arrow-left-circle.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/arrow-left.svg
+-rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/arrow-right-circle.svg
+-rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/arrow-right.svg
+-rw-rw-rw-   0        0        0      352 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/arrow-up-circle.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/arrow-up-left.svg
+-rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/arrow-up-right.svg
+-rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/arrow-up.svg
+-rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/at-sign.svg
+-rw-rw-rw-   0        0        0      320 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/award.svg
+-rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/bar-chart-2.svg
+-rw-rw-rw-   0        0        0      348 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/bar-chart.svg
+-rw-rw-rw-   0        0        0      422 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/battery-charging.svg
+-rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/battery.svg
+-rw-rw-rw-   0        0        0      455 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/bell-off.svg
+-rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/bell.svg
+-rw-rw-rw-   0        0        0      293 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/bluetooth.svg
+-rw-rw-rw-   0        0        0      322 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/bold.svg
+-rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/book-open.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/book.svg
+-rw-rw-rw-   0        0        0      282 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/bookmark.svg
+-rw-rw-rw-   0        0        0      457 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/box.svg
+-rw-rw-rw-   0        0        0      338 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/briefcase.svg
+-rw-rw-rw-   0        0        0      405 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/calendar.svg
+-rw-rw-rw-   0        0        0      380 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/camera-off.svg
+-rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/camera.svg
+-rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/cast.svg
+-rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/check-circle.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/check-square.svg
+-rw-rw-rw-   0        0        0      257 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/check.svg
+-rw-rw-rw-   0        0        0      264 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/chevron-down.svg
+-rw-rw-rw-   0        0        0      265 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/chevron-left.svg
+-rw-rw-rw-   0        0        0      265 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/chevron-right.svg
+-rw-rw-rw-   0        0        0      263 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/chevron-up.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/chevrons-down.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/chevrons-left.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/chevrons-right.svg
+-rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/chevrons-up.svg
+-rw-rw-rw-   0        0        0      443 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/chrome.svg
+-rw-rw-rw-   0        0        0      253 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/circle.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/clipboard.svg
+-rw-rw-rw-   0        0        0      299 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/clock.svg
+-rw-rw-rw-   0        0        0      552 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/cloud-drizzle.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/cloud-lightning.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/cloud-off.svg
+-rw-rw-rw-   0        0        0      416 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/cloud-rain.svg
+-rw-rw-rw-   0        0        0      567 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/cloud-snow.svg
+-rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/cloud.svg
+-rw-rw-rw-   0        0        0      302 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/code.svg
+-rw-rw-rw-   0        0        0      481 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/codepen.svg
+-rw-rw-rw-   0        0        0      633 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/codesandbox.svg
+-rw-rw-rw-   0        0        0      442 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/coffee.svg
+-rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/columns.svg
+-rw-rw-rw-   0        0        0      416 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/command.svg
+-rw-rw-rw-   0        0        0      337 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/compass.svg
+-rw-rw-rw-   0        0        0      346 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/copy.svg
+-rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/corner-down-left.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/corner-down-right.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/corner-left-down.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/corner-left-up.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/corner-right-down.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/corner-right-up.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/corner-up-left.svg
+-rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/corner-up-right.svg
+-rw-rw-rw-   0        0        0      662 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/cpu.svg
+-rw-rw-rw-   0        0        0      324 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/credit-card.svg
+-rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/crop.svg
+-rw-rw-rw-   0        0        0      432 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/crosshair.svg
+-rw-rw-rw-   0        0        0      367 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/database.svg
+-rw-rw-rw-   0        0        0      369 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/delete.svg
+-rw-rw-rw-   0        0        0      290 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/disc.svg
+-rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/divide-circle.svg
+-rw-rw-rw-   0        0        0      414 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/divide-square.svg
+-rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/divide.svg
+-rw-rw-rw-   0        0        0      329 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/dollar-sign.svg
+-rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/download-cloud.svg
+-rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/download.svg
+-rw-rw-rw-   0        0        0      419 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/dribbble.svg
+-rw-rw-rw-   0        0        0      269 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/droplet.svg
+-rw-rw-rw-   0        0        0      286 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/edit-2.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/edit-3.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/edit.svg
+-rw-rw-rw-   0        0        0      383 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/external-link.svg
+-rw-rw-rw-   0        0        0      455 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/eye-off.svg
+-rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/eye.svg
+-rw-rw-rw-   0        0        0      298 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/facebook.svg
+-rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/fast-forward.svg
+-rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/feather.svg
+-rw-rw-rw-   0        0        0      548 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/figma.svg
+-rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/file-minus.svg
+-rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/file-plus.svg
+-rw-rw-rw-   0        0        0      468 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/file-text.svg
+-rw-rw-rw-   0        0        0      332 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/file.svg
+-rw-rw-rw-   0        0        0      581 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/film.svg
+-rw-rw-rw-   0        0        0      285 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/filter.svg
+-rw-rw-rw-   0        0        0      329 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/flag.svg
+-rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/folder-minus.svg
+-rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/folder-plus.svg
+-rw-rw-rw-   0        0        0      306 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/folder.svg
+-rw-rw-rw-   0        0        0      273 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/framer.svg
+-rw-rw-rw-   0        0        0      385 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/frown.svg
+-rw-rw-rw-   0        0        0      476 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/gift.svg
+-rw-rw-rw-   0        0        0      372 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/git-branch.svg
+-rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/git-commit.svg
+-rw-rw-rw-   0        0        0      331 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/git-merge.svg
+-rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/git-pull-request.svg
+-rw-rw-rw-   0        0        0      522 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/github.svg
+-rw-rw-rw-   0        0        0      485 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/gitlab.svg
+-rw-rw-rw-   0        0        0      404 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/globe.svg
+-rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/grid.svg
+-rw-rw-rw-   0        0        0      479 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/hard-drive.svg
+-rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/hash.svg
+-rw-rw-rw-   0        0        0      390 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/headphones.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/heart.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/help-circle.svg
+-rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/hexagon.svg
+-rw-rw-rw-   0        0        0      327 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/home.svg
+-rw-rw-rw-   0        0        0      364 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/image.svg
+-rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/inbox.svg
+-rw-rw-rw-   0        0        0      342 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/info.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/instagram.svg
+-rw-rw-rw-   0        0        0      343 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/italic.svg
+-rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/key.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/layers.svg
+-rw-rw-rw-   0        0        0      359 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/layout.svg
+-rw-rw-rw-   0        0        0      570 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/life-buoy.svg
+-rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/link-2.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/link.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/linkedin.svg
+-rw-rw-rw-   0        0        0      477 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/list.svg
+-rw-rw-rw-   0        0        0      609 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/loader.svg
+-rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/lock.svg
+-rw-rw-rw-   0        0        0      363 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/log-in.svg
+-rw-rw-rw-   0        0        0      362 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/log-out.svg
+-rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/mail.svg
+-rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/map-pin.svg
+-rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/map.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/maximize-2.svg
+-rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/maximize.svg
+-rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/meh.svg
+-rw-rw-rw-   0        0        0      341 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/menu.svg
+-rw-rw-rw-   0        0        0      423 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/message-circle.svg
+-rw-rw-rw-   0        0        0      300 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/message-square.svg
+-rw-rw-rw-   0        0        0      489 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/mic-off.svg
+-rw-rw-rw-   0        0        0      413 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/mic.svg
+-rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/minimize-2.svg
+-rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/minimize.svg
+-rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/minus-circle.svg
+-rw-rw-rw-   0        0        0      325 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/minus-square.svg
+-rw-rw-rw-   0        0        0      256 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/minus.svg
+-rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/monitor.svg
+-rw-rw-rw-   0        0        0      276 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/moon.svg
+-rw-rw-rw-   0        0        0      338 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/more-horizontal.svg
+-rw-rw-rw-   0        0        0      336 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/more-vertical.svg
+-rw-rw-rw-   0        0        0      306 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/mouse-pointer.svg
+-rw-rw-rw-   0        0        0      481 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/move.svg
+-rw-rw-rw-   0        0        0      322 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/music.svg
+-rw-rw-rw-   0        0        0      274 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/navigation-2.svg
+-rw-rw-rw-   0        0        0      272 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/navigation.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/octagon.svg
+-rw-rw-rw-   0        0        0      512 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/package.svg
+-rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/paperclip.svg
+-rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/pause-circle.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/pause.svg
+-rw-rw-rw-   0        0        0      386 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/pen-tool.svg
+-rw-rw-rw-   0        0        0      345 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/percent.svg
+-rw-rw-rw-   0        0        0      571 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/phone-call.svg
+-rw-rw-rw-   0        0        0      613 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/phone-forwarded.svg
+-rw-rw-rw-   0        0        0      612 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/phone-incoming.svg
+-rw-rw-rw-   0        0        0      608 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/phone-missed.svg
+-rw-rw-rw-   0        0        0      586 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/phone-off.svg
+-rw-rw-rw-   0        0        0      612 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/phone-outgoing.svg
+-rw-rw-rw-   0        0        0      515 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/phone.svg
+-rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/pie-chart.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/play-circle.svg
+-rw-rw-rw-   0        0        0      258 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/play.svg
+-rw-rw-rw-   0        0        0      345 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/plus-circle-gray.svg
+-rw-rw-rw-   0        0        0      346 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/plus-circle.svg
+-rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/plus-square.svg
+-rw-rw-rw-   0        0        0      299 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/plus.svg
+-rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/pocket.svg
+-rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/power.svg
+-rw-rw-rw-   0        0        0      402 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/printer.svg
+-rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/radio.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/refresh-ccw.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/refresh-cw.svg
+-rw-rw-rw-   0        0        0      387 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/repeat.svg
+-rw-rw-rw-   0        0        0      314 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/rewind.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/rotate-ccw.svg
+-rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/rotate-cw.svg
+-rw-rw-rw-   0        0        0      325 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/rss.svg
+-rw-rw-rw-   0        0        0      387 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/save.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/schedule.svg
+-rw-rw-rw-   0        0        0      439 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/scissors.svg
+-rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/search.svg
+-rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/send.svg
+-rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/server.svg
+-rw-rw-rw-   0        0        0     1006 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/settings.svg
+-rw-rw-rw-   0        0        0      440 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/share-2.svg
+-rw-rw-rw-   0        0        0      359 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/share.svg
+-rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/shield-off.svg
+-rw-rw-rw-   0        0        0      274 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/shield.svg
+-rw-rw-rw-   0        0        0      367 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/shopping-bag.svg
+-rw-rw-rw-   0        0        0      378 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/shopping-cart.svg
+-rw-rw-rw-   0        0        0      436 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/shuffle.svg
+-rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/sidebar.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/skip-back.svg
+-rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/skip-forward.svg
+-rw-rw-rw-   0        0        0      994 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/slack.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/slash.svg
+-rw-rw-rw-   0        0        0      606 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/sliders.svg
+-rw-rw-rw-   0        0        0      327 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/smartphone.svg
+-rw-rw-rw-   0        0        0      383 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/smile.svg
+-rw-rw-rw-   0        0        0      361 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/speaker.svg
+-rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/square.svg
+-rw-rw-rw-   0        0        0      391 2023-04-06 21:10:35.000000 qcontext-1.1.0/src/qcontext/.assets/star-fill.svg
+-rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/star.svg
+-rw-rw-rw-   0        0        0      304 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/stop-circle.svg
+-rw-rw-rw-   0        0        0      645 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/sun.svg
+-rw-rw-rw-   0        0        0      584 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/sunrise.svg
+-rw-rw-rw-   0        0        0      583 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/sunset.svg
+-rw-rw-rw-   0        0        0      335 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/table.svg
+-rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/tablet.svg
+-rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/tag.svg
+-rw-rw-rw-   0        0        0      331 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/target.svg
+-rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/terminal.svg
+-rw-rw-rw-   0        0        0      292 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/thermometer.svg
+-rw-rw-rw-   0        0        0      369 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/thumbs-down.svg
+-rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/thumbs-up.svg
+-rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/toggle-left.svg
+-rw-rw-rw-   0        0        0      320 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/toggle-right.svg
+-rw-rw-rw-   0        0        0      381 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/tool.svg
+-rw-rw-rw-   0        0        0      443 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/trash-2.svg
+-rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/trash.svg
+-rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/trello.svg
+-rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/trending-down.svg
+-rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/trending-up.svg
+-rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/triangle.svg
+-rw-rw-rw-   0        0        0      410 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/truck.svg
+-rw-rw-rw-   0        0        0      315 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/tv.svg
+-rw-rw-rw-   0        0        0      272 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/twitch.svg
+-rw-rw-rw-   0        0        0      403 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/twitter.svg
+-rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/type.svg
+-rw-rw-rw-   0        0        0      285 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/umbrella.svg
+-rw-rw-rw-   0        0        0      314 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/underline.svg
+-rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/unlock.svg
+-rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/upload-cloud.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/upload.svg
+-rw-rw-rw-   0        0        0      362 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/user-check.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/user-minus.svg
+-rw-rw-rw-   0        0        0      403 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/user-plus.svg
+-rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/user-x.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/user.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/users.svg
+-rw-rw-rw-   0        0        0      374 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/video-off.svg
+-rw-rw-rw-   0        0        0      324 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/video.svg
+-rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/voicemail.svg
+-rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/volume-1.svg
+-rw-rw-rw-   0        0        0      354 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/volume-2.svg
+-rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/volume-x.svg
+-rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/volume.svg
+-rw-rw-rw-   0        0        0      457 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/watch.svg
+-rw-rw-rw-   0        0        0      564 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/wifi-off.svg
+-rw-rw-rw-   0        0        0      396 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/wifi.svg
+-rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/wind.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/x-circle-gray.svg
+-rw-rw-rw-   0        0        0      341 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/x-circle.svg
+-rw-rw-rw-   0        0        0      401 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/x-octagon.svg
+-rw-rw-rw-   0        0        0      363 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/x-square.svg
+-rw-rw-rw-   0        0        0      294 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/x.svg
+-rw-rw-rw-   0        0        0      560 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/youtube.svg
+-rw-rw-rw-   0        0        0      428 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/zap-off.svg
+-rw-rw-rw-   0        0        0      277 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/zap.svg
+-rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/zoom-in.svg
+-rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 qcontext-1.1.0/src/qcontext/.assets/zoom-out.svg
+-rw-rw-rw-   0        0        0      154 2023-05-13 21:47:42.000000 qcontext-1.1.0/src/qcontext/__init__.py
+-rw-rw-rw-   0        0        0      428 2023-05-13 21:23:09.000000 qcontext-1.1.0/src/qcontext/contextapi.py
+drwxrwxrwx   0        0        0        0 2023-05-13 22:11:01.584479 qcontext-1.1.0/src/qcontext/misc/
+-rw-rw-rw-   0        0        0      217 2023-05-02 22:09:11.000000 qcontext-1.1.0/src/qcontext/misc/__init__.py
+-rw-rw-rw-   0        0        0     1931 2023-05-12 16:41:32.000000 qcontext-1.1.0/src/qcontext/misc/aiorequest.py
+-rw-rw-rw-   0        0        0     1062 2023-05-02 22:09:01.000000 qcontext-1.1.0/src/qcontext/misc/conditional_thread_queue.py
+-rw-rw-rw-   0        0        0     3537 2023-05-13 21:25:18.000000 qcontext-1.1.0/src/qcontext/misc/icon.py
+-rw-rw-rw-   0        0        0      274 2023-04-20 15:54:13.000000 qcontext-1.1.0/src/qcontext/misc/size.py
+-rw-rw-rw-   0        0        0     2181 2023-05-09 19:37:01.000000 qcontext-1.1.0/src/qcontext/misc/stylesheet_parser.py
+-rw-rw-rw-   0        0        0      679 2023-05-13 21:25:59.000000 qcontext-1.1.0/src/qcontext/misc/utils.py
+-rw-rw-rw-   0        0        0      642 2023-05-13 19:40:41.000000 qcontext-1.1.0/src/qcontext/misc/uvicorn_threaded_server.py
+-rw-rw-rw-   0        0        0     1079 2023-05-13 21:26:28.000000 qcontext-1.1.0/src/qcontext/qasyncio.py
+drwxrwxrwx   0        0        0        0 2023-05-13 22:11:01.619461 qcontext-1.1.0/src/qcontext/widgets/
+-rw-rw-rw-   0        0        0      571 2023-05-13 21:26:53.000000 qcontext-1.1.0/src/qcontext/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1147 2023-05-13 21:19:10.000000 qcontext-1.1.0/src/qcontext/widgets/button.py
+drwxrwxrwx   0        0        0        0 2023-05-13 22:11:01.718459 qcontext-1.1.0/src/qcontext/widgets/custom/
+-rw-rw-rw-   0        0        0      279 2023-05-02 20:21:51.000000 qcontext-1.1.0/src/qcontext/widgets/custom/__init__.py
+-rw-rw-rw-   0        0        0     5584 2023-05-13 21:23:43.000000 qcontext-1.1.0/src/qcontext/widgets/custom/date_picker.py
+-rw-rw-rw-   0        0        0     1934 2023-05-13 21:24:47.000000 qcontext-1.1.0/src/qcontext/widgets/custom/error_label.py
+-rw-rw-rw-   0        0        0     2022 2023-05-13 21:24:47.000000 qcontext-1.1.0/src/qcontext/widgets/custom/favourite_button.py
+-rw-rw-rw-   0        0        0     2682 2023-05-13 21:24:47.000000 qcontext-1.1.0/src/qcontext/widgets/custom/image_button.py
+-rw-rw-rw-   0        0        0     1323 2023-05-13 21:24:47.000000 qcontext-1.1.0/src/qcontext/widgets/custom/label_extended.py
+-rw-rw-rw-   0        0        0     1464 2023-05-13 21:24:47.000000 qcontext-1.1.0/src/qcontext/widgets/custom/menu_button.py
+-rw-rw-rw-   0        0        0     1008 2023-05-13 21:24:47.000000 qcontext-1.1.0/src/qcontext/widgets/custom/search_bar.py
+drwxrwxrwx   0        0        0        0 2023-05-13 22:11:01.737461 qcontext-1.1.0/src/qcontext/widgets/extensions/
+-rw-rw-rw-   0        0        0      299 2023-05-13 22:08:39.000000 qcontext-1.1.0/src/qcontext/widgets/extensions/__init__.py
+-rw-rw-rw-   0        0        0      654 2023-05-13 21:23:09.000000 qcontext-1.1.0/src/qcontext/widgets/extensions/alignment.py
+-rw-rw-rw-   0        0        0     2131 2023-05-13 21:23:34.000000 qcontext-1.1.0/src/qcontext/widgets/extensions/context_object.py
+-rw-rw-rw-   0        0        0      223 2023-05-13 22:08:15.000000 qcontext-1.1.0/src/qcontext/widgets/extensions/event.py
+-rw-rw-rw-   0        0        0     1899 2023-05-13 21:23:34.000000 qcontext-1.1.0/src/qcontext/widgets/extensions/layout.py
+-rw-rw-rw-   0        0        0      152 2023-05-13 21:23:34.000000 qcontext-1.1.0/src/qcontext/widgets/extensions/orientation.py
+-rw-rw-rw-   0        0        0      227 2023-05-13 21:23:34.000000 qcontext-1.1.0/src/qcontext/widgets/extensions/policy.py
+-rw-rw-rw-   0        0        0      676 2023-05-13 21:23:34.000000 qcontext-1.1.0/src/qcontext/widgets/extensions/side_menu.py
+-rw-rw-rw-   0        0        0     1901 2023-05-13 21:23:34.000000 qcontext-1.1.0/src/qcontext/widgets/extensions/splitter_widget.py
+-rw-rw-rw-   0        0        0      780 2023-05-13 21:23:09.000000 qcontext-1.1.0/src/qcontext/widgets/frame.py
+-rw-rw-rw-   0        0        0     1707 2023-05-13 21:23:09.000000 qcontext-1.1.0/src/qcontext/widgets/label.py
+-rw-rw-rw-   0        0        0     1309 2023-05-13 21:23:09.000000 qcontext-1.1.0/src/qcontext/widgets/layout.py
+-rw-rw-rw-   0        0        0     1122 2023-05-13 21:23:09.000000 qcontext-1.1.0/src/qcontext/widgets/line_input.py
+-rw-rw-rw-   0        0        0     4009 2023-05-13 22:10:18.000000 qcontext-1.1.0/src/qcontext/widgets/popup.py
+-rw-rw-rw-   0        0        0     1691 2023-05-13 21:23:09.000000 qcontext-1.1.0/src/qcontext/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0     1330 2023-05-13 21:23:09.000000 qcontext-1.1.0/src/qcontext/widgets/selector.py
+-rw-rw-rw-   0        0        0      927 2023-05-13 21:23:09.000000 qcontext-1.1.0/src/qcontext/widgets/slider.py
+-rw-rw-rw-   0        0        0      371 2023-05-13 21:23:09.000000 qcontext-1.1.0/src/qcontext/widgets/spacer.py
+-rw-rw-rw-   0        0        0     1745 2023-05-13 21:23:09.000000 qcontext-1.1.0/src/qcontext/widgets/splitter.py
+-rw-rw-rw-   0        0        0     1066 2023-05-13 21:23:09.000000 qcontext-1.1.0/src/qcontext/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0      394 2023-05-13 21:23:09.000000 qcontext-1.1.0/src/qcontext/widgets/statusbar.py
+-rw-rw-rw-   0        0        0      781 2023-05-13 21:23:09.000000 qcontext-1.1.0/src/qcontext/widgets/text_input.py
+-rw-rw-rw-   0        0        0      679 2023-05-13 21:23:09.000000 qcontext-1.1.0/src/qcontext/widgets/widget.py
+-rw-rw-rw-   0        0        0      337 2023-05-13 21:23:09.000000 qcontext-1.1.0/src/qcontext/widgets/window.py
+drwxrwxrwx   0        0        0        0 2023-05-13 22:10:59.427255 qcontext-1.1.0/src/qcontext.egg-info/
+-rw-rw-rw-   0        0        0     2758 2023-05-13 22:10:59.000000 qcontext-1.1.0/src/qcontext.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11866 2023-05-13 22:10:59.000000 qcontext-1.1.0/src/qcontext.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-13 22:10:59.000000 qcontext-1.1.0/src/qcontext.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-05-13 22:10:59.000000 qcontext-1.1.0/src/qcontext.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-13 22:10:59.000000 qcontext-1.1.0/src/qcontext.egg-info/top_level.txt
```

### Comparing `qcontext-1.0.9/LICENSE.txt` & `qcontext-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/PKG-INFO` & `qcontext-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcontext
-Version: 1.0.9
+Version: 1.1.0
 Summary: One of the most controversial things
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
         
@@ -36,24 +36,24 @@
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-ToDo:
-    move to pyside6
-    favourite_label is actually a TwoStateIconLabel
-    error_label is actually a PopupTextLabel
-    make all widgets to have:
-        min_height
-        min_width
-        min_size
-        max_height
-        max_width
-        max_size
-        policy
-        margins (in abstract frame)
-        padding (in abstract frame)
-        alignment (in abstract frame)
-    make popup to be generic (configure different buttons (ok, cancel, no, yes)
-    crete generic animation class to create simple animations
+# ToDo:
+- move to pyside6
+- favourite_label is actually a TwoStateIconLabel
+- error_label is actually a PopupTextLabel
+- make all widgets to have:
+    - min_height
+    - min_width
+    - min_size
+    - max_height
+    - max_width
+    - max_size
+    - policy
+    - margins (in abstract frame)
+    - padding (in abstract frame)
+    - alignment (in abstract frame)
+- make popup to be generic (configure different buttons (ok, cancel, no, yes)
+- crete generic animation class to create simple animations
```

### Comparing `qcontext-1.0.9/README.md` & `qcontext-1.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-ToDo:
-    move to pyside6
-    favourite_label is actually a TwoStateIconLabel
-    error_label is actually a PopupTextLabel
-    make all widgets to have:
-        min_height
-        min_width
-        min_size
-        max_height
-        max_width
-        max_size
-        policy
-        margins (in abstract frame)
-        padding (in abstract frame)
-        alignment (in abstract frame)
-    make popup to be generic (configure different buttons (ok, cancel, no, yes)
-    crete generic animation class to create simple animations
+# ToDo:
+- move to pyside6
+- favourite_label is actually a TwoStateIconLabel
+- error_label is actually a PopupTextLabel
+- make all widgets to have:
+    - min_height
+    - min_width
+    - min_size
+    - max_height
+    - max_width
+    - max_size
+    - policy
+    - margins (in abstract frame)
+    - padding (in abstract frame)
+    - alignment (in abstract frame)
+- make popup to be generic (configure different buttons (ok, cancel, no, yes)
+- crete generic animation class to create simple animations
```

### Comparing `qcontext-1.0.9/pyproject.toml` & `qcontext-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qcontext"
-version = "1.0.9"
+version = "1.1.0"
 authors = [
     { name="cxllmerichie", email="cxllmerichie@gmail.com" },
 ]
 maintainers = [
     { name="cxllmerichie", email="cxllmerichie@gmail.com" },
 ]
 description = "One of the most controversial things"
```

### Comparing `qcontext-1.0.9/src/qcontext/.assets/aperture.svg` & `qcontext-1.1.0/src/qcontext/.assets/aperture.svg`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/.assets/cloud-drizzle.svg` & `qcontext-1.1.0/src/qcontext/.assets/cloud-drizzle.svg`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/.assets/cloud-snow.svg` & `qcontext-1.1.0/src/qcontext/.assets/cloud-snow.svg`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/.assets/codesandbox.svg` & `qcontext-1.1.0/src/qcontext/.assets/codesandbox.svg`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/.assets/cpu.svg` & `qcontext-1.1.0/src/qcontext/.assets/cpu.svg`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/.assets/figma.svg` & `qcontext-1.1.0/src/qcontext/.assets/figma.svg`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/.assets/film.svg` & `qcontext-1.1.0/src/qcontext/.assets/film.svg`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/.assets/github.svg` & `qcontext-1.1.0/src/qcontext/.assets/github.svg`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/.assets/life-buoy.svg` & `qcontext-1.1.0/src/qcontext/.assets/life-buoy.svg`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/.assets/loader.svg` & `qcontext-1.1.0/src/qcontext/.assets/loader.svg`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/.assets/package.svg` & `qcontext-1.1.0/src/qcontext/.assets/package.svg`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/.assets/phone-call.svg` & `qcontext-1.1.0/src/qcontext/.assets/phone-call.svg`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/.assets/phone-forwarded.svg` & `qcontext-1.1.0/src/qcontext/.assets/phone-forwarded.svg`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/.assets/phone-incoming.svg` & `qcontext-1.1.0/src/qcontext/.assets/phone-incoming.svg`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/.assets/phone-missed.svg` & `qcontext-1.1.0/src/qcontext/.assets/phone-missed.svg`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/.assets/phone-off.svg` & `qcontext-1.1.0/src/qcontext/.assets/phone-off.svg`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/.assets/phone-outgoing.svg` & `qcontext-1.1.0/src/qcontext/.assets/phone-outgoing.svg`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/.assets/phone.svg` & `qcontext-1.1.0/src/qcontext/.assets/phone.svg`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/.assets/settings.svg` & `qcontext-1.1.0/src/qcontext/.assets/settings.svg`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/.assets/slack.svg` & `qcontext-1.1.0/src/qcontext/.assets/slack.svg`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/.assets/sliders.svg` & `qcontext-1.1.0/src/qcontext/.assets/sliders.svg`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/.assets/sun.svg` & `qcontext-1.1.0/src/qcontext/.assets/sun.svg`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/.assets/sunrise.svg` & `qcontext-1.1.0/src/qcontext/.assets/sunrise.svg`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/.assets/sunset.svg` & `qcontext-1.1.0/src/qcontext/.assets/sunset.svg`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/.assets/wifi-off.svg` & `qcontext-1.1.0/src/qcontext/.assets/wifi-off.svg`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/.assets/youtube.svg` & `qcontext-1.1.0/src/qcontext/.assets/youtube.svg`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/misc/aiorequest.py` & `qcontext-1.1.0/src/qcontext/misc/aiorequest.py`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/misc/conditional_thread_queue.py` & `qcontext-1.1.0/src/qcontext/misc/conditional_thread_queue.py`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/misc/icon.py` & `qcontext-1.1.0/src/qcontext/misc/icon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from PyQt5.QtGui import QPixmap, QIcon, QImage
-from PyQt5.QtCore import QSize, QBuffer, QIODevice
+from PySide6.QtGui import QPixmap, QIcon, QImage
+from PySide6.QtCore import QSize, QBuffer, QIODevice
 # from loguru import logger
 import base64
 import site
 import os
 
 from .size import Size
```

### Comparing `qcontext-1.0.9/src/qcontext/misc/stylesheet_parser.py` & `qcontext-1.1.0/src/qcontext/misc/stylesheet_parser.py`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/misc/uvicorn_threaded_server.py` & `qcontext-1.1.0/src/qcontext/misc/uvicorn_threaded_server.py`

 * *Files identical despite different names*

### Comparing `qcontext-1.0.9/src/qcontext/qasyncio.py` & `qcontext-1.1.0/src/qcontext/qasyncio.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 import functools
 import asyncio
 import qasync
 import sys
 from qasync import asyncSlot  # to import `asyncSlot` from `qasyncio`
 
 
+# def callableAsyncSlot(to_call):
+#     @asyncSlot()
+#     async def wrapped():
+#         print(type(to_call))
+#         if to_call.__class__.__name__ in ('function', 'method'):
+#             await to_call()
+#         # elif
+#     return wrapped
+
+
 class AsyncApp:
     @staticmethod
     def run(run_app):
         async def wrap():
             def close_future(future, loop):
                 loop.call_later(10, future.cancel)
                 future.cancel()
```

### Comparing `qcontext-1.0.9/src/qcontext/widgets/__init__.py` & `qcontext-1.1.0/src/qcontext/widgets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 from .statusbar import StatusBar
 from .window import Window
 from .slider import Slider
 
 from .layout import Layout
 from .spacer import Spacer
 
-from PyQt5.QtWidgets import QWidget
+from PySide6.QtWidgets import QWidget
```

### Comparing `qcontext-1.0.9/src/qcontext/widgets/button.py` & `qcontext-1.1.0/src/qcontext/widgets/button.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from PyQt5.QtWidgets import QPushButton, QWidget, QSizePolicy
-from PyQt5.QtCore import QSize
-from PyQt5.QtGui import QIcon
+from PySide6.QtWidgets import QPushButton, QWidget, QSizePolicy
+from PySide6.QtCore import QSize
+from PySide6.QtGui import QIcon
 from contextlib import suppress
 
 from ..misc import Icon
 from .extensions import ContextObjectExt
 
 
 class Button(ContextObjectExt, QPushButton):
```

### Comparing `qcontext-1.0.9/src/qcontext/widgets/custom/date_picker.py` & `qcontext-1.1.0/src/qcontext/widgets/custom/date_picker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from PyQt5.QtWidgets import QWidget
+from PySide6.QtWidgets import QWidget
 from datetime import datetime, time, date, timezone
-from PyQt5.QtCore import Qt
+from PySide6.QtCore import Qt
 from calendar import monthrange
 from dateutil import parser
 
 from ..frame import Frame
 from ..layout import Layout
 from ..selector import Selector
 from ..label import Label
```

### Comparing `qcontext-1.0.9/src/qcontext/widgets/custom/error_label.py` & `qcontext-1.1.0/src/qcontext/widgets/custom/error_label.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from PyQt5.QtCore import QPropertyAnimation, pyqtProperty
-from PyQt5.QtWidgets import QWidget
+from PySide6.QtCore import QPropertyAnimation, pyqtProperty
+from PySide6.QtWidgets import QWidget
 from time import sleep
 from qasync import asyncSlot
 
 from ...misc import ConditionalThreadQueue
 from ..label import Label
 from ..button import Button
```

### Comparing `qcontext-1.0.9/src/qcontext/widgets/custom/favourite_button.py` & `qcontext-1.1.0/src/qcontext/widgets/custom/favourite_button.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from PyQt5.QtWidgets import QWidget
-from PyQt5.QtGui import QIcon
+from PySide6.QtWidgets import QWidget
+from PySide6.QtGui import QIcon
 from typing import Callable
 from qasync import asyncSlot
 
 from ..button import Button
 from ...misc import Icon
```

### Comparing `qcontext-1.0.9/src/qcontext/widgets/custom/image_button.py` & `qcontext-1.1.0/src/qcontext/widgets/custom/image_button.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from PyQt5.QtWidgets import QWidget, QFileDialog
-from PyQt5.QtCore import QSize
-from PyQt5.QtGui import QIcon
+from PySide6.QtWidgets import QWidget, QFileDialog
+from PySide6.QtCore import QSize
+from PySide6.QtGui import QIcon
 from contextlib import suppress
 from qasync import asyncSlot
 
 from ..button import Button
 from ..popup import Popup
 from ...misc import Icon
```

### Comparing `qcontext-1.0.9/src/qcontext/widgets/custom/label_extended.py` & `qcontext-1.1.0/src/qcontext/widgets/custom/label_extended.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from PyQt5.QtWidgets import QWidget, QSizePolicy
-from PyQt5.QtCore import Qt, QSize
+from PySide6.QtWidgets import QWidget, QSizePolicy
+from PySide6.QtCore import Qt, QSize
 
 from ..frame import Frame
 from ..label import Label
 from ..layout import Layout
 from ...misc import Icon
```

### Comparing `qcontext-1.0.9/src/qcontext/widgets/custom/menu_button.py` & `qcontext-1.1.0/src/qcontext/widgets/custom/menu_button.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from PyQt5.QtWidgets import QWidget, QSizePolicy
-from PyQt5.QtCore import Qt
+from PySide6.QtWidgets import QWidget, QSizePolicy
+from PySide6.QtCore import Qt
 
 from ..button import Button
 from ..label import Label
 from ..layout import Layout
 from ...misc import Icon
```

### Comparing `qcontext-1.0.9/src/qcontext/widgets/custom/search_bar.py` & `qcontext-1.1.0/src/qcontext/widgets/custom/search_bar.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from PyQt5.QtWidgets import QWidget, QCompleter, QStyledItemDelegate
-from PyQt5.QtCore import Qt
+from PySide6.QtWidgets import QWidget, QCompleter, QStyledItemDelegate
+from PySide6.QtCore import Qt
 from typing import Iterable
 
 from ..line_input import LineInput
 
 
 class SearchBar(LineInput):
     def __init__(self, parent: QWidget, name: str = None, visible: bool = True):
```

### Comparing `qcontext-1.0.9/src/qcontext/widgets/extensions/alignment_ext.py` & `qcontext-1.1.0/src/qcontext/widgets/extensions/alignment.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyQt5.QtCore import Qt
+from PySide6.QtCore import Qt
 
 
 class AlignmentExt:
     Left = Qt.AlignLeft
     LeftTop = Qt.AlignLeft | Qt.AlignTop
     LeftCenter = Qt.AlignLeft | Qt.AlignVCenter
     LeftBottom = Qt.AlignLeft | Qt.AlignBottom
```

### Comparing `qcontext-1.0.9/src/qcontext/widgets/extensions/context_object_ext.py` & `qcontext-1.1.0/src/qcontext/widgets/extensions/context_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyQt5.QtWidgets import QWidget
+from PySide6.QtWidgets import QWidget
 from loguru import logger as _logger
 from contextlib import suppress as _suppress
 import uuid
 
 from ...contextapi import CONTEXT
 
 
@@ -28,15 +28,15 @@
                 attributes.append('`name`')
             if CONTEXT.debug:
                 _logger.warning(f"{self.__class__.__name__} not registered in `ContextAPI` since {' and '.join(attributes)} not specified")
 
         with _suppress(Exception):
             self.setVisible(visible)
 
-    def register(self, parent: QWidget, name: str, child: QWidget) -> None:
+    def register(self, parent: object, name: str, child: QWidget) -> None:
         """
         Check if object not in `blacklist`, then register, otherwise show warning
         Check if object already registered, push its name to `blacklist` unregister and show warning otherwise register
         :param parent:
         :param name:
         :param child:
         :return:
```

### Comparing `qcontext-1.0.9/src/qcontext/widgets/extensions/layout_ext.py` & `qcontext-1.1.0/src/qcontext/widgets/extensions/layout.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from PyQt5.QtWidgets import QWidget, QLayoutItem, QSpacerItem
-from PyQt5.QtCore import Qt, QObject
+from PySide6.QtWidgets import QWidget, QLayoutItem, QSpacerItem
+from PySide6.QtCore import Qt, QObject
 from typing import Sequence, Iterable
 
 
 class LayoutExt:
     async def init(
             self, *,
             margins: tuple[int, ...] = (0, 0, 0, 0), spacing: int = 0, alignment: Qt.Alignment = None,
```

### Comparing `qcontext-1.0.9/src/qcontext/widgets/extensions/side_menu_ext.py` & `qcontext-1.1.0/src/qcontext/widgets/extensions/side_menu.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyQt5.QtCore import Qt
+from PySide6.QtCore import Qt
 
 
 class SideMenuExt:
     def __init__(self, expand_to, expand_orientation: Qt.Orientation = Qt.Horizontal):
         self.expand_to = expand_to
         self.expand_orientation = expand_orientation
```

### Comparing `qcontext-1.0.9/src/qcontext/widgets/extensions/splitter_widget_ext.py` & `qcontext-1.1.0/src/qcontext/widgets/extensions/splitter_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from PyQt5.QtWidgets import QSplitter, QSizePolicy
-from PyQt5.QtCore import Qt
+from PySide6.QtWidgets import QSplitter, QSizePolicy
+from PySide6.QtCore import Qt
 from loguru import logger as _logger
 
 
 class SplitterWidgetExt:
     splitter: QSplitter
 
     def __init__(self, expand_to: int,
```

### Comparing `qcontext-1.0.9/src/qcontext/widgets/frame.py` & `qcontext-1.1.0/src/qcontext/widgets/frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyQt5.QtWidgets import QFrame, QWidget, QLayout, QSizePolicy
+from PySide6.QtWidgets import QFrame, QWidget, QLayout, QSizePolicy
 
 from .extensions import ContextObjectExt
 
 
 class Frame(ContextObjectExt, QFrame):
     def __init__(self, parent: QWidget, name: str, visible: bool = True, stylesheet: str = None):
         QFrame.__init__(self, parent)
```

### Comparing `qcontext-1.0.9/src/qcontext/widgets/label.py` & `qcontext-1.1.0/src/qcontext/widgets/label.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from PyQt5.QtGui import QFontMetrics, QPaintEvent
-from PyQt5.QtWidgets import QLabel, QWidget, QSizePolicy
-from PyQt5.QtCore import Qt, QSize
+from PySide6.QtGui import QFontMetrics, QPaintEvent
+from PySide6.QtWidgets import QLabel, QWidget, QSizePolicy
+from PySide6.QtCore import Qt, QSize
 
 from ..misc import Icon
 from .extensions import ContextObjectExt, AlignmentExt
 
 
 class Label(ContextObjectExt, AlignmentExt, QLabel):
     __elided = False
```

### Comparing `qcontext-1.0.9/src/qcontext/widgets/layout.py` & `qcontext-1.1.0/src/qcontext/widgets/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from PyQt5.QtWidgets import QVBoxLayout, QWidget, QHBoxLayout
-from PyQt5.QtCore import Qt
+from PySide6.QtWidgets import QVBoxLayout, QWidget, QHBoxLayout
+from PySide6.QtCore import Qt
 from typing import Union
 from abc import ABC
 
 from .extensions import ContextObjectExt, LayoutExt, AlignmentExt, PolicyExt, OrientationExt
 
 
 class Layout(ABC, AlignmentExt, PolicyExt, OrientationExt):
```

### Comparing `qcontext-1.0.9/src/qcontext/widgets/line_input.py` & `qcontext-1.1.0/src/qcontext/widgets/line_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from PyQt5.QtWidgets import QLineEdit, QWidget
-from PyQt5.QtCore import Qt
+from PySide6.QtWidgets import QLineEdit, QWidget
+from PySide6.QtCore import Qt
 
 from .extensions import ContextObjectExt
 
 
 class LineInput(ContextObjectExt, QLineEdit):
     def __init__(self, parent: QWidget, name: str, visible: bool = True):
         QLineEdit.__init__(self, parent)
```

### Comparing `qcontext-1.0.9/src/qcontext/widgets/popup.py` & `qcontext-1.1.0/src/qcontext/widgets/popup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from PyQt5.QtGui import QResizeEvent
-from PyQt5.QtWidgets import QMessageBox, QWidget
+from PySide6.QtGui import QResizeEvent
+from PySide6.QtWidgets import QMessageBox, QWidget
 from qasync import asyncSlot
 from typing import Iterable
 
 from .widget import Widget
 from .layout import Layout
 from .button import Button
 from .label import Label
 from .frame import Frame
 
 
 class Popup(Widget):
-    YES = QMessageBox.Yes
-    NO = QMessageBox.No
-    OK = QMessageBox.Ok
-    CANCEL = QMessageBox.Cancel
+    YES = QMessageBox.StandardButton.Yes
+    NO = QMessageBox.StandardButton.No
+    OK = QMessageBox.StandardButton.Ok
+    CANCEL = QMessageBox.StandardButton.Cancel
 
     stylesheet = f'''
         #Popup {{
             background-color: rgba(255, 255, 255, 0.1);
         }}
 
         #PopupFrame {{
```

### Comparing `qcontext-1.0.9/src/qcontext/widgets/scroll_area.py` & `qcontext-1.1.0/src/qcontext/widgets/scroll_area.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from PyQt5.QtWidgets import QScrollArea, QWidget, QSizePolicy
-from PyQt5.QtCore import Qt, QObject
+from PySide6.QtWidgets import QScrollArea, QWidget, QSizePolicy
+from PySide6.QtCore import Qt, QObject
 from typing import Sequence, Iterable
 
 from .frame import Frame
 from .layout import Layout
 from .extensions import ContextObjectExt
```

### Comparing `qcontext-1.0.9/src/qcontext/widgets/selector.py` & `qcontext-1.1.0/src/qcontext/widgets/selector.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyQt5.QtWidgets import QComboBox, QWidget
+from PySide6.QtWidgets import QComboBox, QWidget
 from typing import Iterable, Any
 
 from ..misc import Icon
 from .extensions import ContextObjectExt
 
 
 class Selector(ContextObjectExt, QComboBox):
```

### Comparing `qcontext-1.0.9/src/qcontext/widgets/slider.py` & `qcontext-1.1.0/src/qcontext/widgets/slider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyQt5.QtWidgets import QSlider, QWidget
+from PySide6.QtWidgets import QSlider, QWidget
 
 from .extensions import ContextObjectExt, OrientationExt
 
 
 class Slider(ContextObjectExt, OrientationExt, QSlider):
     def __init__(self, parent: QWidget, name: str, visible: bool = True):
         QSlider.__init__(self, parent)
```

### Comparing `qcontext-1.0.9/src/qcontext/widgets/splitter.py` & `qcontext-1.1.0/src/qcontext/widgets/splitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from PyQt5.QtWidgets import QWidget, QSplitter, QSizePolicy
-from PyQt5.QtCore import Qt
+from PySide6.QtWidgets import QWidget, QSplitter, QSizePolicy
+from PySide6.QtCore import Qt
 from typing import Iterable
 
 from .widget import Widget
 from .extensions import ContextObjectExt, SplitterWidgetExt
 
 
 class SplitterHandle(Widget):
```

### Comparing `qcontext-1.0.9/src/qcontext/widgets/stacked_widget.py` & `qcontext-1.1.0/src/qcontext/widgets/stacked_widget.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from PyQt5.QtWidgets import QWidget, QStackedWidget
-from PyQt5.QtCore import Qt
+from PySide6.QtWidgets import QWidget, QStackedWidget
+from PySide6.QtCore import Qt
 
 from .extensions import ContextObjectExt
 
 
 class StackedWidget(ContextObjectExt, QStackedWidget):
     def __init__(self, parent: QWidget, name: str, visible: bool = True, stylesheet: str = None):
         QStackedWidget.__init__(self, parent)
```

### Comparing `qcontext-1.0.9/src/qcontext/widgets/text_input.py` & `qcontext-1.1.0/src/qcontext/widgets/text_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyQt5.QtWidgets import QTextEdit, QWidget, QSizePolicy
+from PySide6.QtWidgets import QTextEdit, QWidget, QSizePolicy
 
 from .extensions import ContextObjectExt
 
 
 class TextInput(ContextObjectExt, QTextEdit):
     def __init__(self, parent: QWidget, name: str, visible: bool = True):
         QTextEdit.__init__(self, parent)
```

### Comparing `qcontext-1.0.9/src/qcontext/widgets/widget.py` & `qcontext-1.1.0/src/qcontext/widgets/widget.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from PyQt5.QtWidgets import QWidget, QLayout
-from PyQt5.QtCore import Qt
+from PySide6.QtWidgets import QWidget, QLayout
+from PySide6.QtCore import Qt
 
 from .extensions import ContextObjectExt
 
 
 class Widget(ContextObjectExt, QWidget):
     def __init__(self, parent: QWidget, name: str, visible: bool = True, stylesheet: str = None):
         QWidget.__init__(self, parent)
```

### Comparing `qcontext-1.0.9/src/qcontext.egg-info/PKG-INFO` & `qcontext-1.1.0/src/qcontext.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcontext
-Version: 1.0.9
+Version: 1.1.0
 Summary: One of the most controversial things
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
         
@@ -36,24 +36,24 @@
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-ToDo:
-    move to pyside6
-    favourite_label is actually a TwoStateIconLabel
-    error_label is actually a PopupTextLabel
-    make all widgets to have:
-        min_height
-        min_width
-        min_size
-        max_height
-        max_width
-        max_size
-        policy
-        margins (in abstract frame)
-        padding (in abstract frame)
-        alignment (in abstract frame)
-    make popup to be generic (configure different buttons (ok, cancel, no, yes)
-    crete generic animation class to create simple animations
+# ToDo:
+- move to pyside6
+- favourite_label is actually a TwoStateIconLabel
+- error_label is actually a PopupTextLabel
+- make all widgets to have:
+    - min_height
+    - min_width
+    - min_size
+    - max_height
+    - max_width
+    - max_size
+    - policy
+    - margins (in abstract frame)
+    - padding (in abstract frame)
+    - alignment (in abstract frame)
+- make popup to be generic (configure different buttons (ok, cancel, no, yes)
+- crete generic animation class to create simple animations
```

### Comparing `qcontext-1.0.9/src/qcontext.egg-info/SOURCES.txt` & `qcontext-1.1.0/src/qcontext.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -331,14 +331,15 @@
 src/qcontext/widgets/custom/error_label.py
 src/qcontext/widgets/custom/favourite_button.py
 src/qcontext/widgets/custom/image_button.py
 src/qcontext/widgets/custom/label_extended.py
 src/qcontext/widgets/custom/menu_button.py
 src/qcontext/widgets/custom/search_bar.py
 src/qcontext/widgets/extensions/__init__.py
-src/qcontext/widgets/extensions/alignment_ext.py
-src/qcontext/widgets/extensions/context_object_ext.py
-src/qcontext/widgets/extensions/layout_ext.py
-src/qcontext/widgets/extensions/orientation_ext.py
-src/qcontext/widgets/extensions/policy_ext.py
-src/qcontext/widgets/extensions/side_menu_ext.py
-src/qcontext/widgets/extensions/splitter_widget_ext.py
+src/qcontext/widgets/extensions/alignment.py
+src/qcontext/widgets/extensions/context_object.py
+src/qcontext/widgets/extensions/event.py
+src/qcontext/widgets/extensions/layout.py
+src/qcontext/widgets/extensions/orientation.py
+src/qcontext/widgets/extensions/policy.py
+src/qcontext/widgets/extensions/side_menu.py
+src/qcontext/widgets/extensions/splitter_widget.py
```

