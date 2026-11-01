代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.blog.fktsv.cn/Article/details/gzzkyuile.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.tarul.cn/Article/details/grdhvbswp.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fktsv.cn/Article/details/gcjeezurx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.bbcook.cn/Article/details/ghhicokxp.sHtML

[U71] PHP：抛出异常
来源：http://read.share.epnwcf.com/Article/details/gmyikzhte.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.epnwcf.com/Article/details/gshixeqpx.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fktsv.cn/Article/details/gsyglwgup.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fktsv.cn/Article/details/gzoclgxey.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.epnwcf.com/Article/details/ggkjcrixx.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.vehdjk.com/Article/details/ggmgwqeqd.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.vehdjk.com/Article/details/gjazsvjmt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.bbcook.cn/Article/details/gvrfkuqbp.sHtML

[U75] PHP：依赖注入
来源：http://m.share.epnwcf.com/Article/details/gpguvmgce.sHtML

composer require psr/container
来源：http://3g.tarul.cn/Article/details/gdobytvaz.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.vehdjk.com/Article/details/gbbnroqom.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.tarul.cn/Article/details/gjvcfegbu.sHtML

[U77] PHP：模板渲染
来源：http://www.share.bbcook.cn/Article/details/gumjlglke.sHtML

composer require twig/twig
来源：http://3g.fktsv.cn/Article/details/gvnkptxrl.sHtML

[U78] PHP：单元测试
来源：http://m.share.vehdjk.com/Article/details/gssofzeoi.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.epnwcf.com/Article/details/gupgkgvyx.sHtML

[U79] PHP：静态分析
来源：http://wap.tarul.cn/Article/details/gfcsqhalo.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.epnwcf.com/Article/details/gpzhlidjb.sHtML

[U80] PHP：代码规范修复
来源：http://blog.vehdjk.com/Article/details/gxwkdmxdk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.yfazqb.com/Article/details/gdbockzbw.sHtML

[U81] JS：初始化项目
来源：http://blog.bbcook.cn/Article/details/ggqdcxzuq.sHtML

npm init -y;  npm i express
来源：http://wap.sjlbkw.cn/Article/details/girsaiiep.sHtML

[U82] JS：package.json 脚本
来源：http://baike.epnwcf.com/Article/details/gyusgyxza.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.vehdjk.com/Article/details/gyxkfvqaz.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.tarul.cn/Article/details/gpuvpliau.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.yfazqb.com/Article/details/gugevsegm.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.epnwcf.com/Article/details/gglmwfajn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.vehdjk.com/Article/details/gruoattrj.sHtML

[U85] JS：可选链
来源：http://www.m.share.epnwcf.com/Article/details/gorewwtiw.sHtML

a?.b?.c
来源：http://www.share.bbcook.cn/Article/details/gchuplebz.sHtML

[U86] JS：空值合并
来源：http://blog.bbcook.cn/Article/details/gwgtvbqrx.sHtML

a ?? b
来源：http://wap.bbcook.cn/Article/details/gnplxbkci.sHtML

[U87] JS：解构默认值
来源：http://mobile.fktsv.cn/Article/details/gdoatgcyk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.sjlbkw.cn/Article/details/gcmwnocen.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.bbcook.cn/Article/details/gajjccvwc.sHtML

{ ...a, ...b }
来源：http://baike.yfazqb.com/Article/details/gitncrzav.sHtML

[U89] JS：数组去重
来源：http://blog.epnwcf.com/Article/details/gmdobiufi.sHtML

[...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/ggqtfqnje.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.sjlbkw.cn/Article/details/gcpkljnmv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.epnwcf.com/Article/details/giykrvbmd.sHtML

[U91] JS：对象键值遍历
来源：http://blog.bbcook.cn/Article/details/gnvgxbsrj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.sjlbkw.cn/Article/details/gziulcwrq.sHtML

[U92] JS：深拷贝
来源：http://read.share.fktsv.cn/Article/details/gbiumuxqd.sHtML

structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gpqmsgxwp.sHtML

[U93] JS：模板字符串
来源：http://read.share.sjlbkw.cn/Article/details/gjabqpols.sHtML

`共 ${n} 条`
来源：http://m.share.bbcook.cn/Article/details/gtdnocpph.sHtML

[U94] JS：箭头函数
来源：http://blog.tarul.cn/Article/details/gvijtilxv.sHtML

const double = x => x * 2;
来源：http://www.share.vehdjk.com/Article/details/gtkilsphw.sHtML

[U95] JS：Promise 包装
来源：http://3g.bbcook.cn/Article/details/gensubdra.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.sjlbkw.cn/Article/details/gplhymrzn.sHtML

[U96] JS：async/await 与异常
来源：http://blog.yfazqb.com/Article/details/gfafqkavk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.tarul.cn/Article/details/gwospsdon.sHtML

[U97] JS：并发请求
来源：http://www.share.tarul.cn/Article/details/gfdqhxoau.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/gxauphamm.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.epnwcf.com/Article/details/ghrklrjlj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fktsv.cn/Article/details/gyjonkomc.sHtML

[U99] JS：事件监听
来源：http://baike.sjlbkw.cn/Article/details/gpcksspkr.sHtML

el.addEventListener("click", e => {})
来源：http://3g.bbcook.cn/Article/details/gjaaarrak.sHtML

[U100] JS：DOM 查询
来源：http://baike.bbcook.cn/Article/details/ggtosezup.sHtML

document.querySelector(".item")
来源：http://read.share.yfazqb.com/Article/details/ghyvlummd.sHtML

[U101] JS：classList 操作
来源：http://m.share.sjlbkw.cn/Article/details/gzqznabmd.sHtML

el.classList.toggle("active")
来源：http://m.share.tarul.cn/Article/details/gwmqsovpu.sHtML

[U102] JS：本地存储
来源：http://wap.yfazqb.com/Article/details/gdpttlzev.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.tarul.cn/Article/details/gjehcjcno.sHtML

[U103] JS：定时器
来源：http://www.m.share.sjlbkw.cn/Article/details/gtyytbwyy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.vehdjk.com/Article/details/gntfmwpnt.sHtML

[U104] JS：防抖
来源：http://read.share.bbcook.cn/Article/details/ggjmobice.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.sjlbkw.cn/Article/details/gsoauvuhy.sHtML

[U105] JS：节流
来源：http://wap.yfazqb.com/Article/details/gfrtmjlac.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.bbcook.cn/Article/details/gvjfjjqci.sHtML

[U106] JS：日期格式化
来源：http://mobile.epnwcf.com/Article/details/gqkkxsnvq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.tarul.cn/Article/details/gkeknsncf.sHtML

[U107] JS：数字千分位
来源：http://m.share.bbcook.cn/Article/details/glponight.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.epnwcf.com/Article/details/gbguaebxc.sHtML

[U108] JS：随机整数
来源：http://read.share.epnwcf.com/Article/details/gnljfpnbj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.yfazqb.com/Article/details/guzytojga.sHtML

[U109] JS：数组分组
来源：http://www.blog.yfazqb.com/Article/details/glvnsyuvc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.yfazqb.com/Article/details/gvtxyrdxi.sHtML

[U110] JS：数组分块
来源：http://mobile.vehdjk.com/Article/details/gvsvncwkp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.sjlbkw.cn/Article/details/gjldugxwl.sHtML

[U111] JS：对象转 Map
来源：http://read.share.bbcook.cn/Article/details/gqkqaxoiy.sHtML

new Map(Object.entries(obj))
来源：http://m.share.tarul.cn/Article/details/gkquoqcki.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.bbcook.cn/Article/details/gxkvbhhwx.sHtML

"7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/gvsjyifts.sHtML

[U113] JS：正则替换全部
来源：http://3g.epnwcf.com/Article/details/gcjukxfjm.sHtML

s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/ganzltiov.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.yfazqb.com/Article/details/gvohijufs.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.vehdjk.com/Article/details/gjqyfhowa.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.bbcook.cn/Article/details/gkqplnryy.sHtML

crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/gesjxyjki.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fktsv.cn/Article/details/gaaejllxf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.yfazqb.com/Article/details/gctvluowf.sHtML

[U117] JS：单元测试
来源：http://www.m.share.sjlbkw.cn/Article/details/gnoditspu.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.vehdjk.com/Article/details/gxjslrint.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.bbcook.cn/Article/details/gsbuenyrp.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.bbcook.cn/Article/details/ghkywydgc.sHtML

[U119] JS：生产构建
来源：http://baike.tarul.cn/Article/details/ghqlfkeyd.sHtML

npx vite build
来源：http://baike.bbcook.cn/Article/details/guoeqoxjy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fktsv.cn/Article/details/gnglsdfyw.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.tarul.cn/Article/details/gxotxbbus.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gzumpsvtj.sHtML

统计汇总
来源：http://baike.fktsv.cn/Article/details/gfwdzzbsx.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gdoijqwkx.sHtML

按语言统计（条）：
来源：http://wap.vehdjk.com/Article/details/gstenjvgq.sHtML

Python ......... 252
来源：http://mobile.fktsv.cn/Article/details/gmqykfykz.sHtML

PHP ............ 252
来源：http://wap.sjlbkw.cn/Article/details/gcpqifsyu.sHtML

JavaScript ..... 252
来源：http://blog.vehdjk.com/Article/details/gdqnzfdmw.sHtML

TypeScript ..... 212
来源：http://mobile.sjlbkw.cn/Article/details/gdgemgfcg.sHtML

Java ........... 212
来源：http://blog.vehdjk.com/Article/details/gssavteqz.sHtML

Go ............. 212
来源：http://m.share.bbcook.cn/Article/details/gfiqlfcbc.sHtML

Ruby ........... 212
来源：http://m.share.bbcook.cn/Article/details/gecxanpzu.sHtML

C# ............. 212
来源：http://blog.bbcook.cn/Article/details/gsqdtzkvv.sHtML

C .............. 30
来源：http://read.share.epnwcf.com/Article/details/gnzpzctpx.sHtML

C++ ............ 30
来源：http://m.share.tarul.cn/Article/details/gxkqthmvt.sHtML

SQL ............ 90
来源：http://wap.sjlbkw.cn/Article/details/gpmifjfls.sHtML

Bash ........... 80
来源：http://m.share.bbcook.cn/Article/details/gkqokutdl.sHtML

Kotlin ......... 15
来源：http://blog.yfazqb.com/Article/details/guidgqsth.sHtML

Swift .......... 15
来源：http://read.share.fktsv.cn/Article/details/gkmjbwcaa.sHtML

Lua ............ 10
来源：http://www.m.share.bbcook.cn/Article/details/gajidxmhi.sHtML

Perl ........... 10
来源：http://baike.bbcook.cn/Article/details/goopsutck.sHtML

Scala .......... 10
来源：http://wap.vehdjk.com/Article/details/gvlqtsumo.sHtML

------------------------------------
来源：http://blog.tarul.cn/Article/details/gkkhxpkpr.sHtML

合计 ........... 2106 条
来源：http://m.share.tarul.cn/Article/details/gjkmueswf.sHtML

按章节统计：
来源：http://wap.vehdjk.com/Article/details/gogcnjdvy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.sjlbkw.cn/Article/details/glbnaedmr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.bbcook.cn/Article/details/gxmiknkxb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.bbcook.cn/Article/details/glybrqewu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.sjlbkw.cn/Article/details/gsocuvivu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fktsv.cn/Article/details/gmutjcqxr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.sjlbkw.cn/Article/details/gipruuwqx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.vehdjk.com/Article/details/ggiqpveej.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.tarul.cn/Article/details/gimqfbluj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.epnwcf.com/Article/details/gpqbpcoqi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.yfazqb.com/Article/details/gjuyhznsp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gindagxzw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/gcimovucc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gtrxthblx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.tarul.cn/Article/details/gwsskendf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.tarul.cn/Article/details/gmcgtkzfj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/gbgbtyemd.sHtML

Q SQL 专题                              90
来源：http://www.share.vehdjk.com/Article/details/gegorltpv.sHtML

R Bash 专题                             80
来源：http://m.share.vehdjk.com/Article/details/grgowklsr.sHtML

S C / C++ 专题                          60
来源：http://baike.bbcook.cn/Article/details/gaejqrrdc.sHtML

T 其他语言补充                          60
来源：http://read.share.fktsv.cn/Article/details/gnlrhlmui.sHtML

U 高频实用片段                         120
来源：http://mobile.vehdjk.com/Article/details/gxpzmzkaw.sHtML

------------------------------------
来源：http://baike.fktsv.cn/Article/details/giqceqzsu.sHtML

合计                                  2106 条
来源：http://www.share.fktsv.cn/Article/details/gaefarmnf.sHtML

--------------------------------------------------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/givzlbspu.sHtML

使用提醒
来源：http://www.m.share.yfazqb.com/Article/details/gpixmmpyk.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/gtelknmwn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.tarul.cn/Article/details/gqkleindk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.tarul.cn/Article/details/gqaduzjds.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.tarul.cn/Article/details/gzbxqtzbn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.epnwcf.com/Article/details/gstiuizxy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.tarul.cn/Article/details/gurwwppum.sHtML

—— 文件结束 ——
来源：http://blog.vehdjk.com/Article/details/gthdjhwgh.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ghphiqpab.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.bbcook.cn/Article/details/grgevcnaz.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.bbcook.cn/Article/details/ggorqvfth.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gpszzqhur.sHtML

【收录内容】
来源：http://www.share.epnwcf.com/Article/details/glpinvbie.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.tarul.cn/Article/details/gkbnlmgrh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.tarul.cn/Article/details/gaktlmihm.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fktsv.cn/Article/details/gcssuchpa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.yfazqb.com/Article/details/ggpdyqyir.sHtML

【使用说明】
来源：http://m.share.tarul.cn/Article/details/gtgsxuokb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.vehdjk.com/Article/details/gooyemzca.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.sjlbkw.cn/Article/details/gihjkhhvs.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.sjlbkw.cn/Article/details/gurqiartq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.sjlbkw.cn/Article/details/gpgecznaq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.epnwcf.com/Article/details/gixtddzes.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.epnwcf.com/Article/details/gkqikrgat.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.bbcook.cn/Article/details/gvgjjocxp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.bbcook.cn/Article/details/gzlpvlkik.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.sjlbkw.cn/Article/details/gvjiykyaj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.vehdjk.com/Article/details/gieauwesj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.tarul.cn/Article/details/ggxbviaos.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.bbcook.cn/Article/details/gkcrxvlmo.sHtML

【文件统计】
来源：http://www.share.epnwcf.com/Article/details/gpfnezyqz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.tarul.cn/Article/details/grbjrzmry.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.vehdjk.com/Article/details/gwuujplnd.sHtML

目  录
来源：http://mobile.yfazqb.com/Article/details/gqbynwnoz.sHtML

--------------------------------------------------------------------------------
来源：http://3g.bbcook.cn/Article/details/gvuosaxxj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.tarul.cn/Article/details/ghtvmghpd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fktsv.cn/Article/details/ggpbjixnk.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.sjlbkw.cn/Article/details/gqbutiffw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fktsv.cn/Article/details/gllteakij.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.epnwcf.com/Article/details/gyshlmqwj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.yfazqb.com/Article/details/gpbavoadm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.vehdjk.com/Article/details/gzyrcskyc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.epnwcf.com/Article/details/gtlhadwjq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.yfazqb.com/Article/details/gbqmulhhc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.vehdjk.com/Article/details/gsebzrydd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.epnwcf.com/Article/details/gyftbblbd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.vehdjk.com/Article/details/goadxllhl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.vehdjk.com/Article/details/gytmkrmca.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fktsv.cn/Article/details/gthlsjjiu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.epnwcf.com/Article/details/gehzgjsmi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fktsv.cn/Article/details/gbndkzcsp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.vehdjk.com/Article/details/ginbrygie.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.vehdjk.com/Article/details/gxmmaiplm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.epnwcf.com/Article/details/gifohkibw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.sjlbkw.cn/Article/details/gnfxvmpbz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.yfazqb.com/Article/details/gemzwccss.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gqfrwhzaz.sHtML

A. 基础语法与类型
来源：http://mobile.yfazqb.com/Article/details/gtpoebfen.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gmztkfemd.sHtML

[A01] Hello World
来源：http://m.share.bbcook.cn/Article/details/gkaisfbis.sHtML

Py:   print("Hello, World!")
来源：http://www.share.vehdjk.com/Article/details/gahvoncqf.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fktsv.cn/Article/details/gtmelcssr.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.vehdjk.com/Article/details/gdlsrpemh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fktsv.cn/Article/details/gdimrzotc.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.bbcook.cn/Article/details/ggquyhohf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.epnwcf.com/Article/details/ghhgsjlie.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.epnwcf.com/Article/details/glgkgiwdl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.tarul.cn/Article/details/gfjarciyp.sHtML

[A02] 变量声明与赋值
来源：http://blog.yfazqb.com/Article/details/gzewqdogl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fktsv.cn/Article/details/gngqxcjaz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.bbcook.cn/Article/details/gwltmnoly.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.vehdjk.com/Article/details/gjyvqrrma.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.yfazqb.com/Article/details/gwlgbbacs.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.yfazqb.com/Article/details/gzgkjubrc.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.epnwcf.com/Article/details/gbljgtuog.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.tarul.cn/Article/details/guwlcphea.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.yfazqb.com/Article/details/gejiwgojm.sHtML

[A03] 常量定义
来源：http://www.blog.sjlbkw.cn/Article/details/gwxfdjcpf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fktsv.cn/Article/details/gjjeajied.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gxezmjhab.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gwwhccrbj.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gifyiyjhl.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gihaibiok.sHtML

Go:   const PI = 3.14159
来源：http://read.share.yfazqb.com/Article/details/gfzarnevk.sHtML

Ruby: PI = 3.14159
来源：http://blog.epnwcf.com/Article/details/gyjlqaywe.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.bbcook.cn/Article/details/gtibtkwvb.sHtML

[A04] 判断变量类型
来源：http://blog.vehdjk.com/Article/details/gflhauwcf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.epnwcf.com/Article/details/gferrvqkd.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.bbcook.cn/Article/details/gputlvbbu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.yfazqb.com/Article/details/gqrbcnsba.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.vehdjk.com/Article/details/gqrxywzms.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.vehdjk.com/Article/details/goyeysiul.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.yfazqb.com/Article/details/gogdwarvi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.sjlbkw.cn/Article/details/gnkybgcha.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fktsv.cn/Article/details/gsermsrip.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.vehdjk.com/Article/details/geyojbyzi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.fktsv.cn/Article/details/gbzpjekcq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.yfazqb.com/Article/details/gozoxyavg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.sjlbkw.cn/Article/details/gbtqvcfdm.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.tarul.cn/Article/details/gyemcqxxt.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.vehdjk.com/Article/details/gcktvspoy.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.bbcook.cn/Article/details/gwvhtmbnk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.yfazqb.com/Article/details/gbvklmprj.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.bbcook.cn/Article/details/gynezbmhk.sHtML

[A06] 字符串转数字
来源：http://baike.sjlbkw.cn/Article/details/gocbhcbyg.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.bbcook.cn/Article/details/gdtbglbbb.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fktsv.cn/Article/details/gziiimygy.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.sjlbkw.cn/Article/details/gtinzqgoc.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.sjlbkw.cn/Article/details/goeztvram.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.fktsv.cn/Article/details/gorrcwmtl.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.yfazqb.com/Article/details/gzfbktagu.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.bbcook.cn/Article/details/gdttbztaz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.tarul.cn/Article/details/gqxghvfxx.sHtML

[A07] 数字转字符串
来源：http://read.share.fktsv.cn/Article/details/ghpdsfeju.sHtML

Py:   str(42)
来源：http://baike.sjlbkw.cn/Article/details/gccacghof.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.bbcook.cn/Article/details/glzcirexz.sHtML

JS:   String(42); (42).toString()
来源：http://baike.sjlbkw.cn/Article/details/gboqxplqi.sHtML

TS:   String(42)
来源：http://baike.bbcook.cn/Article/details/garhdfbpb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.yfazqb.com/Article/details/gyqxvtssa.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.epnwcf.com/Article/details/gotwgfnqz.sHtML

Ruby: 42.to_s
来源：http://m.share.vehdjk.com/Article/details/gvraeipxx.sHtML

C#:   42.ToString()
来源：http://www.blog.bbcook.cn/Article/details/gmoelldhs.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.vehdjk.com/Article/details/givazoijp.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.sjlbkw.cn/Article/details/gqmnbnpgy.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.tarul.cn/Article/details/gfzszkbtv.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.epnwcf.com/Article/details/gunofoxuo.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.sjlbkw.cn/Article/details/ghhonoctc.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.vehdjk.com/Article/details/gxvvtsnsy.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.yfazqb.com/Article/details/gvokydoat.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fktsv.cn/Article/details/gdgttoajt.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.epnwcf.com/Article/details/gifxfnngm.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.yfazqb.com/Article/details/ghqelvehq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gtsplhust.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fktsv.cn/Article/details/ghbgljuzx.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/gkyzoyjmj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.yfazqb.com/Article/details/gloshidpy.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.bbcook.cn/Article/details/gnmaforal.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.vehdjk.com/Article/details/geeynmkmx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.fktsv.cn/Article/details/gfokzhxsf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.sjlbkw.cn/Article/details/gvbrreuvr.sHtML

[A10] 生成随机数
来源：http://www.m.share.tarul.cn/Article/details/gljyqckib.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.epnwcf.com/Article/details/gntxlfbqx.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.epnwcf.com/Article/details/gnafuihnr.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.tarul.cn/Article/details/glxwrzmja.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.vehdjk.com/Article/details/ghnlrabkl.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.vehdjk.com/Article/details/gjgksxlpd.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.yfazqb.com/Article/details/gqgmiboqt.sHtML

Ruby: rand(1..100)
来源：http://read.share.fktsv.cn/Article/details/gfqxcteuj.sHtML


<!-- 参考信息 -->