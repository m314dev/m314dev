<img width="720" height="720" alt="m314dev-avatar" src="https://github.com/user-attachments/assets/99181816-0c5a-4bc2-8efa-086fa042a377" />


m314 is open-source multimedia engineering: tools and libraries that work at the level of streaming formats, encryption, live packaging and audio signal analysis. Everything is MIT licensed.

m314dl is a streaming media engine for HLS, DASH and Smooth Streaming. It decrypts all four Common Encryption schemes (cenc, cbcs, cens and cbc1) with keys you supply, natively and one fragment at a time in memory, with output identical to the reference tools. It also extracts WebVTT, TTML and fMP4 wvtt/stpp subtitles. VOD and live share one pipeline, whose concurrency adjusts itself to the network and which resumes byte for byte after a hard kill. It can record a live channel and repackage it on the fly as HLS, MPEG-TS or DASH, and its worker mode runs many channels in one process under a controller.

m314ss decides whether a subtitle belongs to a video by listening to the audio. It detects speech onsets, searches thousands of timing offsets and frame-rate ratios, and accepts a match only when the best offset stands out clearly from the rest. The same search gives the sync correction, including 23.976, 24 and 25 fps drift.

subapi is one Go interface to SubDL and OpenSubtitles.

Docs, benchmarks and releases are at m314.dev
