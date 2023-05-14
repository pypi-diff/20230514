# Comparing `tmp/chitose-0.0.4.tar.gz` & `tmp/chitose-0.0.5.tar.gz`

## Comparing `chitose-0.0.4.tar` & `chitose-0.0.5.tar`

### file list

```diff
@@ -1,156 +1,170 @@
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 chitose-0.0.4/.gitmodules
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 chitose-0.0.4/.readthedocs.yaml
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/__init__.py
--rw-r--r--   0        0        0     7775 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/agent.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/blob.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/link.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/object.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/record.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/xrpc.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/__init__.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/__init__.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/actor/__init__.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/actor/defs.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/actor/get_profile.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/actor/get_profiles.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/actor/get_suggestions.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/actor/profile.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/actor/search_actors.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/actor/search_actors_typeahead.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/embed/__init__.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/embed/external.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/embed/images.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/embed/record.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/embed/record_with_media.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/feed/__init__.py
--rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/feed/defs.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/feed/get_author_feed.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/feed/get_likes.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/feed/get_post_thread.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/feed/get_posts.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/feed/get_reposted_by.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/feed/get_timeline.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/feed/like.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/feed/post.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/feed/repost.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/graph/__init__.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/graph/block.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/graph/follow.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/graph/get_blocks.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/graph/get_followers.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/graph/get_follows.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/graph/get_mutes.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/graph/mute_actor.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/graph/unmute_actor.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/notification/__init__.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/notification/get_unread_count.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/notification/list_notifications.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/notification/update_seen.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/richtext/__init__.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/richtext/facet.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/unspecced/__init__.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/app/bsky/unspecced/get_popular.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/__init__.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/__init__.py
--rw-r--r--   0        0        0     4961 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/admin/__init__.py
--rw-r--r--   0        0        0    12283 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/admin/defs.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/admin/disable_invite_codes.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/admin/get_invite_codes.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/admin/get_moderation_action.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/admin/get_moderation_actions.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/admin/get_moderation_report.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/admin/get_moderation_reports.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/admin/get_record.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/admin/get_repo.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/admin/resolve_moderation_reports.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/admin/reverse_moderation_action.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/admin/search_repos.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/admin/take_moderation_action.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/admin/update_account_email.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/admin/update_account_handle.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/identity/__init__.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/identity/resolve_handle.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/identity/update_handle.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/label/__init__.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/label/defs.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/label/query_labels.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/label/subscribe_labels.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/moderation/__init__.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/moderation/create_report.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/moderation/defs.py
--rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/repo/__init__.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/repo/apply_writes.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/repo/create_record.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/repo/delete_record.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/repo/describe_repo.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/repo/get_record.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/repo/list_records.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/repo/put_record.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/repo/strong_ref.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/repo/upload_blob.py
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/server/__init__.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/server/create_account.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/server/create_app_password.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/server/create_invite_code.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/server/create_invite_codes.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/server/create_session.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/server/defs.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/server/delete_account.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/server/delete_session.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/server/describe_server.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/server/get_account_invite_codes.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/server/get_session.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/server/list_app_passwords.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/server/refresh_session.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/server/request_account_delete.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/server/request_password_reset.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/server/reset_password.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/server/revoke_app_password.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/sync/__init__.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/sync/get_blob.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/sync/get_blocks.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/sync/get_checkout.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/sync/get_commit_path.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/sync/get_head.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/sync/get_record.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/sync/get_repo.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/sync/list_blobs.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/sync/list_repos.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/sync/notify_of_update.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/sync/request_crawl.py
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 chitose-0.0.4/chitose/com/atproto/sync/subscribe_repos.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 chitose-0.0.4/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 chitose-0.0.4/docs/make.bat
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 chitose-0.0.4/docs/source/chitose.app.bsky.actor.rst
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 chitose-0.0.4/docs/source/chitose.app.bsky.embed.rst
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 chitose-0.0.4/docs/source/chitose.app.bsky.feed.rst
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 chitose-0.0.4/docs/source/chitose.app.bsky.graph.rst
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 chitose-0.0.4/docs/source/chitose.app.bsky.notification.rst
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 chitose-0.0.4/docs/source/chitose.app.bsky.richtext.rst
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 chitose-0.0.4/docs/source/chitose.app.bsky.rst
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 chitose-0.0.4/docs/source/chitose.app.bsky.unspecced.rst
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 chitose-0.0.4/docs/source/chitose.app.rst
--rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 chitose-0.0.4/docs/source/chitose.com.atproto.admin.rst
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 chitose-0.0.4/docs/source/chitose.com.atproto.identity.rst
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 chitose-0.0.4/docs/source/chitose.com.atproto.label.rst
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 chitose-0.0.4/docs/source/chitose.com.atproto.moderation.rst
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 chitose-0.0.4/docs/source/chitose.com.atproto.repo.rst
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 chitose-0.0.4/docs/source/chitose.com.atproto.rst
--rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 chitose-0.0.4/docs/source/chitose.com.atproto.server.rst
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 chitose-0.0.4/docs/source/chitose.com.atproto.sync.rst
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 chitose-0.0.4/docs/source/chitose.com.rst
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 chitose-0.0.4/docs/source/chitose.rst
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 chitose-0.0.4/docs/source/conf.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 chitose-0.0.4/docs/source/index.rst
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 chitose-0.0.4/docs/source/modules.rst
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 chitose-0.0.4/examples/get_profiles.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 chitose-0.0.4/examples/get_timeline.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 chitose-0.0.4/examples/post.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 chitose-0.0.4/examples/post_with_image.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 chitose-0.0.4/examples/simple_get_timeline.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 chitose-0.0.4/examples/simple_post.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 chitose-0.0.4/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 chitose-0.0.4/LICENSE
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 chitose-0.0.4/README.md
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 chitose-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 chitose-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 chitose-0.0.5/.gitmodules
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 chitose-0.0.5/.readthedocs.yaml
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/__init__.py
+-rw-r--r--   0        0        0     7877 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/agent.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/blob.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/link.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/object.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/record.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/xrpc.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/__init__.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/__init__.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/actor/__init__.py
+-rw-r--r--   0        0        0     4950 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/actor/defs.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/actor/get_preferences.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/actor/get_profile.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/actor/get_profiles.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/actor/get_suggestions.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/actor/profile.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/actor/put_preferences.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/actor/search_actors.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/actor/search_actors_typeahead.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/embed/__init__.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/embed/external.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/embed/images.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/embed/record.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/embed/record_with_media.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/feed/__init__.py
+-rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/feed/defs.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/feed/get_author_feed.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/feed/get_likes.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/feed/get_post_thread.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/feed/get_posts.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/feed/get_reposted_by.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/feed/get_timeline.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/feed/like.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/feed/post.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/feed/repost.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/__init__.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/block.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/defs.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/follow.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/get_blocks.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/get_followers.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/get_follows.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/get_list.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/get_list_mutes.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/get_lists.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/get_mutes.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/list.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/listitem.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/mute_actor.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/mute_actor_list.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/unmute_actor.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/graph/unmute_actor_list.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/notification/__init__.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/notification/get_unread_count.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/notification/list_notifications.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/notification/update_seen.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/richtext/__init__.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/richtext/facet.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/unspecced/__init__.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/app/bsky/unspecced/get_popular.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/__init__.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/__init__.py
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/__init__.py
+-rw-r--r--   0        0        0    12486 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/defs.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/disable_account_invites.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/disable_invite_codes.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/enable_account_invites.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/get_invite_codes.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/get_moderation_action.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/get_moderation_actions.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/get_moderation_report.py
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/get_moderation_reports.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/get_record.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/get_repo.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/resolve_moderation_reports.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/reverse_moderation_action.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/search_repos.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/take_moderation_action.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/update_account_email.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/admin/update_account_handle.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/identity/__init__.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/identity/resolve_handle.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/identity/update_handle.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/label/__init__.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/label/defs.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/label/query_labels.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/label/subscribe_labels.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/moderation/__init__.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/moderation/create_report.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/moderation/defs.py
+-rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/repo/__init__.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/repo/apply_writes.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/repo/create_record.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/repo/delete_record.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/repo/describe_repo.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/repo/get_record.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/repo/list_records.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/repo/put_record.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/repo/rebase_repo.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/repo/strong_ref.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/repo/upload_blob.py
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/create_account.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/create_app_password.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/create_invite_code.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/create_invite_codes.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/create_session.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/defs.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/delete_account.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/delete_session.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/describe_server.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/get_account_invite_codes.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/get_session.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/list_app_passwords.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/refresh_session.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/request_account_delete.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/request_password_reset.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/reset_password.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/server/revoke_app_password.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/sync/__init__.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/sync/get_blob.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/sync/get_blocks.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/sync/get_checkout.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/sync/get_commit_path.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/sync/get_head.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/sync/get_record.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/sync/get_repo.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/sync/list_blobs.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/sync/list_repos.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/sync/notify_of_update.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/sync/request_crawl.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 chitose-0.0.5/chitose/com/atproto/sync/subscribe_repos.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/make.bat
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.app.bsky.actor.rst
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.app.bsky.embed.rst
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.app.bsky.feed.rst
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.app.bsky.graph.rst
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.app.bsky.notification.rst
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.app.bsky.richtext.rst
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.app.bsky.rst
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.app.bsky.unspecced.rst
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.app.rst
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.com.atproto.admin.rst
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.com.atproto.identity.rst
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.com.atproto.label.rst
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.com.atproto.moderation.rst
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.com.atproto.repo.rst
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.com.atproto.rst
+-rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.com.atproto.server.rst
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.com.atproto.sync.rst
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.com.rst
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/chitose.rst
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/conf.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/index.rst
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 chitose-0.0.5/docs/source/modules.rst
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 chitose-0.0.5/examples/get_profiles.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 chitose-0.0.5/examples/get_timeline.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 chitose-0.0.5/examples/post.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 chitose-0.0.5/examples/post_with_image.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 chitose-0.0.5/examples/quote_post.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 chitose-0.0.5/examples/simple_get_timeline.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 chitose-0.0.5/examples/simple_post.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 chitose-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 chitose-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 chitose-0.0.5/README.md
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 chitose-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 chitose-0.0.5/PKG-INFO
```

### Comparing `chitose-0.0.4/chitose/agent.py` & `chitose-0.0.5/chitose/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 from datetime import datetime
+from datetime import timezone
 import typing
 import json
 
 from chitose.app.bsky.feed.like import Like
 from chitose.app.bsky.feed.post import Post
 from chitose.app.bsky.feed.repost import Repost
 from chitose.app.bsky.graph.follow import Follow
@@ -80,15 +81,15 @@
         return self.app.bsky.actor.search_actors_typeahead(**kwargs)
 
     def list_notifications(self, **kwargs: dict[str, typing.Any]) -> bytes:
         """See :doc:`chitose.app.bsky.notification` for available arguments."""
         return self.app.bsky.notification.list_notifications(**kwargs)
 
     def count_unread_notifications(self, **kwargs: dict[str, typing.Any]) -> bytes:
-        """See :doc:`chitose.app.bsky.notification` for available arguments."""
+        """See `get_unread_count()` in :doc:`chitose.app.bsky.notification` for available arguments."""
         return self.app.bsky.notification.get_unread_count(**kwargs)
 
     def post(self, record: Post) -> bytes:
         if not self.session:
             raise Exception('Not logged in')
 
         return self.com.atproto.repo.create_record(
@@ -116,15 +117,15 @@
 
     def like(self, uri: str, cid: str) -> bytes:
         if not self.session:
             raise Exception('Not logged in')
 
         subject = StrongRef(uri=uri, cid=cid)
         record = Like(subject=subject,
-                      created_at=datetime.now().isoformat())
+                      created_at=datetime.now(timezone.utc).isoformat())
 
         return self.com.atproto.repo.create_record(
             repo=self.session['did'],
             collection='app.bsky.feed.like',
             record=record)
 
     def delete_like(self, like_uri: str) -> bytes:
@@ -139,15 +140,15 @@
 
     def repost(self, uri: str, cid: str) -> bytes:
         if not self.session:
             raise Exception('Not logged in')
 
         subject = StrongRef(uri=uri, cid=cid)
         record = Repost(subject=subject,
-                        created_at=datetime.now().isoformat())
+                        created_at=datetime.now(timezone.utc).isoformat())
 
         return self.com.atproto.repo.create_record(
             repo=self.session['did'],
             collection='app.bsky.feed.repost',
             record=record)
 
     def delete_repost(self, repost_uri: str) -> bytes:
@@ -161,15 +162,15 @@
             rkey=rkey)
 
     def follow(self, subject_did: str) -> bytes:
         if not self.session:
             raise Exception('Not logged in')
 
         record = Follow(subject=subject_did,
-                        created_at=datetime.now().isoformat())
+                        created_at=datetime.now(timezone.utc).isoformat())
 
         return self.com.atproto.repo.create_record(
             repo=self.session['did'],
             collection='app.bsky.graph.follow',
             record=record)
 
     def delete_follow(self, follow_uri: str) -> bytes:
@@ -186,15 +187,15 @@
         return self.app.bsky.graph.mute_actor(actor=actor)
 
     def unmute_actor(self, actor: str) -> bytes:
         return self.app.bsky.graph.unmute_actor(actor=actor)
 
     def update_seen_notifications(self, seen_at: typing.Optional[str]) -> bytes:
         if seen_at is None:
-            seen_at = datetime.now().isoformat()
+            seen_at = datetime.now(timezone.utc).isoformat()
 
         return self.app.bsky.notification.update_seen(seen_at=seen_at)
 
     def login(self, identifier: str, password: str) -> None:
         self.session = json.loads(
             self.com.atproto.server.create_session(
                 identifier=identifier, password=password))
```

### Comparing `chitose-0.0.4/chitose/xrpc.py` & `chitose-0.0.5/chitose/xrpc.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/app/bsky/__init__.py` & `chitose-0.0.5/chitose/app/bsky/__init__.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/app/bsky/actor/defs.py` & `chitose-0.0.5/chitose/app/bsky/actor/defs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # GENERATED CODE - DO NOT MODIFY
 """A reference to an actor in the network."""
 from __future__ import annotations
 import chitose
 import chitose.app.bsky.actor.defs
+import chitose.app.bsky.graph.defs
 import chitose.com.atproto.label.defs
 import typing
 
 class ProfileViewBasic(chitose.Object):
     """"""
 
     def __init__(self, did: str, handle: str, display_name: typing.Optional[str]=None, avatar: typing.Optional[str]=None, viewer: typing.Optional[chitose.app.bsky.actor.defs.ViewerState]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None) -> None:
@@ -55,16 +56,37 @@
 
     def to_dict(self) -> dict:
         return {'did': self.did, 'handle': self.handle, 'displayName': self.display_name, 'description': self.description, 'avatar': self.avatar, 'banner': self.banner, 'followersCount': self.followers_count, 'followsCount': self.follows_count, 'postsCount': self.posts_count, 'indexedAt': self.indexed_at, 'viewer': self.viewer, 'labels': self.labels, '$type': 'app.bsky.actor.defs#profileViewDetailed'}
 
 class ViewerState(chitose.Object):
     """"""
 
-    def __init__(self, muted: typing.Optional[str]=None, blocked_by: typing.Optional[str]=None, blocking: typing.Optional[str]=None, following: typing.Optional[str]=None, followed_by: typing.Optional[str]=None) -> None:
+    def __init__(self, muted: typing.Optional[str]=None, muted_by_list: typing.Optional[chitose.app.bsky.graph.defs.ListViewBasic]=None, blocked_by: typing.Optional[str]=None, blocking: typing.Optional[str]=None, following: typing.Optional[str]=None, followed_by: typing.Optional[str]=None) -> None:
         self.muted = muted
+        self.muted_by_list = muted_by_list
         self.blocked_by = blocked_by
         self.blocking = blocking
         self.following = following
         self.followed_by = followed_by
 
     def to_dict(self) -> dict:
-        return {'muted': self.muted, 'blockedBy': self.blocked_by, 'blocking': self.blocking, 'following': self.following, 'followedBy': self.followed_by, '$type': 'app.bsky.actor.defs#viewerState'}
+        return {'muted': self.muted, 'mutedByList': self.muted_by_list, 'blockedBy': self.blocked_by, 'blocking': self.blocking, 'following': self.following, 'followedBy': self.followed_by, '$type': 'app.bsky.actor.defs#viewerState'}
+Preferences = list[typing.Union['chitose.app.bsky.actor.defs.AdultContentPref', 'chitose.app.bsky.actor.defs.ContentLabelPref']]
+
+class AdultContentPref(chitose.Object):
+    """"""
+
+    def __init__(self, enabled: str) -> None:
+        self.enabled = enabled
+
+    def to_dict(self) -> dict:
+        return {'enabled': self.enabled, '$type': 'app.bsky.actor.defs#adultContentPref'}
+
+class ContentLabelPref(chitose.Object):
+    """"""
+
+    def __init__(self, label: str, visibility: typing.Literal['show', 'warn', 'hide']) -> None:
+        self.label = label
+        self.visibility = visibility
+
+    def to_dict(self) -> dict:
+        return {'label': self.label, 'visibility': self.visibility, '$type': 'app.bsky.actor.defs#contentLabelPref'}
```

### Comparing `chitose-0.0.4/chitose/app/bsky/actor/profile.py` & `chitose-0.0.5/chitose/app/bsky/actor/profile.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/app/bsky/embed/external.py` & `chitose-0.0.5/chitose/app/bsky/embed/external.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/app/bsky/embed/images.py` & `chitose-0.0.5/chitose/app/bsky/embed/images.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/app/bsky/embed/record.py` & `chitose-0.0.5/chitose/app/bsky/embed/record.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/app/bsky/embed/record_with_media.py` & `chitose-0.0.5/chitose/app/bsky/embed/record_with_media.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/app/bsky/feed/__init__.py` & `chitose-0.0.5/chitose/app/bsky/feed/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 from .get_author_feed import _get_author_feed
 from .get_likes import _get_likes
 from .get_post_thread import _get_post_thread
 from .get_posts import _get_posts
 from .get_reposted_by import _get_reposted_by
 from .get_timeline import _get_timeline
-import chitose
+import chitose.app.bsky.actor.defs
 import typing
 
 class Feed_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
     def __init__(self, service: str, headers: dict[str, str]) -> None:
         self.service = service
```

### Comparing `chitose-0.0.4/chitose/app/bsky/feed/defs.py` & `chitose-0.0.5/chitose/app/bsky/feed/defs.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/app/bsky/feed/get_likes.py` & `chitose-0.0.5/chitose/app/bsky/feed/get_likes.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/app/bsky/feed/post.py` & `chitose-0.0.5/chitose/app/bsky/feed/post.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/app/bsky/graph/__init__.py` & `chitose-0.0.5/chitose/app/bsky/graph/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,65 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 from .get_blocks import _get_blocks
 from .get_followers import _get_followers
 from .get_follows import _get_follows
+from .get_list import _get_list
+from .get_list_mutes import _get_list_mutes
+from .get_lists import _get_lists
 from .get_mutes import _get_mutes
 from .mute_actor import _mute_actor
+from .mute_actor_list import _mute_actor_list
 from .unmute_actor import _unmute_actor
+from .unmute_actor_list import _unmute_actor_list
 import typing
 
 class Graph_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
     def __init__(self, service: str, headers: dict[str, str]) -> None:
         self.service = service
         self.headers = headers
 
+    def unmute_actor_list(self, list: str) -> bytes:
+        """Unmute a list of actors."""
+        return _unmute_actor_list(self.service, self.headers, list)
+
+    def mute_actor_list(self, list: str) -> bytes:
+        """Mute a list of actors."""
+        return _mute_actor_list(self.service, self.headers, list)
+
+    def get_lists(self, actor: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
+        """Fetch a list of lists that belong to an actor"""
+        return _get_lists(self.service, self.headers, actor, limit, cursor)
+
     def get_followers(self, actor: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """Who is following an actor?"""
         return _get_followers(self.service, self.headers, actor, limit, cursor)
 
     def mute_actor(self, actor: str) -> bytes:
         """Mute an actor by did or handle."""
         return _mute_actor(self.service, self.headers, actor)
 
     def get_mutes(self, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """Who does the viewer mute?"""
         return _get_mutes(self.service, self.headers, limit, cursor)
 
+    def get_list_mutes(self, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
+        """Which lists is the requester's account muting?"""
+        return _get_list_mutes(self.service, self.headers, limit, cursor)
+
     def get_follows(self, actor: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """Who is an actor following?"""
         return _get_follows(self.service, self.headers, actor, limit, cursor)
 
     def get_blocks(self, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """Who is the requester's account blocking?"""
         return _get_blocks(self.service, self.headers, limit, cursor)
 
     def unmute_actor(self, actor: str) -> bytes:
         """Unmute an actor by did or handle."""
-        return _unmute_actor(self.service, self.headers, actor)
+        return _unmute_actor(self.service, self.headers, actor)
+
+    def get_list(self, list: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
+        """Fetch a list of actors"""
+        return _get_list(self.service, self.headers, list, limit, cursor)
```

### Comparing `chitose-0.0.4/chitose/app/bsky/notification/__init__.py` & `chitose-0.0.5/chitose/app/bsky/notification/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 from .get_unread_count import _get_unread_count
 from .list_notifications import _list_notifications
 from .update_seen import _update_seen
-import chitose
+import chitose.app.bsky.actor.defs
+import chitose.com.atproto.label.defs
 import typing
 
 class Notification_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
     def __init__(self, service: str, headers: dict[str, str]) -> None:
         self.service = service
```

### Comparing `chitose-0.0.4/chitose/app/bsky/notification/list_notifications.py` & `chitose-0.0.5/chitose/app/bsky/notification/list_notifications.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 class Notification(chitose.Object):
     """
 
 
     :param reason: Expected values are 'like', 'repost', 'follow', 'mention', 'reply', and 'quote'.
     """
 
-    def __init__(self, uri: str, cid: str, author: chitose.app.bsky.actor.defs.ProfileView, reason: str, record: typing.Any, is_read: str, indexed_at: str, reason_subject: typing.Optional[str]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None) -> None:
+    def __init__(self, uri: str, cid: str, author: chitose.app.bsky.actor.defs.ProfileView, reason: typing.Literal['like', 'repost', 'follow', 'mention', 'reply', 'quote'], record: typing.Any, is_read: str, indexed_at: str, reason_subject: typing.Optional[str]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None) -> None:
         self.uri = uri
         self.cid = cid
         self.author = author
         self.reason = reason
         self.record = record
         self.is_read = is_read
         self.indexed_at = indexed_at
```

### Comparing `chitose-0.0.4/chitose/app/bsky/richtext/facet.py` & `chitose-0.0.5/chitose/app/bsky/richtext/facet.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/app/bsky/unspecced/__init__.py` & `chitose-0.0.5/chitose/app/bsky/unspecced/__init__.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/__init__.py` & `chitose-0.0.5/chitose/com/atproto/__init__.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/admin/__init__.py` & `chitose-0.0.5/chitose/com/atproto/server/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,85 +1,94 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
-from .disable_invite_codes import _disable_invite_codes
-from .get_invite_codes import _get_invite_codes
-from .get_moderation_action import _get_moderation_action
-from .get_moderation_actions import _get_moderation_actions
-from .get_moderation_report import _get_moderation_report
-from .get_moderation_reports import _get_moderation_reports
-from .get_record import _get_record
-from .get_repo import _get_repo
-from .resolve_moderation_reports import _resolve_moderation_reports
-from .reverse_moderation_action import _reverse_moderation_action
-from .search_repos import _search_repos
-from .take_moderation_action import _take_moderation_action
-from .update_account_email import _update_account_email
-from .update_account_handle import _update_account_handle
-import chitose
+from .create_account import _create_account
+from .create_app_password import _create_app_password
+from .create_invite_code import _create_invite_code
+from .create_invite_codes import _create_invite_codes
+from .create_session import _create_session
+from .delete_account import _delete_account
+from .delete_session import _delete_session
+from .describe_server import _describe_server
+from .get_account_invite_codes import _get_account_invite_codes
+from .get_session import _get_session
+from .list_app_passwords import _list_app_passwords
+from .refresh_session import _refresh_session
+from .request_account_delete import _request_account_delete
+from .request_password_reset import _request_password_reset
+from .reset_password import _reset_password
+from .revoke_app_password import _revoke_app_password
 import typing
 
-class Admin_:
+class Server_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
     def __init__(self, service: str, headers: dict[str, str]) -> None:
         self.service = service
         self.headers = headers
 
-    def get_repo(self, did: str) -> bytes:
-        """View details about a repository."""
-        return _get_repo(self.service, self.headers, did)
+    def get_account_invite_codes(self, include_used: typing.Optional[str]=None, create_available: typing.Optional[str]=None) -> bytes:
+        """Get all invite codes for a given account"""
+        return _get_account_invite_codes(self.service, self.headers, include_used, create_available)
 
-    def get_moderation_reports(self, subject: typing.Optional[str]=None, resolved: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
-        """List moderation reports related to a subject."""
-        return _get_moderation_reports(self.service, self.headers, subject, resolved, limit, cursor)
+    def create_session(self, identifier: str, password: str) -> bytes:
+        """Create an authentication session.
 
-    def take_moderation_action(self, action: str, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reason: str, created_by: str, subject_blob_cids: typing.Optional[list[str]]=None, create_label_vals: typing.Optional[list[str]]=None, negate_label_vals: typing.Optional[list[str]]=None) -> bytes:
-        """Take a moderation action on a repo."""
-        return _take_moderation_action(self.service, self.headers, action, subject, reason, created_by, subject_blob_cids, create_label_vals, negate_label_vals)
 
-    def update_account_email(self, account: str, email: str) -> bytes:
-        """Administrative action to update an account's email
-
-
-        :param account: The handle or DID of the repo.
+        :param identifier: Handle or other identifier supported by the server for the authenticating user.
         """
-        return _update_account_email(self.service, self.headers, account, email)
+        return _create_session(self.service, self.headers, identifier, password)
 
-    def get_moderation_action(self, id: int) -> bytes:
-        """View details about a moderation action."""
-        return _get_moderation_action(self.service, self.headers, id)
-
-    def update_account_handle(self, did: str, handle: str) -> bytes:
-        """Administrative action to update an account's handle"""
-        return _update_account_handle(self.service, self.headers, did, handle)
-
-    def get_invite_codes(self, sort: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
-        """Admin view of invite codes"""
-        return _get_invite_codes(self.service, self.headers, sort, limit, cursor)
-
-    def get_moderation_report(self, id: int) -> bytes:
-        """View details about a moderation report."""
-        return _get_moderation_report(self.service, self.headers, id)
-
-    def disable_invite_codes(self, codes: typing.Optional[list[str]]=None, accounts: typing.Optional[list[str]]=None) -> bytes:
-        """Disable some set of codes and/or all codes associated with a set of users"""
-        return _disable_invite_codes(self.service, self.headers, codes, accounts)
-
-    def reverse_moderation_action(self, id: int, reason: str, created_by: str) -> bytes:
-        """Reverse a moderation action."""
-        return _reverse_moderation_action(self.service, self.headers, id, reason, created_by)
-
-    def get_record(self, uri: str, cid: typing.Optional[str]=None) -> bytes:
-        """View details about a record."""
-        return _get_record(self.service, self.headers, uri, cid)
-
-    def resolve_moderation_reports(self, action_id: int, report_ids: list[int], created_by: str) -> bytes:
-        """Resolve moderation reports by an action."""
-        return _resolve_moderation_reports(self.service, self.headers, action_id, report_ids, created_by)
-
-    def search_repos(self, term: typing.Optional[str]=None, invited_by: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
-        """Find repositories based on a search term."""
-        return _search_repos(self.service, self.headers, term, invited_by, limit, cursor)
-
-    def get_moderation_actions(self, subject: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
-        """List moderation actions related to a subject."""
-        return _get_moderation_actions(self.service, self.headers, subject, limit, cursor)
+    def list_app_passwords(self) -> bytes:
+        """List all app-specific passwords."""
+        return _list_app_passwords(self.service, self.headers)
+
+    def create_invite_codes(self, code_count: int, use_count: int, for_accounts: typing.Optional[list[str]]=None) -> bytes:
+        """Create an invite code."""
+        return _create_invite_codes(self.service, self.headers, code_count, use_count, for_accounts)
+
+    def delete_session(self) -> bytes:
+        """Delete the current session."""
+        return _delete_session(self.service, self.headers)
+
+    def revoke_app_password(self, name: str) -> bytes:
+        """Revoke an app-specific password by name."""
+        return _revoke_app_password(self.service, self.headers, name)
+
+    def create_app_password(self, name: str) -> bytes:
+        """Create an app-specific password."""
+        return _create_app_password(self.service, self.headers, name)
+
+    def describe_server(self) -> bytes:
+        """Get a document describing the service's accounts configuration."""
+        return _describe_server(self.service, self.headers)
+
+    def get_session(self) -> bytes:
+        """Get information about the current session."""
+        return _get_session(self.service, self.headers)
+
+    def refresh_session(self) -> bytes:
+        """Refresh an authentication session."""
+        return _refresh_session(self.service, self.headers)
+
+    def reset_password(self, token: str, password: str) -> bytes:
+        """Reset a user account password using a token."""
+        return _reset_password(self.service, self.headers, token, password)
+
+    def request_password_reset(self, email: str) -> bytes:
+        """Initiate a user account password reset via email."""
+        return _request_password_reset(self.service, self.headers, email)
+
+    def request_account_delete(self) -> bytes:
+        """Initiate a user account deletion via email."""
+        return _request_account_delete(self.service, self.headers)
+
+    def create_account(self, email: str, handle: str, password: str, did: typing.Optional[str]=None, invite_code: typing.Optional[str]=None, recovery_key: typing.Optional[str]=None) -> bytes:
+        """Create an account."""
+        return _create_account(self.service, self.headers, email, handle, password, did, invite_code, recovery_key)
+
+    def delete_account(self, did: str, password: str, token: str) -> bytes:
+        """Delete a user account with a token and password."""
+        return _delete_account(self.service, self.headers, did, password, token)
+
+    def create_invite_code(self, use_count: int, for_account: typing.Optional[str]=None) -> bytes:
+        """Create an invite code."""
+        return _create_invite_code(self.service, self.headers, use_count, for_account)
```

### Comparing `chitose-0.0.4/chitose/com/atproto/admin/defs.py` & `chitose-0.0.5/chitose/com/atproto/admin/defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from __future__ import annotations
 import chitose
 import chitose.com.atproto.admin.defs
 import chitose.com.atproto.label.defs
 import chitose.com.atproto.moderation.defs
 import chitose.com.atproto.repo.strong_ref
 import chitose.com.atproto.server.defs
-import enum
 import typing
 
 class ActionView(chitose.Object):
     """"""
 
     def __init__(self, id: int, action: chitose.com.atproto.admin.defs.ActionType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], subject_blob_cids: list[str], reason: str, created_by: str, created_at: str, resolved_report_ids: list[int], create_label_vals: typing.Optional[list[str]]=None, negate_label_vals: typing.Optional[list[str]]=None, reversal: typing.Optional[chitose.com.atproto.admin.defs.ActionReversal]=None) -> None:
         self.id = id
@@ -64,20 +63,15 @@
     def __init__(self, reason: str, created_by: str, created_at: str) -> None:
         self.reason = reason
         self.created_by = created_by
         self.created_at = created_at
 
     def to_dict(self) -> dict:
         return {'reason': self.reason, 'createdBy': self.created_by, 'createdAt': self.created_at, '$type': 'com.atproto.admin.defs#actionReversal'}
-
-class ActionType(enum.Enum):
-    TAKEDOWN = '#takedown'
-    FLAG = '#flag'
-    ACKNOWLEDGE = '#acknowledge'
-    ESCALATE = '#escalate'
+ActionType = typing.Literal['#takedown', '#flag', '#acknowledge', '#escalate']
 TAKEDOWN = 'com.atproto.admin.defs#takedown'
 FLAG = 'com.atproto.admin.defs#flag'
 ACKNOWLEDGE = 'com.atproto.admin.defs#acknowledge'
 ESCALATE = 'com.atproto.admin.defs#escalate'
 
 class ReportView(chitose.Object):
     """"""
@@ -108,42 +102,44 @@
 
     def to_dict(self) -> dict:
         return {'id': self.id, 'reasonType': self.reason_type, 'subject': self.subject, 'reportedBy': self.reported_by, 'createdAt': self.created_at, 'resolvedByActions': self.resolved_by_actions, 'reason': self.reason, '$type': 'com.atproto.admin.defs#reportViewDetail'}
 
 class RepoView(chitose.Object):
     """"""
 
-    def __init__(self, did: str, handle: str, related_records: list[typing.Any], indexed_at: str, moderation: chitose.com.atproto.admin.defs.Moderation, email: typing.Optional[str]=None, invited_by: typing.Optional[chitose.com.atproto.server.defs.InviteCode]=None) -> None:
+    def __init__(self, did: str, handle: str, related_records: list[typing.Any], indexed_at: str, moderation: chitose.com.atproto.admin.defs.Moderation, email: typing.Optional[str]=None, invited_by: typing.Optional[chitose.com.atproto.server.defs.InviteCode]=None, invites_disabled: typing.Optional[str]=None) -> None:
         self.did = did
         self.handle = handle
         self.related_records = related_records
         self.indexed_at = indexed_at
         self.moderation = moderation
         self.email = email
         self.invited_by = invited_by
+        self.invites_disabled = invites_disabled
 
     def to_dict(self) -> dict:
-        return {'did': self.did, 'handle': self.handle, 'relatedRecords': self.related_records, 'indexedAt': self.indexed_at, 'moderation': self.moderation, 'email': self.email, 'invitedBy': self.invited_by, '$type': 'com.atproto.admin.defs#repoView'}
+        return {'did': self.did, 'handle': self.handle, 'relatedRecords': self.related_records, 'indexedAt': self.indexed_at, 'moderation': self.moderation, 'email': self.email, 'invitedBy': self.invited_by, 'invitesDisabled': self.invites_disabled, '$type': 'com.atproto.admin.defs#repoView'}
 
 class RepoViewDetail(chitose.Object):
     """"""
 
-    def __init__(self, did: str, handle: str, related_records: list[typing.Any], indexed_at: str, moderation: chitose.com.atproto.admin.defs.ModerationDetail, email: typing.Optional[str]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None, invited_by: typing.Optional[chitose.com.atproto.server.defs.InviteCode]=None, invites: typing.Optional[list[chitose.com.atproto.server.defs.InviteCode]]=None) -> None:
+    def __init__(self, did: str, handle: str, related_records: list[typing.Any], indexed_at: str, moderation: chitose.com.atproto.admin.defs.ModerationDetail, email: typing.Optional[str]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None, invited_by: typing.Optional[chitose.com.atproto.server.defs.InviteCode]=None, invites: typing.Optional[list[chitose.com.atproto.server.defs.InviteCode]]=None, invites_disabled: typing.Optional[str]=None) -> None:
         self.did = did
         self.handle = handle
         self.related_records = related_records
         self.indexed_at = indexed_at
         self.moderation = moderation
         self.email = email
         self.labels = labels
         self.invited_by = invited_by
         self.invites = invites
+        self.invites_disabled = invites_disabled
 
     def to_dict(self) -> dict:
-        return {'did': self.did, 'handle': self.handle, 'relatedRecords': self.related_records, 'indexedAt': self.indexed_at, 'moderation': self.moderation, 'email': self.email, 'labels': self.labels, 'invitedBy': self.invited_by, 'invites': self.invites, '$type': 'com.atproto.admin.defs#repoViewDetail'}
+        return {'did': self.did, 'handle': self.handle, 'relatedRecords': self.related_records, 'indexedAt': self.indexed_at, 'moderation': self.moderation, 'email': self.email, 'labels': self.labels, 'invitedBy': self.invited_by, 'invites': self.invites, 'invitesDisabled': self.invites_disabled, '$type': 'com.atproto.admin.defs#repoViewDetail'}
 
 class RepoRef(chitose.Object):
     """"""
 
     def __init__(self, did: str) -> None:
         self.did = did
```

### Comparing `chitose-0.0.4/chitose/com/atproto/admin/disable_invite_codes.py` & `chitose-0.0.5/chitose/com/atproto/admin/disable_invite_codes.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/admin/get_moderation_reports.py` & `chitose-0.0.5/chitose/com/atproto/admin/get_moderation_reports.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _get_moderation_reports(service: str, headers: dict[str, str], subject: typing.Optional[str]=None, resolved: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
+def _get_moderation_reports(service: str, headers: dict[str, str], subject: typing.Optional[str]=None, resolved: typing.Optional[str]=None, action_type: typing.Optional[typing.Literal['com.atproto.admin.defs#takedown', 'com.atproto.admin.defs#flag', 'com.atproto.admin.defs#acknowledge', 'com.atproto.admin.defs#escalate']]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
     """List moderation reports related to a subject."""
-    return chitose.xrpc.call('com.atproto.admin.getModerationReports', [('subject', subject), ('resolved', resolved), ('limit', limit), ('cursor', cursor)], None, service, {} | headers)
+    return chitose.xrpc.call('com.atproto.admin.getModerationReports', [('subject', subject), ('resolved', resolved), ('actionType', action_type), ('limit', limit), ('cursor', cursor)], None, service, {} | headers)
```

### Comparing `chitose-0.0.4/chitose/com/atproto/admin/search_repos.py` & `chitose-0.0.5/chitose/com/atproto/admin/search_repos.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/admin/take_moderation_action.py` & `chitose-0.0.5/chitose/com/atproto/admin/take_moderation_action.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,10 +2,10 @@
 """"""
 from __future__ import annotations
 import chitose
 import chitose.com.atproto.admin.defs
 import chitose.com.atproto.repo.strong_ref
 import typing
 
-def _take_moderation_action(service: str, headers: dict[str, str], action: str, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reason: str, created_by: str, subject_blob_cids: typing.Optional[list[str]]=None, create_label_vals: typing.Optional[list[str]]=None, negate_label_vals: typing.Optional[list[str]]=None) -> bytes:
+def _take_moderation_action(service: str, headers: dict[str, str], action: typing.Literal['com.atproto.admin.defs#takedown', 'com.atproto.admin.defs#flag', 'com.atproto.admin.defs#acknowledge'], subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reason: str, created_by: str, subject_blob_cids: typing.Optional[list[str]]=None, create_label_vals: typing.Optional[list[str]]=None, negate_label_vals: typing.Optional[list[str]]=None) -> bytes:
     """Take a moderation action on a repo."""
     return chitose.xrpc.call('com.atproto.admin.takeModerationAction', [], {'action': action, 'subject': subject, 'subjectBlobCids': subject_blob_cids, 'createLabelVals': create_label_vals, 'negateLabelVals': negate_label_vals, 'reason': reason, 'createdBy': created_by}, service, {'Content-Type': 'application/json'} | headers)
```

### Comparing `chitose-0.0.4/chitose/com/atproto/identity/__init__.py` & `chitose-0.0.5/chitose/com/atproto/identity/__init__.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/label/__init__.py` & `chitose-0.0.5/chitose/com/atproto/label/__init__.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/label/defs.py` & `chitose-0.0.5/chitose/com/atproto/label/defs.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/label/query_labels.py` & `chitose-0.0.5/chitose/com/atproto/label/query_labels.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/label/subscribe_labels.py` & `chitose-0.0.5/chitose/com/atproto/label/subscribe_labels.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,13 +14,13 @@
 
     def to_dict(self) -> dict:
         return {'seq': self.seq, 'labels': self.labels, '$type': 'com.atproto.label.subscribeLabels#labels'}
 
 class Info(chitose.Object):
     """"""
 
-    def __init__(self, name: str, message: typing.Optional[str]=None) -> None:
+    def __init__(self, name: typing.Literal['OutdatedCursor',], message: typing.Optional[str]=None) -> None:
         self.name = name
         self.message = message
 
     def to_dict(self) -> dict:
         return {'name': self.name, 'message': self.message, '$type': 'com.atproto.label.subscribeLabels#info'}
```

### Comparing `chitose-0.0.4/chitose/com/atproto/moderation/__init__.py` & `chitose-0.0.5/chitose/com/atproto/moderation/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 from .create_report import _create_report
-import chitose
+import chitose.com.atproto.admin.defs
+import chitose.com.atproto.moderation.defs
+import chitose.com.atproto.repo.strong_ref
 import typing
 
 class Moderation_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
     def __init__(self, service: str, headers: dict[str, str]) -> None:
         self.service = service
```

### Comparing `chitose-0.0.4/chitose/com/atproto/moderation/create_report.py` & `chitose-0.0.5/chitose/com/atproto/moderation/create_report.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/moderation/defs.py` & `chitose-0.0.5/chitose/com/atproto/moderation/defs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,11 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
-import enum
-
-class ReasonType(enum.Enum):
-    REASON_SPAM = 'com.atproto.moderation.defs#reasonSpam'
-    REASON_VIOLATION = 'com.atproto.moderation.defs#reasonViolation'
-    REASON_MISLEADING = 'com.atproto.moderation.defs#reasonMisleading'
-    REASON_SEXUAL = 'com.atproto.moderation.defs#reasonSexual'
-    REASON_RUDE = 'com.atproto.moderation.defs#reasonRude'
-    REASON_OTHER = 'com.atproto.moderation.defs#reasonOther'
+import typing
+ReasonType = typing.Literal['com.atproto.moderation.defs#reasonSpam', 'com.atproto.moderation.defs#reasonViolation', 'com.atproto.moderation.defs#reasonMisleading', 'com.atproto.moderation.defs#reasonSexual', 'com.atproto.moderation.defs#reasonRude', 'com.atproto.moderation.defs#reasonOther']
 REASON_SPAM = 'com.atproto.moderation.defs#reasonSpam'
 REASON_VIOLATION = 'com.atproto.moderation.defs#reasonViolation'
 REASON_MISLEADING = 'com.atproto.moderation.defs#reasonMisleading'
 REASON_SEXUAL = 'com.atproto.moderation.defs#reasonSexual'
 REASON_RUDE = 'com.atproto.moderation.defs#reasonRude'
 REASON_OTHER = 'com.atproto.moderation.defs#reasonOther'
```

### Comparing `chitose-0.0.4/chitose/com/atproto/repo/__init__.py` & `chitose-0.0.5/chitose/com/atproto/repo/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from .apply_writes import _apply_writes
 from .create_record import _create_record
 from .delete_record import _delete_record
 from .describe_repo import _describe_repo
 from .get_record import _get_record
 from .list_records import _list_records
 from .put_record import _put_record
+from .rebase_repo import _rebase_repo
 from .upload_blob import _upload_blob
-import chitose
+import chitose.com.atproto.repo.apply_writes
 import typing
 
 class Repo_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
     def __init__(self, service: str, headers: dict[str, str]) -> None:
         self.service = service
@@ -68,14 +69,24 @@
 
         :param swap_record: Compare and swap with the previous record by cid.
 
         :param swap_commit: Compare and swap with the previous commit by cid.
         """
         return _put_record(self.service, self.headers, repo, collection, rkey, record, validate, swap_record, swap_commit)
 
+    def rebase_repo(self, repo: str, swap_commit: typing.Optional[str]=None) -> bytes:
+        """Simple rebase of repo that deletes history
+
+
+        :param repo: The handle or DID of the repo.
+
+        :param swap_commit: Compare and swap with the previous commit by cid.
+        """
+        return _rebase_repo(self.service, self.headers, repo, swap_commit)
+
     def upload_blob(self, input_: bytes) -> bytes:
         """Upload a new blob to be added to repo in a later request."""
         return _upload_blob(self.service, self.headers, input_)
 
     def describe_repo(self, repo: str) -> bytes:
         """Get information about the repo, including the list of collections.
```

### Comparing `chitose-0.0.4/chitose/com/atproto/repo/apply_writes.py` & `chitose-0.0.5/chitose/com/atproto/repo/apply_writes.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/repo/create_record.py` & `chitose-0.0.5/chitose/com/atproto/repo/create_record.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/repo/delete_record.py` & `chitose-0.0.5/chitose/com/atproto/repo/delete_record.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/repo/get_record.py` & `chitose-0.0.5/chitose/com/atproto/repo/get_record.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/repo/list_records.py` & `chitose-0.0.5/chitose/com/atproto/repo/list_records.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/repo/put_record.py` & `chitose-0.0.5/chitose/com/atproto/repo/put_record.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/server/create_account.py` & `chitose-0.0.5/chitose/com/atproto/server/create_account.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _create_account(service: str, headers: dict[str, str], email: str, handle: str, password: str, invite_code: typing.Optional[str]=None, recovery_key: typing.Optional[str]=None) -> bytes:
+def _create_account(service: str, headers: dict[str, str], email: str, handle: str, password: str, did: typing.Optional[str]=None, invite_code: typing.Optional[str]=None, recovery_key: typing.Optional[str]=None) -> bytes:
     """Create an account."""
-    return chitose.xrpc.call('com.atproto.server.createAccount', [], {'email': email, 'handle': handle, 'inviteCode': invite_code, 'password': password, 'recoveryKey': recovery_key}, service, {'Content-Type': 'application/json'} | headers)
+    return chitose.xrpc.call('com.atproto.server.createAccount', [], {'email': email, 'handle': handle, 'did': did, 'inviteCode': invite_code, 'password': password, 'recoveryKey': recovery_key}, service, {'Content-Type': 'application/json'} | headers)
```

### Comparing `chitose-0.0.4/chitose/com/atproto/server/create_app_password.py` & `chitose-0.0.5/chitose/com/atproto/server/create_app_password.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/server/create_invite_codes.py` & `chitose-0.0.5/chitose/com/atproto/server/create_invite_codes.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/server/create_session.py` & `chitose-0.0.5/chitose/com/atproto/server/create_session.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/server/defs.py` & `chitose-0.0.5/chitose/com/atproto/server/defs.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/server/describe_server.py` & `chitose-0.0.5/chitose/com/atproto/server/describe_server.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/server/list_app_passwords.py` & `chitose-0.0.5/chitose/com/atproto/server/list_app_passwords.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/sync/__init__.py` & `chitose-0.0.5/chitose/com/atproto/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/sync/get_commit_path.py` & `chitose-0.0.5/chitose/com/atproto/sync/get_commit_path.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/sync/get_record.py` & `chitose-0.0.5/chitose/com/atproto/sync/get_record.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/sync/get_repo.py` & `chitose-0.0.5/chitose/com/atproto/sync/get_repo.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/sync/list_blobs.py` & `chitose-0.0.5/chitose/com/atproto/sync/list_blobs.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/sync/list_repos.py` & `chitose-0.0.5/chitose/com/atproto/sync/list_repos.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/sync/notify_of_update.py` & `chitose-0.0.5/chitose/com/atproto/sync/notify_of_update.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/chitose/com/atproto/sync/subscribe_repos.py` & `chitose-0.0.5/chitose/com/atproto/sync/subscribe_repos.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,24 +61,24 @@
 
     def to_dict(self) -> dict:
         return {'seq': self.seq, 'did': self.did, 'time': self.time, '$type': 'com.atproto.sync.subscribeRepos#tombstone'}
 
 class Info(chitose.Object):
     """"""
 
-    def __init__(self, name: str, message: typing.Optional[str]=None) -> None:
+    def __init__(self, name: typing.Literal['OutdatedCursor',], message: typing.Optional[str]=None) -> None:
         self.name = name
         self.message = message
 
     def to_dict(self) -> dict:
         return {'name': self.name, 'message': self.message, '$type': 'com.atproto.sync.subscribeRepos#info'}
 
 class RepoOp(chitose.Object):
     """"""
 
-    def __init__(self, action: str, path: str, cid: typing.Any) -> None:
+    def __init__(self, action: typing.Literal['create', 'update', 'delete'], path: str, cid: typing.Any) -> None:
         self.action = action
         self.path = path
         self.cid = cid
 
     def to_dict(self) -> dict:
         return {'action': self.action, 'path': self.path, 'cid': self.cid, '$type': 'com.atproto.sync.subscribeRepos#repoOp'}
```

### Comparing `chitose-0.0.4/docs/Makefile` & `chitose-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/docs/make.bat` & `chitose-0.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/docs/source/chitose.app.bsky.actor.rst` & `chitose-0.0.5/docs/source/chitose.app.bsky.actor.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/docs/source/chitose.app.bsky.embed.rst` & `chitose-0.0.5/docs/source/chitose.app.bsky.embed.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/docs/source/chitose.app.bsky.feed.rst` & `chitose-0.0.5/docs/source/chitose.app.bsky.feed.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/docs/source/chitose.app.bsky.graph.rst` & `chitose-0.0.5/docs/source/chitose.app.bsky.graph.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/docs/source/chitose.app.bsky.notification.rst` & `chitose-0.0.5/docs/source/chitose.app.bsky.notification.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/docs/source/chitose.com.atproto.admin.rst` & `chitose-0.0.5/docs/source/chitose.com.atproto.admin.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/docs/source/chitose.com.atproto.identity.rst` & `chitose-0.0.5/docs/source/chitose.com.atproto.identity.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/docs/source/chitose.com.atproto.label.rst` & `chitose-0.0.5/docs/source/chitose.com.atproto.label.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/docs/source/chitose.com.atproto.moderation.rst` & `chitose-0.0.5/docs/source/chitose.com.atproto.moderation.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/docs/source/chitose.com.atproto.repo.rst` & `chitose-0.0.5/docs/source/chitose.com.atproto.repo.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/docs/source/chitose.com.atproto.server.rst` & `chitose-0.0.5/docs/source/chitose.com.atproto.server.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/docs/source/chitose.com.atproto.sync.rst` & `chitose-0.0.5/docs/source/chitose.com.atproto.sync.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/docs/source/chitose.rst` & `chitose-0.0.5/docs/source/chitose.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/docs/source/conf.py` & `chitose-0.0.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/docs/source/index.rst` & `chitose-0.0.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/examples/post.py` & `chitose-0.0.5/examples/post.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from datetime import datetime
+from datetime import timezone
+
 from chitose import BskyAgent
 from chitose.app.bsky.feed.post import Post
 
 
 # Replace YOUR_USERNAME, YOUR_PASSWORD AND YOUR_DID
 def main():
     agent = BskyAgent(service='https://bsky.social')
     agent.login(identifier='YOUR_USERNAME', password='YOUR_PASSWORD')
 
-    record = Post(text='Hello, world!', created_at=datetime.now().isoformat())
+    record = Post(text='Hello, world!',
+                  created_at=datetime.now(timezone.utc).isoformat())
     agent.com.atproto.repo.create_record(
         repo='YOUR_DID', collection='app.bsky.feed.post', record=record)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `chitose-0.0.4/examples/post_with_image.py` & `chitose-0.0.5/examples/post_with_image.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from datetime import datetime
+from datetime import timezone
 import json
 
 from chitose import BskyAgent
 from chitose import Blob
 from chitose import Link
 from chitose.app.bsky.feed.post import Post
 from chitose.app.bsky.embed.images import Image
@@ -22,14 +23,14 @@
     blob = Blob(ref=ref, mime_type=d['mimeType'], size=d['size'])
 
     image = Image(image=blob, alt='example')
 
     images = Images(images=[image])
 
     record = Post(text='post with an image test',
-                  created_at=datetime.now().isoformat(), embed=images)
+                  created_at=datetime.now(timezone.utc).isoformat(), embed=images)
     agent.com.atproto.repo.create_record(
         repo='YOUR_DID', collection='app.bsky.feed.post', record=record)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `chitose-0.0.4/.gitignore` & `chitose-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/LICENSE` & `chitose-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chitose-0.0.4/README.md` & `chitose-0.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -30,21 +30,23 @@
 >>> agent.login(identifier='YOUR_USERNAME', password='YOUR_PASSWORD')
 >>> agent.app.bsky.feed.get_timeline(limit=1)
 ```
 
 You can also post with `com.atproto.repo.create_record()`:
 ```python
 from datetime import datetime
+from datetime import timezone
 from chitose import BskyAgent
 from chitose.app.bsky.feed.post import Post
 
 agent = BskyAgent(service='https://example.com')
 agent.login(identifier='alice@mail.com', password='hunter2')
 
-record = Post(text='Hello, world!', created_at=datetime.now().isoformat())
+record = Post(text='Hello, world!',
+              created_at=datetime.now(timezone.utc).isoformat())
 agent.com.atproto.repo.create_record(
     repo=alice.did, collection='app.bsky.feed.post', record=record)
 ```
 
 See also the [`examples`](https://github.com/mnogu/chitose/tree/main/examples) directory for sample code.
 
 ## Documentation
@@ -67,15 +69,15 @@
 $ python3 -m pip install dist/chitose-*-py3-none-any.whl
 ```
 
 ## Generating Code
 
 Most source files of Chitose are generated from the Lexicon files in the `atproto` directory, and you can generate Python code from these files by yourself:
 ```
-$ git clone https://github.com/mnogu/chitose.git
+$ git clone --recursive https://github.com/mnogu/chitose.git
 $ cd chitose
 $ python3 generate.py
 ```
 
 You can also update the `atproto` directory and regenerate Python code:
 ```
 $ git submodule update --remote atproto
```

### Comparing `chitose-0.0.4/pyproject.toml` & `chitose-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "chitose"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Muneyuki Noguchi", email="nogu.dev@gmail.com" },
 ]
 description = "A client library for the AT Protocol (Bluesky) "
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `chitose-0.0.4/PKG-INFO` & `chitose-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chitose
-Version: 0.0.4
+Version: 0.0.5
 Summary: A client library for the AT Protocol (Bluesky) 
 Project-URL: Homepage, https://github.com/mnogu/chitose
 Project-URL: Bug Tracker, https://github.com/mnogu/chitose/issues
 Author-email: Muneyuki Noguchi <nogu.dev@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -46,21 +46,23 @@
 >>> agent.login(identifier='YOUR_USERNAME', password='YOUR_PASSWORD')
 >>> agent.app.bsky.feed.get_timeline(limit=1)
 ```
 
 You can also post with `com.atproto.repo.create_record()`:
 ```python
 from datetime import datetime
+from datetime import timezone
 from chitose import BskyAgent
 from chitose.app.bsky.feed.post import Post
 
 agent = BskyAgent(service='https://example.com')
 agent.login(identifier='alice@mail.com', password='hunter2')
 
-record = Post(text='Hello, world!', created_at=datetime.now().isoformat())
+record = Post(text='Hello, world!',
+              created_at=datetime.now(timezone.utc).isoformat())
 agent.com.atproto.repo.create_record(
     repo=alice.did, collection='app.bsky.feed.post', record=record)
 ```
 
 See also the [`examples`](https://github.com/mnogu/chitose/tree/main/examples) directory for sample code.
 
 ## Documentation
@@ -83,15 +85,15 @@
 $ python3 -m pip install dist/chitose-*-py3-none-any.whl
 ```
 
 ## Generating Code
 
 Most source files of Chitose are generated from the Lexicon files in the `atproto` directory, and you can generate Python code from these files by yourself:
 ```
-$ git clone https://github.com/mnogu/chitose.git
+$ git clone --recursive https://github.com/mnogu/chitose.git
 $ cd chitose
 $ python3 generate.py
 ```
 
 You can also update the `atproto` directory and regenerate Python code:
 ```
 $ git submodule update --remote atproto
```

