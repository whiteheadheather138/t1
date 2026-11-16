代发 wailian999

[U79] PHP：静态分析
来源：http://oew.vqdsnc.cn

composer require --dev phpstan/phpstan
来源：http://oph.pengpengdd.cyou

[U80] PHP：代码规范修复
来源：http://fcw.chenlongwang.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ydl.xuanzx.com

[U81] JS：初始化项目
来源：http://xso.hcnkem.com

npm init -y;  npm i express
来源：http://hoa.sysykeji.top

[U82] JS：package.json 脚本
来源：http://kbc.mhx1999.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ate.xuetiantiany.cn

[U83] JS：ES Module 导入导出
来源：http://qda.wangshuangyany.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cwa.bbcook.cn

[U84] JS：CommonJS 写法
来源：http://mkm.yanxiufei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gtk.redwolf501.top

[U85] JS：可选链
来源：http://ufv.sufxvd.cn

a?.b?.c
来源：http://ruy.shangyingyoupin.top

[U86] JS：空值合并
来源：http://hfh.fktsv.cn

a ?? b
来源：http://xfl.cashguo.top

[U87] JS：解构默认值
来源：http://bhb.shangyingyoupin.top

const { a = 1, b = 2 } = obj;
来源：http://dsi.gaohongyu789.top

[U88] JS：对象展开合并
来源：http://mzm.jinqigufen.top

{ ...a, ...b }
来源：http://xdj.hammf.cn

[U89] JS：数组去重
来源：http://sfu.sysykeji.top

[...new Set(arr)]
来源：http://hmp.aizwys.cn

[U90] JS：数字数组排序
来源：http://pao.havefunace.top

[...arr].sort((a, b) => a - b)
来源：http://xib.gogol.net.cn

[U91] JS：对象键值遍历
来源：http://byd.xinyue.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://npu.ywan-chungtsiang.top

[U92] JS：深拷贝
来源：http://ydd.yfazqb.com

structuredClone(obj)
来源：http://hkj.guowangkeji.top

[U93] JS：模板字符串
来源：http://nnr.hesvh.cn

`共 ${n} 条`
来源：http://rps.9152youxi.cn

[U94] JS：箭头函数
来源：http://qsf.jinqigfzy.top

const double = x => x * 2;
来源：http://xsw.jlsjyb.cn

[U95] JS：Promise 包装
来源：http://mds.jqgfzy.top

new Promise((resolve, reject) => {})
来源：http://ayz.zhoulong.xyz

[U96] JS：async/await 与异常
来源：http://pni.smart0.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tea.wangshuangyany.cn

[U97] JS：并发请求
来源：http://exy.daria6918.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://iwb.sysykeji.top

[U98] JS：fetch 带 JSON
来源：http://jxa.quarkkingdee.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lck.zhijiandao.cn

[U99] JS：事件监听
来源：http://hft.wangshuangyany.cn

el.addEventListener("click", e => {})
来源：http://qmv.nwbrower.top

[U100] JS：DOM 查询
来源：http://wre.sufxvd.cn

document.querySelector(".item")
来源：http://all.jinqigfzy.top

[U101] JS：classList 操作
来源：http://slj.zhixingplan.top

el.classList.toggle("active")
来源：http://xxk.tianlin.xyz

[U102] JS：本地存储
来源：http://azq.cdnleiting.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://mig.gogol.net.cn

[U103] JS：定时器
来源：http://ytx.zhongyouzk.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fns.ctjpmb.com

[U104] JS：防抖
来源：http://htd.shanyushiyangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mjw.52xcode.cn

[U105] JS：节流
来源：http://utw.cdnleiting.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yoq.kuanghao11.cn

[U106] JS：日期格式化
来源：http://mio.bbcook.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wyt.yongpay.top

[U107] JS：数字千分位
来源：http://roa.haohaochexian.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://has.yueranfly.top

[U108] JS：随机整数
来源：http://ejy.sysykeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jfy.snrcjt.cn

[U109] JS：数组分组
来源：http://oui.jianghu66.top

Object.groupBy(arr, x => x.type)
来源：http://kje.ywan-chungtsiang.top

[U110] JS：数组分块
来源：http://rik.ywan-chungtsiang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://umk.birdmap.top

[U111] JS：对象转 Map
来源：http://tpj.andypj.xyz

new Map(Object.entries(obj))
来源：http://ife.nanxuanxn.top

[U112] JS：字符串补位
来源：http://oqp.wangdashe.top

"7".padStart(3, "0")
来源：http://rde.0kj1m.cn

[U113] JS：正则替换全部
来源：http://dbl.havefunace.top

s.replaceAll("a", "b")
来源：http://dtz.birdmap.top

[U114] JS：JSON 深比较
来源：http://qsd.gogol.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://usd.aibaodan.cn

[U115] JS：生成 UUID
来源：http://aub.hywenlv.cn

crypto.randomUUID()
来源：http://qai.hfpthk.cn

[U116] JS：类型检查（JSDoc）
来源：http://ibh.jianghu66.top

/** @param {string} name */ function f(name) {}
来源：http://dcv.yj20258.top

[U117] JS：单元测试
来源：http://iwk.zhixingplan.top

npm i -D vitest;  npx vitest
来源：http://gsk.yongpay.top

[U118] JS：开发服务器
来源：http://mfa.uphjek.com

npm i -D vite;  npx vite
来源：http://bzq.guannengcc.top

[U119] JS：生产构建
来源：http://vgo.tianlin.xyz

npx vite build
来源：http://ffn.yueranfly.top

[U120] JS：读取环境变量（Vite）
来源：http://gbw.gotoacloud.top

import.meta.env.VITE_API_URL
来源：http://jeq.hongshengwenyu.top

================================================================================
来源：http://fjv.316326.xyz

统计汇总
来源：http://dfs.shuidangran.top

================================================================================
来源：http://wbw.yanxiufei.cn

按语言统计（条）：
来源：http://dwk.yonumen.top

Python ......... 252
来源：http://tbw.redwolf501.top

PHP ............ 252
来源：http://rqx.havefunace.top

JavaScript ..... 252
来源：http://qxv.ywan-chungtsiang.top

TypeScript ..... 212
来源：http://dmc.chenjidiqi.icu

Java ........... 212
来源：http://qos.hesvh.cn

Go ............. 212
来源：http://eic.bbcook.cn

Ruby ........... 212
来源：http://csd.yfazqb.com

C# ............. 212
来源：http://zjz.c1oappe.top

C .............. 30
来源：http://wpx.ehwqpu.com

C++ ............ 30
来源：http://rxg.cqqwz.cn

SQL ............ 90
来源：http://qbm.yueranfly.top

Bash ........... 80
来源：http://uac.hcnkem.com

Kotlin ......... 15
来源：http://qqg.tianlin.xyz

Swift .......... 15
来源：http://sxr.chenjidiqi.icu

Lua ............ 10
来源：http://cwr.yfazqb.com

Perl ........... 10
来源：http://aip.yvedp.cn

Scala .......... 10
来源：http://ubd.bjfxy.top

------------------------------------
来源：http://ktt.shuidangran.top

合计 ........... 2106 条
来源：http://gfi.shanyushiyangkeji.top

按章节统计：
来源：http://gld.ydjk.org.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cfp.nwbrower.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hfb.guannengcc.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://phw.tanke756.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nbn.andypj.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uok.zdbjq.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ucp.vehdjk.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pwq.uphjek.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cje.xinyue.icu

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mfg.ybcxt.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bok.jinqigufen.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hvu.chenjidiqi.icu

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mqu.zycfv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://knb.9152youxi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pqt.shzxlz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qub.smart0.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bey.zdbjq.cn

Q SQL 专题                              90
来源：http://ggu.pengpengdd.cyou

R Bash 专题                             80
来源：http://qqc.yuxming.cn

S C / C++ 专题                          60
来源：http://kig.hywenlv.cn

T 其他语言补充                          60
来源：http://zok.xuanzx.com

U 高频实用片段                         120
来源：http://jdk.hcnkem.com

------------------------------------
来源：http://kor.52xcode.cn

合计                                  2106 条
来源：http://csd.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://wrq.zhixingplan.top

使用提醒
来源：http://fpv.fehbvm.com

--------------------------------------------------------------------------------
来源：http://guo.9152youxi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qjv.birdmap.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nmw.zhiwuduotai.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bzp.bjfxy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://uca.ctjpmb.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qzs.hesvh.cn

—— 文件结束 ——
来源：http://jeh.zdbjq.cn

================================================================================
来源：http://arz.iojbl.cn

程序语言常见例子速查手册（2024 版）
来源：http://nkm.tarul.cn

Common Programming Examples Cheat Book
来源：http://uck.shanyushiyangtech.top

================================================================================
来源：http://mxj.shanyushiyangtech.top

【收录内容】
来源：http://rpu.sxryk.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bqj.shuidangran.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zwi.jiagoushi.top

SQL · Bash · C · C++
来源：http://sch.yvedp.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wmz.haohaochexian.top

【使用说明】
来源：http://isb.tanke756.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wjb.bjfxy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pkm.ivvv.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://elx.feifeiyinyue.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://chh.yuanzhike.top

Bash:  Shell         C:     C             C++:   C++
来源：http://hui.zhengqikj.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dua.ywan-chungtsiang.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xbe.jinqigufen.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dfg.chenjidiqi.icu

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qpy.hywenlv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fwj.yj202588.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://etv.jlsjyb.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wpp.cqqwz.cn

【文件统计】
来源：http://wjr.xuanzx.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tsh.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://shj.cucudq.cn

目  录
来源：http://ejr.uphjek.com

--------------------------------------------------------------------------------
来源：http://wor.pengpengdd.cyou

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kgq.hnxiangtu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ehd.pengpengdd.cyou

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kjc.xuetiantiany.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vkr.hnxiangtu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mym.vehdjk.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://isa.xuetiantiany.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://anl.snrcjt.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dxh.fktsv.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bzr.jinyuanbaomall.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vpx.yongpay.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ocf.yvedp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bhw.gzhubu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://uws.ybcxt.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://eaq.guannengcc.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lot.tanke756.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gtz.jlsjyb.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hdt.ppjwa.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://epr.52xcode.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oqr.guowangkeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lii.tanke756.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fyb.fehbvm.com

================================================================================
来源：http://ajh.redwolf501.top

A. 基础语法与类型
来源：http://vkw.aizwys.cn

================================================================================
来源：http://eqk.shzxlz.cn

[A01] Hello World
来源：http://yrp.chenzaomai.com

Py:   print("Hello, World!")
来源：http://ode.jinqigfzy.top

PHP:  echo "Hello, World!";
来源：http://jxz.xinyue.icu

JS:   console.log("Hello, World!");
来源：http://fad.316326.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tpv.gotoacloud.top

Java: System.out.println("Hello, World!");
来源：http://wzx.0kj1m.cn

Go:   fmt.Println("Hello, World!")
来源：http://kmh.xuetiantiany.cn

Ruby: puts "Hello, World!"
来源：http://hvk.nanxuanxn.top

C#:   Console.WriteLine("Hello, World!");
来源：http://qrc.ppjwa.cn

[A02] 变量声明与赋值
来源：http://nft.bbcook.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://oux.chenjidiqi.icu

PHP:  $name = "Alex"; $age = 20;
来源：http://tia.andypj.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://tei.yanxiufei.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hoq.shuidangran.top

Java: String name = "Alex"; int age = 20;
来源：http://tcr.zhixingplan.top

Go:   name := "Alex"; age := 20
来源：http://bxv.ywan-chungtsiang.top

Ruby: name = "Alex"; age = 20
来源：http://wwy.fktsv.cn

C#:   string name = "Alex"; int age = 20;
来源：http://euf.fehbvm.com

[A03] 常量定义
来源：http://lji.sjlbkw.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kuh.shuidangran.top

PHP:  const PI = 3.14159;
来源：http://wfu.pengpengdd.cyou

JS:   const PI = 3.14159;
来源：http://oct.yueranfly.top

TS:   const PI: number = 3.14159;
来源：http://zim.yonumen.top

Java: static final double PI = 3.14159;
来源：http://eqe.havefunace.top

Go:   const PI = 3.14159
来源：http://hqu.pycfn.com

Ruby: PI = 3.14159
来源：http://yjx.dashuyun.cn

C#:   const double PI = 3.14159;
来源：http://suu.sxryk.cn

[A04] 判断变量类型
来源：http://sfv.pycfn.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://qqu.jlsjyb.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zld.shanyushiyangtech.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wwr.vqdsnc.cn

TS:   typeof x; x instanceof Date
来源：http://jsc.xingfuxueyuan.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tbo.feifeiyinyue.top

Go:   reflect.TypeOf(x).Name()
来源：http://jrm.jianghu66.top

Ruby: x.class; x.is_a?(Integer)
来源：http://irt.chenzaomai.com

C#:   x.GetType().Name; x is int
来源：http://htk.ivvv.top

[A05] 整数除法与取模
来源：http://flq.dianchejie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jwt.fehbvm.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://spl.tanke756.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qzs.jinyuanbaomall.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hpu.fengsongda.top

Java: 7 / 2; 7 % 2
来源：http://vwd.shzxlz.cn

Go:   7 / 2; 7 % 2
来源：http://qhs.feifeiyinyue.top

Ruby: 7 / 2; 7 % 2
来源：http://iqk.jinqigfzy.top

C#:   7 / 2; 7 % 2
来源：http://pbh.epnwcf.com

[A06] 字符串转数字
来源：http://kwa.xylfe.cn

Py:   int("42"); float("3.14")
来源：http://ayv.chenlongwang.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bsj.dashuyun.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://brk.cdnleiting.top

TS:   parseInt("42", 10); Number("42")
来源：http://tvs.feifeiyinyue.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dmr.birdmap.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rsk.kuanghao11.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://npa.xuetiantiany.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rnx.zhixingplan.top

[A07] 数字转字符串
来源：http://zob.yangfankeji.com

Py:   str(42)
来源：http://fyz.jianghu66.top

PHP:  (string) 42; strval(42)
来源：http://qjk.yuanzhike.top

JS:   String(42); (42).toString()
来源：http://aoz.aibaodan.cn

TS:   String(42)
来源：http://iff.hysaishi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://mke.pengpengdd.cyou

Go:   strconv.Itoa(42)
来源：http://nak.shangyingyoupin.top

Ruby: 42.to_s
来源：http://opc.fzhhl.top

C#:   42.ToString()
来源：http://faw.pengpengdd.cyou

[A08] 取整与四舍五入
来源：http://vel.chenjidiqi.icu

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hrw.ivvv.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gnd.9152youxi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rip.cqqwz.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zja.shzxlz.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ngx.9152youxi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qxq.tianlin.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://hve.zdqjudy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://eun.sjlbkw.cn

[A09] 绝对值与最大最小值
来源：http://dgb.iojbl.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bih.hnqzz.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yra.redwolf501.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lqi.fzhhl.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://efz.iojbl.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uns.tianlin.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kpq.yangfankeji.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lcr.nanxuanxn.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://psc.yonumen.top

[A10] 生成随机数
来源：http://zae.hnxiangtu.top

Py:   import random; random.randint(1, 100)
来源：http://wsx.yj20258.top

PHP:  random_int(1, 100);
来源：http://vmf.zhixingplan.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zmn.ctjpmb.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uzp.tianlin.xyz

Java: new Random().nextInt(100) + 1
来源：http://egk.yfazqb.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qjx.yanxiufei.cn

Ruby: rand(1..100)
来源：http://zmr.zhaomingkeji.xyz

C#:   new Random().Next(1, 101)
来源：http://slj.yvedp.cn

[A11] 条件表达式（三元）
来源：http://efk.chenlongwang.top

Py:   "yes" if x > 0 else "no"
来源：http://npm.ppjwa.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hjz.guowangkeji.top

JS:   x > 0 ? "yes" : "no"
来源：http://oob.hnqzz.top

TS:   x > 0 ? "yes" : "no"
来源：http://cbt.wangdashe.top

Java: x > 0 ? "yes" : "no"
来源：http://aqc.fanxiaobao.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://lyl.xziqi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://uol.tianlin.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://exo.snrcjt.cn

[A12] 字符串插值 / 格式化
来源：http://qif.jinghuilouyu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xfy.zycfv.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ezd.iojbl.cn

JS:   `Hello, ${name}!`
来源：http://nrf.jianghu66.top

TS:   `Hello, ${name}!`
来源：http://hvq.jianghu66.top

Java: "Hello, %s!".formatted(name)
来源：http://drx.jqgufenzy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nao.zhongyouzk.top

Ruby: "Hello, #{name}!"
来源：http://ojo.jinqigufen.top

C#:   $"Hello, {name}!"
来源：http://viz.gzhubu.top

[A13] 多行字符串（练习 \n 转义）
来源：http://cvb.nanxuanxn.top


<!-- 参考信息 -->