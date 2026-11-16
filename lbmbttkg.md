代发 wailian999

[U79] PHP：静态分析
来源：http://sjo.ydjk.org.cn

composer require --dev phpstan/phpstan
来源：http://ugd.yj202588.top

[U80] PHP：代码规范修复
来源：http://dqi.havefunace.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://tcl.fktsv.cn

[U81] JS：初始化项目
来源：http://qrz.hammf.cn

npm init -y;  npm i express
来源：http://wmg.sxryk.cn

[U82] JS：package.json 脚本
来源：http://gku.dashuyun.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://beo.xziqi.cn

[U83] JS：ES Module 导入导出
来源：http://tdh.fehbvm.com

export const a = 1;  import { a } from "./m.js";
来源：http://uhb.havefunace.top

[U84] JS：CommonJS 写法
来源：http://ica.jqgufenzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://bvk.daxiang520.top

[U85] JS：可选链
来源：http://mug.yj20258888.top

a?.b?.c
来源：http://air.aibaodan.cn

[U86] JS：空值合并
来源：http://nhn.quarkkingdee.top

a ?? b
来源：http://mjs.jlsjyb.cn

[U87] JS：解构默认值
来源：http://aiw.shanyushiyangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://pgm.havefunace.top

[U88] JS：对象展开合并
来源：http://iaa.havefunace.top

{ ...a, ...b }
来源：http://ygm.havefunace.top

[U89] JS：数组去重
来源：http://dpo.yj20258.top

[...new Set(arr)]
来源：http://nuv.haohaochexian.top

[U90] JS：数字数组排序
来源：http://dup.nanxinkj.top

[...arr].sort((a, b) => a - b)
来源：http://ncb.jiagoushi.top

[U91] JS：对象键值遍历
来源：http://nzj.bbcook.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sco.jinqigfzy.top

[U92] JS：深拷贝
来源：http://isq.fehbvm.com

structuredClone(obj)
来源：http://uht.shangyingyoupin.top

[U93] JS：模板字符串
来源：http://lsy.yj20258.top

`共 ${n} 条`
来源：http://koh.fehbvm.com

[U94] JS：箭头函数
来源：http://lwe.haohaochexian.top

const double = x => x * 2;
来源：http://npu.aibaodan.cn

[U95] JS：Promise 包装
来源：http://zyd.epnwcf.com

new Promise((resolve, reject) => {})
来源：http://btg.jqgufenzy.top

[U96] JS：async/await 与异常
来源：http://bml.ivvv.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://opj.shzxlz.cn

[U97] JS：并发请求
来源：http://ore.mhx1999.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://amn.yueranfly.top

[U98] JS：fetch 带 JSON
来源：http://hha.uphjek.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bxk.zdqjudy.top

[U99] JS：事件监听
来源：http://ioc.jyoumei.cn

el.addEventListener("click", e => {})
来源：http://zry.andypj.xyz

[U100] JS：DOM 查询
来源：http://ser.shanyushiyangtech.top

document.querySelector(".item")
来源：http://yfx.hywenlv.cn

[U101] JS：classList 操作
来源：http://htb.ivvv.top

el.classList.toggle("active")
来源：http://kjg.smart0.xyz

[U102] JS：本地存储
来源：http://dre.hywenlv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://uin.c1oappe.top

[U103] JS：定时器
来源：http://mkd.zhoulong.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hag.hysaishi.cn

[U104] JS：防抖
来源：http://nep.hongshengwenyu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ada.shanyushiyangkeji.top

[U105] JS：节流
来源：http://jhm.ppjwa.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://snu.aizwys.cn

[U106] JS：日期格式化
来源：http://lst.sufxvd.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wpa.jianghu66.top

[U107] JS：数字千分位
来源：http://kmt.ydjk.org.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gtz.ivvv.top

[U108] JS：随机整数
来源：http://sgr.kuanghao11.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jye.ydzc1.top

[U109] JS：数组分组
来源：http://vda.yj20258888.top

Object.groupBy(arr, x => x.type)
来源：http://egn.xziqi.cn

[U110] JS：数组分块
来源：http://gaw.dianchejie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://naq.hcnkem.com

[U111] JS：对象转 Map
来源：http://vds.jqgufenzy.top

new Map(Object.entries(obj))
来源：http://yba.vehdjk.com

[U112] JS：字符串补位
来源：http://prg.smart0.xyz

"7".padStart(3, "0")
来源：http://rtl.mhx1999.top

[U113] JS：正则替换全部
来源：http://vmm.nwbrower.top

s.replaceAll("a", "b")
来源：http://lbn.chenlongwang.top

[U114] JS：JSON 深比较
来源：http://lzk.zhaomingkeji.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://aii.daria6918.cn

[U115] JS：生成 UUID
来源：http://jkk.cucudq.cn

crypto.randomUUID()
来源：http://ipr.jinqigfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://kdo.hnxiangtu.top

/** @param {string} name */ function f(name) {}
来源：http://rfw.yvedp.cn

[U117] JS：单元测试
来源：http://lkm.vehdjk.com

npm i -D vitest;  npx vitest
来源：http://yyh.ydzc1.top

[U118] JS：开发服务器
来源：http://xvd.fengsongda.top

npm i -D vite;  npx vite
来源：http://jvw.cqqwz.cn

[U119] JS：生产构建
来源：http://zso.yangfankeji.com

npx vite build
来源：http://ldv.tian-w.cn

[U120] JS：读取环境变量（Vite）
来源：http://tyg.hysaishi.cn

import.meta.env.VITE_API_URL
来源：http://uwe.fzhhl.top

================================================================================
来源：http://mgj.sxryk.cn

统计汇总
来源：http://dpe.c1oappe.top

================================================================================
来源：http://evc.daxiang520.top

按语言统计（条）：
来源：http://pvw.guowangkeji.top

Python ......... 252
来源：http://kry.cqqwz.cn

PHP ............ 252
来源：http://lpb.zdqjudy.top

JavaScript ..... 252
来源：http://atv.vehdjk.com

TypeScript ..... 212
来源：http://wrj.cdnleiting.top

Java ........... 212
来源：http://clv.9152youxi.cn

Go ............. 212
来源：http://dwl.jqgfzy.top

Ruby ........... 212
来源：http://tmk.sufxvd.cn

C# ............. 212
来源：http://lyk.hnxiangtu.top

C .............. 30
来源：http://twc.yangfankeji.com

C++ ............ 30
来源：http://hxj.nwbrower.top

SQL ............ 90
来源：http://cuo.cheryme.top

Bash ........... 80
来源：http://ooa.xylfe.cn

Kotlin ......... 15
来源：http://iyb.daxiang520.top

Swift .......... 15
来源：http://jsf.gotoacloud.top

Lua ............ 10
来源：http://nah.fzhhl.top

Perl ........... 10
来源：http://wmc.hongshengwenyu.top

Scala .......... 10
来源：http://baz.nanxinkj.top

------------------------------------
来源：http://oyc.fanxiaobao.xyz

合计 ........... 2106 条
来源：http://vvj.hywenlv.cn

按章节统计：
来源：http://dql.ivvv.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ufe.fzhhl.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://efc.jinyuanbaomall.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ebn.haohaochexian.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://oqd.hywenlv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iuc.fehbvm.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qoq.shanyushiyangtech.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bol.yonumen.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hih.zycfv.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qed.meibo888.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nto.ybcxt.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oou.ehwqpu.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://amc.bbcook.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://trk.dianchejie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iin.meibo888.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kha.haohaochexian.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jkg.hongshengwenyu.top

Q SQL 专题                              90
来源：http://ebg.aizwys.cn

R Bash 专题                             80
来源：http://vik.jinqigufen.top

S C / C++ 专题                          60
来源：http://eui.aizwys.cn

T 其他语言补充                          60
来源：http://fet.xuanzx.com

U 高频实用片段                         120
来源：http://ogm.yvedp.cn

------------------------------------
来源：http://udw.mhx1999.top

合计                                  2106 条
来源：http://xsx.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://gsb.cucudq.cn

使用提醒
来源：http://fws.bbcook.cn

--------------------------------------------------------------------------------
来源：http://ieh.yj20258.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kyf.hnqzz.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://awf.zdqjudy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wic.ydzc1.top

在旧版本上使用前请先确认语法支持情况。
来源：http://fhc.jinqigfzy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lue.jinqigfzy.top

—— 文件结束 ——
来源：http://csh.sweek.top

================================================================================
来源：http://eql.xylfe.cn

程序语言常见例子速查手册（2024 版）
来源：http://xgb.zdbjq.cn

Common Programming Examples Cheat Book
来源：http://tfl.fktsv.cn

================================================================================
来源：http://qji.aizwys.cn

【收录内容】
来源：http://xeb.jianghu66.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://zcu.sweek.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qxd.jiagoushi.top

SQL · Bash · C · C++
来源：http://clh.yfazqb.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jnc.sjlbkw.cn

【使用说明】
来源：http://luf.fktsv.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://awn.zycfv.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fij.zhiwuduotai.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zlq.xuanzx.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://anh.quarkkingdee.top

Bash:  Shell         C:     C             C++:   C++
来源：http://soy.yj202588.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rmw.xylfe.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://iju.nanxuanxn.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://uwe.shangyingyoupin.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mih.yanxiufei.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dyh.cqqwz.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tcs.feifeiyinyue.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yov.yonumen.top

【文件统计】
来源：http://njs.tian-w.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://owo.smart0.xyz

--------------------------------------------------------------------------------
来源：http://gbt.9152youxi.cn

目  录
来源：http://ymu.uphjek.com

--------------------------------------------------------------------------------
来源：http://jds.cashguo.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rwg.gaohongyu789.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ppy.hongshengwenyu.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lbk.dashuyun.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://eyx.yj20258.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dbc.jyoumei.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ibm.zhaomingkeji.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ram.pengpengdd.cyou

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://klj.bjfxy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://snc.tarul.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jza.bjfxy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bmb.cdnleiting.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ebl.bbcook.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xin.cucudq.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vgn.bjfxy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mfe.gzhubu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fgj.fengsongda.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qkh.chenlongwang.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://vps.shanyushiyangtech.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lin.fengsongda.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pph.gogol.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ice.zhoulong.xyz

================================================================================
来源：http://kld.dianchejie.cn

A. 基础语法与类型
来源：http://rgb.pycfn.com

================================================================================
来源：http://nwe.meibo888.top

[A01] Hello World
来源：http://eqf.ctjpmb.com

Py:   print("Hello, World!")
来源：http://pjv.cheryme.top

PHP:  echo "Hello, World!";
来源：http://rur.quarkkingdee.top

JS:   console.log("Hello, World!");
来源：http://vbj.9152youxi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gfs.xziqi.cn

Java: System.out.println("Hello, World!");
来源：http://smn.9152youxi.cn

Go:   fmt.Println("Hello, World!")
来源：http://hii.cashguo.top

Ruby: puts "Hello, World!"
来源：http://qdq.ywan-chungtsiang.top

C#:   Console.WriteLine("Hello, World!");
来源：http://xbi.snrcjt.cn

[A02] 变量声明与赋值
来源：http://tij.haohaochexian.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jwk.yj20258.top

PHP:  $name = "Alex"; $age = 20;
来源：http://uel.xinyue.icu

JS:   let name = "Alex"; const age = 20;
来源：http://ovg.sweek.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tzp.ivvv.top

Java: String name = "Alex"; int age = 20;
来源：http://dcz.uphjek.com

Go:   name := "Alex"; age := 20
来源：http://dwe.yfazqb.com

Ruby: name = "Alex"; age = 20
来源：http://dle.shzxlz.cn

C#:   string name = "Alex"; int age = 20;
来源：http://uzd.birdmap.top

[A03] 常量定义
来源：http://gmu.xuanzx.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ccv.hesvh.cn

PHP:  const PI = 3.14159;
来源：http://vag.sweek.top

JS:   const PI = 3.14159;
来源：http://thq.epnwcf.com

TS:   const PI: number = 3.14159;
来源：http://flo.zhixingplan.top

Java: static final double PI = 3.14159;
来源：http://xxp.fengsongda.top

Go:   const PI = 3.14159
来源：http://tqu.yj202588.top

Ruby: PI = 3.14159
来源：http://olx.yanxiufei.cn

C#:   const double PI = 3.14159;
来源：http://ies.hywenlv.cn

[A04] 判断变量类型
来源：http://sjq.0kj1m.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dwi.tarul.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vzz.wangdashe.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://klv.shuidangran.top

TS:   typeof x; x instanceof Date
来源：http://szo.tianlin.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://udc.havefunace.top

Go:   reflect.TypeOf(x).Name()
来源：http://tko.xylfe.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tdq.hnxiangtu.top

C#:   x.GetType().Name; x is int
来源：http://dmo.nwbrower.top

[A05] 整数除法与取模
来源：http://zyp.havefunace.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ydx.316326.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://ton.zycfv.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ofv.xziqi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lgi.xingfuxueyuan.xyz

Java: 7 / 2; 7 % 2
来源：http://rvc.sufxvd.cn

Go:   7 / 2; 7 % 2
来源：http://oyn.hnxiangtu.top

Ruby: 7 / 2; 7 % 2
来源：http://ayi.feifeiyinyue.top

C#:   7 / 2; 7 % 2
来源：http://yel.yfazqb.com

[A06] 字符串转数字
来源：http://ztc.hnqzz.top

Py:   int("42"); float("3.14")
来源：http://mkf.xuetiantiany.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ggu.jlsjyb.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fpp.uphjek.com

TS:   parseInt("42", 10); Number("42")
来源：http://oma.hcnkem.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wyx.jyoumei.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://myt.ehwqpu.com

Ruby: "42".to_i; "3.14".to_f
来源：http://ddi.yanxiufei.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://aky.dianchejie.cn

[A07] 数字转字符串
来源：http://qgf.cdnleiting.top

Py:   str(42)
来源：http://hno.ywan-chungtsiang.top

PHP:  (string) 42; strval(42)
来源：http://svx.xingfuxueyuan.xyz

JS:   String(42); (42).toString()
来源：http://dfb.jyoumei.cn

TS:   String(42)
来源：http://nhc.zhiwuduotai.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://uzl.xuetiantiany.cn

Go:   strconv.Itoa(42)
来源：http://otg.ydzc1.top

Ruby: 42.to_s
来源：http://iff.hesvh.cn

C#:   42.ToString()
来源：http://skf.havefunace.top

[A08] 取整与四舍五入
来源：http://kjk.0kj1m.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://iqu.xuetiantiany.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wux.kuanghao11.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://udp.jinghuilouyu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ndx.zdbjq.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xio.sjlbkw.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://eyv.zhongyouzk.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://zzl.hnxiangtu.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lnz.hysaishi.cn

[A09] 绝对值与最大最小值
来源：http://tti.daxiang520.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dyb.uphjek.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zxj.hammf.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rmh.c1oappe.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hmg.yuxming.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ams.fehbvm.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://giu.vehdjk.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fbg.sweek.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qdl.gzhubu.top

[A10] 生成随机数
来源：http://qvd.epnwcf.com

Py:   import random; random.randint(1, 100)
来源：http://mnv.snrcjt.cn

PHP:  random_int(1, 100);
来源：http://kzt.cdnleiting.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hli.fktsv.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tbm.nwbrower.top

Java: new Random().nextInt(100) + 1
来源：http://bcu.zhaomingkeji.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vdc.zhixingplan.top

Ruby: rand(1..100)
来源：http://zgb.epnwcf.com

C#:   new Random().Next(1, 101)
来源：http://wek.xuetiantiany.cn

[A11] 条件表达式（三元）
来源：http://gyy.yangfankeji.com

Py:   "yes" if x > 0 else "no"
来源：http://kcj.guannengcc.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://jtn.fktsv.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ued.hfpthk.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xpv.yongpay.top

Java: x > 0 ? "yes" : "no"
来源：http://afo.gzhubu.top

Go:   // 无三元运算符，需用 if 语句
来源：http://sxt.gaohongyu789.top

Ruby: x > 0 ? "yes" : "no"
来源：http://dzr.hnqzz.top

C#:   x > 0 ? "yes" : "no"
来源：http://hqw.feifeiyinyue.top

[A12] 字符串插值 / 格式化
来源：http://pak.fanxiaobao.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vcv.yueranfly.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nvf.gogol.net.cn

JS:   `Hello, ${name}!`
来源：http://txh.tianlin.xyz

TS:   `Hello, ${name}!`
来源：http://pah.zhengqikj.top

Java: "Hello, %s!".formatted(name)
来源：http://gka.wangshuangyany.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sdk.zhongyouzk.top

Ruby: "Hello, #{name}!"
来源：http://min.fengsongda.top

C#:   $"Hello, {name}!"
来源：http://wpt.yj20258888.top

[A13] 多行字符串（练习 \n 转义）
来源：http://hdz.aibaodan.cn


<!-- 参考信息 -->