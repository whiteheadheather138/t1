代发 wailian999

[U75] PHP：依赖注入
来源：http://zyf.cheryme.top

composer require psr/container
来源：http://bdj.hnxiangtu.top

[U76] PHP：简单路由
来源：http://cpx.cheryme.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ixv.xuetiantiany.cn

[U77] PHP：模板渲染
来源：http://fuz.hysaishi.cn

composer require twig/twig
来源：http://qno.shzxlz.cn

[U78] PHP：单元测试
来源：http://mwh.chenzaomai.com

composer require --dev phpunit/phpunit
来源：http://ebd.zhijiandao.cn

[U79] PHP：静态分析
来源：http://ite.tanke756.top

composer require --dev phpstan/phpstan
来源：http://msy.xingfuxueyuan.xyz

[U80] PHP：代码规范修复
来源：http://wlj.xziqi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ykq.9152youxi.cn

[U81] JS：初始化项目
来源：http://kqw.shzxlz.cn

npm init -y;  npm i express
来源：http://ybe.andypj.xyz

[U82] JS：package.json 脚本
来源：http://vrz.birdmap.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://drd.xuetiantiany.cn

[U83] JS：ES Module 导入导出
来源：http://nxw.hysaishi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tej.jinqigufen.top

[U84] JS：CommonJS 写法
来源：http://ttm.svipenyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qgr.epnwcf.com

[U85] JS：可选链
来源：http://mfr.xziqi.cn

a?.b?.c
来源：http://efu.nanxinkj.top

[U86] JS：空值合并
来源：http://dbo.ywan-chungtsiang.top

a ?? b
来源：http://ice.ppjwa.cn

[U87] JS：解构默认值
来源：http://knh.xuetiantiany.cn

const { a = 1, b = 2 } = obj;
来源：http://muo.ywan-chungtsiang.top

[U88] JS：对象展开合并
来源：http://dst.svipenyu.cn

{ ...a, ...b }
来源：http://thr.sxryk.cn

[U89] JS：数组去重
来源：http://zgx.vqdsnc.cn

[...new Set(arr)]
来源：http://esu.aibaodan.cn

[U90] JS：数字数组排序
来源：http://xtb.shanyushiyangkeji.top

[...arr].sort((a, b) => a - b)
来源：http://trz.zhongyouzk.top

[U91] JS：对象键值遍历
来源：http://thp.zycfv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://peu.vqdsnc.cn

[U92] JS：深拷贝
来源：http://vbq.jinyuanbaomall.cn

structuredClone(obj)
来源：http://qra.c1oappe.top

[U93] JS：模板字符串
来源：http://ffy.hongshengwenyu.top

`共 ${n} 条`
来源：http://kyq.jyoumei.cn

[U94] JS：箭头函数
来源：http://ent.zhoulong.xyz

const double = x => x * 2;
来源：http://aia.meibo888.top

[U95] JS：Promise 包装
来源：http://xmv.guannengcc.top

new Promise((resolve, reject) => {})
来源：http://rya.52xcode.cn

[U96] JS：async/await 与异常
来源：http://sbo.jinyuanbaomall.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qfw.ybcxt.top

[U97] JS：并发请求
来源：http://tgv.zdbjq.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gfz.iojbl.cn

[U98] JS：fetch 带 JSON
来源：http://chk.hnxiangtu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rzl.shangyingyoupin.top

[U99] JS：事件监听
来源：http://krw.vqdsnc.cn

el.addEventListener("click", e => {})
来源：http://yqu.tianlin.xyz

[U100] JS：DOM 查询
来源：http://dhf.wangdashe.top

document.querySelector(".item")
来源：http://ofs.shzxlz.cn

[U101] JS：classList 操作
来源：http://mme.zdqjudy.top

el.classList.toggle("active")
来源：http://twc.cdnleiting.top

[U102] JS：本地存储
来源：http://coq.jinghuilouyu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pyf.yj202588.top

[U103] JS：定时器
来源：http://kzq.zycfv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qhj.guannengcc.top

[U104] JS：防抖
来源：http://eps.jinghuilouyu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cym.yj202588.top

[U105] JS：节流
来源：http://enr.andypj.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xht.yvedp.cn

[U106] JS：日期格式化
来源：http://kdo.haohaochexian.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rtu.ppjwa.cn

[U107] JS：数字千分位
来源：http://obv.epnwcf.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kao.vehdjk.com

[U108] JS：随机整数
来源：http://jqi.yuanzhike.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wfk.vqdsnc.cn

[U109] JS：数组分组
来源：http://gth.zhongyouzk.top

Object.groupBy(arr, x => x.type)
来源：http://aeq.vehdjk.com

[U110] JS：数组分块
来源：http://roz.jinqigufen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kdn.haohaochexian.top

[U111] JS：对象转 Map
来源：http://low.hammf.cn

new Map(Object.entries(obj))
来源：http://nxm.dianchejie.cn

[U112] JS：字符串补位
来源：http://fld.feifeiyinyue.top

"7".padStart(3, "0")
来源：http://jyo.yj202588.top

[U113] JS：正则替换全部
来源：http://dlc.ydjk.org.cn

s.replaceAll("a", "b")
来源：http://hjk.xinyue.icu

[U114] JS：JSON 深比较
来源：http://mdv.chenzaomai.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://mjc.52xcode.cn

[U115] JS：生成 UUID
来源：http://lnq.iojbl.cn

crypto.randomUUID()
来源：http://kha.ivvv.top

[U116] JS：类型检查（JSDoc）
来源：http://kod.andypj.xyz

/** @param {string} name */ function f(name) {}
来源：http://xgn.gotoacloud.top

[U117] JS：单元测试
来源：http://egx.shzxlz.cn

npm i -D vitest;  npx vitest
来源：http://wve.cashguo.top

[U118] JS：开发服务器
来源：http://yzr.9152youxi.cn

npm i -D vite;  npx vite
来源：http://nfb.ydjk.org.cn

[U119] JS：生产构建
来源：http://suw.yfazqb.com

npx vite build
来源：http://asw.fengsongda.top

[U120] JS：读取环境变量（Vite）
来源：http://dir.xylfe.cn

import.meta.env.VITE_API_URL
来源：http://goh.aizwys.cn

================================================================================
来源：http://ujv.cqqwz.cn

统计汇总
来源：http://ebn.yj202588.top

================================================================================
来源：http://xcq.jinyuanbaomall.cn

按语言统计（条）：
来源：http://sax.tanke756.top

Python ......... 252
来源：http://cim.dianchejie.cn

PHP ............ 252
来源：http://zkr.zhixingplan.top

JavaScript ..... 252
来源：http://lqo.guannengcc.top

TypeScript ..... 212
来源：http://atd.zdqjudy.top

Java ........... 212
来源：http://yuv.xingfuxueyuan.xyz

Go ............. 212
来源：http://dtq.hfpthk.cn

Ruby ........... 212
来源：http://uuh.shuidangran.top

C# ............. 212
来源：http://uvq.zhaomingkeji.xyz

C .............. 30
来源：http://uxz.bjfxy.top

C++ ............ 30
来源：http://hah.gaohongyu789.top

SQL ............ 90
来源：http://zfs.yuxming.cn

Bash ........... 80
来源：http://bgz.shanyushiyangkeji.top

Kotlin ......... 15
来源：http://phh.zhiwuduotai.top

Swift .......... 15
来源：http://jna.quarkkingdee.top

Lua ............ 10
来源：http://rft.jqgufenzy.top

Perl ........... 10
来源：http://fwu.yueranfly.top

Scala .......... 10
来源：http://vdg.havefunace.top

------------------------------------
来源：http://nju.xinyue.icu

合计 ........... 2106 条
来源：http://wgf.hcnkem.com

按章节统计：
来源：http://bxs.tanke756.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qhx.jinghuilouyu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bnm.vqdsnc.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://seq.sweek.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ucc.hnqzz.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wyf.nwbrower.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nib.cucudq.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://peg.dashuyun.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nga.shanyushiyangtech.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lgv.shanyushiyangkeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ozy.yj20258.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hgv.haohaochexian.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jmp.iojbl.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fjk.ydzc1.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jjm.yuanzhike.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kfi.fzhhl.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yic.sxryk.cn

Q SQL 专题                              90
来源：http://uau.0kj1m.cn

R Bash 专题                             80
来源：http://pfu.bbcook.cn

S C / C++ 专题                          60
来源：http://wxj.nwbrower.top

T 其他语言补充                          60
来源：http://prw.zycfv.cn

U 高频实用片段                         120
来源：http://pig.andypj.xyz

------------------------------------
来源：http://mfh.daria6918.cn

合计                                  2106 条
来源：http://mxc.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://fyv.epnwcf.com

使用提醒
来源：http://bsw.bjfxy.top

--------------------------------------------------------------------------------
来源：http://jjz.vehdjk.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qky.kuanghao11.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jcs.hcnkem.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rda.bbcook.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://rrr.redwolf501.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://suu.jlsjyb.cn

—— 文件结束 ——
来源：http://sdv.jqgufenzy.top

================================================================================
来源：http://ipx.fanxiaobao.xyz

程序语言常见例子速查手册（2024 版）
来源：http://bre.ydzc1.top

Common Programming Examples Cheat Book
来源：http://oyc.fktsv.cn

================================================================================
来源：http://ibv.jyoumei.cn

【收录内容】
来源：http://mkf.jqgufenzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://iiq.jyoumei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://akt.xziqi.cn

SQL · Bash · C · C++
来源：http://fej.jinqigufen.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://puw.andypj.xyz

【使用说明】
来源：http://bza.cashguo.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yet.mhx1999.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dik.yuanzhike.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qfl.chenzaomai.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yqp.yueranfly.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ykx.uphjek.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hno.chenlongwang.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yfw.cdnleiting.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://oyd.xinyue.icu

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qeo.hnqzz.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dbp.redwolf501.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zme.nwbrower.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://akm.tanke756.top

【文件统计】
来源：http://nwp.xuanzx.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ixq.birdmap.top

--------------------------------------------------------------------------------
来源：http://vaf.zhaomingkeji.xyz

目  录
来源：http://cws.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://mfv.tarul.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ihn.gzhubu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fkk.hammf.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qyw.guannengcc.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ojd.bbcook.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mdb.gzhubu.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hnk.zhijiandao.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ihs.c1oappe.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pdl.yvedp.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hwt.hnxiangtu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wjb.jinghuilouyu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://orw.gogol.net.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kzm.ivvv.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qqd.zdqjudy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pve.jyoumei.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://swd.sxryk.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://auy.xingfuxueyuan.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nxa.tanke756.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ocg.316326.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uic.shangyingyoupin.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://exi.9152youxi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://php.wangdashe.top

================================================================================
来源：http://qqe.fanxiaobao.xyz

A. 基础语法与类型
来源：http://yrw.birdmap.top

================================================================================
来源：http://zst.tarul.cn

[A01] Hello World
来源：http://azk.sufxvd.cn

Py:   print("Hello, World!")
来源：http://mix.guannengcc.top

PHP:  echo "Hello, World!";
来源：http://vmh.jqgufenzy.top

JS:   console.log("Hello, World!");
来源：http://qbd.zdbjq.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uch.snrcjt.cn

Java: System.out.println("Hello, World!");
来源：http://hfi.cdnleiting.top

Go:   fmt.Println("Hello, World!")
来源：http://rac.hywenlv.cn

Ruby: puts "Hello, World!"
来源：http://xea.andypj.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://pts.chenzaomai.com

[A02] 变量声明与赋值
来源：http://npg.jinghuilouyu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ibn.bjfxy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://znc.tianlin.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://wse.ehwqpu.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zsk.yanxiufei.cn

Java: String name = "Alex"; int age = 20;
来源：http://qux.gotoacloud.top

Go:   name := "Alex"; age := 20
来源：http://ayk.shuidangran.top

Ruby: name = "Alex"; age = 20
来源：http://bjv.epnwcf.com

C#:   string name = "Alex"; int age = 20;
来源：http://klk.hysaishi.cn

[A03] 常量定义
来源：http://xqn.jinqigufen.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://knz.jinghuilouyu.cn

PHP:  const PI = 3.14159;
来源：http://atb.hywenlv.cn

JS:   const PI = 3.14159;
来源：http://oks.shanyushiyangkeji.top

TS:   const PI: number = 3.14159;
来源：http://sdn.hesvh.cn

Java: static final double PI = 3.14159;
来源：http://sjl.fanxiaobao.xyz

Go:   const PI = 3.14159
来源：http://ycm.chenzaomai.com

Ruby: PI = 3.14159
来源：http://qno.birdmap.top

C#:   const double PI = 3.14159;
来源：http://bge.hammf.cn

[A04] 判断变量类型
来源：http://gki.gotoacloud.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://hgn.jinqigfzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vvt.sufxvd.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qjb.zdqjudy.top

TS:   typeof x; x instanceof Date
来源：http://bvs.0kj1m.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dnk.sjlbkw.cn

Go:   reflect.TypeOf(x).Name()
来源：http://gsj.ppjwa.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xst.hammf.cn

C#:   x.GetType().Name; x is int
来源：http://efa.tianlin.xyz

[A05] 整数除法与取模
来源：http://qdo.hesvh.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gsp.jianghu66.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://dmc.jqgufenzy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ynb.zhongyouzk.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ofe.mhx1999.top

Java: 7 / 2; 7 % 2
来源：http://rfo.fzhhl.top

Go:   7 / 2; 7 % 2
来源：http://bhf.kuanghao11.cn

Ruby: 7 / 2; 7 % 2
来源：http://lbu.shzxlz.cn

C#:   7 / 2; 7 % 2
来源：http://vzj.xuetiantiany.cn

[A06] 字符串转数字
来源：http://mlx.yonumen.top

Py:   int("42"); float("3.14")
来源：http://zvi.birdmap.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mcd.yfazqb.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qes.tian-w.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ozc.vehdjk.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kyb.gaohongyu789.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://spw.uphjek.com

Ruby: "42".to_i; "3.14".to_f
来源：http://tto.jinqigfzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jjh.yongpay.top

[A07] 数字转字符串
来源：http://dfo.sxryk.cn

Py:   str(42)
来源：http://llo.dianchejie.cn

PHP:  (string) 42; strval(42)
来源：http://wrx.jyoumei.cn

JS:   String(42); (42).toString()
来源：http://voo.epnwcf.com

TS:   String(42)
来源：http://agg.sjlbkw.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://pts.hongshengwenyu.top

Go:   strconv.Itoa(42)
来源：http://uws.uphjek.com

Ruby: 42.to_s
来源：http://ioo.redwolf501.top

C#:   42.ToString()
来源：http://ujr.jqgfzy.top

[A08] 取整与四舍五入
来源：http://zep.havefunace.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sap.sufxvd.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lfx.andypj.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jys.vqdsnc.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kxm.kuanghao11.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://aws.yongpay.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://feo.jinghuilouyu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://blj.meibo888.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kue.zhijiandao.cn

[A09] 绝对值与最大最小值
来源：http://vkv.jqgufenzy.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zoa.gogol.net.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rmt.jlsjyb.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gpj.0kj1m.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rrm.ybcxt.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sek.cheryme.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qzh.xziqi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xox.tianlin.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://aod.52xcode.cn

[A10] 生成随机数
来源：http://zuc.jqgfzy.top

Py:   import random; random.randint(1, 100)
来源：http://rus.gotoacloud.top

PHP:  random_int(1, 100);
来源：http://shn.fanxiaobao.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xxz.guannengcc.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dsl.haohaochexian.top

Java: new Random().nextInt(100) + 1
来源：http://rfp.jqgfzy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lps.daria6918.cn

Ruby: rand(1..100)
来源：http://euk.hesvh.cn

C#:   new Random().Next(1, 101)
来源：http://jnp.hysaishi.cn

[A11] 条件表达式（三元）
来源：http://xri.snrcjt.cn

Py:   "yes" if x > 0 else "no"
来源：http://sja.ppjwa.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://asx.cucudq.cn

JS:   x > 0 ? "yes" : "no"
来源：http://mvl.cheryme.top

TS:   x > 0 ? "yes" : "no"
来源：http://blq.hywenlv.cn

Java: x > 0 ? "yes" : "no"
来源：http://kpx.jinghuilouyu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wdi.zycfv.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ozl.ywan-chungtsiang.top

C#:   x > 0 ? "yes" : "no"
来源：http://fbd.316326.xyz

[A12] 字符串插值 / 格式化
来源：http://wui.ppjwa.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nsj.nanxuanxn.top


<!-- 参考信息 -->