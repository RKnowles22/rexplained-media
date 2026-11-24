# rexplained-media

Public, temporary hosting for Rex-plained (and other channel) videos, only so Metricool can fetch them.
The project itself lives in dcknowles04/Agent-Testing (`rexplained/`, see its CLAUDE.md "Publishing an episode").

Rules:
- Files here are public. Only put finished, ready-to-post videos and thumbnails here, under `epNN/`.
- GitHub rejects files over 100 MB: re-encode the episode first (two-pass x264, -tune animation, ~900k video for a
  12-minute episode keeps SSIM above 0.99).
- As soon as Metricool has accepted the posts (it copies media to static.metricool.com when a post is created),
  remove the files by resetting the repo to a single fresh commit with just README.md and this file, then
  force-push main. A plain delete commit would leave the videos in the public history.
