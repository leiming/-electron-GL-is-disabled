# Electron 14.x Error: GL is disabled in Windows 10.

### How to reproduce errors

```bash
yarn start

#or

.\node_modules\.bin\electron main.js
```
### Error log

```bash
$ yarn start
yarn run v1.22.18
$ electron main.js

(node:13640) electron: The default of nativeWindowOpen is deprecated and will be changing from false to true in Electron 15.  See https://github.com/electron/electron/issues/28511 for more information.
(Use `electron --trace-warnings ...` to show where the warning was created)
[7776:0426/021213.441:ERROR:command_buffer_proxy_impl.cc(125)] ContextResult::kTransientFailure: Failed to send GpuControl.CreateCommandBuffer.
[10868:0426/021411.430:ERROR:gpu_init.cc(441)] Passthrough is not supported, GL is disabled
```