代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://blog.vehdjk.com/Article/details/grsfdjalc.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.sjlbkw.cn/Article/details/gadjkwfgw.sHtML

[U74] PHP：读取环境变量
来源：http://blog.tarul.cn/Article/details/gcsjaohhf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.bbcook.cn/Article/details/ggyexjcdv.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.bbcook.cn/Article/details/gvyddqqpq.sHtML

composer require psr/container
来源：http://baike.tarul.cn/Article/details/goifnulne.sHtML

[U76] PHP：简单路由
来源：http://blog.epnwcf.com/Article/details/gbqwsokca.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.sjlbkw.cn/Article/details/gcdtyknzw.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.vehdjk.com/Article/details/gcvczxbug.sHtML

composer require twig/twig
来源：http://m.share.sjlbkw.cn/Article/details/gykesgxtz.sHtML

[U78] PHP：单元测试
来源：http://read.share.bbcook.cn/Article/details/gmggryjhn.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.vehdjk.com/Article/details/ggtoieyka.sHtML

[U79] PHP：静态分析
来源：http://www.blog.epnwcf.com/Article/details/gejcdxjbx.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.yfazqb.com/Article/details/gbcbspnxp.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fktsv.cn/Article/details/gupcbpxlt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.yfazqb.com/Article/details/glgbiiikm.sHtML

[U81] JS：初始化项目
来源：http://blog.vehdjk.com/Article/details/gnvjdvmxd.sHtML

npm init -y;  npm i express
来源：http://blog.vehdjk.com/Article/details/gbflijigc.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwleuave.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.sjlbkw.cn/Article/details/gswgyxufb.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.bbcook.cn/Article/details/gsxobyquh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.bbcook.cn/Article/details/gjjolkrwe.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.tarul.cn/Article/details/goyfhalwb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fktsv.cn/Article/details/gmcrxvemm.sHtML

[U85] JS：可选链
来源：http://read.share.yfazqb.com/Article/details/gttecfopu.sHtML

a?.b?.c
来源：http://blog.bbcook.cn/Article/details/ggmjkshjo.sHtML

[U86] JS：空值合并
来源：http://www.m.share.sjlbkw.cn/Article/details/grbtutsza.sHtML

a ?? b
来源：http://m.share.vehdjk.com/Article/details/grskeynkd.sHtML

[U87] JS：解构默认值
来源：http://www.share.yfazqb.com/Article/details/gjvmgzaov.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fktsv.cn/Article/details/gprtjkfgp.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fktsv.cn/Article/details/ghyyyxznu.sHtML

{ ...a, ...b }
来源：http://mobile.vehdjk.com/Article/details/gguyfnixg.sHtML

[U89] JS：数组去重
来源：http://baike.vehdjk.com/Article/details/gctjgxwda.sHtML

[...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/gxtknqvcv.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fktsv.cn/Article/details/gnyqpfzfj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gldvbcxhn.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.epnwcf.com/Article/details/gfukfxyyt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fktsv.cn/Article/details/gwcgnqbbq.sHtML

[U92] JS：深拷贝
来源：http://www.share.vehdjk.com/Article/details/gurmwhuir.sHtML

structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/gymjzbgof.sHtML

[U93] JS：模板字符串
来源：http://read.share.sjlbkw.cn/Article/details/gormlhncz.sHtML

`共 ${n} 条`
来源：http://www.blog.fktsv.cn/Article/details/grfbdfzgo.sHtML

[U94] JS：箭头函数
来源：http://www.blog.yfazqb.com/Article/details/gccuepxrk.sHtML

const double = x => x * 2;
来源：http://www.share.tarul.cn/Article/details/gqsmfeqgy.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.yfazqb.com/Article/details/gqgdikjmw.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.yfazqb.com/Article/details/gbjmqixzq.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.epnwcf.com/Article/details/gexdydyds.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.bbcook.cn/Article/details/gojilhtws.sHtML

[U97] JS：并发请求
来源：http://www.blog.tarul.cn/Article/details/glhuxtfzp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gxvqskudo.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.yfazqb.com/Article/details/gevrhgcbv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.vehdjk.com/Article/details/gbfrrdctn.sHtML

[U99] JS：事件监听
来源：http://www.share.sjlbkw.cn/Article/details/gbwyicryb.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.tarul.cn/Article/details/gggrpilzt.sHtML

[U100] JS：DOM 查询
来源：http://baike.yfazqb.com/Article/details/gszekpjur.sHtML

document.querySelector(".item")
来源：http://baike.vehdjk.com/Article/details/gbtkmduan.sHtML

[U101] JS：classList 操作
来源：http://www.share.yfazqb.com/Article/details/gnkfqnzrj.sHtML

el.classList.toggle("active")
来源：http://www.share.vehdjk.com/Article/details/gbiqzqshs.sHtML

[U102] JS：本地存储
来源：http://m.share.tarul.cn/Article/details/gucqklmql.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.vehdjk.com/Article/details/gqxkbjivf.sHtML

[U103] JS：定时器
来源：http://blog.epnwcf.com/Article/details/ggaalkbnv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.tarul.cn/Article/details/gzijpyaxk.sHtML

[U104] JS：防抖
来源：http://mobile.bbcook.cn/Article/details/gzbpsomzv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/ghtaotgkj.sHtML

[U105] JS：节流
来源：http://blog.yfazqb.com/Article/details/gpmcmdxms.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.vehdjk.com/Article/details/ggjygutjn.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.epnwcf.com/Article/details/gvmgypfhs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.yfazqb.com/Article/details/gympltgzr.sHtML

[U107] JS：数字千分位
来源：http://m.share.epnwcf.com/Article/details/gddoludeb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.yfazqb.com/Article/details/gsactmtfr.sHtML

[U108] JS：随机整数
来源：http://wap.tarul.cn/Article/details/guwdvmqrr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.vehdjk.com/Article/details/gncwhjzgg.sHtML

[U109] JS：数组分组
来源：http://3g.vehdjk.com/Article/details/goksfjqyw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.bbcook.cn/Article/details/gtzdohznv.sHtML

[U110] JS：数组分块
来源：http://3g.yfazqb.com/Article/details/gcnnemknt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.vehdjk.com/Article/details/gzcnitygk.sHtML

[U111] JS：对象转 Map
来源：http://mobile.bbcook.cn/Article/details/gywaxxsze.sHtML

new Map(Object.entries(obj))
来源：http://mobile.epnwcf.com/Article/details/giaexjpyc.sHtML

[U112] JS：字符串补位
来源：http://3g.vehdjk.com/Article/details/gafcgqfbk.sHtML

"7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/gaypxbmel.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.yfazqb.com/Article/details/groguopvr.sHtML

s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gedcyprnf.sHtML

[U114] JS：JSON 深比较
来源：http://baike.yfazqb.com/Article/details/gjhacisea.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.vehdjk.com/Article/details/gudmvbmpz.sHtML

[U115] JS：生成 UUID
来源：http://3g.sjlbkw.cn/Article/details/gobpnwfep.sHtML

crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/gzueawksm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.bbcook.cn/Article/details/gpzujhqty.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.yfazqb.com/Article/details/guacuzday.sHtML

[U117] JS：单元测试
来源：http://mobile.yfazqb.com/Article/details/ghgktejaw.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fktsv.cn/Article/details/gwfjrxhem.sHtML

[U118] JS：开发服务器
来源：http://wap.fktsv.cn/Article/details/grbhzmcjw.sHtML

npm i -D vite;  npx vite
来源：http://3g.fktsv.cn/Article/details/gbllzeljs.sHtML

[U119] JS：生产构建
来源：http://mobile.yfazqb.com/Article/details/gwccrmxno.sHtML

npx vite build
来源：http://mobile.vehdjk.com/Article/details/gxuodrkzp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.vehdjk.com/Article/details/gprfkvlka.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.bbcook.cn/Article/details/gulandqbx.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gcghmdvqd.sHtML

统计汇总
来源：http://baike.tarul.cn/Article/details/grbktnpls.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gufvagste.sHtML

按语言统计（条）：
来源：http://read.share.fktsv.cn/Article/details/gsdmaskkz.sHtML

Python ......... 252
来源：http://www.share.fktsv.cn/Article/details/godyxknjf.sHtML

PHP ............ 252
来源：http://blog.vehdjk.com/Article/details/gnvyxblzv.sHtML

JavaScript ..... 252
来源：http://mobile.bbcook.cn/Article/details/gklfqxvde.sHtML

TypeScript ..... 212
来源：http://www.share.tarul.cn/Article/details/gakozviva.sHtML

Java ........... 212
来源：http://www.m.share.yfazqb.com/Article/details/geshusiii.sHtML

Go ............. 212
来源：http://www.share.fktsv.cn/Article/details/guvtbqjdt.sHtML

Ruby ........... 212
来源：http://mobile.yfazqb.com/Article/details/gyjbvkxqd.sHtML

C# ............. 212
来源：http://read.share.epnwcf.com/Article/details/gyofyosmv.sHtML

C .............. 30
来源：http://read.share.tarul.cn/Article/details/gnvsaqyvj.sHtML

C++ ............ 30
来源：http://baike.bbcook.cn/Article/details/gljtldwef.sHtML

SQL ............ 90
来源：http://blog.yfazqb.com/Article/details/gsirqpelj.sHtML

Bash ........... 80
来源：http://mobile.epnwcf.com/Article/details/gwilvcpxr.sHtML

Kotlin ......... 15
来源：http://blog.vehdjk.com/Article/details/gxmesylke.sHtML

Swift .......... 15
来源：http://read.share.yfazqb.com/Article/details/gwgoystbs.sHtML

Lua ............ 10
来源：http://www.m.share.vehdjk.com/Article/details/gamdcpyys.sHtML

Perl ........... 10
来源：http://www.share.tarul.cn/Article/details/gubpbprbz.sHtML

Scala .......... 10
来源：http://3g.yfazqb.com/Article/details/gdesouegr.sHtML

------------------------------------
来源：http://blog.yfazqb.com/Article/details/gdbutuapx.sHtML

合计 ........... 2106 条
来源：http://www.m.share.sjlbkw.cn/Article/details/gfywlqwhg.sHtML

按章节统计：
来源：http://www.m.share.sjlbkw.cn/Article/details/gsywrnhbm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.sjlbkw.cn/Article/details/gwnmbnqzr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.vehdjk.com/Article/details/glsdywdjn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/goaleaedk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.bbcook.cn/Article/details/gnbdeotou.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.sjlbkw.cn/Article/details/gxxwyoupi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.tarul.cn/Article/details/gkdexxemq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.sjlbkw.cn/Article/details/gwwzzcujk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fktsv.cn/Article/details/ghvaugkji.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gvzhzamxt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.yfazqb.com/Article/details/ghejuvfoh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gdobmsdhm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gliyzzrln.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/gmvemsgps.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.epnwcf.com/Article/details/gfzajuhrl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.tarul.cn/Article/details/gkbqaqxwe.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.tarul.cn/Article/details/gszuzcwsj.sHtML

Q SQL 专题                              90
来源：http://www.blog.sjlbkw.cn/Article/details/guctajasx.sHtML

R Bash 专题                             80
来源：http://baike.vehdjk.com/Article/details/gxwfimlah.sHtML

S C / C++ 专题                          60
来源：http://baike.yfazqb.com/Article/details/ghikayvpu.sHtML

T 其他语言补充                          60
来源：http://wap.tarul.cn/Article/details/ghmlrtndq.sHtML

U 高频实用片段                         120
来源：http://mobile.vehdjk.com/Article/details/gfnfgixto.sHtML

------------------------------------
来源：http://3g.yfazqb.com/Article/details/gimvhcsnn.sHtML

合计                                  2106 条
来源：http://www.blog.yfazqb.com/Article/details/gzvwaazqc.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.vehdjk.com/Article/details/gxrbbokxw.sHtML

使用提醒
来源：http://www.m.share.tarul.cn/Article/details/gtqudvnso.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.tarul.cn/Article/details/gcutqsfza.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.vehdjk.com/Article/details/gupiawlyd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.yfazqb.com/Article/details/gtcqwkmob.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.epnwcf.com/Article/details/gduhenrbm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.vehdjk.com/Article/details/gtrurceuu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.tarul.cn/Article/details/gzjvlcgqj.sHtML

—— 文件结束 ——
来源：http://m.share.vehdjk.com/Article/details/gsfqmnheb.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gjizfbyod.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.yfazqb.com/Article/details/gbngbzntl.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.bbcook.cn/Article/details/gvtfjtbyv.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gygzuvjxt.sHtML

【收录内容】
来源：http://read.share.epnwcf.com/Article/details/gklitaswz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.sjlbkw.cn/Article/details/gxadnanno.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.yfazqb.com/Article/details/gjgvhlllf.sHtML

SQL · Bash · C · C++
来源：http://m.share.fktsv.cn/Article/details/grayposve.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.epnwcf.com/Article/details/goyhyzewg.sHtML

【使用说明】
来源：http://www.m.share.bbcook.cn/Article/details/gtrdtwajf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fktsv.cn/Article/details/gbstuiyis.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fktsv.cn/Article/details/gnqvnhmlu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.yfazqb.com/Article/details/gzkaasloi.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.epnwcf.com/Article/details/gmlvkdezx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.bbcook.cn/Article/details/gtdndijip.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.epnwcf.com/Article/details/ghktgsamp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.epnwcf.com/Article/details/gversbort.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.yfazqb.com/Article/details/glbcuebnn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.epnwcf.com/Article/details/gageghdmp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.yfazqb.com/Article/details/gvrcgnjqe.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.epnwcf.com/Article/details/gxalowkyn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fktsv.cn/Article/details/gqdidaeyc.sHtML

【文件统计】
来源：http://www.blog.epnwcf.com/Article/details/gahdgskht.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.vehdjk.com/Article/details/gvzmqqhuw.sHtML

--------------------------------------------------------------------------------
来源：http://blog.tarul.cn/Article/details/gujdupjth.sHtML

目  录
来源：http://mobile.sjlbkw.cn/Article/details/gkbwcldyk.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.epnwcf.com/Article/details/gnmnktymi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.bbcook.cn/Article/details/gmblsztop.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.sjlbkw.cn/Article/details/gtsmzxhsg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.vehdjk.com/Article/details/gjbqpqkun.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fktsv.cn/Article/details/gexvxnpqu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.epnwcf.com/Article/details/gjuljcmtp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.epnwcf.com/Article/details/gogsrlimy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.tarul.cn/Article/details/grzzxwmdo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.tarul.cn/Article/details/guspwtllz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fktsv.cn/Article/details/gsxybacmc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.vehdjk.com/Article/details/gurvgvtjb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.yfazqb.com/Article/details/gwqbfyekm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/gqllldmyo.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.vehdjk.com/Article/details/gnkddcipf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.vehdjk.com/Article/details/gckaoglfp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.sjlbkw.cn/Article/details/gccmhqmnb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.yfazqb.com/Article/details/godthxnln.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fktsv.cn/Article/details/gvdnqibhg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.yfazqb.com/Article/details/grpcbsqfo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fktsv.cn/Article/details/gyrvapwfd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fktsv.cn/Article/details/gudssvkzb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fktsv.cn/Article/details/gxqgxspto.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ghcqmbftc.sHtML

A. 基础语法与类型
来源：http://www.blog.bbcook.cn/Article/details/gaqnqaaae.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gmkbvuxqi.sHtML

[A01] Hello World
来源：http://read.share.bbcook.cn/Article/details/gatsacybq.sHtML

Py:   print("Hello, World!")
来源：http://m.share.bbcook.cn/Article/details/guirndbcg.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.yfazqb.com/Article/details/gvcitldzi.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.sjlbkw.cn/Article/details/ghjsmijaq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.vehdjk.com/Article/details/gvrlsgqwl.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.vehdjk.com/Article/details/grmzkgmoe.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.bbcook.cn/Article/details/gezyutkot.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.tarul.cn/Article/details/gvzoabzax.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.bbcook.cn/Article/details/gmnzglvnk.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.tarul.cn/Article/details/gdqushlal.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.bbcook.cn/Article/details/gtcvlnpua.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.vehdjk.com/Article/details/gebhbktap.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fktsv.cn/Article/details/gjdhhqipd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fktsv.cn/Article/details/grevkmars.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fktsv.cn/Article/details/gmtgyvkth.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.yfazqb.com/Article/details/gdcajsexz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.yfazqb.com/Article/details/gtiqhaxmk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.epnwcf.com/Article/details/gspnulcgh.sHtML

[A03] 常量定义
来源：http://m.share.tarul.cn/Article/details/gthkrvmik.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.vehdjk.com/Article/details/gufklxnac.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gplzhokyw.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gvvjwkfsv.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.bbcook.cn/Article/details/gmerklvap.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/guvdnuuaa.sHtML

Go:   const PI = 3.14159
来源：http://blog.tarul.cn/Article/details/gkkyqnbuu.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fktsv.cn/Article/details/gklwdbjlz.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gbgazxfjq.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fktsv.cn/Article/details/gkoumzgab.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fktsv.cn/Article/details/gtabjmrpr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.bbcook.cn/Article/details/gxhienfbp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.tarul.cn/Article/details/gqbvvrrcb.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.bbcook.cn/Article/details/gpjculrtv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.epnwcf.com/Article/details/gttmotifd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.vehdjk.com/Article/details/gqkgepixj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.yfazqb.com/Article/details/gcjvwczld.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.sjlbkw.cn/Article/details/guzrbteko.sHtML

[A05] 整数除法与取模
来源：http://www.share.fktsv.cn/Article/details/gkhynkiak.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.fktsv.cn/Article/details/gbwjjrwqg.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.epnwcf.com/Article/details/geeivkogr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.yfazqb.com/Article/details/gclvhawco.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.tarul.cn/Article/details/gfjjndpzr.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.tarul.cn/Article/details/ggjugavzu.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.yfazqb.com/Article/details/gilineasz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fktsv.cn/Article/details/gqaiqfqyg.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.vehdjk.com/Article/details/gobxzzmqw.sHtML

[A06] 字符串转数字
来源：http://blog.epnwcf.com/Article/details/gykpbuaqd.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.sjlbkw.cn/Article/details/gvymxiovi.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.sjlbkw.cn/Article/details/gfwckvwkz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fktsv.cn/Article/details/gbeindlqk.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.vehdjk.com/Article/details/gmumzqsxg.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.bbcook.cn/Article/details/gocmwuzrl.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.vehdjk.com/Article/details/gqiimkdve.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.bbcook.cn/Article/details/ghgprcizv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.yfazqb.com/Article/details/ggotmbmws.sHtML

[A07] 数字转字符串
来源：http://read.share.epnwcf.com/Article/details/gljfcvrvn.sHtML

Py:   str(42)
来源：http://read.share.yfazqb.com/Article/details/gwnlwltky.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.epnwcf.com/Article/details/gcesgvyle.sHtML

JS:   String(42); (42).toString()
来源：http://blog.vehdjk.com/Article/details/gufzpmrpg.sHtML

TS:   String(42)
来源：http://mobile.sjlbkw.cn/Article/details/ghxeypzzw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmhxxatz.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.tarul.cn/Article/details/gnqgmpteu.sHtML

Ruby: 42.to_s
来源：http://wap.fktsv.cn/Article/details/gtcfhkptq.sHtML

C#:   42.ToString()
来源：http://www.share.fktsv.cn/Article/details/gjsocfldy.sHtML

[A08] 取整与四舍五入
来源：http://mobile.yfazqb.com/Article/details/giziygney.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.epnwcf.com/Article/details/gfyhnonhh.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.vehdjk.com/Article/details/gnbyfnccs.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.bbcook.cn/Article/details/gabfpoddr.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.yfazqb.com/Article/details/gnijpvssn.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.epnwcf.com/Article/details/gbiqosrzu.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.fktsv.cn/Article/details/gswfkiujo.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.fktsv.cn/Article/details/ggnskguqp.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.yfazqb.com/Article/details/gqrisdddu.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.bbcook.cn/Article/details/gpthtjwsi.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gluhfbkzk.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqfhpgoj.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gcapntmvi.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/gxduyfldv.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.epnwcf.com/Article/details/gihiznypu.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.epnwcf.com/Article/details/gzndvpove.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.vehdjk.com/Article/details/gqmsspbbk.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gbhfismnq.sHtML

[A10] 生成随机数
来源：http://blog.sjlbkw.cn/Article/details/goafndckw.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.fktsv.cn/Article/details/gtypzadbs.sHtML

PHP:  random_int(1, 100);
来源：http://blog.yfazqb.com/Article/details/gwrdzucof.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.epnwcf.com/Article/details/ghahllijq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.vehdjk.com/Article/details/gvvejpxcb.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.bbcook.cn/Article/details/gsxazriob.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.sjlbkw.cn/Article/details/ghsagcuku.sHtML

Ruby: rand(1..100)
来源：http://m.share.tarul.cn/Article/details/glxchqfcy.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.tarul.cn/Article/details/giiygmiof.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fktsv.cn/Article/details/gcbmbdqll.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.bbcook.cn/Article/details/gacevxpzz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.bbcook.cn/Article/details/ghuzrijef.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.epnwcf.com/Article/details/gutqbdysg.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.sjlbkw.cn/Article/details/gchimusjv.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.vehdjk.com/Article/details/gjqsyfqjx.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.yfazqb.com/Article/details/glrvmzwjd.sHtML


<!-- 参考信息 -->