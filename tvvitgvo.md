代发 wailian999

[U79] PHP：静态分析
来源：http://uud.haohaochexian.top

composer require --dev phpstan/phpstan
来源：http://nuz.jinqigufen.top

[U80] PHP：代码规范修复
来源：http://kav.vqdsnc.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nsl.yueranfly.top

[U81] JS：初始化项目
来源：http://yyt.aibaodan.cn

npm init -y;  npm i express
来源：http://amr.yonumen.top

[U82] JS：package.json 脚本
来源：http://rxu.bjfxy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://clg.gogol.net.cn

[U83] JS：ES Module 导入导出
来源：http://mdv.yongpay.top

export const a = 1;  import { a } from "./m.js";
来源：http://ttk.nanxinkj.top

[U84] JS：CommonJS 写法
来源：http://qmh.yanxiufei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gtb.vehdjk.com

[U85] JS：可选链
来源：http://ogr.yuanzhike.top

a?.b?.c
来源：http://qwi.zhijiandao.cn

[U86] JS：空值合并
来源：http://eim.jinqigfzy.top

a ?? b
来源：http://cvw.tian-w.cn

[U87] JS：解构默认值
来源：http://mmm.nwbrower.top

const { a = 1, b = 2 } = obj;
来源：http://qms.gotoacloud.top

[U88] JS：对象展开合并
来源：http://msh.ivvv.top

{ ...a, ...b }
来源：http://ybj.fanxiaobao.xyz

[U89] JS：数组去重
来源：http://ahj.jinqigfzy.top

[...new Set(arr)]
来源：http://jrk.sxryk.cn

[U90] JS：数字数组排序
来源：http://tmh.nanxinkj.top

[...arr].sort((a, b) => a - b)
来源：http://jbb.yfazqb.com

[U91] JS：对象键值遍历
来源：http://azq.zhixingplan.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kha.ctjpmb.com

[U92] JS：深拷贝
来源：http://xnh.shanyushiyangtech.top

structuredClone(obj)
来源：http://kvc.fengsongda.top

[U93] JS：模板字符串
来源：http://htv.tanke756.top

`共 ${n} 条`
来源：http://vkb.gaohongyu789.top

[U94] JS：箭头函数
来源：http://gvc.zhengqikj.top

const double = x => x * 2;
来源：http://iqb.jiagoushi.top

[U95] JS：Promise 包装
来源：http://nlr.yj202588.top

new Promise((resolve, reject) => {})
来源：http://jhn.zdbjq.cn

[U96] JS：async/await 与异常
来源：http://hux.snrcjt.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hfm.jlsjyb.cn

[U97] JS：并发请求
来源：http://jdx.chenlongwang.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://hwj.shzxlz.cn

[U98] JS：fetch 带 JSON
来源：http://cel.zhiwuduotai.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ikh.zhongyouzk.top

[U99] JS：事件监听
来源：http://hla.cucudq.cn

el.addEventListener("click", e => {})
来源：http://kfu.gogol.net.cn

[U100] JS：DOM 查询
来源：http://swk.wangshuangyany.cn

document.querySelector(".item")
来源：http://edr.52xcode.cn

[U101] JS：classList 操作
来源：http://inm.ctjpmb.com

el.classList.toggle("active")
来源：http://hwo.xziqi.cn

[U102] JS：本地存储
来源：http://gkx.bjfxy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://afr.sysykeji.top

[U103] JS：定时器
来源：http://wdu.nwbrower.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kqq.zhaomingkeji.xyz

[U104] JS：防抖
来源：http://jeq.redwolf501.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://akz.zhongyouzk.top

[U105] JS：节流
来源：http://zvz.jqgufenzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://aeb.jyoumei.cn

[U106] JS：日期格式化
来源：http://qxg.gaohongyu789.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hvy.meibo888.top

[U107] JS：数字千分位
来源：http://vzo.mhx1999.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ovt.ctjpmb.com

[U108] JS：随机整数
来源：http://ahs.ybcxt.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xus.ppjwa.cn

[U109] JS：数组分组
来源：http://glm.tian-w.cn

Object.groupBy(arr, x => x.type)
来源：http://adg.xylfe.cn

[U110] JS：数组分块
来源：http://olk.nanxuanxn.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qqb.sjlbkw.cn

[U111] JS：对象转 Map
来源：http://ign.sufxvd.cn

new Map(Object.entries(obj))
来源：http://nzx.hnxiangtu.top

[U112] JS：字符串补位
来源：http://ses.yj202588.top

"7".padStart(3, "0")
来源：http://ihy.wangdashe.top

[U113] JS：正则替换全部
来源：http://mqr.cheryme.top

s.replaceAll("a", "b")
来源：http://llk.xingfuxueyuan.xyz

[U114] JS：JSON 深比较
来源：http://cok.yj20258888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jfd.xinyue.icu

[U115] JS：生成 UUID
来源：http://vps.hcnkem.com

crypto.randomUUID()
来源：http://cvj.aizwys.cn

[U116] JS：类型检查（JSDoc）
来源：http://qos.zhaomingkeji.xyz

/** @param {string} name */ function f(name) {}
来源：http://czk.zhixingplan.top

[U117] JS：单元测试
来源：http://hbe.shangyingyoupin.top

npm i -D vitest;  npx vitest
来源：http://sty.tian-w.cn

[U118] JS：开发服务器
来源：http://wsc.jinqigfzy.top

npm i -D vite;  npx vite
来源：http://wux.gaohongyu789.top

[U119] JS：生产构建
来源：http://clz.xuetiantiany.cn

npx vite build
来源：http://klz.yongpay.top

[U120] JS：读取环境变量（Vite）
来源：http://bap.dianchejie.cn

import.meta.env.VITE_API_URL
来源：http://onp.316326.xyz

================================================================================
来源：http://gyq.yongpay.top

统计汇总
来源：http://pvu.jinqigufen.top

================================================================================
来源：http://ipu.xinyue.icu

按语言统计（条）：
来源：http://hka.ctjpmb.com

Python ......... 252
来源：http://zbf.fzhhl.top

PHP ............ 252
来源：http://gad.yanxiufei.cn

JavaScript ..... 252
来源：http://pjy.hnqzz.top

TypeScript ..... 212
来源：http://rom.nanxuanxn.top

Java ........... 212
来源：http://jrh.andypj.xyz

Go ............. 212
来源：http://lje.jinqigfzy.top

Ruby ........... 212
来源：http://mvn.yangfankeji.com

C# ............. 212
来源：http://wwq.iojbl.cn

C .............. 30
来源：http://cgn.ydjk.org.cn

C++ ............ 30
来源：http://azf.mhx1999.top

SQL ............ 90
来源：http://wfd.pengpengdd.cyou

Bash ........... 80
来源：http://xcu.jinqigufen.top

Kotlin ......... 15
来源：http://vwq.yueranfly.top

Swift .......... 15
来源：http://rhi.jiagoushi.top

Lua ............ 10
来源：http://fst.hammf.cn

Perl ........... 10
来源：http://exb.yuanzhike.top

Scala .......... 10
来源：http://kwh.316326.xyz

------------------------------------
来源：http://xuf.yj20258888.top

合计 ........... 2106 条
来源：http://rrw.sweek.top

按章节统计：
来源：http://dib.tarul.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rpq.jianghu66.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://shu.havefunace.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qii.52xcode.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yfw.guowangkeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hrv.ppjwa.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wfq.hongshengwenyu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wlk.nwbrower.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bcb.wangdashe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qsx.tian-w.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://iun.fktsv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uwg.sjlbkw.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ogl.andypj.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bdc.xylfe.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rsg.nanxuanxn.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://etf.dashuyun.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nen.iojbl.cn

Q SQL 专题                              90
来源：http://kbd.meibo888.top

R Bash 专题                             80
来源：http://xza.sjlbkw.cn

S C / C++ 专题                          60
来源：http://gyr.yj20258.top

T 其他语言补充                          60
来源：http://xuu.daria6918.cn

U 高频实用片段                         120
来源：http://nmg.gogol.net.cn

------------------------------------
来源：http://xsy.jinghuilouyu.cn

合计                                  2106 条
来源：http://oih.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://gxo.redwolf501.top

使用提醒
来源：http://vug.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://vqj.quarkkingdee.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yir.aizwys.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zeg.hysaishi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kxn.zhaomingkeji.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://osc.aizwys.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hft.316326.xyz

—— 文件结束 ——
来源：http://inz.cashguo.top

================================================================================
来源：http://mij.yfazqb.com

程序语言常见例子速查手册（2024 版）
来源：http://ree.gotoacloud.top

Common Programming Examples Cheat Book
来源：http://pja.yanxiufei.cn

================================================================================
来源：http://grg.yongpay.top

【收录内容】
来源：http://gtw.xuetiantiany.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rzm.yanxiufei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ssn.shzxlz.cn

SQL · Bash · C · C++
来源：http://kii.fengsongda.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://smj.daxiang520.top

【使用说明】
来源：http://xlr.andypj.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qtb.cheryme.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://quo.cashguo.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xfl.tarul.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nne.xinyue.icu

Bash:  Shell         C:     C             C++:   C++
来源：http://son.xuanzx.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qzt.fanxiaobao.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qud.ivvv.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hcw.daria6918.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://shf.fehbvm.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rdr.ppjwa.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nbm.yvedp.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ilq.yangfankeji.com

【文件统计】
来源：http://kgp.wangshuangyany.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sjq.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://wsb.shangyingyoupin.top

目  录
来源：http://rjn.ivvv.top

--------------------------------------------------------------------------------
来源：http://utq.jinghuilouyu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mot.nwbrower.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dla.shangyingyoupin.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zvm.bbcook.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://twi.iojbl.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uen.ybcxt.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ggk.shanyushiyangkeji.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mns.wangdashe.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ahr.hongshengwenyu.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qkx.sufxvd.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wnx.ctjpmb.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://snb.sjlbkw.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zxt.xuetiantiany.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://oif.vqdsnc.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://esy.jqgufenzy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://npg.jinqigfzy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vtr.dashuyun.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://snq.vqdsnc.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://iso.chenjidiqi.icu

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sqg.jinqigufen.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://toa.xuanzx.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gvt.316326.xyz

================================================================================
来源：http://uik.dashuyun.cn

A. 基础语法与类型
来源：http://lws.vehdjk.com

================================================================================
来源：http://whu.gotoacloud.top

[A01] Hello World
来源：http://fjp.zhijiandao.cn

Py:   print("Hello, World!")
来源：http://wql.fanxiaobao.xyz

PHP:  echo "Hello, World!";
来源：http://awc.feifeiyinyue.top

JS:   console.log("Hello, World!");
来源：http://rfs.jqgufenzy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yhq.xinyue.icu

Java: System.out.println("Hello, World!");
来源：http://twk.316326.xyz

Go:   fmt.Println("Hello, World!")
来源：http://adr.zdqjudy.top

Ruby: puts "Hello, World!"
来源：http://dgn.hammf.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xxw.hongshengwenyu.top

[A02] 变量声明与赋值
来源：http://dwc.hammf.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ikg.zhengqikj.top

PHP:  $name = "Alex"; $age = 20;
来源：http://zlh.hywenlv.cn

JS:   let name = "Alex"; const age = 20;
来源：http://pao.hnqzz.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dxn.jiagoushi.top

Java: String name = "Alex"; int age = 20;
来源：http://yff.fktsv.cn

Go:   name := "Alex"; age := 20
来源：http://kht.yanxiufei.cn

Ruby: name = "Alex"; age = 20
来源：http://cqr.bjfxy.top

C#:   string name = "Alex"; int age = 20;
来源：http://gic.tarul.cn

[A03] 常量定义
来源：http://zir.vqdsnc.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://uew.ywan-chungtsiang.top

PHP:  const PI = 3.14159;
来源：http://sou.yuanzhike.top

JS:   const PI = 3.14159;
来源：http://hht.yfazqb.com

TS:   const PI: number = 3.14159;
来源：http://cjp.hysaishi.cn

Java: static final double PI = 3.14159;
来源：http://qtl.aibaodan.cn

Go:   const PI = 3.14159
来源：http://ogt.wangdashe.top

Ruby: PI = 3.14159
来源：http://qxu.ehwqpu.com

C#:   const double PI = 3.14159;
来源：http://qoj.shangyingyoupin.top

[A04] 判断变量类型
来源：http://pcu.zhiwuduotai.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://fgv.dashuyun.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ldn.316326.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zbr.aizwys.cn

TS:   typeof x; x instanceof Date
来源：http://avg.cqqwz.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kxl.fehbvm.com

Go:   reflect.TypeOf(x).Name()
来源：http://mti.yonumen.top

Ruby: x.class; x.is_a?(Integer)
来源：http://dmb.shanyushiyangkeji.top

C#:   x.GetType().Name; x is int
来源：http://gpm.jyoumei.cn

[A05] 整数除法与取模
来源：http://neg.yanxiufei.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kkf.zhengqikj.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://mkp.jinqigfzy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://uhi.havefunace.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uca.daxiang520.top

Java: 7 / 2; 7 % 2
来源：http://vmp.hcnkem.com

Go:   7 / 2; 7 % 2
来源：http://pkn.snrcjt.cn

Ruby: 7 / 2; 7 % 2
来源：http://ugv.ybcxt.top

C#:   7 / 2; 7 % 2
来源：http://ypu.tianlin.xyz

[A06] 字符串转数字
来源：http://cuk.tian-w.cn

Py:   int("42"); float("3.14")
来源：http://nsu.fanxiaobao.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tyt.guowangkeji.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wrk.wangdashe.top

TS:   parseInt("42", 10); Number("42")
来源：http://wgr.jiagoushi.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tih.sysykeji.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jlz.zhixingplan.top

Ruby: "42".to_i; "3.14".to_f
来源：http://hxx.ppjwa.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ytn.haohaochexian.top

[A07] 数字转字符串
来源：http://una.hnqzz.top

Py:   str(42)
来源：http://ygj.andypj.xyz

PHP:  (string) 42; strval(42)
来源：http://xef.hnqzz.top

JS:   String(42); (42).toString()
来源：http://wnv.cucudq.cn

TS:   String(42)
来源：http://buv.bbcook.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://npd.aibaodan.cn

Go:   strconv.Itoa(42)
来源：http://phl.wangdashe.top

Ruby: 42.to_s
来源：http://wze.fzhhl.top

C#:   42.ToString()
来源：http://bvt.meibo888.top

[A08] 取整与四舍五入
来源：http://hly.ppjwa.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://syr.jinqigfzy.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jeb.feifeiyinyue.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dzd.yanxiufei.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://khv.cdnleiting.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ozc.xinyue.icu

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jgf.birdmap.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://nur.nanxuanxn.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qaj.chenzaomai.com

[A09] 绝对值与最大最小值
来源：http://mkt.daxiang520.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://aou.quarkkingdee.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wdk.hysaishi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zah.ydzc1.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wxr.yvedp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ksn.ywan-chungtsiang.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sjo.ydzc1.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hch.daria6918.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://moo.sweek.top

[A10] 生成随机数
来源：http://lnc.sweek.top

Py:   import random; random.randint(1, 100)
来源：http://ysz.hnqzz.top

PHP:  random_int(1, 100);
来源：http://mcm.yangfankeji.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lww.yuanzhike.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tvk.jinqigufen.top

Java: new Random().nextInt(100) + 1
来源：http://ztl.gotoacloud.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bto.tian-w.cn

Ruby: rand(1..100)
来源：http://oip.chenzaomai.com

C#:   new Random().Next(1, 101)
来源：http://rqi.pengpengdd.cyou

[A11] 条件表达式（三元）
来源：http://spk.xziqi.cn

Py:   "yes" if x > 0 else "no"
来源：http://wko.xylfe.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://znc.xuanzx.com

JS:   x > 0 ? "yes" : "no"
来源：http://npz.zhaomingkeji.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://jlq.yongpay.top

Java: x > 0 ? "yes" : "no"
来源：http://cyd.nanxinkj.top

Go:   // 无三元运算符，需用 if 语句
来源：http://fwk.andypj.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://qpe.fzhhl.top

C#:   x > 0 ? "yes" : "no"
来源：http://mex.smart0.xyz

[A12] 字符串插值 / 格式化
来源：http://xae.sufxvd.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wle.pengpengdd.cyou

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lgv.feifeiyinyue.top

JS:   `Hello, ${name}!`
来源：http://hff.c1oappe.top

TS:   `Hello, ${name}!`
来源：http://sgq.smart0.xyz

Java: "Hello, %s!".formatted(name)
来源：http://wpq.dianchejie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xen.0kj1m.cn

Ruby: "Hello, #{name}!"
来源：http://ljo.iojbl.cn

C#:   $"Hello, {name}!"
来源：http://bjb.zhijiandao.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://owa.fzhhl.top


<!-- 参考信息 -->