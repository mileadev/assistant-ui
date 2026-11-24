## aui-perf nightly record

_4 points · 2026-11-21T12:51:12.315Z to 2026-11-24T15:04:04.106Z · latest runner: AMD EPYC 9V74 80-Core Processor · Node v26.13.0_

| bench | latest | Δ7d | Δ30d | min | max | points |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 chunks from one source stream | 689.26µs |  |  | 562.66µs | 864.09µs | 4 |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 controller.enqueue calls | 1.028ms |  |  | 822.27µs | 1.250ms | 4 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 16 deltas × 250 chars | 43.47µs |  |  | 34.47µs | 54.94µs | 4 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 250 deltas × 16 chars | 507.92µs |  |  | 361.97µs | 620.90µs | 4 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 4000 deltas × 1 char (per-token) | 7.865ms |  |  | 5.637ms | 9.844ms | 4 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 100 deltas | 212.62µs |  |  | 154.08µs | 270.45µs | 4 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 1000 deltas | 2.007ms |  |  | 1.401ms | 2.437ms | 4 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 4000 deltas | 7.815ms |  |  | 5.626ms | 9.492ms | 4 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 100 deltas | 8.25µs |  |  | 6.53µs | 9.72µs | 4 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 1000 deltas | 69.05µs |  |  | 54.52µs | 86.60µs | 4 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 4000 deltas | 270.39µs |  |  | 216.62µs | 345.36µs | 4 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 128 parts, distinct providers (stress) | 83.24µs |  |  | 55.48µs | 141.09µs | 4 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 16 parts, one repeated provider | 44.36µs |  |  | 30.54µs | 83.64µs | 4 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 2 parts, one repeated provider | 42.15µs |  |  | 32.19µs | 84.50µs | 4 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 512 parts, distinct providers (stress) | 256.85µs |  |  | 198.42µs | 325.10µs | 4 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 10 static tools | 53.39µs |  |  | 46.55µs | 73.88µs | 4 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 100 static tools | 523.62µs |  |  | 479.64µs | 682.18µs | 4 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 10 static tools | 7.57µs |  |  | 6.33µs | 10.06µs | 4 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 100 static tools | 62.35µs |  |  | 53.75µs | 84.85µs | 4 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 100 deltas | 602.69µs |  |  | 438.13µs | 779.38µs | 4 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 1000 deltas | 5.065ms |  |  | 3.682ms | 6.103ms | 4 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 4000 deltas | 20.006ms |  |  | 14.390ms | 23.734ms | 4 |
| data-stream › assistant-stream: data stream decode + accumulate, one tool-call start per part › 100 parts | 2.970ms |  |  | 2.504ms | 4.137ms | 4 |
| data-stream › assistant-stream: data stream decode + accumulate, one tool-call start per part › 2000 parts | 90.390ms |  |  | 66.274ms | 110.087ms | 4 |
| data-stream › assistant-stream: data stream decode + accumulate, one tool-call start per part › 500 parts | 14.683ms |  |  | 12.617ms | 19.358ms | 4 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 100 deltas | 283.91µs |  |  | 209.03µs | 355.47µs | 4 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 1000 deltas | 2.769ms |  |  | 2.018ms | 3.374ms | 4 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 4000 deltas | 11.055ms |  |  | 8.079ms | 13.348ms | 4 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 1000 messages, 6-part replies | 196.34µs |  |  | 196.34µs | 244.76µs | 4 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 5000 messages, 20-part replies | 1.645ms |  |  | 1.397ms | 2.023ms | 4 |
| external-message-conversion › core: external message reasoning continuations › 100 matches | 50.19µs |  |  | 43.58µs | 70.55µs | 4 |
| external-message-conversion › core: external message reasoning continuations › 1000 matches | 507.14µs |  |  | 436.74µs | 710.10µs | 4 |
| external-message-conversion › core: external message reasoning continuations › 5000 matches | 2.699ms |  |  | 2.340ms | 3.782ms | 4 |
| external-message-conversion › core: external message tool results › 100 matches | 59.45µs |  |  | 54.53µs | 82.75µs | 4 |
| external-message-conversion › core: external message tool results › 1000 matches | 607.65µs |  |  | 552.05µs | 812.56µs | 4 |
| external-message-conversion › core: external message tool results › 5000 matches | 3.157ms |  |  | 2.943ms | 4.248ms | 4 |
| external-message-conversion › core: external message unique tool calls › 100 matches | 31.86µs |  |  | 28.45µs | 41.97µs | 4 |
| external-message-conversion › core: external message unique tool calls › 1000 matches | 303.81µs |  |  | 271.93µs | 417.56µs | 4 |
| external-message-conversion › core: external message unique tool calls › 5000 matches | 1.634ms |  |  | 1.471ms | 2.186ms | 4 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 1 text parts | 0.22µs |  |  | 0.18µs | 0.29µs | 4 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 10 text parts | 0.36µs |  |  | 0.30µs | 0.47µs | 4 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 100 text parts | 2.14µs |  |  | 1.57µs | 2.45µs | 4 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 1 tool calls | 0.48µs |  |  | 0.39µs | 0.67µs | 4 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 10 tool calls | 2.49µs |  |  | 2.34µs | 3.58µs | 4 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 100 tool calls | 23.27µs |  |  | 20.42µs | 32.40µs | 4 |
| interactable-array-patches › core: id-keyed interactable array patches › 1000 items and patches | 114.98µs |  |  | 112.90µs | 142.89µs | 4 |
| interactable-array-patches › core: id-keyed interactable array patches › 5000 items and patches | 593.91µs |  |  | 593.91µs | 836.45µs | 4 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tilde runs on one line | 2.115ms |  |  | 1.951ms | 2.848ms | 4 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tildes after prose | 161.27µs |  |  | 118.59µs | 207.24µs | 4 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 triple-backtick spans on one line | 2.744ms |  |  | 2.563ms | 3.690ms | 4 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 5,000 code spans in one paragraph | 391.27µs |  |  | 330.36µs | 515.49µs | 4 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, mixed message, 100 sections | 506.12µs |  |  | 506.12µs | 726.14µs | 4 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tilde runs on one line | 6.113ms |  |  | 5.197ms | 7.207ms | 4 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tildes after prose | 759.78µs |  |  | 480.79µs | 923.44µs | 4 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 triple-backtick spans on one line | 16.302ms |  |  | 14.911ms | 24.337ms | 4 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 5,000 code spans in one paragraph | 2.728ms |  |  | 2.380ms | 3.810ms | 4 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, mixed message, 100 sections | 1.940ms |  |  | 1.794ms | 2.824ms | 4 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown | 2.359ms |  |  | 1.979ms | 3.184ms | 4 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown deferred | 2.488ms |  |  | 2.213ms | 3.476ms | 4 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown | 16.713ms |  |  | 13.413ms | 22.200ms | 4 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown deferred | 18.376ms |  |  | 14.726ms | 23.850ms | 4 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 1 paragraphs | 1.010ms |  |  | 1.010ms | 1.612ms | 4 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 10 paragraphs | 2.155ms |  |  | 1.904ms | 3.357ms | 4 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 50 paragraphs | 7.531ms |  |  | 6.700ms | 10.933ms | 4 |
| markdown-streaming › react-markdown: the same token with defer on › 1 paragraphs deferred | 1.442ms |  |  | 1.192ms | 1.445ms | 4 |
| markdown-streaming › react-markdown: the same token with defer on › 10 paragraphs deferred | 1.367ms |  |  | 1.367ms | 1.861ms | 4 |
| markdown-streaming › react-markdown: the same token with defer on › 50 paragraphs deferred | 4.264ms |  |  | 3.852ms | 4.992ms | 4 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 1000 character argument in 16-character deltas | 257.48µs |  |  | 209.50µs | 323.54µs | 4 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 10000 character argument in 16-character deltas | 2.142ms |  |  | 1.677ms | 2.548ms | 4 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 500 short object entries in 16-character deltas | 217.839ms |  |  | 182.549ms | 300.906ms | 4 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 50000 character argument in 16-character deltas | 10.590ms |  |  | 8.390ms | 12.252ms | 4 |
| react-pi-message-projection › react-pi: streaming tail projection › 10 stable messages | 1.84µs |  |  | 1.24µs | 2.34µs | 4 |
| react-pi-message-projection › react-pi: streaming tail projection › 1000 stable messages | 9.32µs |  |  | 5.36µs | 9.86µs | 4 |
| react-pi-message-projection › react-pi: streaming tail projection › 5000 stable messages | 36.63µs |  |  | 25.67µs | 43.67µs | 4 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 1 chunks | 7.35µs |  |  | 4.71µs | 7.35µs | 4 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 101 chunks | 19.95µs |  |  | 15.50µs | 21.08µs | 4 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1 chunks | 72.54µs |  |  | 45.79µs | 72.54µs | 4 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1025 chunks | 244.93µs |  |  | 189.72µs | 283.03µs | 4 |
| thread-scaling › external-store thread: mount+unmount by message count › 10 messages | 4.734ms |  |  | 4.522ms | 7.319ms | 4 |
| thread-scaling › external-store thread: mount+unmount by message count › 100 messages | 30.856ms |  |  | 27.716ms | 49.201ms | 4 |
| thread-scaling › external-store thread: mount+unmount by message count › 1000 messages | 388.032ms |  |  | 329.350ms | 491.960ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 10 messages | 522.72µs |  |  | 354.12µs | 644.98µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 100 messages | 743.44µs |  |  | 633.87µs | 928.31µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 1000 messages | 3.290ms |  |  | 2.877ms | 4.859ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 10 messages | 542.95µs |  |  | 363.37µs | 610.45µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 100 messages | 1.083ms |  |  | 1.083ms | 1.628ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 1000 messages | 10.603ms |  |  | 8.622ms | 18.151ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 10 messages | 477.46µs |  |  | 354.28µs | 608.03µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 100 messages | 821.30µs |  |  | 821.30µs | 1.168ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 1000 messages | 6.297ms |  |  | 5.889ms | 10.609ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 10 messages | 268.32µs |  |  | 150.05µs | 322.01µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 100 messages | 414.41µs |  |  | 345.49µs | 575.20µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 1000 messages | 2.903ms |  |  | 2.455ms | 4.094ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 10 messages | 13.70µs |  |  | 11.28µs | 26.66µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 100 messages | 28.57µs |  |  | 23.02µs | 43.45µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 1000 messages | 212.44µs |  |  | 196.45µs | 267.48µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 10 messages | 442.00µs |  |  | 383.74µs | 746.28µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 100 messages | 809.08µs |  |  | 809.08µs | 1.248ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 1000 messages | 6.667ms |  |  | 5.634ms | 11.557ms | 4 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 1000 bytes | 197.53µs |  |  | 159.62µs | 259.07µs | 4 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 10000 bytes | 1.779ms |  |  | 1.455ms | 2.208ms | 4 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 5000 bytes | 878.87µs |  |  | 738.37µs | 1.115ms | 4 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 1000 bytes | 239.95µs |  |  | 178.76µs | 321.72µs | 4 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 10000 bytes | 2.131ms |  |  | 1.562ms | 2.601ms | 4 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 5000 bytes | 1.074ms |  |  | 794.71µs | 1.322ms | 4 |
| tool-args › assistant-stream: complete accumulated arguments (single delta) › 10,000 array elements | 267.37µs |  |  | 248.39µs | 353.42µs | 4 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 array entries | 20.957ms |  |  | 17.226ms | 26.627ms | 4 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 object entries | 469.467ms |  |  | 469.467ms | 674.679ms | 4 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 1000 bytes | 187.74µs |  |  | 132.17µs | 241.42µs | 4 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 10000 bytes | 1.560ms |  |  | 1.089ms | 1.879ms | 4 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 5000 bytes | 795.63µs |  |  | 553.29µs | 962.81µs | 4 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 10000 bytes | 164.75µs |  |  | 153.99µs | 211.44µs | 4 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 50000 bytes | 746.17µs |  |  | 726.07µs | 949.94µs | 4 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 10000 bytes | 179.76µs |  |  | 167.29µs | 235.70µs | 4 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 50000 bytes | 789.26µs |  |  | 779.38µs | 1.030ms | 4 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRoot | 2.671ms |  |  | 2.297ms | 4.382ms | 4 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootDeps | 2.719ms |  |  | 2.332ms | 4.416ms | 4 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootStable | 2.641ms |  |  | 2.254ms | 4.322ms | 4 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › react | 2.651ms |  |  | 2.160ms | 3.763ms | 4 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › tapRoot | 1.761ms |  |  | 1.456ms | 3.503ms | 4 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRoot | 2.598ms |  |  | 2.125ms | 3.302ms | 4 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootDeps | 2.588ms |  |  | 2.123ms | 3.441ms | 4 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootStable | 199.83µs |  |  | 199.83µs | 358.85µs | 4 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › react | 107.66µs |  |  | 94.78µs | 147.23µs | 4 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › tapRoot | 1.364ms |  |  | 1.135ms | 1.750ms | 4 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › deps | 1.440ms |  |  | 1.236ms | 2.071ms | 4 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › no-deps | 1.507ms |  |  | 1.299ms | 2.141ms | 4 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › deps | 38.25µs |  |  | 30.33µs | 54.97µs | 4 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › no-deps | 39.89µs |  |  | 33.26µs | 54.13µs | 4 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › deps | 53.43µs |  |  | 50.61µs | 70.04µs | 4 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › no-deps | 1.141ms |  |  | 959.30µs | 1.558ms | 4 |

informational; points come from different runners of the same class, so read trends, not single deltas.
