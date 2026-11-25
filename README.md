## aui-perf nightly record

_5 points · 2026-11-21T12:51:12.315Z to 2026-11-25T14:36:42.656Z · latest runner: Intel(R) Xeon(R) 6975P-C · Node v26.13.0_

| bench | latest | Δ7d | Δ30d | min | max | points |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 chunks from one source stream | 560.48µs |  |  | 560.48µs | 864.09µs | 5 |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 controller.enqueue calls | 803.53µs |  |  | 803.53µs | 1.250ms | 5 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 16 deltas × 250 chars | 34.98µs |  |  | 34.47µs | 54.94µs | 5 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 250 deltas × 16 chars | 372.36µs |  |  | 361.97µs | 620.90µs | 5 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 4000 deltas × 1 char (per-token) | 5.804ms |  |  | 5.637ms | 9.844ms | 5 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 100 deltas | 156.88µs |  |  | 154.08µs | 270.45µs | 5 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 1000 deltas | 1.422ms |  |  | 1.401ms | 2.437ms | 5 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 4000 deltas | 5.711ms |  |  | 5.626ms | 9.492ms | 5 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 100 deltas | 6.61µs |  |  | 6.53µs | 9.72µs | 5 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 1000 deltas | 55.70µs |  |  | 54.52µs | 86.60µs | 5 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 4000 deltas | 223.02µs |  |  | 216.62µs | 345.36µs | 5 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 128 parts, distinct providers (stress) | 56.56µs |  |  | 55.48µs | 141.09µs | 5 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 16 parts, one repeated provider | 32.56µs |  |  | 30.54µs | 83.64µs | 5 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 2 parts, one repeated provider | 32.57µs |  |  | 32.19µs | 84.50µs | 5 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 512 parts, distinct providers (stress) | 202.16µs |  |  | 198.42µs | 325.10µs | 5 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 10 static tools | 47.71µs |  |  | 46.55µs | 73.88µs | 5 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 100 static tools | 500.61µs |  |  | 479.64µs | 682.18µs | 5 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 10 static tools | 6.41µs |  |  | 6.33µs | 10.06µs | 5 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 100 static tools | 55.03µs |  |  | 53.75µs | 84.85µs | 5 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 100 deltas | 451.75µs |  |  | 438.13µs | 779.38µs | 5 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 1000 deltas | 3.792ms |  |  | 3.682ms | 6.103ms | 5 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 4000 deltas | 14.879ms |  |  | 14.390ms | 23.734ms | 5 |
| data-stream › assistant-stream: data stream decode + accumulate, one tool-call start per part › 100 parts | 2.867ms |  |  | 2.504ms | 4.137ms | 5 |
| data-stream › assistant-stream: data stream decode + accumulate, one tool-call start per part › 2000 parts | 71.203ms |  |  | 66.274ms | 110.087ms | 5 |
| data-stream › assistant-stream: data stream decode + accumulate, one tool-call start per part › 500 parts | 12.666ms |  |  | 12.617ms | 19.358ms | 5 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 100 deltas | 209.87µs |  |  | 209.03µs | 355.47µs | 5 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 1000 deltas | 2.068ms |  |  | 2.018ms | 3.374ms | 5 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 4000 deltas | 8.393ms |  |  | 8.079ms | 13.348ms | 5 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 1000 messages, 6-part replies | 225.05µs |  |  | 196.34µs | 244.76µs | 5 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 5000 messages, 20-part replies | 1.914ms |  |  | 1.397ms | 2.023ms | 5 |
| external-message-conversion › core: external message reasoning continuations › 100 matches | 44.18µs |  |  | 43.58µs | 70.55µs | 5 |
| external-message-conversion › core: external message reasoning continuations › 1000 matches | 439.60µs |  |  | 436.74µs | 710.10µs | 5 |
| external-message-conversion › core: external message reasoning continuations › 5000 matches | 2.398ms |  |  | 2.340ms | 3.782ms | 5 |
| external-message-conversion › core: external message tool results › 100 matches | 54.25µs |  |  | 54.25µs | 82.75µs | 5 |
| external-message-conversion › core: external message tool results › 1000 matches | 560.76µs |  |  | 552.05µs | 812.56µs | 5 |
| external-message-conversion › core: external message tool results › 5000 matches | 3.023ms |  |  | 2.943ms | 4.248ms | 5 |
| external-message-conversion › core: external message unique tool calls › 100 matches | 27.98µs |  |  | 27.98µs | 41.97µs | 5 |
| external-message-conversion › core: external message unique tool calls › 1000 matches | 275.03µs |  |  | 271.93µs | 417.56µs | 5 |
| external-message-conversion › core: external message unique tool calls › 5000 matches | 1.484ms |  |  | 1.471ms | 2.186ms | 5 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 1 text parts | 0.18µs |  |  | 0.18µs | 0.29µs | 5 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 10 text parts | 0.31µs |  |  | 0.30µs | 0.47µs | 5 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 100 text parts | 1.60µs |  |  | 1.57µs | 2.45µs | 5 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 1 tool calls | 0.39µs |  |  | 0.39µs | 0.67µs | 5 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 10 tool calls | 2.37µs |  |  | 2.34µs | 3.58µs | 5 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 100 tool calls | 20.86µs |  |  | 20.42µs | 32.40µs | 5 |
| interactable-array-patches › core: id-keyed interactable array patches › 1000 items and patches | 116.17µs |  |  | 112.90µs | 142.89µs | 5 |
| interactable-array-patches › core: id-keyed interactable array patches › 5000 items and patches | 662.66µs |  |  | 593.91µs | 836.45µs | 5 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tilde runs on one line | 2.005ms |  |  | 1.951ms | 2.848ms | 5 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tildes after prose | 118.89µs |  |  | 118.59µs | 207.24µs | 5 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 triple-backtick spans on one line | 2.581ms |  |  | 2.563ms | 3.690ms | 5 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 5,000 code spans in one paragraph | 351.19µs |  |  | 330.36µs | 515.49µs | 5 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, mixed message, 100 sections | 512.49µs |  |  | 506.12µs | 726.14µs | 5 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tilde runs on one line | 5.790ms |  |  | 5.197ms | 7.207ms | 5 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tildes after prose | 486.36µs |  |  | 480.79µs | 923.44µs | 5 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 triple-backtick spans on one line | 15.089ms |  |  | 14.911ms | 24.337ms | 5 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 5,000 code spans in one paragraph | 2.367ms |  |  | 2.367ms | 3.810ms | 5 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, mixed message, 100 sections | 1.822ms |  |  | 1.794ms | 2.824ms | 5 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown | 1.996ms |  |  | 1.979ms | 3.184ms | 5 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown deferred | 2.225ms |  |  | 2.213ms | 3.476ms | 5 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown | 13.466ms |  |  | 13.413ms | 22.200ms | 5 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown deferred | 14.776ms |  |  | 14.726ms | 23.850ms | 5 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 1 paragraphs | 1.138ms |  |  | 1.010ms | 1.612ms | 5 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 10 paragraphs | 1.950ms |  |  | 1.904ms | 3.357ms | 5 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 50 paragraphs | 6.563ms |  |  | 6.563ms | 10.933ms | 5 |
| markdown-streaming › react-markdown: the same token with defer on › 1 paragraphs deferred | 1.437ms |  |  | 1.192ms | 1.445ms | 5 |
| markdown-streaming › react-markdown: the same token with defer on › 10 paragraphs deferred | 1.433ms |  |  | 1.367ms | 1.861ms | 5 |
| markdown-streaming › react-markdown: the same token with defer on › 50 paragraphs deferred | 3.802ms |  |  | 3.802ms | 4.992ms | 5 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 1000 character argument in 16-character deltas | 212.26µs |  |  | 209.50µs | 323.54µs | 5 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 10000 character argument in 16-character deltas | 1.776ms |  |  | 1.677ms | 2.548ms | 5 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 500 short object entries in 16-character deltas | 186.311ms |  |  | 182.549ms | 300.906ms | 5 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 50000 character argument in 16-character deltas | 9.273ms |  |  | 8.390ms | 12.252ms | 5 |
| react-pi-message-projection › react-pi: streaming tail projection › 10 stable messages | 1.29µs |  |  | 1.24µs | 2.34µs | 5 |
| react-pi-message-projection › react-pi: streaming tail projection › 1000 stable messages | 5.55µs |  |  | 5.36µs | 9.86µs | 5 |
| react-pi-message-projection › react-pi: streaming tail projection › 5000 stable messages | 27.22µs |  |  | 25.67µs | 43.67µs | 5 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 1 chunks | 4.71µs |  |  | 4.71µs | 7.35µs | 5 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 101 chunks | 15.47µs |  |  | 15.47µs | 21.08µs | 5 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1 chunks | 45.79µs |  |  | 45.79µs | 72.54µs | 5 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1025 chunks | 201.75µs |  |  | 189.72µs | 283.03µs | 5 |
| thread-scaling › external-store thread: mount+unmount by message count › 10 messages | 4.536ms |  |  | 4.522ms | 7.319ms | 5 |
| thread-scaling › external-store thread: mount+unmount by message count › 100 messages | 27.830ms |  |  | 27.716ms | 49.201ms | 5 |
| thread-scaling › external-store thread: mount+unmount by message count › 1000 messages | 328.302ms |  |  | 328.302ms | 491.960ms | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 10 messages | 343.35µs |  |  | 343.35µs | 644.98µs | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 100 messages | 639.18µs |  |  | 633.87µs | 928.31µs | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 1000 messages | 3.175ms |  |  | 2.877ms | 4.859ms | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 10 messages | 349.26µs |  |  | 349.26µs | 610.45µs | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 100 messages | 1.229ms |  |  | 1.083ms | 1.628ms | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 1000 messages | 9.277ms |  |  | 8.622ms | 18.151ms | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 10 messages | 378.01µs |  |  | 354.28µs | 608.03µs | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 100 messages | 958.34µs |  |  | 821.30µs | 1.168ms | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 1000 messages | 5.602ms |  |  | 5.602ms | 10.609ms | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 10 messages | 151.99µs |  |  | 150.05µs | 322.01µs | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 100 messages | 352.32µs |  |  | 345.49µs | 575.20µs | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 1000 messages | 2.846ms |  |  | 2.455ms | 4.094ms | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 10 messages | 11.37µs |  |  | 11.28µs | 26.66µs | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 100 messages | 23.16µs |  |  | 23.02µs | 43.45µs | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 1000 messages | 200.62µs |  |  | 196.45µs | 267.48µs | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 10 messages | 418.27µs |  |  | 383.74µs | 746.28µs | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 100 messages | 897.99µs |  |  | 809.08µs | 1.248ms | 5 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 1000 messages | 5.976ms |  |  | 5.634ms | 11.557ms | 5 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 1000 bytes | 163.06µs |  |  | 159.62µs | 259.07µs | 5 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 10000 bytes | 1.485ms |  |  | 1.455ms | 2.208ms | 5 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 5000 bytes | 752.66µs |  |  | 738.37µs | 1.115ms | 5 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 1000 bytes | 183.61µs |  |  | 178.76µs | 321.72µs | 5 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 10000 bytes | 1.622ms |  |  | 1.562ms | 2.601ms | 5 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 5000 bytes | 819.51µs |  |  | 794.71µs | 1.322ms | 5 |
| tool-args › assistant-stream: complete accumulated arguments (single delta) › 10,000 array elements | 245.94µs |  |  | 245.94µs | 353.42µs | 5 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 array entries | 17.366ms |  |  | 17.226ms | 26.627ms | 5 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 object entries | 672.287ms |  |  | 469.467ms | 674.679ms | 5 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 1000 bytes | 135.22µs |  |  | 132.17µs | 241.42µs | 5 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 10000 bytes | 1.094ms |  |  | 1.089ms | 1.879ms | 5 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 5000 bytes | 563.34µs |  |  | 553.29µs | 962.81µs | 5 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 10000 bytes | 158.55µs |  |  | 153.99µs | 211.44µs | 5 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 50000 bytes | 741.36µs |  |  | 726.07µs | 949.94µs | 5 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 10000 bytes | 171.73µs |  |  | 167.29µs | 235.70µs | 5 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 50000 bytes | 792.98µs |  |  | 779.38µs | 1.030ms | 5 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRoot | 2.964ms |  |  | 2.297ms | 4.382ms | 5 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootDeps | 2.893ms |  |  | 2.332ms | 4.416ms | 5 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootStable | 2.896ms |  |  | 2.254ms | 4.322ms | 5 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › react | 2.170ms |  |  | 2.160ms | 3.763ms | 5 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › tapRoot | 2.151ms |  |  | 1.456ms | 3.503ms | 5 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRoot | 2.135ms |  |  | 2.125ms | 3.302ms | 5 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootDeps | 2.129ms |  |  | 2.123ms | 3.441ms | 5 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootStable | 252.23µs |  |  | 199.83µs | 358.85µs | 5 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › react | 95.49µs |  |  | 94.78µs | 147.23µs | 5 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › tapRoot | 1.110ms |  |  | 1.110ms | 1.750ms | 5 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › deps | 1.311ms |  |  | 1.236ms | 2.071ms | 5 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › no-deps | 1.365ms |  |  | 1.299ms | 2.141ms | 5 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › deps | 30.75µs |  |  | 30.33µs | 54.97µs | 5 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › no-deps | 33.38µs |  |  | 33.26µs | 54.13µs | 5 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › deps | 53.84µs |  |  | 50.61µs | 70.04µs | 5 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › no-deps | 1.050ms |  |  | 959.30µs | 1.558ms | 5 |

informational; points come from different runners of the same class, so read trends, not single deltas.
