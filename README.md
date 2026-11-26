## aui-perf nightly record

_6 points · 2026-11-21T12:51:12.315Z to 2026-11-26T14:05:07.485Z · latest runner: Intel(R) Xeon(R) 6975P-C · Node v26.13.0_

| bench | latest | Δ7d | Δ30d | min | max | points |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 chunks from one source stream | 566.59µs |  |  | 560.48µs | 864.09µs | 6 |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 controller.enqueue calls | 847.67µs |  |  | 803.53µs | 1.250ms | 6 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 16 deltas × 250 chars | 34.93µs |  |  | 34.47µs | 54.94µs | 6 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 250 deltas × 16 chars | 367.31µs |  |  | 361.97µs | 620.90µs | 6 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 4000 deltas × 1 char (per-token) | 5.676ms |  |  | 5.637ms | 9.844ms | 6 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 100 deltas | 154.00µs |  |  | 154.00µs | 270.45µs | 6 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 1000 deltas | 1.396ms |  |  | 1.396ms | 2.437ms | 6 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 4000 deltas | 5.693ms |  |  | 5.626ms | 9.492ms | 6 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 100 deltas | 6.33µs |  |  | 6.33µs | 9.72µs | 6 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 1000 deltas | 53.73µs |  |  | 53.73µs | 86.60µs | 6 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 4000 deltas | 214.60µs |  |  | 214.60µs | 345.36µs | 6 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 128 parts, distinct providers (stress) | 59.72µs |  |  | 55.48µs | 141.09µs | 6 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 16 parts, one repeated provider | 31.15µs |  |  | 30.54µs | 83.64µs | 6 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 2 parts, one repeated provider | 32.51µs |  |  | 32.19µs | 84.50µs | 6 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 512 parts, distinct providers (stress) | 202.48µs |  |  | 198.42µs | 325.10µs | 6 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 10 static tools | 46.44µs |  |  | 46.44µs | 73.88µs | 6 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 100 static tools | 477.90µs |  |  | 477.90µs | 682.18µs | 6 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 10 static tools | 6.28µs |  |  | 6.28µs | 10.06µs | 6 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 100 static tools | 53.22µs |  |  | 53.22µs | 84.85µs | 6 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 100 deltas | 446.47µs |  |  | 438.13µs | 779.38µs | 6 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 1000 deltas | 3.757ms |  |  | 3.682ms | 6.103ms | 6 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 4000 deltas | 14.658ms |  |  | 14.390ms | 23.734ms | 6 |
| data-stream › assistant-stream: data stream decode + accumulate, one tool-call start per part › 100 parts | 2.874ms |  |  | 2.504ms | 4.137ms | 6 |
| data-stream › assistant-stream: data stream decode + accumulate, one tool-call start per part › 2000 parts | 67.460ms |  |  | 66.274ms | 110.087ms | 6 |
| data-stream › assistant-stream: data stream decode + accumulate, one tool-call start per part › 500 parts | 12.854ms |  |  | 12.617ms | 19.358ms | 6 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 100 deltas | 208.81µs |  |  | 208.81µs | 355.47µs | 6 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 1000 deltas | 2.033ms |  |  | 2.018ms | 3.374ms | 6 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 4000 deltas | 8.170ms |  |  | 8.079ms | 13.348ms | 6 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 1000 messages, 6-part replies | 183.33µs |  |  | 183.33µs | 244.76µs | 6 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 5000 messages, 20-part replies | 1.458ms |  |  | 1.397ms | 2.023ms | 6 |
| external-message-conversion › core: external message reasoning continuations › 100 matches | 42.96µs |  |  | 42.96µs | 70.55µs | 6 |
| external-message-conversion › core: external message reasoning continuations › 1000 matches | 429.71µs |  |  | 429.71µs | 710.10µs | 6 |
| external-message-conversion › core: external message reasoning continuations › 5000 matches | 2.299ms |  |  | 2.299ms | 3.782ms | 6 |
| external-message-conversion › core: external message tool results › 100 matches | 54.29µs |  |  | 54.25µs | 82.75µs | 6 |
| external-message-conversion › core: external message tool results › 1000 matches | 541.05µs |  |  | 541.05µs | 812.56µs | 6 |
| external-message-conversion › core: external message tool results › 5000 matches | 2.934ms |  |  | 2.934ms | 4.248ms | 6 |
| external-message-conversion › core: external message unique tool calls › 100 matches | 28.28µs |  |  | 27.98µs | 41.97µs | 6 |
| external-message-conversion › core: external message unique tool calls › 1000 matches | 268.55µs |  |  | 268.55µs | 417.56µs | 6 |
| external-message-conversion › core: external message unique tool calls › 5000 matches | 1.474ms |  |  | 1.471ms | 2.186ms | 6 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 1 text parts | 0.18µs |  |  | 0.18µs | 0.29µs | 6 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 10 text parts | 0.30µs |  |  | 0.30µs | 0.47µs | 6 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 100 text parts | 1.58µs |  |  | 1.57µs | 2.45µs | 6 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 1 tool calls | 0.38µs |  |  | 0.38µs | 0.67µs | 6 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 10 tool calls | 2.25µs |  |  | 2.25µs | 3.58µs | 6 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 100 tool calls | 20.08µs |  |  | 20.08µs | 32.40µs | 6 |
| interactable-array-patches › core: id-keyed interactable array patches › 1000 items and patches | 110.97µs |  |  | 110.97µs | 142.89µs | 6 |
| interactable-array-patches › core: id-keyed interactable array patches › 5000 items and patches | 635.71µs |  |  | 593.91µs | 836.45µs | 6 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tilde runs on one line | 1.979ms |  |  | 1.951ms | 2.848ms | 6 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tildes after prose | 119.19µs |  |  | 118.59µs | 207.24µs | 6 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 triple-backtick spans on one line | 2.542ms |  |  | 2.542ms | 3.690ms | 6 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 5,000 code spans in one paragraph | 344.86µs |  |  | 330.36µs | 515.49µs | 6 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, mixed message, 100 sections | 511.64µs |  |  | 506.12µs | 726.14µs | 6 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tilde runs on one line | 5.823ms |  |  | 5.197ms | 7.207ms | 6 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tildes after prose | 470.64µs |  |  | 470.64µs | 923.44µs | 6 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 triple-backtick spans on one line | 14.937ms |  |  | 14.911ms | 24.337ms | 6 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 5,000 code spans in one paragraph | 2.378ms |  |  | 2.367ms | 3.810ms | 6 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, mixed message, 100 sections | 1.820ms |  |  | 1.794ms | 2.824ms | 6 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown | 1.987ms |  |  | 1.979ms | 3.184ms | 6 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown deferred | 2.206ms |  |  | 2.206ms | 3.476ms | 6 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown | 13.487ms |  |  | 13.413ms | 22.200ms | 6 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown deferred | 14.774ms |  |  | 14.726ms | 23.850ms | 6 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 1 paragraphs | 1.133ms |  |  | 1.010ms | 1.612ms | 6 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 10 paragraphs | 1.969ms |  |  | 1.904ms | 3.357ms | 6 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 50 paragraphs | 6.580ms |  |  | 6.563ms | 10.933ms | 6 |
| markdown-streaming › react-markdown: the same token with defer on › 1 paragraphs deferred | 1.433ms |  |  | 1.192ms | 1.445ms | 6 |
| markdown-streaming › react-markdown: the same token with defer on › 10 paragraphs deferred | 1.430ms |  |  | 1.367ms | 1.861ms | 6 |
| markdown-streaming › react-markdown: the same token with defer on › 50 paragraphs deferred | 3.969ms |  |  | 3.802ms | 4.992ms | 6 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 1000 character argument in 16-character deltas | 215.10µs |  |  | 209.50µs | 323.54µs | 6 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 10000 character argument in 16-character deltas | 1.794ms |  |  | 1.677ms | 2.548ms | 6 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 500 short object entries in 16-character deltas | 183.473ms |  |  | 182.549ms | 300.906ms | 6 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 50000 character argument in 16-character deltas | 8.628ms |  |  | 8.390ms | 12.252ms | 6 |
| react-pi-message-projection › react-pi: streaming tail projection › 10 stable messages | 1.26µs |  |  | 1.24µs | 2.34µs | 6 |
| react-pi-message-projection › react-pi: streaming tail projection › 1000 stable messages | 5.31µs |  |  | 5.31µs | 9.86µs | 6 |
| react-pi-message-projection › react-pi: streaming tail projection › 5000 stable messages | 25.21µs |  |  | 25.21µs | 43.67µs | 6 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 1 chunks | 4.73µs |  |  | 4.71µs | 7.35µs | 6 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 101 chunks | 15.57µs |  |  | 15.47µs | 21.08µs | 6 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1 chunks | 46.08µs |  |  | 45.79µs | 72.54µs | 6 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1025 chunks | 199.06µs |  |  | 189.72µs | 283.03µs | 6 |
| thread-scaling › external-store thread: mount+unmount by message count › 10 messages | 4.496ms |  |  | 4.496ms | 7.319ms | 6 |
| thread-scaling › external-store thread: mount+unmount by message count › 100 messages | 26.382ms |  |  | 26.382ms | 49.201ms | 6 |
| thread-scaling › external-store thread: mount+unmount by message count › 1000 messages | 315.189ms |  |  | 315.189ms | 491.960ms | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 10 messages | 371.78µs |  |  | 343.35µs | 644.98µs | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 100 messages | 701.04µs |  |  | 633.87µs | 928.31µs | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 1000 messages | 3.130ms |  |  | 2.877ms | 4.859ms | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 10 messages | 383.91µs |  |  | 349.26µs | 610.45µs | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 100 messages | 1.232ms |  |  | 1.083ms | 1.628ms | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 1000 messages | 8.446ms |  |  | 8.446ms | 18.151ms | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 10 messages | 330.54µs |  |  | 330.54µs | 608.03µs | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 100 messages | 984.75µs |  |  | 821.30µs | 1.168ms | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 1000 messages | 5.817ms |  |  | 5.602ms | 10.609ms | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 10 messages | 154.82µs |  |  | 150.05µs | 322.01µs | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 100 messages | 398.72µs |  |  | 345.49µs | 575.20µs | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 1000 messages | 2.819ms |  |  | 2.455ms | 4.094ms | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 10 messages | 11.20µs |  |  | 11.20µs | 26.66µs | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 100 messages | 23.74µs |  |  | 23.02µs | 43.45µs | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 1000 messages | 201.35µs |  |  | 196.45µs | 267.48µs | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 10 messages | 393.95µs |  |  | 383.74µs | 746.28µs | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 100 messages | 849.42µs |  |  | 809.08µs | 1.248ms | 6 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 1000 messages | 5.639ms |  |  | 5.634ms | 11.557ms | 6 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 1000 bytes | 160.07µs |  |  | 159.62µs | 259.07µs | 6 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 10000 bytes | 1.467ms |  |  | 1.455ms | 2.208ms | 6 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 5000 bytes | 742.33µs |  |  | 738.37µs | 1.115ms | 6 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 1000 bytes | 178.14µs |  |  | 178.14µs | 321.72µs | 6 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 10000 bytes | 1.546ms |  |  | 1.546ms | 2.601ms | 6 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 5000 bytes | 795.11µs |  |  | 794.71µs | 1.322ms | 6 |
| tool-args › assistant-stream: complete accumulated arguments (single delta) › 10,000 array elements | 249.03µs |  |  | 245.94µs | 353.42µs | 6 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 array entries | 17.130ms |  |  | 17.130ms | 26.627ms | 6 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 object entries | 661.098ms |  |  | 469.467ms | 674.679ms | 6 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 1000 bytes | 131.54µs |  |  | 131.54µs | 241.42µs | 6 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 10000 bytes | 1.080ms |  |  | 1.080ms | 1.879ms | 6 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 5000 bytes | 546.27µs |  |  | 546.27µs | 962.81µs | 6 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 10000 bytes | 155.22µs |  |  | 153.99µs | 211.44µs | 6 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 50000 bytes | 734.22µs |  |  | 726.07µs | 949.94µs | 6 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 10000 bytes | 174.94µs |  |  | 167.29µs | 235.70µs | 6 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 50000 bytes | 770.84µs |  |  | 770.84µs | 1.030ms | 6 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRoot | 2.318ms |  |  | 2.297ms | 4.382ms | 6 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootDeps | 2.349ms |  |  | 2.332ms | 4.416ms | 6 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootStable | 2.259ms |  |  | 2.254ms | 4.322ms | 6 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › react | 2.182ms |  |  | 2.160ms | 3.763ms | 6 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › tapRoot | 1.462ms |  |  | 1.456ms | 3.503ms | 6 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRoot | 2.177ms |  |  | 2.125ms | 3.302ms | 6 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootDeps | 2.157ms |  |  | 2.123ms | 3.441ms | 6 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootStable | 171.43µs |  |  | 171.43µs | 358.85µs | 6 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › react | 95.58µs |  |  | 94.78µs | 147.23µs | 6 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › tapRoot | 1.124ms |  |  | 1.110ms | 1.750ms | 6 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › deps | 1.278ms |  |  | 1.236ms | 2.071ms | 6 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › no-deps | 1.346ms |  |  | 1.299ms | 2.141ms | 6 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › deps | 31.02µs |  |  | 30.33µs | 54.97µs | 6 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › no-deps | 33.11µs |  |  | 33.11µs | 54.13µs | 6 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › deps | 53.83µs |  |  | 50.61µs | 70.04µs | 6 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › no-deps | 1.047ms |  |  | 959.30µs | 1.558ms | 6 |

informational; points come from different runners of the same class, so read trends, not single deltas.
