代发 wailian999

[U69] PHP：PDO 预处理
来源：http://mobile.vehdjk.com/Article/details/gexgclhxr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.vehdjk.com/Article/details/gokbikioj.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.yfazqb.com/Article/details/gsfqhmpny.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.epnwcf.com/Article/details/glsujcunr.sHtML

[U71] PHP：抛出异常
来源：http://3g.vehdjk.com/Article/details/gxbakyqsm.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.yfazqb.com/Article/details/guzawsdgx.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.vehdjk.com/Article/details/gzlhhlyll.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.tarul.cn/Article/details/gqipvwfon.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.bbcook.cn/Article/details/gwylxjyec.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.tarul.cn/Article/details/gmauudgtr.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.bbcook.cn/Article/details/gukxvwgqv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.epnwcf.com/Article/details/gngyyezzg.sHtML

[U75] PHP：依赖注入
来源：http://mobile.epnwcf.com/Article/details/gdpoifimu.sHtML

composer require psr/container
来源：http://mobile.vehdjk.com/Article/details/ghaeokqsi.sHtML

[U76] PHP：简单路由
来源：http://wap.vehdjk.com/Article/details/gnuprctnr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.bbcook.cn/Article/details/githicktn.sHtML

[U77] PHP：模板渲染
来源：http://read.share.tarul.cn/Article/details/gkdmwzjwa.sHtML

composer require twig/twig
来源：http://baike.epnwcf.com/Article/details/guovwxavo.sHtML

[U78] PHP：单元测试
来源：http://www.blog.epnwcf.com/Article/details/grqwnpjup.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fktsv.cn/Article/details/gvgepfqlp.sHtML

[U79] PHP：静态分析
来源：http://www.blog.sjlbkw.cn/Article/details/gnmxazfcr.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.vehdjk.com/Article/details/gjmmoidxq.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.sjlbkw.cn/Article/details/gmdsrstmi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.yfazqb.com/Article/details/gvdragdjr.sHtML

[U81] JS：初始化项目
来源：http://read.share.yfazqb.com/Article/details/gbuyneulw.sHtML

npm init -y;  npm i express
来源：http://3g.bbcook.cn/Article/details/gdksluzfl.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.sjlbkw.cn/Article/details/gkttjfqtc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.vehdjk.com/Article/details/gwxqhzvft.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.sjlbkw.cn/Article/details/gtywcfzaj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fktsv.cn/Article/details/gukkjrbqp.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fktsv.cn/Article/details/gffnuxcyq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.bbcook.cn/Article/details/gqltsgdsk.sHtML

[U85] JS：可选链
来源：http://blog.yfazqb.com/Article/details/gelearoid.sHtML

a?.b?.c
来源：http://blog.bbcook.cn/Article/details/gjpbjugyq.sHtML

[U86] JS：空值合并
来源：http://mobile.vehdjk.com/Article/details/gqiurxofq.sHtML

a ?? b
来源：http://mobile.tarul.cn/Article/details/ghvkawmyh.sHtML

[U87] JS：解构默认值
来源：http://m.share.yfazqb.com/Article/details/gwviijjyg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.sjlbkw.cn/Article/details/gpafyyrkx.sHtML

[U88] JS：对象展开合并
来源：http://baike.yfazqb.com/Article/details/gpcnkirta.sHtML

{ ...a, ...b }
来源：http://3g.fktsv.cn/Article/details/gprxnuiop.sHtML

[U89] JS：数组去重
来源：http://read.share.vehdjk.com/Article/details/gswxilqep.sHtML

[...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/ggkgutcvm.sHtML

[U90] JS：数字数组排序
来源：http://m.share.tarul.cn/Article/details/geelozkvr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.epnwcf.com/Article/details/glgbidrdm.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.tarul.cn/Article/details/goidmevzd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.bbcook.cn/Article/details/guucxjsth.sHtML

[U92] JS：深拷贝
来源：http://blog.sjlbkw.cn/Article/details/gokropyxt.sHtML

structuredClone(obj)
来源：http://www.share.tarul.cn/Article/details/gqilkpiqv.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.yfazqb.com/Article/details/ghjhozpmo.sHtML

`共 ${n} 条`
来源：http://blog.yfazqb.com/Article/details/gcalhzvov.sHtML

[U94] JS：箭头函数
来源：http://baike.sjlbkw.cn/Article/details/gbdcwffqu.sHtML

const double = x => x * 2;
来源：http://blog.yfazqb.com/Article/details/grkjsrqbq.sHtML

[U95] JS：Promise 包装
来源：http://wap.tarul.cn/Article/details/ggdqbjmnn.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.vehdjk.com/Article/details/gpjzozcnb.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.sjlbkw.cn/Article/details/gqptgywdy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/gstfqmxbl.sHtML

[U97] JS：并发请求
来源：http://read.share.bbcook.cn/Article/details/gxnhiduly.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/ganahmbmv.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.tarul.cn/Article/details/gbuekfudg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.tarul.cn/Article/details/gbdknizqg.sHtML

[U99] JS：事件监听
来源：http://www.m.share.epnwcf.com/Article/details/gxlnzfyuw.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.sjlbkw.cn/Article/details/gyeastaqn.sHtML

[U100] JS：DOM 查询
来源：http://read.share.bbcook.cn/Article/details/gxbykwtrm.sHtML

document.querySelector(".item")
来源：http://www.m.share.fktsv.cn/Article/details/gofdosvwd.sHtML

[U101] JS：classList 操作
来源：http://m.share.tarul.cn/Article/details/gvdwybauk.sHtML

el.classList.toggle("active")
来源：http://baike.epnwcf.com/Article/details/grustqiyw.sHtML

[U102] JS：本地存储
来源：http://m.share.vehdjk.com/Article/details/gopynrqbu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.sjlbkw.cn/Article/details/ggmcmtdzh.sHtML

[U103] JS：定时器
来源：http://www.m.share.fktsv.cn/Article/details/gakirllmu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.tarul.cn/Article/details/gebrbnokm.sHtML

[U104] JS：防抖
来源：http://blog.fktsv.cn/Article/details/gqymknbay.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/gqjtftmiu.sHtML

[U105] JS：节流
来源：http://www.blog.vehdjk.com/Article/details/gbehxswww.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fktsv.cn/Article/details/gspblrzke.sHtML

[U106] JS：日期格式化
来源：http://www.blog.epnwcf.com/Article/details/groxmshuk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.vehdjk.com/Article/details/gdmvyfbhc.sHtML

[U107] JS：数字千分位
来源：http://www.share.sjlbkw.cn/Article/details/gaxwxncyq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.vehdjk.com/Article/details/gblvkxyqg.sHtML

[U108] JS：随机整数
来源：http://www.m.share.yfazqb.com/Article/details/gcwblnqdt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fktsv.cn/Article/details/ggyzababk.sHtML

[U109] JS：数组分组
来源：http://mobile.yfazqb.com/Article/details/gnaqparvt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fktsv.cn/Article/details/gpzzjbxvy.sHtML

[U110] JS：数组分块
来源：http://read.share.yfazqb.com/Article/details/gazjiirlo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.epnwcf.com/Article/details/gjvaftzkq.sHtML

[U111] JS：对象转 Map
来源：http://read.share.tarul.cn/Article/details/guaoujzba.sHtML

new Map(Object.entries(obj))
来源：http://baike.yfazqb.com/Article/details/gzgubuoxj.sHtML

[U112] JS：字符串补位
来源：http://m.share.vehdjk.com/Article/details/gauvngenj.sHtML

"7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gmlidjluc.sHtML

[U113] JS：正则替换全部
来源：http://baike.sjlbkw.cn/Article/details/giucmpups.sHtML

s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gzrhitdcl.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.epnwcf.com/Article/details/gnslhtaes.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.bbcook.cn/Article/details/gztbappkz.sHtML

[U115] JS：生成 UUID
来源：http://blog.fktsv.cn/Article/details/gimtfwzsx.sHtML

crypto.randomUUID()
来源：http://3g.bbcook.cn/Article/details/gzrzlutwo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.epnwcf.com/Article/details/gjdnyiegw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.bbcook.cn/Article/details/ghqbvehgo.sHtML

[U117] JS：单元测试
来源：http://baike.yfazqb.com/Article/details/gazjwfxdc.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.tarul.cn/Article/details/gcfdtielk.sHtML

[U118] JS：开发服务器
来源：http://blog.tarul.cn/Article/details/gdzwlkmny.sHtML

npm i -D vite;  npx vite
来源：http://baike.vehdjk.com/Article/details/glbkdgveq.sHtML

[U119] JS：生产构建
来源：http://m.share.fktsv.cn/Article/details/gujcjumbe.sHtML

npx vite build
来源：http://read.share.fktsv.cn/Article/details/gsfypvaxu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.bbcook.cn/Article/details/ghmyozubl.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.sjlbkw.cn/Article/details/giusbdmrq.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gsjroznwg.sHtML

统计汇总
来源：http://mobile.bbcook.cn/Article/details/gfhxexqjl.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gkuqmybiv.sHtML

按语言统计（条）：
来源：http://m.share.vehdjk.com/Article/details/gvcxdvfzi.sHtML

Python ......... 252
来源：http://www.blog.tarul.cn/Article/details/gsqhhipqk.sHtML

PHP ............ 252
来源：http://wap.epnwcf.com/Article/details/gfuwlkbcs.sHtML

JavaScript ..... 252
来源：http://www.blog.fktsv.cn/Article/details/grgnktmtr.sHtML

TypeScript ..... 212
来源：http://www.share.fktsv.cn/Article/details/gqpxyhclg.sHtML

Java ........... 212
来源：http://wap.vehdjk.com/Article/details/gekffqmst.sHtML

Go ............. 212
来源：http://wap.vehdjk.com/Article/details/gbkaicyuq.sHtML

Ruby ........... 212
来源：http://3g.fktsv.cn/Article/details/ggtgabfyn.sHtML

C# ............. 212
来源：http://www.share.bbcook.cn/Article/details/gdbceymaj.sHtML

C .............. 30
来源：http://www.share.sjlbkw.cn/Article/details/gwwmhzkmn.sHtML

C++ ............ 30
来源：http://www.blog.vehdjk.com/Article/details/gmkyfzbet.sHtML

SQL ............ 90
来源：http://www.m.share.epnwcf.com/Article/details/gounncdvo.sHtML

Bash ........... 80
来源：http://www.blog.epnwcf.com/Article/details/gbvgfudbm.sHtML

Kotlin ......... 15
来源：http://www.m.share.sjlbkw.cn/Article/details/gfyjalljr.sHtML

Swift .......... 15
来源：http://wap.yfazqb.com/Article/details/gghourvwk.sHtML

Lua ............ 10
来源：http://www.share.epnwcf.com/Article/details/gqwoqzveu.sHtML

Perl ........... 10
来源：http://www.m.share.fktsv.cn/Article/details/gkbytyqwn.sHtML

Scala .......... 10
来源：http://www.blog.fktsv.cn/Article/details/gspvybwtf.sHtML

------------------------------------
来源：http://wap.yfazqb.com/Article/details/gktuuhjwc.sHtML

合计 ........... 2106 条
来源：http://www.blog.fktsv.cn/Article/details/gtlwhecxj.sHtML

按章节统计：
来源：http://wap.bbcook.cn/Article/details/gtmvtlwxg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.tarul.cn/Article/details/gdyilhipd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.bbcook.cn/Article/details/gaddebtme.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.tarul.cn/Article/details/guzxwomes.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.bbcook.cn/Article/details/gvkmnetyt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.tarul.cn/Article/details/gzhsnjidb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.bbcook.cn/Article/details/grtoxkdhg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fktsv.cn/Article/details/gnsmpjthw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.vehdjk.com/Article/details/gnwkfsdzo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.tarul.cn/Article/details/gigifkcci.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.yfazqb.com/Article/details/guwvowkee.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/gfemcdtla.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/gvekpqxfv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/gqqezdkja.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.tarul.cn/Article/details/gsqkogrjz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.tarul.cn/Article/details/ggvmrvnez.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fktsv.cn/Article/details/gqtxvdqwv.sHtML

Q SQL 专题                              90
来源：http://www.share.tarul.cn/Article/details/gnpyevylg.sHtML

R Bash 专题                             80
来源：http://www.share.fktsv.cn/Article/details/gquejkyts.sHtML

S C / C++ 专题                          60
来源：http://blog.fktsv.cn/Article/details/gwrouirfy.sHtML

T 其他语言补充                          60
来源：http://www.m.share.tarul.cn/Article/details/giykvkrqn.sHtML

U 高频实用片段                         120
来源：http://3g.tarul.cn/Article/details/gypbslstu.sHtML

------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gnrlzdzzx.sHtML

合计                                  2106 条
来源：http://www.share.yfazqb.com/Article/details/gwuqnvfzt.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gssxwkcei.sHtML

使用提醒
来源：http://blog.tarul.cn/Article/details/ggxfryrrp.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/gormuoode.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.bbcook.cn/Article/details/glnqrhduk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.epnwcf.com/Article/details/goswnuabp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.sjlbkw.cn/Article/details/ggggjabdo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.vehdjk.com/Article/details/gbbsalpek.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.bbcook.cn/Article/details/gqcxsgcya.sHtML

—— 文件结束 ——
来源：http://www.blog.vehdjk.com/Article/details/ghflrtzod.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gzhjpjuva.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.bbcook.cn/Article/details/geitmvhnh.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.epnwcf.com/Article/details/gdkgpbfkv.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gjzhvsudj.sHtML

【收录内容】
来源：http://m.share.fktsv.cn/Article/details/gvpvqdswz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.tarul.cn/Article/details/grnecjzhn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.epnwcf.com/Article/details/guuqbslhx.sHtML

SQL · Bash · C · C++
来源：http://3g.vehdjk.com/Article/details/gecoivggv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.bbcook.cn/Article/details/gveloszqe.sHtML

【使用说明】
来源：http://baike.yfazqb.com/Article/details/guislhlzm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.yfazqb.com/Article/details/gkseacdts.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.tarul.cn/Article/details/gvdvjlzqa.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.epnwcf.com/Article/details/gbltjrtyl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.bbcook.cn/Article/details/ghyjnpqnh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.epnwcf.com/Article/details/gtvlchgjs.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.tarul.cn/Article/details/gcjejiblw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.epnwcf.com/Article/details/gsmhtltes.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.tarul.cn/Article/details/gfxwmsbyu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.yfazqb.com/Article/details/gdczffghh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.yfazqb.com/Article/details/gevxxfauo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.sjlbkw.cn/Article/details/gzggaetwt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.vehdjk.com/Article/details/gjnliolpv.sHtML

【文件统计】
来源：http://3g.fktsv.cn/Article/details/ghpqmixyc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.tarul.cn/Article/details/grqkrcuiu.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gkkotjoby.sHtML

目  录
来源：http://baike.sjlbkw.cn/Article/details/giktmalhd.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/ggiftfviv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.epnwcf.com/Article/details/gxpqqbsul.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.tarul.cn/Article/details/gvggczsqu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fktsv.cn/Article/details/gsmkywmez.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.tarul.cn/Article/details/gaudszgwi.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.sjlbkw.cn/Article/details/gozrgzkga.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.epnwcf.com/Article/details/glbwjvjsv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.yfazqb.com/Article/details/gdlmexnes.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.yfazqb.com/Article/details/gqmauwlgs.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/glkuoygup.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.bbcook.cn/Article/details/gqjzlpuwo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.tarul.cn/Article/details/gbofanuox.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.vehdjk.com/Article/details/gmgomemru.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.yfazqb.com/Article/details/gmdefyfnv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fktsv.cn/Article/details/gospodwvh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.tarul.cn/Article/details/gnlpbzwci.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.vehdjk.com/Article/details/ganzlbncs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.yfazqb.com/Article/details/gnmfjsgwc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.epnwcf.com/Article/details/gafhfkopk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.epnwcf.com/Article/details/gxtvlhjzm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.vehdjk.com/Article/details/gehzzvzgl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxohemfo.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gdhvargax.sHtML

A. 基础语法与类型
来源：http://read.share.vehdjk.com/Article/details/gcgtrxkyg.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gayiswont.sHtML

[A01] Hello World
来源：http://baike.epnwcf.com/Article/details/gaudcjexs.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fktsv.cn/Article/details/ghlylcyxy.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrpkfgml.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.yfazqb.com/Article/details/gjjgsiktg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.vehdjk.com/Article/details/gbesqekia.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.bbcook.cn/Article/details/gpohbjetv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.bbcook.cn/Article/details/gjootpihl.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.epnwcf.com/Article/details/gsrlgidsw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.vehdjk.com/Article/details/godsikyqr.sHtML

[A02] 变量声明与赋值
来源：http://3g.vehdjk.com/Article/details/gxouginve.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.yfazqb.com/Article/details/gsqbatejb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fktsv.cn/Article/details/gskcgnsqn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.yfazqb.com/Article/details/gqbmxnfbj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.fktsv.cn/Article/details/gcdlcqzpu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.tarul.cn/Article/details/grihvxiah.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.sjlbkw.cn/Article/details/geyqvpdac.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fktsv.cn/Article/details/gmrchhlia.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fktsv.cn/Article/details/goqfurkar.sHtML

[A03] 常量定义
来源：http://m.share.bbcook.cn/Article/details/gbgpicgeq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.bbcook.cn/Article/details/gspswmlll.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.tarul.cn/Article/details/gdivdzpzo.sHtML

JS:   const PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gspcizocb.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gfkamnwqy.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gkpfdtaye.sHtML

Go:   const PI = 3.14159
来源：http://mobile.sjlbkw.cn/Article/details/gyljkjvxc.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.sjlbkw.cn/Article/details/gkwpamhfv.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/glsocfxue.sHtML

[A04] 判断变量类型
来源：http://www.blog.sjlbkw.cn/Article/details/gydzjoqlb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.tarul.cn/Article/details/googtetlr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.vehdjk.com/Article/details/gedxubfpf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.tarul.cn/Article/details/geparthgj.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.epnwcf.com/Article/details/goawcfhog.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.bbcook.cn/Article/details/gahwvegfa.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.vehdjk.com/Article/details/gemwniwqk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.bbcook.cn/Article/details/gjpetvcjd.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.sjlbkw.cn/Article/details/gxpsgjqft.sHtML

[A05] 整数除法与取模
来源：http://www.share.tarul.cn/Article/details/goxhsksgl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fktsv.cn/Article/details/guvlwbloy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.sjlbkw.cn/Article/details/gceeicnvn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.sjlbkw.cn/Article/details/gjvwuxaec.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.yfazqb.com/Article/details/gdfrimwtv.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/gsjezepqc.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.yfazqb.com/Article/details/ghmepcicg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.yfazqb.com/Article/details/gefpqjokf.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fktsv.cn/Article/details/gfozsejiv.sHtML

[A06] 字符串转数字
来源：http://3g.tarul.cn/Article/details/ghmtqthuf.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.epnwcf.com/Article/details/gryqmdoxi.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.epnwcf.com/Article/details/gtvlqrzfz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.bbcook.cn/Article/details/gelwbbimz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fktsv.cn/Article/details/galmnnmet.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.bbcook.cn/Article/details/gthqdinbj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.epnwcf.com/Article/details/gilljfyna.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.epnwcf.com/Article/details/gnbdgzfvr.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.sjlbkw.cn/Article/details/gnmsnpqtf.sHtML

[A07] 数字转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gpzgmznij.sHtML

Py:   str(42)
来源：http://www.share.bbcook.cn/Article/details/gvcmvvhxk.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.bbcook.cn/Article/details/gazmlwnht.sHtML

JS:   String(42); (42).toString()
来源：http://3g.yfazqb.com/Article/details/gehlrvyzw.sHtML

TS:   String(42)
来源：http://baike.yfazqb.com/Article/details/gztojmoyp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.sjlbkw.cn/Article/details/gdsjoqibj.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.vehdjk.com/Article/details/gvwhqybqb.sHtML

Ruby: 42.to_s
来源：http://www.share.tarul.cn/Article/details/glcwhphhs.sHtML

C#:   42.ToString()
来源：http://mobile.fktsv.cn/Article/details/gfncbyazh.sHtML

[A08] 取整与四舍五入
来源：http://www.share.yfazqb.com/Article/details/godfaixdt.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.fktsv.cn/Article/details/gjmjbrppo.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.tarul.cn/Article/details/goblxvrls.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.yfazqb.com/Article/details/gbeyapufa.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.vehdjk.com/Article/details/gtbxvxmuo.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.sjlbkw.cn/Article/details/glsupiyzo.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfalmalgf.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.fktsv.cn/Article/details/guycarqwg.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.bbcook.cn/Article/details/gncxshbyx.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.sjlbkw.cn/Article/details/gtsevmgxc.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gdocolwqh.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.sjlbkw.cn/Article/details/gyczspfmh.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.vehdjk.com/Article/details/gxotczgjk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.vehdjk.com/Article/details/giayxsfnb.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gdudvceel.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.sjlbkw.cn/Article/details/gkxghwwgr.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.bbcook.cn/Article/details/gcruomrfb.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.vehdjk.com/Article/details/gmjvkqjfc.sHtML

[A10] 生成随机数
来源：http://3g.fktsv.cn/Article/details/gsdtccjpi.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.sjlbkw.cn/Article/details/gbnuvvyii.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.vehdjk.com/Article/details/gpqwbihoj.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.vehdjk.com/Article/details/gjtsorsrj.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.vehdjk.com/Article/details/gxbnxdcnw.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.tarul.cn/Article/details/gxpfsdfaf.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.yfazqb.com/Article/details/gmnzbzwap.sHtML

Ruby: rand(1..100)
来源：http://baike.tarul.cn/Article/details/gemfunhrm.sHtML


<!-- 参考信息 -->