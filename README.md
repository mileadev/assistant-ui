## aui-perf nightly record

_1 points · 2026-11-21T12:51:12.315Z to 2026-11-21T12:51:12.315Z · latest runner: Intel(R) Xeon(R) 6975P-C · Node v26.13.0_

| bench | latest | Δ7d | Δ30d | min | max | points |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 chunks from one source stream | 574.89µs |  |  | 574.89µs | 574.89µs | 1 |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 controller.enqueue calls | 845.04µs |  |  | 845.04µs | 845.04µs | 1 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 16 deltas × 250 chars | 34.65µs |  |  | 34.65µs | 34.65µs | 1 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 250 deltas × 16 chars | 371.59µs |  |  | 371.59µs | 371.59µs | 1 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 4000 deltas × 1 char (per-token) | 5.760ms |  |  | 5.760ms | 5.760ms | 1 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 100 deltas | 155.17µs |  |  | 155.17µs | 155.17µs | 1 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 1000 deltas | 1.414ms |  |  | 1.414ms | 1.414ms | 1 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 4000 deltas | 5.688ms |  |  | 5.688ms | 5.688ms | 1 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 100 deltas | 6.61µs |  |  | 6.61µs | 6.61µs | 1 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 1000 deltas | 56.16µs |  |  | 56.16µs | 56.16µs | 1 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 4000 deltas | 224.16µs |  |  | 224.16µs | 224.16µs | 1 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 128 parts, distinct providers (stress) | 55.48µs |  |  | 55.48µs | 55.48µs | 1 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 16 parts, one repeated provider | 32.24µs |  |  | 32.24µs | 32.24µs | 1 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 2 parts, one repeated provider | 32.34µs |  |  | 32.34µs | 32.34µs | 1 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 512 parts, distinct providers (stress) | 198.42µs |  |  | 198.42µs | 198.42µs | 1 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 10 static tools | 46.55µs |  |  | 46.55µs | 46.55µs | 1 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 100 static tools | 479.64µs |  |  | 479.64µs | 479.64µs | 1 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 10 static tools | 6.35µs |  |  | 6.35µs | 6.35µs | 1 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 100 static tools | 55.24µs |  |  | 55.24µs | 55.24µs | 1 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 100 deltas | 446.97µs |  |  | 446.97µs | 446.97µs | 1 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 1000 deltas | 3.762ms |  |  | 3.762ms | 3.762ms | 1 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 4000 deltas | 14.667ms |  |  | 14.667ms | 14.667ms | 1 |
| data-stream › assistant-stream: data stream decode + accumulate, one tool-call start per part › 100 parts | 2.504ms |  |  | 2.504ms | 2.504ms | 1 |
| data-stream › assistant-stream: data stream decode + accumulate, one tool-call start per part › 2000 parts | 67.085ms |  |  | 67.085ms | 67.085ms | 1 |
| data-stream › assistant-stream: data stream decode + accumulate, one tool-call start per part › 500 parts | 12.617ms |  |  | 12.617ms | 12.617ms | 1 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 100 deltas | 209.03µs |  |  | 209.03µs | 209.03µs | 1 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 1000 deltas | 2.046ms |  |  | 2.046ms | 2.046ms | 1 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 4000 deltas | 8.208ms |  |  | 8.208ms | 8.208ms | 1 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 1000 messages, 6-part replies | 221.82µs |  |  | 221.82µs | 221.82µs | 1 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 5000 messages, 20-part replies | 1.733ms |  |  | 1.733ms | 1.733ms | 1 |
| external-message-conversion › core: external message reasoning continuations › 100 matches | 44.42µs |  |  | 44.42µs | 44.42µs | 1 |
| external-message-conversion › core: external message reasoning continuations › 1000 matches | 444.65µs |  |  | 444.65µs | 444.65µs | 1 |
| external-message-conversion › core: external message reasoning continuations › 5000 matches | 2.394ms |  |  | 2.394ms | 2.394ms | 1 |
| external-message-conversion › core: external message tool results › 100 matches | 54.53µs |  |  | 54.53µs | 54.53µs | 1 |
| external-message-conversion › core: external message tool results › 1000 matches | 552.86µs |  |  | 552.86µs | 552.86µs | 1 |
| external-message-conversion › core: external message tool results › 5000 matches | 2.943ms |  |  | 2.943ms | 2.943ms | 1 |
| external-message-conversion › core: external message unique tool calls › 100 matches | 28.46µs |  |  | 28.46µs | 28.46µs | 1 |
| external-message-conversion › core: external message unique tool calls › 1000 matches | 274.33µs |  |  | 274.33µs | 274.33µs | 1 |
| external-message-conversion › core: external message unique tool calls › 5000 matches | 1.485ms |  |  | 1.485ms | 1.485ms | 1 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 1 text parts | 0.18µs |  |  | 0.18µs | 0.18µs | 1 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 10 text parts | 0.31µs |  |  | 0.31µs | 0.31µs | 1 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 100 text parts | 1.58µs |  |  | 1.58µs | 1.58µs | 1 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 1 tool calls | 0.39µs |  |  | 0.39µs | 0.39µs | 1 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 10 tool calls | 2.42µs |  |  | 2.42µs | 2.42µs | 1 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 100 tool calls | 20.42µs |  |  | 20.42µs | 20.42µs | 1 |
| interactable-array-patches › core: id-keyed interactable array patches › 1000 items and patches | 112.90µs |  |  | 112.90µs | 112.90µs | 1 |
| interactable-array-patches › core: id-keyed interactable array patches › 5000 items and patches | 634.66µs |  |  | 634.66µs | 634.66µs | 1 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tilde runs on one line | 1.951ms |  |  | 1.951ms | 1.951ms | 1 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tildes after prose | 118.76µs |  |  | 118.76µs | 118.76µs | 1 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 triple-backtick spans on one line | 2.563ms |  |  | 2.563ms | 2.563ms | 1 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 5,000 code spans in one paragraph | 330.36µs |  |  | 330.36µs | 330.36µs | 1 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, mixed message, 100 sections | 521.83µs |  |  | 521.83µs | 521.83µs | 1 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tilde runs on one line | 5.769ms |  |  | 5.769ms | 5.769ms | 1 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tildes after prose | 480.79µs |  |  | 480.79µs | 480.79µs | 1 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 triple-backtick spans on one line | 14.985ms |  |  | 14.985ms | 14.985ms | 1 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 5,000 code spans in one paragraph | 2.387ms |  |  | 2.387ms | 2.387ms | 1 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, mixed message, 100 sections | 1.794ms |  |  | 1.794ms | 1.794ms | 1 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown | 1.979ms |  |  | 1.979ms | 1.979ms | 1 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown deferred | 2.219ms |  |  | 2.219ms | 2.219ms | 1 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown | 13.413ms |  |  | 13.413ms | 13.413ms | 1 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown deferred | 14.726ms |  |  | 14.726ms | 14.726ms | 1 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 1 paragraphs | 1.112ms |  |  | 1.112ms | 1.112ms | 1 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 10 paragraphs | 1.904ms |  |  | 1.904ms | 1.904ms | 1 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 50 paragraphs | 6.724ms |  |  | 6.724ms | 6.724ms | 1 |
| markdown-streaming › react-markdown: the same token with defer on › 1 paragraphs deferred | 1.435ms |  |  | 1.435ms | 1.435ms | 1 |
| markdown-streaming › react-markdown: the same token with defer on › 10 paragraphs deferred | 1.408ms |  |  | 1.408ms | 1.408ms | 1 |
| markdown-streaming › react-markdown: the same token with defer on › 50 paragraphs deferred | 3.852ms |  |  | 3.852ms | 3.852ms | 1 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 1000 character argument in 16-character deltas | 210.45µs |  |  | 210.45µs | 210.45µs | 1 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 10000 character argument in 16-character deltas | 1.677ms |  |  | 1.677ms | 1.677ms | 1 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 500 short object entries in 16-character deltas | 182.549ms |  |  | 182.549ms | 182.549ms | 1 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 50000 character argument in 16-character deltas | 8.390ms |  |  | 8.390ms | 8.390ms | 1 |
| react-pi-message-projection › react-pi: streaming tail projection › 10 stable messages | 1.24µs |  |  | 1.24µs | 1.24µs | 1 |
| react-pi-message-projection › react-pi: streaming tail projection › 1000 stable messages | 5.36µs |  |  | 5.36µs | 5.36µs | 1 |
| react-pi-message-projection › react-pi: streaming tail projection › 5000 stable messages | 25.67µs |  |  | 25.67µs | 25.67µs | 1 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 1 chunks | 4.74µs |  |  | 4.74µs | 4.74µs | 1 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 101 chunks | 15.50µs |  |  | 15.50µs | 15.50µs | 1 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1 chunks | 46.05µs |  |  | 46.05µs | 46.05µs | 1 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1025 chunks | 195.20µs |  |  | 195.20µs | 195.20µs | 1 |
| thread-scaling › external-store thread: mount+unmount by message count › 10 messages | 4.551ms |  |  | 4.551ms | 4.551ms | 1 |
| thread-scaling › external-store thread: mount+unmount by message count › 100 messages | 28.118ms |  |  | 28.118ms | 28.118ms | 1 |
| thread-scaling › external-store thread: mount+unmount by message count › 1000 messages | 344.257ms |  |  | 344.257ms | 344.257ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 10 messages | 369.38µs |  |  | 369.38µs | 369.38µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 100 messages | 663.52µs |  |  | 663.52µs | 663.52µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 1000 messages | 2.877ms |  |  | 2.877ms | 2.877ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 10 messages | 370.38µs |  |  | 370.38µs | 370.38µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 100 messages | 1.129ms |  |  | 1.129ms | 1.129ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 1000 messages | 8.622ms |  |  | 8.622ms | 8.622ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 10 messages | 354.28µs |  |  | 354.28µs | 354.28µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 100 messages | 839.14µs |  |  | 839.14µs | 839.14µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 1000 messages | 6.762ms |  |  | 6.762ms | 6.762ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 10 messages | 151.64µs |  |  | 151.64µs | 151.64µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 100 messages | 370.06µs |  |  | 370.06µs | 370.06µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 1000 messages | 2.619ms |  |  | 2.619ms | 2.619ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 10 messages | 11.28µs |  |  | 11.28µs | 11.28µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 100 messages | 23.34µs |  |  | 23.34µs | 23.34µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 1000 messages | 210.07µs |  |  | 210.07µs | 210.07µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 10 messages | 383.74µs |  |  | 383.74µs | 383.74µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 100 messages | 869.78µs |  |  | 869.78µs | 869.78µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 1000 messages | 5.634ms |  |  | 5.634ms | 5.634ms | 1 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 1000 bytes | 159.62µs |  |  | 159.62µs | 159.62µs | 1 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 10000 bytes | 1.455ms |  |  | 1.455ms | 1.455ms | 1 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 5000 bytes | 738.37µs |  |  | 738.37µs | 738.37µs | 1 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 1000 bytes | 183.47µs |  |  | 183.47µs | 183.47µs | 1 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 10000 bytes | 1.620ms |  |  | 1.620ms | 1.620ms | 1 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 5000 bytes | 814.34µs |  |  | 814.34µs | 814.34µs | 1 |
| tool-args › assistant-stream: complete accumulated arguments (single delta) › 10,000 array elements | 249.48µs |  |  | 249.48µs | 249.48µs | 1 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 array entries | 17.502ms |  |  | 17.502ms | 17.502ms | 1 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 object entries | 674.679ms |  |  | 674.679ms | 674.679ms | 1 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 1000 bytes | 132.17µs |  |  | 132.17µs | 132.17µs | 1 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 10000 bytes | 1.089ms |  |  | 1.089ms | 1.089ms | 1 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 5000 bytes | 553.29µs |  |  | 553.29µs | 553.29µs | 1 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 10000 bytes | 155.80µs |  |  | 155.80µs | 155.80µs | 1 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 50000 bytes | 730.84µs |  |  | 730.84µs | 730.84µs | 1 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 10000 bytes | 171.21µs |  |  | 171.21µs | 171.21µs | 1 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 50000 bytes | 789.57µs |  |  | 789.57µs | 789.57µs | 1 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRoot | 2.303ms |  |  | 2.303ms | 2.303ms | 1 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootDeps | 2.372ms |  |  | 2.372ms | 2.372ms | 1 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootStable | 2.273ms |  |  | 2.273ms | 2.273ms | 1 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › react | 2.160ms |  |  | 2.160ms | 2.160ms | 1 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › tapRoot | 1.456ms |  |  | 1.456ms | 1.456ms | 1 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRoot | 2.252ms |  |  | 2.252ms | 2.252ms | 1 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootDeps | 2.238ms |  |  | 2.238ms | 2.238ms | 1 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootStable | 230.19µs |  |  | 230.19µs | 230.19µs | 1 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › react | 94.78µs |  |  | 94.78µs | 94.78µs | 1 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › tapRoot | 1.175ms |  |  | 1.175ms | 1.175ms | 1 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › deps | 1.236ms |  |  | 1.236ms | 1.236ms | 1 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › no-deps | 1.299ms |  |  | 1.299ms | 1.299ms | 1 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › deps | 30.33µs |  |  | 30.33µs | 30.33µs | 1 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › no-deps | 33.26µs |  |  | 33.26µs | 33.26µs | 1 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › deps | 50.61µs |  |  | 50.61µs | 50.61µs | 1 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › no-deps | 1.024ms |  |  | 1.024ms | 1.024ms | 1 |

informational; points come from different runners of the same class, so read trends, not single deltas.
