## aui-perf nightly record

_2 points · 2026-11-21T12:51:12.315Z to 2026-11-22T12:46:47.011Z · latest runner: Intel(R) Xeon(R) 6975P-C · Node v26.13.0_

| bench | latest | Δ7d | Δ30d | min | max | points |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 chunks from one source stream | 562.66µs |  |  | 562.66µs | 574.89µs | 2 |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 controller.enqueue calls | 822.27µs |  |  | 822.27µs | 845.04µs | 2 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 16 deltas × 250 chars | 34.47µs |  |  | 34.47µs | 34.65µs | 2 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 250 deltas × 16 chars | 361.97µs |  |  | 361.97µs | 371.59µs | 2 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 4000 deltas × 1 char (per-token) | 5.637ms |  |  | 5.637ms | 5.760ms | 2 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 100 deltas | 154.08µs |  |  | 154.08µs | 155.17µs | 2 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 1000 deltas | 1.401ms |  |  | 1.401ms | 1.414ms | 2 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 4000 deltas | 5.626ms |  |  | 5.626ms | 5.688ms | 2 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 100 deltas | 6.53µs |  |  | 6.53µs | 6.61µs | 2 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 1000 deltas | 54.52µs |  |  | 54.52µs | 56.16µs | 2 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 4000 deltas | 216.62µs |  |  | 216.62µs | 224.16µs | 2 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 128 parts, distinct providers (stress) | 59.68µs |  |  | 55.48µs | 59.68µs | 2 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 16 parts, one repeated provider | 30.54µs |  |  | 30.54µs | 32.24µs | 2 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 2 parts, one repeated provider | 32.19µs |  |  | 32.19µs | 32.34µs | 2 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 512 parts, distinct providers (stress) | 204.23µs |  |  | 198.42µs | 204.23µs | 2 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 10 static tools | 47.08µs |  |  | 46.55µs | 47.08µs | 2 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 100 static tools | 492.33µs |  |  | 479.64µs | 492.33µs | 2 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 10 static tools | 6.33µs |  |  | 6.33µs | 6.35µs | 2 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 100 static tools | 53.75µs |  |  | 53.75µs | 55.24µs | 2 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 100 deltas | 438.13µs |  |  | 438.13µs | 446.97µs | 2 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 1000 deltas | 3.682ms |  |  | 3.682ms | 3.762ms | 2 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 4000 deltas | 14.390ms |  |  | 14.390ms | 14.667ms | 2 |
| data-stream › assistant-stream: data stream decode + accumulate, one tool-call start per part › 100 parts | 2.734ms |  |  | 2.504ms | 2.734ms | 2 |
| data-stream › assistant-stream: data stream decode + accumulate, one tool-call start per part › 2000 parts | 66.274ms |  |  | 66.274ms | 67.085ms | 2 |
| data-stream › assistant-stream: data stream decode + accumulate, one tool-call start per part › 500 parts | 12.935ms |  |  | 12.617ms | 12.935ms | 2 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 100 deltas | 209.72µs |  |  | 209.03µs | 209.72µs | 2 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 1000 deltas | 2.018ms |  |  | 2.018ms | 2.046ms | 2 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 4000 deltas | 8.079ms |  |  | 8.079ms | 8.208ms | 2 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 1000 messages, 6-part replies | 218.97µs |  |  | 218.97µs | 221.82µs | 2 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 5000 messages, 20-part replies | 1.397ms |  |  | 1.397ms | 1.733ms | 2 |
| external-message-conversion › core: external message reasoning continuations › 100 matches | 43.58µs |  |  | 43.58µs | 44.42µs | 2 |
| external-message-conversion › core: external message reasoning continuations › 1000 matches | 436.74µs |  |  | 436.74µs | 444.65µs | 2 |
| external-message-conversion › core: external message reasoning continuations › 5000 matches | 2.340ms |  |  | 2.340ms | 2.394ms | 2 |
| external-message-conversion › core: external message tool results › 100 matches | 54.57µs |  |  | 54.53µs | 54.57µs | 2 |
| external-message-conversion › core: external message tool results › 1000 matches | 552.05µs |  |  | 552.05µs | 552.86µs | 2 |
| external-message-conversion › core: external message tool results › 5000 matches | 2.966ms |  |  | 2.943ms | 2.966ms | 2 |
| external-message-conversion › core: external message unique tool calls › 100 matches | 28.45µs |  |  | 28.45µs | 28.46µs | 2 |
| external-message-conversion › core: external message unique tool calls › 1000 matches | 271.93µs |  |  | 271.93µs | 274.33µs | 2 |
| external-message-conversion › core: external message unique tool calls › 5000 matches | 1.471ms |  |  | 1.471ms | 1.485ms | 2 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 1 text parts | 0.18µs |  |  | 0.18µs | 0.18µs | 2 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 10 text parts | 0.30µs |  |  | 0.30µs | 0.31µs | 2 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 100 text parts | 1.57µs |  |  | 1.57µs | 1.58µs | 2 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 1 tool calls | 0.40µs |  |  | 0.39µs | 0.40µs | 2 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 10 tool calls | 2.34µs |  |  | 2.34µs | 2.42µs | 2 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 100 tool calls | 20.47µs |  |  | 20.42µs | 20.47µs | 2 |
| interactable-array-patches › core: id-keyed interactable array patches › 1000 items and patches | 115.79µs |  |  | 112.90µs | 115.79µs | 2 |
| interactable-array-patches › core: id-keyed interactable array patches › 5000 items and patches | 660.63µs |  |  | 634.66µs | 660.63µs | 2 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tilde runs on one line | 1.989ms |  |  | 1.951ms | 1.989ms | 2 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tildes after prose | 118.59µs |  |  | 118.59µs | 118.76µs | 2 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 triple-backtick spans on one line | 2.573ms |  |  | 2.563ms | 2.573ms | 2 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 5,000 code spans in one paragraph | 353.94µs |  |  | 330.36µs | 353.94µs | 2 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, mixed message, 100 sections | 509.48µs |  |  | 509.48µs | 521.83µs | 2 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tilde runs on one line | 5.197ms |  |  | 5.197ms | 5.769ms | 2 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tildes after prose | 483.46µs |  |  | 480.79µs | 483.46µs | 2 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 triple-backtick spans on one line | 14.911ms |  |  | 14.911ms | 14.985ms | 2 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 5,000 code spans in one paragraph | 2.380ms |  |  | 2.380ms | 2.387ms | 2 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, mixed message, 100 sections | 1.801ms |  |  | 1.794ms | 1.801ms | 2 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown | 1.993ms |  |  | 1.979ms | 1.993ms | 2 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown deferred | 2.213ms |  |  | 2.213ms | 2.219ms | 2 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown | 13.479ms |  |  | 13.413ms | 13.479ms | 2 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown deferred | 14.831ms |  |  | 14.726ms | 14.831ms | 2 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 1 paragraphs | 1.127ms |  |  | 1.112ms | 1.127ms | 2 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 10 paragraphs | 1.943ms |  |  | 1.904ms | 1.943ms | 2 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 50 paragraphs | 6.700ms |  |  | 6.700ms | 6.724ms | 2 |
| markdown-streaming › react-markdown: the same token with defer on › 1 paragraphs deferred | 1.445ms |  |  | 1.435ms | 1.445ms | 2 |
| markdown-streaming › react-markdown: the same token with defer on › 10 paragraphs deferred | 1.405ms |  |  | 1.405ms | 1.408ms | 2 |
| markdown-streaming › react-markdown: the same token with defer on › 50 paragraphs deferred | 3.856ms |  |  | 3.852ms | 3.856ms | 2 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 1000 character argument in 16-character deltas | 209.50µs |  |  | 209.50µs | 210.45µs | 2 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 10000 character argument in 16-character deltas | 1.739ms |  |  | 1.677ms | 1.739ms | 2 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 500 short object entries in 16-character deltas | 183.912ms |  |  | 182.549ms | 183.912ms | 2 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 50000 character argument in 16-character deltas | 8.421ms |  |  | 8.390ms | 8.421ms | 2 |
| react-pi-message-projection › react-pi: streaming tail projection › 10 stable messages | 1.29µs |  |  | 1.24µs | 1.29µs | 2 |
| react-pi-message-projection › react-pi: streaming tail projection › 1000 stable messages | 5.57µs |  |  | 5.36µs | 5.57µs | 2 |
| react-pi-message-projection › react-pi: streaming tail projection › 5000 stable messages | 26.70µs |  |  | 25.67µs | 26.70µs | 2 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 1 chunks | 4.71µs |  |  | 4.71µs | 4.74µs | 2 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 101 chunks | 15.72µs |  |  | 15.50µs | 15.72µs | 2 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1 chunks | 45.79µs |  |  | 45.79µs | 46.05µs | 2 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1025 chunks | 189.72µs |  |  | 189.72µs | 195.20µs | 2 |
| thread-scaling › external-store thread: mount+unmount by message count › 10 messages | 4.522ms |  |  | 4.522ms | 4.551ms | 2 |
| thread-scaling › external-store thread: mount+unmount by message count › 100 messages | 27.716ms |  |  | 27.716ms | 28.118ms | 2 |
| thread-scaling › external-store thread: mount+unmount by message count › 1000 messages | 329.350ms |  |  | 329.350ms | 344.257ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 10 messages | 354.12µs |  |  | 354.12µs | 369.38µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 100 messages | 633.87µs |  |  | 633.87µs | 663.52µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 1000 messages | 3.053ms |  |  | 2.877ms | 3.053ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 10 messages | 363.37µs |  |  | 363.37µs | 370.38µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 100 messages | 1.187ms |  |  | 1.129ms | 1.187ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 1000 messages | 9.698ms |  |  | 8.622ms | 9.698ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 10 messages | 361.61µs |  |  | 354.28µs | 361.61µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 100 messages | 903.94µs |  |  | 839.14µs | 903.94µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 1000 messages | 5.889ms |  |  | 5.889ms | 6.762ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 10 messages | 150.05µs |  |  | 150.05µs | 151.64µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 100 messages | 345.49µs |  |  | 345.49µs | 370.06µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 1000 messages | 2.455ms |  |  | 2.455ms | 2.619ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 10 messages | 11.48µs |  |  | 11.28µs | 11.48µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 100 messages | 23.02µs |  |  | 23.02µs | 23.34µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 1000 messages | 196.45µs |  |  | 196.45µs | 210.07µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 10 messages | 420.23µs |  |  | 383.74µs | 420.23µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 100 messages | 869.89µs |  |  | 869.78µs | 869.89µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 1000 messages | 5.980ms |  |  | 5.634ms | 5.980ms | 2 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 1000 bytes | 162.82µs |  |  | 159.62µs | 162.82µs | 2 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 10000 bytes | 1.477ms |  |  | 1.455ms | 1.477ms | 2 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 5000 bytes | 745.47µs |  |  | 738.37µs | 745.47µs | 2 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 1000 bytes | 178.76µs |  |  | 178.76µs | 183.47µs | 2 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 10000 bytes | 1.562ms |  |  | 1.562ms | 1.620ms | 2 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 5000 bytes | 794.71µs |  |  | 794.71µs | 814.34µs | 2 |
| tool-args › assistant-stream: complete accumulated arguments (single delta) › 10,000 array elements | 248.39µs |  |  | 248.39µs | 249.48µs | 2 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 array entries | 17.226ms |  |  | 17.226ms | 17.502ms | 2 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 object entries | 669.307ms |  |  | 669.307ms | 674.679ms | 2 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 1000 bytes | 132.75µs |  |  | 132.17µs | 132.75µs | 2 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 10000 bytes | 1.104ms |  |  | 1.089ms | 1.104ms | 2 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 5000 bytes | 553.85µs |  |  | 553.29µs | 553.85µs | 2 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 10000 bytes | 153.99µs |  |  | 153.99µs | 155.80µs | 2 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 50000 bytes | 726.07µs |  |  | 726.07µs | 730.84µs | 2 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 10000 bytes | 167.29µs |  |  | 167.29µs | 171.21µs | 2 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 50000 bytes | 779.38µs |  |  | 779.38µs | 789.57µs | 2 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRoot | 2.297ms |  |  | 2.297ms | 2.303ms | 2 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootDeps | 2.332ms |  |  | 2.332ms | 2.372ms | 2 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootStable | 2.254ms |  |  | 2.254ms | 2.273ms | 2 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › react | 2.161ms |  |  | 2.160ms | 2.161ms | 2 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › tapRoot | 1.530ms |  |  | 1.456ms | 1.530ms | 2 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRoot | 2.125ms |  |  | 2.125ms | 2.252ms | 2 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootDeps | 2.123ms |  |  | 2.123ms | 2.238ms | 2 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootStable | 237.85µs |  |  | 230.19µs | 237.85µs | 2 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › react | 95.17µs |  |  | 94.78µs | 95.17µs | 2 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › tapRoot | 1.135ms |  |  | 1.135ms | 1.175ms | 2 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › deps | 1.269ms |  |  | 1.236ms | 1.269ms | 2 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › no-deps | 1.323ms |  |  | 1.299ms | 1.323ms | 2 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › deps | 31.04µs |  |  | 30.33µs | 31.04µs | 2 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › no-deps | 33.54µs |  |  | 33.26µs | 33.54µs | 2 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › deps | 55.34µs |  |  | 50.61µs | 55.34µs | 2 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › no-deps | 959.30µs |  |  | 959.30µs | 1.024ms | 2 |

informational; points come from different runners of the same class, so read trends, not single deltas.
