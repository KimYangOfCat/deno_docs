# 文档测试

Deno 支持对文档示例进行类型检查。

这可以确保文档中的示例是最新且能正常工作的。

基本的想法是这样的：

````ts
/**
 * # 示例
 *
 * ```ts
 * const x = 42;
 * ```
 */
````

三个反引号标记代码块的开头和结尾，语言由语言标识符指定，可以是以下任何一种：

- `js`
- `jsx`
- `ts`
- `tsx`

如果未指定语言标识符，则从代码块所提取的源文档的媒体类型中推断语言。

如果此示例位于名为 foo.ts 的文件中，则运行 `deno test --doc foo.ts`
将提取此示例，然后将其作为一个独立的模块与文档所在目录中的模块进行类型检查。

要记录您的导出项，请使用相对路径说明符导入模块：

````ts
/**
 * # 示例
 *
 * ```ts
 * import { foo } from "./foo.ts";
 * ```
 */
export function foo(): string {
  return "foo";
}
````