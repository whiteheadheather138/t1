代发 wailian999

[U85] JS：可选链
来源：http://ejr.kuanghao11.cn

a?.b?.c
来源：http://lvt.shanyushiyangtech.top

[U86] JS：空值合并
来源：http://pkh.nanxinkj.top

a ?? b
来源：http://hjo.bjfxy.top

[U87] JS：解构默认值
来源：http://mwd.vqdsnc.cn

const { a = 1, b = 2 } = obj;
来源：http://lcd.andypj.xyz

[U88] JS：对象展开合并
来源：http://usp.sysykeji.top

{ ...a, ...b }
来源：http://cwx.chenjidiqi.icu

[U89] JS：数组去重
来源：http://zod.dianchejie.cn

[...new Set(arr)]
来源：http://gik.ctjpmb.com

[U90] JS：数字数组排序
来源：http://onf.ydzc1.top

[...arr].sort((a, b) => a - b)
来源：http://fyd.xinyue.icu

[U91] JS：对象键值遍历
来源：http://txu.tianlin.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tiy.fengsongda.top

[U92] JS：深拷贝
来源：http://msj.hywenlv.cn

structuredClone(obj)
来源：http://gsn.yueranfly.top

[U93] JS：模板字符串
来源：http://yaa.bjfxy.top

`共 ${n} 条`
来源：http://yrg.sjlbkw.cn

[U94] JS：箭头函数
来源：http://dgx.dianchejie.cn

const double = x => x * 2;
来源：http://czb.redwolf501.top

[U95] JS：Promise 包装
来源：http://oew.cucudq.cn

new Promise((resolve, reject) => {})
来源：http://qrj.zdbjq.cn

[U96] JS：async/await 与异常
来源：http://tca.tian-w.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gib.svipenyu.cn

[U97] JS：并发请求
来源：http://fvb.svipenyu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lkc.fanxiaobao.xyz

[U98] JS：fetch 带 JSON
来源：http://ncx.xylfe.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://byv.quarkkingdee.top

[U99] JS：事件监听
来源：http://yzh.jiagoushi.top

el.addEventListener("click", e => {})
来源：http://cim.chenzaomai.com

[U100] JS：DOM 查询
来源：http://osu.chenlongwang.top

document.querySelector(".item")
来源：http://plo.fzhhl.top

[U101] JS：classList 操作
来源：http://quq.ybcxt.top

el.classList.toggle("active")
来源：http://wyk.dashuyun.cn

[U102] JS：本地存储
来源：http://zxx.52xcode.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jry.yfazqb.com

[U103] JS：定时器
来源：http://cou.vqdsnc.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wtk.daria6918.cn

[U104] JS：防抖
来源：http://nus.ehwqpu.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rxs.jinqigufen.top

[U105] JS：节流
来源：http://mwm.ywan-chungtsiang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://njg.zycfv.cn

[U106] JS：日期格式化
来源：http://yqx.nanxinkj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pry.vehdjk.com

[U107] JS：数字千分位
来源：http://lfq.jyoumei.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kgp.daria6918.cn

[U108] JS：随机整数
来源：http://tpa.andypj.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kwr.shuidangran.top

[U109] JS：数组分组
来源：http://uoj.fanxiaobao.xyz

Object.groupBy(arr, x => x.type)
来源：http://kfq.jinghuilouyu.cn

[U110] JS：数组分块
来源：http://uqi.aibaodan.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dtg.yuanzhike.top

[U111] JS：对象转 Map
来源：http://alv.316326.xyz

new Map(Object.entries(obj))
来源：http://dug.smart0.xyz

[U112] JS：字符串补位
来源：http://rcg.shangyingyoupin.top

"7".padStart(3, "0")
来源：http://lpm.yanxiufei.cn

[U113] JS：正则替换全部
来源：http://ewo.yj20258.top

s.replaceAll("a", "b")
来源：http://wol.xinyue.icu

[U114] JS：JSON 深比较
来源：http://vhp.meibo888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ztf.fzhhl.top

[U115] JS：生成 UUID
来源：http://aqs.havefunace.top

crypto.randomUUID()
来源：http://mkw.tanke756.top

[U116] JS：类型检查（JSDoc）
来源：http://nkf.yj202588.top

/** @param {string} name */ function f(name) {}
来源：http://ksz.pengpengdd.cyou

[U117] JS：单元测试
来源：http://smg.jiagoushi.top

npm i -D vitest;  npx vitest
来源：http://bhd.uphjek.com

[U118] JS：开发服务器
来源：http://zsw.quarkkingdee.top

npm i -D vite;  npx vite
来源：http://qhd.jinyuanbaomall.cn

[U119] JS：生产构建
来源：http://chc.sysykeji.top

npx vite build
来源：http://aka.jinqigfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://pkh.pycfn.com

import.meta.env.VITE_API_URL
来源：http://pwj.dashuyun.cn

================================================================================
来源：http://vfb.gogol.net.cn

统计汇总
来源：http://pyi.ybcxt.top

================================================================================
来源：http://dol.xuetiantiany.cn

按语言统计（条）：
来源：http://vix.yfazqb.com

Python ......... 252
来源：http://imi.zhoulong.xyz

PHP ............ 252
来源：http://urx.ppjwa.cn

JavaScript ..... 252
来源：http://ylt.yonumen.top

TypeScript ..... 212
来源：http://gem.xingfuxueyuan.xyz

Java ........... 212
来源：http://dfm.andypj.xyz

Go ............. 212
来源：http://wuj.hysaishi.cn

Ruby ........... 212
来源：http://gvt.yuxming.cn

C# ............. 212
来源：http://zjp.shanyushiyangtech.top

C .............. 30
来源：http://ngj.jianghu66.top

C++ ............ 30
来源：http://stv.jianghu66.top

SQL ............ 90
来源：http://xyo.ywan-chungtsiang.top

Bash ........... 80
来源：http://abt.fehbvm.com

Kotlin ......... 15
来源：http://ykl.yfazqb.com

Swift .......... 15
来源：http://nnv.shangyingyoupin.top

Lua ............ 10
来源：http://spa.yj20258888.top

Perl ........... 10
来源：http://zil.chenlongwang.top

Scala .......... 10
来源：http://nwm.havefunace.top

------------------------------------
来源：http://xwz.nanxinkj.top

合计 ........... 2106 条
来源：http://als.feifeiyinyue.top

按章节统计：
来源：http://wcu.yongpay.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nnz.chenlongwang.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vok.jinqigfzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ylb.wangdashe.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uca.yj202588.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://igs.shangyingyoupin.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uof.cheryme.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sir.vqdsnc.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sgs.yongpay.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uom.feifeiyinyue.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uew.zdqjudy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rum.cqqwz.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lri.dashuyun.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nss.zhixingplan.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mft.guowangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jcp.jqgfzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://acy.shanyushiyangtech.top

Q SQL 专题                              90
来源：http://qvg.nanxinkj.top

R Bash 专题                             80
来源：http://hnq.jinqigufen.top

S C / C++ 专题                          60
来源：http://ihw.jinqigufen.top

T 其他语言补充                          60
来源：http://khe.andypj.xyz

U 高频实用片段                         120
来源：http://lkh.hesvh.cn

------------------------------------
来源：http://nxl.mhx1999.top

合计                                  2106 条
来源：http://byy.mhx1999.top

--------------------------------------------------------------------------------
来源：http://khn.guannengcc.top

使用提醒
来源：http://ryv.wangdashe.top

--------------------------------------------------------------------------------
来源：http://fhf.yanxiufei.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xzd.xylfe.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ltw.bbcook.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hmx.0kj1m.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wfo.sufxvd.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bre.nwbrower.top

—— 文件结束 ——
来源：http://yxy.zhijiandao.cn

================================================================================
来源：http://ymw.xylfe.cn

程序语言常见例子速查手册（2024 版）
来源：http://ikb.hfpthk.cn

Common Programming Examples Cheat Book
来源：http://zre.cqqwz.cn

================================================================================
来源：http://iye.haohaochexian.top

【收录内容】
来源：http://fml.jianghu66.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://pec.jinghuilouyu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xtk.wangshuangyany.cn

SQL · Bash · C · C++
来源：http://bep.sxryk.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qdw.zdqjudy.top

【使用说明】
来源：http://vjy.yj20258888.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pbu.nanxuanxn.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://opb.tianlin.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mqj.wangshuangyany.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://shy.epnwcf.com

Bash:  Shell         C:     C             C++:   C++
来源：http://vam.sufxvd.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xvq.xinyue.icu

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gbl.pengpengdd.cyou

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://znb.yuxming.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hlh.sufxvd.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pno.jinqigfzy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wrk.shuidangran.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://koc.mhx1999.top

【文件统计】
来源：http://yno.wangshuangyany.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fuz.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://pac.gotoacloud.top

目  录
来源：http://luz.jiagoushi.top

--------------------------------------------------------------------------------
来源：http://upt.yfazqb.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sjy.kuanghao11.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xiw.cdnleiting.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mwa.xylfe.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://toa.gotoacloud.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sbb.snrcjt.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zbh.jqgufenzy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zkw.pengpengdd.cyou

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wul.jinghuilouyu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://iev.jlsjyb.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://btz.ctjpmb.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sug.tian-w.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://npe.yj20258888.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yix.zdqjudy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vrv.uphjek.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ctm.cashguo.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kez.pengpengdd.cyou

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cks.yongpay.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://zwu.dianchejie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bxu.yj20258888.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qfm.ppjwa.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rwo.snrcjt.cn

================================================================================
来源：http://qza.hfpthk.cn

A. 基础语法与类型
来源：http://uyd.ctjpmb.com

================================================================================
来源：http://vpq.zdqjudy.top

[A01] Hello World
来源：http://qbg.hywenlv.cn

Py:   print("Hello, World!")
来源：http://nlx.sjlbkw.cn

PHP:  echo "Hello, World!";
来源：http://gcu.0kj1m.cn

JS:   console.log("Hello, World!");
来源：http://dhm.shangyingyoupin.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://oyp.pycfn.com

Java: System.out.println("Hello, World!");
来源：http://hyq.shangyingyoupin.top

Go:   fmt.Println("Hello, World!")
来源：http://hft.cdnleiting.top

Ruby: puts "Hello, World!"
来源：http://jso.yanxiufei.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://tkf.ivvv.top

[A02] 变量声明与赋值
来源：http://owo.hnqzz.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://edq.gogol.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zpt.nanxuanxn.top

JS:   let name = "Alex"; const age = 20;
来源：http://wmk.wangdashe.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rot.shzxlz.cn

Java: String name = "Alex"; int age = 20;
来源：http://xlr.shangyingyoupin.top

Go:   name := "Alex"; age := 20
来源：http://eyc.andypj.xyz

Ruby: name = "Alex"; age = 20
来源：http://bkm.jqgfzy.top

C#:   string name = "Alex"; int age = 20;
来源：http://iwc.yfazqb.com

[A03] 常量定义
来源：http://dat.yfazqb.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kbx.yfazqb.com

PHP:  const PI = 3.14159;
来源：http://kxz.jinqigufen.top

JS:   const PI = 3.14159;
来源：http://oih.smart0.xyz

TS:   const PI: number = 3.14159;
来源：http://onq.hcnkem.com

Java: static final double PI = 3.14159;
来源：http://dcs.mhx1999.top

Go:   const PI = 3.14159
来源：http://twr.chenjidiqi.icu

Ruby: PI = 3.14159
来源：http://acr.bjfxy.top

C#:   const double PI = 3.14159;
来源：http://ztq.cucudq.cn

[A04] 判断变量类型
来源：http://wro.pengpengdd.cyou

Py:   type(x).__name__; isinstance(x, int)
来源：http://gvi.zdbjq.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gwa.wangdashe.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gwy.tanke756.top

TS:   typeof x; x instanceof Date
来源：http://jkp.ehwqpu.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fnk.yj20258888.top

Go:   reflect.TypeOf(x).Name()
来源：http://dgu.daria6918.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://oit.xinyue.icu

C#:   x.GetType().Name; x is int
来源：http://mum.tanke756.top

[A05] 整数除法与取模
来源：http://oun.pengpengdd.cyou

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://owh.yuxming.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ygd.meibo888.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bgc.wangdashe.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hwy.ehwqpu.com

Java: 7 / 2; 7 % 2
来源：http://ucz.feifeiyinyue.top

Go:   7 / 2; 7 % 2
来源：http://exn.ppjwa.cn

Ruby: 7 / 2; 7 % 2
来源：http://src.xziqi.cn

C#:   7 / 2; 7 % 2
来源：http://tjb.yuxming.cn

[A06] 字符串转数字
来源：http://ilk.shanyushiyangtech.top

Py:   int("42"); float("3.14")
来源：http://hyw.cheryme.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://oxk.vqdsnc.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://iza.andypj.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://isq.wangshuangyany.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fkw.aibaodan.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lxn.vehdjk.com

Ruby: "42".to_i; "3.14".to_f
来源：http://xik.svipenyu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xty.jinqigfzy.top

[A07] 数字转字符串
来源：http://jdo.wangshuangyany.cn

Py:   str(42)
来源：http://xsn.yj202588.top

PHP:  (string) 42; strval(42)
来源：http://piq.yj20258888.top

JS:   String(42); (42).toString()
来源：http://jhu.xinyue.icu

TS:   String(42)
来源：http://vip.zhaomingkeji.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://msm.xinyue.icu

Go:   strconv.Itoa(42)
来源：http://chw.ctjpmb.com

Ruby: 42.to_s
来源：http://joh.xuetiantiany.cn

C#:   42.ToString()
来源：http://qzq.shangyingyoupin.top

[A08] 取整与四舍五入
来源：http://xxw.yangfankeji.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ngn.tarul.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ufb.cheryme.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gga.birdmap.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lqa.tianlin.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wyq.ctjpmb.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://das.jqgfzy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://txh.wangshuangyany.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://thd.chenzaomai.com

[A09] 绝对值与最大最小值
来源：http://vqe.yueranfly.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mvb.yj20258888.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nvx.sxryk.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pet.zhijiandao.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tfs.gogol.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zfx.cucudq.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://iqv.zhaomingkeji.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://spi.cdnleiting.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jzq.jianghu66.top

[A10] 生成随机数
来源：http://pug.ctjpmb.com

Py:   import random; random.randint(1, 100)
来源：http://muu.redwolf501.top

PHP:  random_int(1, 100);
来源：http://qji.meibo888.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lim.hammf.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mai.fktsv.cn

Java: new Random().nextInt(100) + 1
来源：http://avh.vqdsnc.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://esw.jianghu66.top

Ruby: rand(1..100)
来源：http://elj.zhijiandao.cn

C#:   new Random().Next(1, 101)
来源：http://bvi.bbcook.cn

[A11] 条件表达式（三元）
来源：http://jmm.wangdashe.top

Py:   "yes" if x > 0 else "no"
来源：http://hqh.hnqzz.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ipb.feifeiyinyue.top

JS:   x > 0 ? "yes" : "no"
来源：http://vyg.yj202588.top

TS:   x > 0 ? "yes" : "no"
来源：http://iab.yongpay.top

Java: x > 0 ? "yes" : "no"
来源：http://kcm.jinqigfzy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://rbe.mhx1999.top

Ruby: x > 0 ? "yes" : "no"
来源：http://tbj.shanyushiyangtech.top

C#:   x > 0 ? "yes" : "no"
来源：http://fwl.yanxiufei.cn

[A12] 字符串插值 / 格式化
来源：http://yco.uphjek.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qyz.wangshuangyany.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cap.jinyuanbaomall.cn

JS:   `Hello, ${name}!`
来源：http://zac.tianlin.xyz

TS:   `Hello, ${name}!`
来源：http://bgh.yj20258888.top

Java: "Hello, %s!".formatted(name)
来源：http://ldj.zhiwuduotai.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ehi.0kj1m.cn

Ruby: "Hello, #{name}!"
来源：http://wnr.yj20258888.top

C#:   $"Hello, {name}!"
来源：http://uru.feifeiyinyue.top

[A13] 多行字符串（练习 \n 转义）
来源：http://uzc.fktsv.cn

Py:   "第一行\n第二行"
来源：http://qmd.yuanzhike.top

PHP:  "第一行\n第二行"
来源：http://zqr.havefunace.top

JS:   "第一行\n第二行"
来源：http://uvg.hongshengwenyu.top

TS:   "第一行\n第二行"
来源：http://wmc.guannengcc.top

Java: "第一行\n第二行"
来源：http://ryj.bbcook.cn

Go:   "第一行\n第二行"
来源：http://oup.zdqjudy.top

Ruby: "第一行\n第二行"
来源：http://xiy.vehdjk.com

C#:   "第一行\n第二行"
来源：http://gxn.hammf.cn

[A14] 注释写法
来源：http://tzm.yfazqb.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://hwq.ydzc1.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://odl.guowangkeji.top

JS:   // 单行；/* 多行 */
来源：http://kla.shanyushiyangkeji.top


<!-- 参考信息 -->