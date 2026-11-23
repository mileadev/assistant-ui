## aui-perf nightly record

_3 points · 2026-11-21T12:51:12.315Z to 2026-11-23T14:53:50.894Z · latest runner: AMD EPYC 7763 64-Core Processor · Node v26.13.0_

| bench | latest | Δ7d | Δ30d | min | max | points |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 chunks from one source stream | 864.09µs |  |  | 562.66µs | 864.09µs | 3 |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 controller.enqueue calls | 1.250ms |  |  | 822.27µs | 1.250ms | 3 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 16 deltas × 250 chars | 54.94µs |  |  | 34.47µs | 54.94µs | 3 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 250 deltas × 16 chars | 620.90µs |  |  | 361.97µs | 620.90µs | 3 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 4000 deltas × 1 char (per-token) | 9.844ms |  |  | 5.637ms | 9.844ms | 3 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 100 deltas | 270.45µs |  |  | 154.08µs | 270.45µs | 3 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 1000 deltas | 2.437ms |  |  | 1.401ms | 2.437ms | 3 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 4000 deltas | 9.492ms |  |  | 5.626ms | 9.492ms | 3 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 100 deltas | 9.72µs |  |  | 6.53µs | 9.72µs | 3 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 1000 deltas | 86.60µs |  |  | 54.52µs | 86.60µs | 3 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 4000 deltas | 345.36µs |  |  | 216.62µs | 345.36µs | 3 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 128 parts, distinct providers (stress) | 141.09µs |  |  | 55.48µs | 141.09µs | 3 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 16 parts, one repeated provider | 83.64µs |  |  | 30.54µs | 83.64µs | 3 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 2 parts, one repeated provider | 84.50µs |  |  | 32.19µs | 84.50µs | 3 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 512 parts, distinct providers (stress) | 325.10µs |  |  | 198.42µs | 325.10µs | 3 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 10 static tools | 73.88µs |  |  | 46.55µs | 73.88µs | 3 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 100 static tools | 682.18µs |  |  | 479.64µs | 682.18µs | 3 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 10 static tools | 10.06µs |  |  | 6.33µs | 10.06µs | 3 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 100 static tools | 84.85µs |  |  | 53.75µs | 84.85µs | 3 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 100 deltas | 779.38µs |  |  | 438.13µs | 779.38µs | 3 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 1000 deltas | 6.103ms |  |  | 3.682ms | 6.103ms | 3 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 4000 deltas | 23.734ms |  |  | 14.390ms | 23.734ms | 3 |
| data-stream › assistant-stream: data stream decode + accumulate, one tool-call start per part › 100 parts | 4.137ms |  |  | 2.504ms | 4.137ms | 3 |
| data-stream › assistant-stream: data stream decode + accumulate, one tool-call start per part › 2000 parts | 110.087ms |  |  | 66.274ms | 110.087ms | 3 |
| data-stream › assistant-stream: data stream decode + accumulate, one tool-call start per part › 500 parts | 19.358ms |  |  | 12.617ms | 19.358ms | 3 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 100 deltas | 355.47µs |  |  | 209.03µs | 355.47µs | 3 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 1000 deltas | 3.374ms |  |  | 2.018ms | 3.374ms | 3 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 4000 deltas | 13.348ms |  |  | 8.079ms | 13.348ms | 3 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 1000 messages, 6-part replies | 244.76µs |  |  | 218.97µs | 244.76µs | 3 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 5000 messages, 20-part replies | 2.023ms |  |  | 1.397ms | 2.023ms | 3 |
| external-message-conversion › core: external message reasoning continuations › 100 matches | 70.55µs |  |  | 43.58µs | 70.55µs | 3 |
| external-message-conversion › core: external message reasoning continuations › 1000 matches | 710.10µs |  |  | 436.74µs | 710.10µs | 3 |
| external-message-conversion › core: external message reasoning continuations › 5000 matches | 3.782ms |  |  | 2.340ms | 3.782ms | 3 |
| external-message-conversion › core: external message tool results › 100 matches | 82.75µs |  |  | 54.53µs | 82.75µs | 3 |
| external-message-conversion › core: external message tool results › 1000 matches | 812.56µs |  |  | 552.05µs | 812.56µs | 3 |
| external-message-conversion › core: external message tool results › 5000 matches | 4.248ms |  |  | 2.943ms | 4.248ms | 3 |
| external-message-conversion › core: external message unique tool calls › 100 matches | 41.97µs |  |  | 28.45µs | 41.97µs | 3 |
| external-message-conversion › core: external message unique tool calls › 1000 matches | 417.56µs |  |  | 271.93µs | 417.56µs | 3 |
| external-message-conversion › core: external message unique tool calls › 5000 matches | 2.186ms |  |  | 1.471ms | 2.186ms | 3 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 1 text parts | 0.29µs |  |  | 0.18µs | 0.29µs | 3 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 10 text parts | 0.47µs |  |  | 0.30µs | 0.47µs | 3 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 100 text parts | 2.45µs |  |  | 1.57µs | 2.45µs | 3 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 1 tool calls | 0.67µs |  |  | 0.39µs | 0.67µs | 3 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 10 tool calls | 3.58µs |  |  | 2.34µs | 3.58µs | 3 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 100 tool calls | 32.40µs |  |  | 20.42µs | 32.40µs | 3 |
| interactable-array-patches › core: id-keyed interactable array patches › 1000 items and patches | 142.89µs |  |  | 112.90µs | 142.89µs | 3 |
| interactable-array-patches › core: id-keyed interactable array patches › 5000 items and patches | 836.45µs |  |  | 634.66µs | 836.45µs | 3 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tilde runs on one line | 2.848ms |  |  | 1.951ms | 2.848ms | 3 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tildes after prose | 207.24µs |  |  | 118.59µs | 207.24µs | 3 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 triple-backtick spans on one line | 3.690ms |  |  | 2.563ms | 3.690ms | 3 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 5,000 code spans in one paragraph | 515.49µs |  |  | 330.36µs | 515.49µs | 3 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, mixed message, 100 sections | 726.14µs |  |  | 509.48µs | 726.14µs | 3 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tilde runs on one line | 7.207ms |  |  | 5.197ms | 7.207ms | 3 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tildes after prose | 923.44µs |  |  | 480.79µs | 923.44µs | 3 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 triple-backtick spans on one line | 24.337ms |  |  | 14.911ms | 24.337ms | 3 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 5,000 code spans in one paragraph | 3.810ms |  |  | 2.380ms | 3.810ms | 3 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, mixed message, 100 sections | 2.824ms |  |  | 1.794ms | 2.824ms | 3 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown | 3.184ms |  |  | 1.979ms | 3.184ms | 3 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown deferred | 3.476ms |  |  | 2.213ms | 3.476ms | 3 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown | 22.200ms |  |  | 13.413ms | 22.200ms | 3 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown deferred | 23.850ms |  |  | 14.726ms | 23.850ms | 3 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 1 paragraphs | 1.612ms |  |  | 1.112ms | 1.612ms | 3 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 10 paragraphs | 3.357ms |  |  | 1.904ms | 3.357ms | 3 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 50 paragraphs | 10.933ms |  |  | 6.700ms | 10.933ms | 3 |
| markdown-streaming › react-markdown: the same token with defer on › 1 paragraphs deferred | 1.192ms |  |  | 1.192ms | 1.445ms | 3 |
| markdown-streaming › react-markdown: the same token with defer on › 10 paragraphs deferred | 1.861ms |  |  | 1.405ms | 1.861ms | 3 |
| markdown-streaming › react-markdown: the same token with defer on › 50 paragraphs deferred | 4.992ms |  |  | 3.852ms | 4.992ms | 3 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 1000 character argument in 16-character deltas | 323.54µs |  |  | 209.50µs | 323.54µs | 3 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 10000 character argument in 16-character deltas | 2.548ms |  |  | 1.677ms | 2.548ms | 3 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 500 short object entries in 16-character deltas | 300.906ms |  |  | 182.549ms | 300.906ms | 3 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 50000 character argument in 16-character deltas | 12.252ms |  |  | 8.390ms | 12.252ms | 3 |
| react-pi-message-projection › react-pi: streaming tail projection › 10 stable messages | 2.34µs |  |  | 1.24µs | 2.34µs | 3 |
| react-pi-message-projection › react-pi: streaming tail projection › 1000 stable messages | 9.86µs |  |  | 5.36µs | 9.86µs | 3 |
| react-pi-message-projection › react-pi: streaming tail projection › 5000 stable messages | 43.67µs |  |  | 25.67µs | 43.67µs | 3 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 1 chunks | 6.43µs |  |  | 4.71µs | 6.43µs | 3 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 101 chunks | 21.08µs |  |  | 15.50µs | 21.08µs | 3 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1 chunks | 62.78µs |  |  | 45.79µs | 62.78µs | 3 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1025 chunks | 283.03µs |  |  | 189.72µs | 283.03µs | 3 |
| thread-scaling › external-store thread: mount+unmount by message count › 10 messages | 7.319ms |  |  | 4.522ms | 7.319ms | 3 |
| thread-scaling › external-store thread: mount+unmount by message count › 100 messages | 49.201ms |  |  | 27.716ms | 49.201ms | 3 |
| thread-scaling › external-store thread: mount+unmount by message count › 1000 messages | 491.960ms |  |  | 329.350ms | 491.960ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 10 messages | 644.98µs |  |  | 354.12µs | 644.98µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 100 messages | 928.31µs |  |  | 633.87µs | 928.31µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 1000 messages | 4.859ms |  |  | 2.877ms | 4.859ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 10 messages | 610.45µs |  |  | 363.37µs | 610.45µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 100 messages | 1.628ms |  |  | 1.129ms | 1.628ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 1000 messages | 18.151ms |  |  | 8.622ms | 18.151ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 10 messages | 608.03µs |  |  | 354.28µs | 608.03µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 100 messages | 1.168ms |  |  | 839.14µs | 1.168ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 1000 messages | 10.609ms |  |  | 5.889ms | 10.609ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 10 messages | 322.01µs |  |  | 150.05µs | 322.01µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 100 messages | 575.20µs |  |  | 345.49µs | 575.20µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 1000 messages | 4.094ms |  |  | 2.455ms | 4.094ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 10 messages | 26.66µs |  |  | 11.28µs | 26.66µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 100 messages | 43.45µs |  |  | 23.02µs | 43.45µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 1000 messages | 267.48µs |  |  | 196.45µs | 267.48µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 10 messages | 746.28µs |  |  | 383.74µs | 746.28µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 100 messages | 1.248ms |  |  | 869.78µs | 1.248ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 1000 messages | 11.557ms |  |  | 5.634ms | 11.557ms | 3 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 1000 bytes | 259.07µs |  |  | 159.62µs | 259.07µs | 3 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 10000 bytes | 2.208ms |  |  | 1.455ms | 2.208ms | 3 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 5000 bytes | 1.115ms |  |  | 738.37µs | 1.115ms | 3 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 1000 bytes | 321.72µs |  |  | 178.76µs | 321.72µs | 3 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 10000 bytes | 2.601ms |  |  | 1.562ms | 2.601ms | 3 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 5000 bytes | 1.322ms |  |  | 794.71µs | 1.322ms | 3 |
| tool-args › assistant-stream: complete accumulated arguments (single delta) › 10,000 array elements | 353.42µs |  |  | 248.39µs | 353.42µs | 3 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 array entries | 26.627ms |  |  | 17.226ms | 26.627ms | 3 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 object entries | 666.486ms |  |  | 666.486ms | 674.679ms | 3 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 1000 bytes | 241.42µs |  |  | 132.17µs | 241.42µs | 3 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 10000 bytes | 1.879ms |  |  | 1.089ms | 1.879ms | 3 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 5000 bytes | 962.81µs |  |  | 553.29µs | 962.81µs | 3 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 10000 bytes | 211.44µs |  |  | 153.99µs | 211.44µs | 3 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 50000 bytes | 949.94µs |  |  | 726.07µs | 949.94µs | 3 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 10000 bytes | 235.70µs |  |  | 167.29µs | 235.70µs | 3 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 50000 bytes | 1.030ms |  |  | 779.38µs | 1.030ms | 3 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRoot | 4.382ms |  |  | 2.297ms | 4.382ms | 3 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootDeps | 4.416ms |  |  | 2.332ms | 4.416ms | 3 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootStable | 4.322ms |  |  | 2.254ms | 4.322ms | 3 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › react | 3.763ms |  |  | 2.160ms | 3.763ms | 3 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › tapRoot | 3.503ms |  |  | 1.456ms | 3.503ms | 3 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRoot | 3.302ms |  |  | 2.125ms | 3.302ms | 3 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootDeps | 3.441ms |  |  | 2.123ms | 3.441ms | 3 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootStable | 358.85µs |  |  | 230.19µs | 358.85µs | 3 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › react | 147.23µs |  |  | 94.78µs | 147.23µs | 3 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › tapRoot | 1.750ms |  |  | 1.135ms | 1.750ms | 3 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › deps | 2.071ms |  |  | 1.236ms | 2.071ms | 3 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › no-deps | 2.141ms |  |  | 1.299ms | 2.141ms | 3 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › deps | 54.97µs |  |  | 30.33µs | 54.97µs | 3 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › no-deps | 54.13µs |  |  | 33.26µs | 54.13µs | 3 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › deps | 70.04µs |  |  | 50.61µs | 70.04µs | 3 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › no-deps | 1.558ms |  |  | 959.30µs | 1.558ms | 3 |

informational; points come from different runners of the same class, so read trends, not single deltas.
