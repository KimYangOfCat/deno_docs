# 运行时 {#runtime}

<<<<<<< HEAD
可以在 [`doc.deno.land`](https://doc.deno.land/deno/stable) 上找到所有运行时功能（Web API +
`Deno` global）的文档。
=======
Documentation for all runtime functions (Web APIs + `Deno` global) can be found
on [`doc.deno.land/deno/stable`](https://doc.deno.land/deno/stable@$CLI_VERSION)
with _unstable_ APIs which are enabled via the `--unstable` flag at
[`doc.deno.land/deno/unstable`](https://doc.deno.land/deno/unstable@$CLI_VERSION).
>>>>>>> 50e20856ff7fef33fafd258b6966ca34afba4b9b

## Web Platform APIs {#web-platform-apis}

对于已经存在的 Web 标准 API（例如，HTTP 请求的 `fetch`），Deno 是去使用这些标准，而不是发明新的专有 API。

更多详细信息，请参见 [Web Platform APIs](./runtime/web_platform_apis.md)。

## `Deno` global {#deno-global}

<<<<<<< HEAD
所有非 Web 标准的 API 都包含在全局 `Deno` 命名空间中。 这些 API 包括：读取文件，打开 TCP 套接字，提供 HTTP
服务以及执行子进程等的。

有关 Deno 命名空间的 TypeScript 定义，请参见
[`lib.deno.ns.d.ts`](https://github.com/denoland/deno/blob/$CLI_VERSION/cli/dts/lib.deno.ns.d.ts)。

有关所有 Deno 特定 API 文档，请参见
[doc.deno.land](https://doc.deno.land/https://raw.githubusercontent.com/denoland/deno/main/cli/dts/lib.deno.ns.d.ts)。
=======
All APIs that are not web standard are contained in the global `Deno` namespace.
It has the APIs for reading from files, opening TCP sockets,
[serving HTTP](./runtime/http_server_apis.md), and executing subprocesses, etc.

The TypeScript definitions for the Deno namespaces can be found in the
[`lib.deno.ns.d.ts`](https://github.com/denoland/deno/blob/$CLI_VERSION/cli/dts/lib.deno.ns.d.ts)
file.
>>>>>>> 50e20856ff7fef33fafd258b6966ca34afba4b9b
