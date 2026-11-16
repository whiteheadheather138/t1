代发 wailian999

[U89] JS：数组去重
来源：http://iun.wangshuangyany.cn

[...new Set(arr)]
来源：http://ltx.yuxming.cn

[U90] JS：数字数组排序
来源：http://lgk.zycfv.cn

[...arr].sort((a, b) => a - b)
来源：http://uzr.bjfxy.top

[U91] JS：对象键值遍历
来源：http://atv.nwbrower.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ilh.shzxlz.cn

[U92] JS：深拷贝
来源：http://ney.zhongyouzk.top

structuredClone(obj)
来源：http://prn.xingfuxueyuan.xyz

[U93] JS：模板字符串
来源：http://suk.zhongyouzk.top

`共 ${n} 条`
来源：http://fym.guowangkeji.top

[U94] JS：箭头函数
来源：http://ygu.ctjpmb.com

const double = x => x * 2;
来源：http://ips.52xcode.cn

[U95] JS：Promise 包装
来源：http://xmd.sufxvd.cn

new Promise((resolve, reject) => {})
来源：http://ycb.cdnleiting.top

[U96] JS：async/await 与异常
来源：http://ggz.jianghu66.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nxg.hesvh.cn

[U97] JS：并发请求
来源：http://hky.yuxming.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://onl.zhoulong.xyz

[U98] JS：fetch 带 JSON
来源：http://xcf.smart0.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ysx.hysaishi.cn

[U99] JS：事件监听
来源：http://boj.yuxming.cn

el.addEventListener("click", e => {})
来源：http://gok.snrcjt.cn

[U100] JS：DOM 查询
来源：http://wpd.dashuyun.cn

document.querySelector(".item")
来源：http://ozz.cdnleiting.top

[U101] JS：classList 操作
来源：http://lia.kuanghao11.cn

el.classList.toggle("active")
来源：http://bfj.chenzaomai.com

[U102] JS：本地存储
来源：http://eoy.ehwqpu.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://uob.jiagoushi.top

[U103] JS：定时器
来源：http://rci.svipenyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ujf.zhongyouzk.top

[U104] JS：防抖
来源：http://pdn.chenzaomai.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mwx.kuanghao11.cn

[U105] JS：节流
来源：http://uev.cdnleiting.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qjp.bjfxy.top

[U106] JS：日期格式化
来源：http://zpk.jinghuilouyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kke.xingfuxueyuan.xyz

[U107] JS：数字千分位
来源：http://exf.shanyushiyangtech.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://eox.shzxlz.cn

[U108] JS：随机整数
来源：http://klz.feifeiyinyue.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wcp.yj20258888.top

[U109] JS：数组分组
来源：http://lsn.jqgfzy.top

Object.groupBy(arr, x => x.type)
来源：http://bgu.hfpthk.cn

[U110] JS：数组分块
来源：http://xwf.jyoumei.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zdn.hnqzz.top

[U111] JS：对象转 Map
来源：http://zfm.0kj1m.cn

new Map(Object.entries(obj))
来源：http://vgq.jqgfzy.top

[U112] JS：字符串补位
来源：http://vmm.nwbrower.top

"7".padStart(3, "0")
来源：http://mmi.birdmap.top

[U113] JS：正则替换全部
来源：http://cbp.chenlongwang.top

s.replaceAll("a", "b")
来源：http://bzh.vqdsnc.cn

[U114] JS：JSON 深比较
来源：http://fow.yueranfly.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://yuq.daria6918.cn

[U115] JS：生成 UUID
来源：http://zwo.52xcode.cn

crypto.randomUUID()
来源：http://phh.meibo888.top

[U116] JS：类型检查（JSDoc）
来源：http://oho.kuanghao11.cn

/** @param {string} name */ function f(name) {}
来源：http://dup.wangdashe.top

[U117] JS：单元测试
来源：http://muj.hongshengwenyu.top

npm i -D vitest;  npx vitest
来源：http://tyg.ivvv.top

[U118] JS：开发服务器
来源：http://gqw.shuidangran.top

npm i -D vite;  npx vite
来源：http://aqw.hfpthk.cn

[U119] JS：生产构建
来源：http://yda.fehbvm.com

npx vite build
来源：http://qiu.fehbvm.com

[U120] JS：读取环境变量（Vite）
来源：http://iyq.guowangkeji.top

import.meta.env.VITE_API_URL
来源：http://hnv.jinyuanbaomall.cn

================================================================================
来源：http://lwo.jqgfzy.top

统计汇总
来源：http://pkm.xylfe.cn

================================================================================
来源：http://fph.haohaochexian.top

按语言统计（条）：
来源：http://jew.zhiwuduotai.top

Python ......... 252
来源：http://szz.zhoulong.xyz

PHP ............ 252
来源：http://tee.dashuyun.cn

JavaScript ..... 252
来源：http://gzw.aibaodan.cn

TypeScript ..... 212
来源：http://knd.ydjk.org.cn

Java ........... 212
来源：http://omd.hcnkem.com

Go ............. 212
来源：http://vvg.zhengqikj.top

Ruby ........... 212
来源：http://nbc.wangdashe.top

C# ............. 212
来源：http://bui.cashguo.top

C .............. 30
来源：http://pjg.vehdjk.com

C++ ............ 30
来源：http://byf.pengpengdd.cyou

SQL ............ 90
来源：http://vfq.zhaomingkeji.xyz

Bash ........... 80
来源：http://peg.jinqigfzy.top

Kotlin ......... 15
来源：http://yno.zhengqikj.top

Swift .......... 15
来源：http://kzf.hnqzz.top

Lua ............ 10
来源：http://jwf.daxiang520.top

Perl ........... 10
来源：http://pxu.smart0.xyz

Scala .......... 10
来源：http://toz.daria6918.cn

------------------------------------
来源：http://kbj.fzhhl.top

合计 ........... 2106 条
来源：http://zrh.zhaomingkeji.xyz

按章节统计：
来源：http://znp.jqgufenzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://flz.ydjk.org.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ytp.jiagoushi.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rvu.fzhhl.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cvi.shangyingyoupin.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vlo.52xcode.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://phq.c1oappe.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dyo.aizwys.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yrb.nanxinkj.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://aey.jinqigufen.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yyu.yuxming.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ktn.jqgfzy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://thy.xylfe.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tfw.bbcook.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ayo.zhijiandao.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mxw.shzxlz.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kmv.fehbvm.com

Q SQL 专题                              90
来源：http://sgk.xinyue.icu

R Bash 专题                             80
来源：http://wml.jinqigufen.top

S C / C++ 专题                          60
来源：http://gxu.nanxinkj.top

T 其他语言补充                          60
来源：http://mgq.jqgfzy.top

U 高频实用片段                         120
来源：http://nae.aibaodan.cn

------------------------------------
来源：http://nnj.xuanzx.com

合计                                  2106 条
来源：http://kqt.yj202588.top

--------------------------------------------------------------------------------
来源：http://bvq.hnqzz.top

使用提醒
来源：http://xnq.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://yxy.xinyue.icu

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xsm.xziqi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gfd.chenzaomai.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mpn.aibaodan.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://noy.ehwqpu.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jkc.vqdsnc.cn

—— 文件结束 ——
来源：http://kwh.vqdsnc.cn

================================================================================
来源：http://trl.pengpengdd.cyou

程序语言常见例子速查手册（2024 版）
来源：http://kfy.c1oappe.top

Common Programming Examples Cheat Book
来源：http://twy.jlsjyb.cn

================================================================================
来源：http://ybt.yj20258888.top

【收录内容】
来源：http://shu.hywenlv.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zzh.tanke756.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dyd.hcnkem.com

SQL · Bash · C · C++
来源：http://xox.mhx1999.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lad.jqgufenzy.top

【使用说明】
来源：http://fkh.dianchejie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ovv.sysykeji.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ohw.cheryme.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nmg.shanyushiyangkeji.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://msf.jyoumei.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xse.ywan-chungtsiang.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wgj.chenjidiqi.icu

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rcd.shangyingyoupin.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sob.aizwys.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bjz.pengpengdd.cyou

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yjb.cheryme.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tjt.jinqigfzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tbz.ppjwa.cn

【文件统计】
来源：http://hbl.fzhhl.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ynk.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://ceh.vqdsnc.cn

目  录
来源：http://fnv.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://tju.zdbjq.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wqz.xinyue.icu

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jbn.quarkkingdee.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vps.shangyingyoupin.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vad.quarkkingdee.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://orf.gaohongyu789.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://glz.yongpay.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dbc.0kj1m.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hix.dashuyun.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zcb.iojbl.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qov.shuidangran.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xoy.hammf.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jag.tanke756.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rdj.dashuyun.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fpr.haohaochexian.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wks.xinyue.icu

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kqo.zhiwuduotai.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ayg.mhx1999.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://idr.yfazqb.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wkw.sweek.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://itd.jianghu66.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ftg.andypj.xyz

================================================================================
来源：http://ilc.sysykeji.top

A. 基础语法与类型
来源：http://hui.jinyuanbaomall.cn

================================================================================
来源：http://ism.jlsjyb.cn

[A01] Hello World
来源：http://jgz.cdnleiting.top

Py:   print("Hello, World!")
来源：http://dhx.shangyingyoupin.top

PHP:  echo "Hello, World!";
来源：http://vxw.ctjpmb.com

JS:   console.log("Hello, World!");
来源：http://tge.xylfe.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dja.yvedp.cn

Java: System.out.println("Hello, World!");
来源：http://dwa.xingfuxueyuan.xyz

Go:   fmt.Println("Hello, World!")
来源：http://rnx.tanke756.top

Ruby: puts "Hello, World!"
来源：http://ubc.iojbl.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rbn.shanyushiyangkeji.top

[A02] 变量声明与赋值
来源：http://jfo.hcnkem.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://iij.jinghuilouyu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://nvk.shanyushiyangtech.top

JS:   let name = "Alex"; const age = 20;
来源：http://vsy.hysaishi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nqg.aizwys.cn

Java: String name = "Alex"; int age = 20;
来源：http://kms.yuanzhike.top

Go:   name := "Alex"; age := 20
来源：http://dhv.gogol.net.cn

Ruby: name = "Alex"; age = 20
来源：http://ryx.zhoulong.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://rzu.shuidangran.top

[A03] 常量定义
来源：http://mhi.epnwcf.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lrg.sweek.top

PHP:  const PI = 3.14159;
来源：http://ujn.xingfuxueyuan.xyz

JS:   const PI = 3.14159;
来源：http://ckc.iojbl.cn

TS:   const PI: number = 3.14159;
来源：http://xsa.sysykeji.top

Java: static final double PI = 3.14159;
来源：http://ixu.pengpengdd.cyou

Go:   const PI = 3.14159
来源：http://cmx.cheryme.top

Ruby: PI = 3.14159
来源：http://uqz.ehwqpu.com

C#:   const double PI = 3.14159;
来源：http://wnh.0kj1m.cn

[A04] 判断变量类型
来源：http://ojf.mhx1999.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://fkr.yfazqb.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://iqm.zhaomingkeji.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zqj.snrcjt.cn

TS:   typeof x; x instanceof Date
来源：http://oim.daxiang520.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cbt.snrcjt.cn

Go:   reflect.TypeOf(x).Name()
来源：http://kqy.yongpay.top

Ruby: x.class; x.is_a?(Integer)
来源：http://yux.yueranfly.top

C#:   x.GetType().Name; x is int
来源：http://lio.zhijiandao.cn

[A05] 整数除法与取模
来源：http://siu.zhijiandao.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qvc.dashuyun.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xgi.wangdashe.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ewg.svipenyu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hvm.yfazqb.com

Java: 7 / 2; 7 % 2
来源：http://ecw.9152youxi.cn

Go:   7 / 2; 7 % 2
来源：http://wao.hongshengwenyu.top

Ruby: 7 / 2; 7 % 2
来源：http://mum.jinqigufen.top

C#:   7 / 2; 7 % 2
来源：http://lkj.snrcjt.cn

[A06] 字符串转数字
来源：http://hbl.cheryme.top

Py:   int("42"); float("3.14")
来源：http://gzx.yonumen.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pfu.52xcode.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pkz.gotoacloud.top

TS:   parseInt("42", 10); Number("42")
来源：http://dst.xinyue.icu

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://olm.hfpthk.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jah.hfpthk.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rzm.gaohongyu789.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jwg.nanxinkj.top

[A07] 数字转字符串
来源：http://wrt.snrcjt.cn

Py:   str(42)
来源：http://rwe.shanyushiyangtech.top

PHP:  (string) 42; strval(42)
来源：http://kgs.shangyingyoupin.top

JS:   String(42); (42).toString()
来源：http://hjp.hysaishi.cn

TS:   String(42)
来源：http://zgs.ydzc1.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://pea.gzhubu.top

Go:   strconv.Itoa(42)
来源：http://bgj.xingfuxueyuan.xyz

Ruby: 42.to_s
来源：http://nty.hongshengwenyu.top

C#:   42.ToString()
来源：http://prz.jqgfzy.top

[A08] 取整与四舍五入
来源：http://sak.chenlongwang.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tui.tanke756.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mpg.pengpengdd.cyou

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vte.zhixingplan.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://utd.vqdsnc.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fwx.yj202588.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://shw.cashguo.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://dyu.gotoacloud.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://def.fanxiaobao.xyz

[A09] 绝对值与最大最小值
来源：http://tdn.cqqwz.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://der.gaohongyu789.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://htv.ywan-chungtsiang.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ybt.hammf.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hpg.mhx1999.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://czm.tarul.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vrs.52xcode.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rds.cheryme.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://adv.hysaishi.cn

[A10] 生成随机数
来源：http://ykx.iojbl.cn

Py:   import random; random.randint(1, 100)
来源：http://vwh.hfpthk.cn

PHP:  random_int(1, 100);
来源：http://bbr.sjlbkw.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bxy.andypj.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qxv.iojbl.cn

Java: new Random().nextInt(100) + 1
来源：http://sjg.redwolf501.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://onb.jinqigufen.top

Ruby: rand(1..100)
来源：http://hvk.cucudq.cn

C#:   new Random().Next(1, 101)
来源：http://feo.fanxiaobao.xyz

[A11] 条件表达式（三元）
来源：http://vil.yvedp.cn

Py:   "yes" if x > 0 else "no"
来源：http://cxt.hnxiangtu.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ozn.cqqwz.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yya.316326.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://jdi.dashuyun.cn

Java: x > 0 ? "yes" : "no"
来源：http://ymu.smart0.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://amq.hesvh.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ddi.iojbl.cn

C#:   x > 0 ? "yes" : "no"
来源：http://cmg.shanyushiyangtech.top

[A12] 字符串插值 / 格式化
来源：http://kdp.bjfxy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kjm.gogol.net.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mts.zhaomingkeji.xyz

JS:   `Hello, ${name}!`
来源：http://vvo.xinyue.icu

TS:   `Hello, ${name}!`
来源：http://hjl.zdbjq.cn

Java: "Hello, %s!".formatted(name)
来源：http://gca.hcnkem.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://haf.pengpengdd.cyou

Ruby: "Hello, #{name}!"
来源：http://ywu.epnwcf.com

C#:   $"Hello, {name}!"
来源：http://cqd.tianlin.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://wcz.nwbrower.top

Py:   "第一行\n第二行"
来源：http://aid.fengsongda.top

PHP:  "第一行\n第二行"
来源：http://tfz.nanxuanxn.top

JS:   "第一行\n第二行"
来源：http://krf.hnxiangtu.top

TS:   "第一行\n第二行"
来源：http://kuu.fktsv.cn

Java: "第一行\n第二行"
来源：http://ftr.yangfankeji.com

Go:   "第一行\n第二行"
来源：http://ymd.jinqigfzy.top

Ruby: "第一行\n第二行"
来源：http://umm.ydjk.org.cn

C#:   "第一行\n第二行"
来源：http://lih.birdmap.top

[A14] 注释写法
来源：http://wlf.yuanzhike.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://zhz.jyoumei.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sfb.cucudq.cn

JS:   // 单行；/* 多行 */
来源：http://aig.cashguo.top

TS:   // 单行；/* 多行 */
来源：http://fqe.hysaishi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yqr.daxiang520.top

Go:   // 单行；/* 多行 */
来源：http://njq.0kj1m.cn

Ruby: # 单行；=begin 多行 =end
来源：http://iyb.meibo888.top

C#:   // 单行；/* 多行 */
来源：http://stk.sxryk.cn

[A15] 空值判断与默认值
来源：http://xvq.xingfuxueyuan.xyz

Py:   value = data or "默认值"
来源：http://zcl.meibo888.top

PHP:  $value = $data ?? "默认值";
来源：http://bbn.tianlin.xyz


<!-- 参考信息 -->