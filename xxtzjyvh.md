代发 wailian999

[U77] PHP：模板渲染
来源：http://anh.nanxuanxn.top

composer require twig/twig
来源：http://nid.xuanzx.com

[U78] PHP：单元测试
来源：http://jhh.feifeiyinyue.top

composer require --dev phpunit/phpunit
来源：http://zqf.jiagoushi.top

[U79] PHP：静态分析
来源：http://thg.smart0.xyz

composer require --dev phpstan/phpstan
来源：http://pkw.xylfe.cn

[U80] PHP：代码规范修复
来源：http://lpy.ivvv.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://yhf.shanyushiyangtech.top

[U81] JS：初始化项目
来源：http://hsv.sufxvd.cn

npm init -y;  npm i express
来源：http://zlq.wangshuangyany.cn

[U82] JS：package.json 脚本
来源：http://elo.c1oappe.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xas.jyoumei.cn

[U83] JS：ES Module 导入导出
来源：http://lqh.dianchejie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bni.gotoacloud.top

[U84] JS：CommonJS 写法
来源：http://yaj.zhongyouzk.top

module.exports = { a };  const { a } = require("./m");
来源：http://myc.yuxming.cn

[U85] JS：可选链
来源：http://obn.chenzaomai.com

a?.b?.c
来源：http://qpr.jinqigfzy.top

[U86] JS：空值合并
来源：http://ied.gzhubu.top

a ?? b
来源：http://emb.pengpengdd.cyou

[U87] JS：解构默认值
来源：http://ihs.guowangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://hju.sxryk.cn

[U88] JS：对象展开合并
来源：http://ohx.zhiwuduotai.top

{ ...a, ...b }
来源：http://kfq.316326.xyz

[U89] JS：数组去重
来源：http://elb.jiagoushi.top

[...new Set(arr)]
来源：http://dqc.meibo888.top

[U90] JS：数字数组排序
来源：http://evw.fzhhl.top

[...arr].sort((a, b) => a - b)
来源：http://ydl.ywan-chungtsiang.top

[U91] JS：对象键值遍历
来源：http://wsh.sxryk.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wmc.jqgfzy.top

[U92] JS：深拷贝
来源：http://jrc.xuanzx.com

structuredClone(obj)
来源：http://ihr.ppjwa.cn

[U93] JS：模板字符串
来源：http://ytu.cucudq.cn

`共 ${n} 条`
来源：http://syw.gzhubu.top

[U94] JS：箭头函数
来源：http://yjs.hywenlv.cn

const double = x => x * 2;
来源：http://hgc.haohaochexian.top

[U95] JS：Promise 包装
来源：http://hcp.jinyuanbaomall.cn

new Promise((resolve, reject) => {})
来源：http://qkx.yj20258888.top

[U96] JS：async/await 与异常
来源：http://xyn.gotoacloud.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ukz.jqgufenzy.top

[U97] JS：并发请求
来源：http://ipv.fktsv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://awc.haohaochexian.top

[U98] JS：fetch 带 JSON
来源：http://kzm.zhixingplan.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tdm.xingfuxueyuan.xyz

[U99] JS：事件监听
来源：http://irh.tian-w.cn

el.addEventListener("click", e => {})
来源：http://nwa.tian-w.cn

[U100] JS：DOM 查询
来源：http://xpo.cqqwz.cn

document.querySelector(".item")
来源：http://acw.fzhhl.top

[U101] JS：classList 操作
来源：http://wks.zhongyouzk.top

el.classList.toggle("active")
来源：http://gyd.pycfn.com

[U102] JS：本地存储
来源：http://jfz.redwolf501.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://uvh.jianghu66.top

[U103] JS：定时器
来源：http://jyw.cqqwz.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gda.wangdashe.top

[U104] JS：防抖
来源：http://wor.gaohongyu789.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jzd.yanxiufei.cn

[U105] JS：节流
来源：http://kmz.gzhubu.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oji.vqdsnc.cn

[U106] JS：日期格式化
来源：http://ulk.iojbl.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pmo.hcnkem.com

[U107] JS：数字千分位
来源：http://srl.zycfv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uyq.hongshengwenyu.top

[U108] JS：随机整数
来源：http://vge.52xcode.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iuv.gotoacloud.top

[U109] JS：数组分组
来源：http://mvq.jlsjyb.cn

Object.groupBy(arr, x => x.type)
来源：http://pqc.zycfv.cn

[U110] JS：数组分块
来源：http://xfo.hywenlv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dpg.ehwqpu.com

[U111] JS：对象转 Map
来源：http://dhz.meibo888.top

new Map(Object.entries(obj))
来源：http://lpq.ydjk.org.cn

[U112] JS：字符串补位
来源：http://jjv.jinghuilouyu.cn

"7".padStart(3, "0")
来源：http://lxr.daxiang520.top

[U113] JS：正则替换全部
来源：http://azx.shanyushiyangkeji.top

s.replaceAll("a", "b")
来源：http://ofn.yongpay.top

[U114] JS：JSON 深比较
来源：http://xlp.sxryk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://svl.redwolf501.top

[U115] JS：生成 UUID
来源：http://qpl.zdqjudy.top

crypto.randomUUID()
来源：http://zpk.jiagoushi.top

[U116] JS：类型检查（JSDoc）
来源：http://rct.hongshengwenyu.top

/** @param {string} name */ function f(name) {}
来源：http://ypo.andypj.xyz

[U117] JS：单元测试
来源：http://ozo.hesvh.cn

npm i -D vitest;  npx vitest
来源：http://bmo.hywenlv.cn

[U118] JS：开发服务器
来源：http://mbr.c1oappe.top

npm i -D vite;  npx vite
来源：http://nky.zdqjudy.top

[U119] JS：生产构建
来源：http://qlv.cashguo.top

npx vite build
来源：http://kwp.jqgfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://uyg.pycfn.com

import.meta.env.VITE_API_URL
来源：http://dmn.gzhubu.top

================================================================================
来源：http://whf.feifeiyinyue.top

统计汇总
来源：http://ejk.jlsjyb.cn

================================================================================
来源：http://zga.ivvv.top

按语言统计（条）：
来源：http://tzx.nwbrower.top

Python ......... 252
来源：http://fvx.nanxuanxn.top

PHP ............ 252
来源：http://seh.gogol.net.cn

JavaScript ..... 252
来源：http://qhh.andypj.xyz

TypeScript ..... 212
来源：http://utc.jinyuanbaomall.cn

Java ........... 212
来源：http://kzt.snrcjt.cn

Go ............. 212
来源：http://wgq.jqgufenzy.top

Ruby ........... 212
来源：http://xts.pengpengdd.cyou

C# ............. 212
来源：http://bwr.quarkkingdee.top

C .............. 30
来源：http://aih.hywenlv.cn

C++ ............ 30
来源：http://rqf.shangyingyoupin.top

SQL ............ 90
来源：http://dti.sjlbkw.cn

Bash ........... 80
来源：http://qcg.ydjk.org.cn

Kotlin ......... 15
来源：http://jgt.zdqjudy.top

Swift .......... 15
来源：http://nsd.yuxming.cn

Lua ............ 10
来源：http://snk.jlsjyb.cn

Perl ........... 10
来源：http://thh.jinqigfzy.top

Scala .......... 10
来源：http://hmj.guowangkeji.top

------------------------------------
来源：http://myy.hnqzz.top

合计 ........... 2106 条
来源：http://fwg.daria6918.cn

按章节统计：
来源：http://vyg.chenzaomai.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://djt.iojbl.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rfo.birdmap.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hmb.tianlin.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://etp.kuanghao11.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rcx.epnwcf.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xtk.aibaodan.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ofx.shzxlz.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jxt.birdmap.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uot.gzhubu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hap.cqqwz.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nwj.gogol.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zgt.ywan-chungtsiang.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://iqv.chenjidiqi.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mxa.chenlongwang.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yna.jinqigufen.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bvv.dashuyun.cn

Q SQL 专题                              90
来源：http://ymo.cheryme.top

R Bash 专题                             80
来源：http://qxv.tanke756.top

S C / C++ 专题                          60
来源：http://ebi.chenlongwang.top

T 其他语言补充                          60
来源：http://tma.sufxvd.cn

U 高频实用片段                         120
来源：http://dpv.hysaishi.cn

------------------------------------
来源：http://ruf.0kj1m.cn

合计                                  2106 条
来源：http://ews.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://qkj.zhoulong.xyz

使用提醒
来源：http://djs.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://nzv.kuanghao11.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://oae.daria6918.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://teq.sxryk.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nww.shuidangran.top

在旧版本上使用前请先确认语法支持情况。
来源：http://vmi.svipenyu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mlb.ydzc1.top

—— 文件结束 ——
来源：http://uar.aibaodan.cn

================================================================================
来源：http://sqw.52xcode.cn

程序语言常见例子速查手册（2024 版）
来源：http://lpx.smart0.xyz

Common Programming Examples Cheat Book
来源：http://okr.fehbvm.com

================================================================================
来源：http://zin.hywenlv.cn

【收录内容】
来源：http://ogi.sjlbkw.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://okt.hesvh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zkj.daria6918.cn

SQL · Bash · C · C++
来源：http://kyx.jlsjyb.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ydx.yuxming.cn

【使用说明】
来源：http://msk.xuetiantiany.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://azk.vqdsnc.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jxr.316326.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fki.shanyushiyangkeji.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zpc.redwolf501.top

Bash:  Shell         C:     C             C++:   C++
来源：http://aqd.chenlongwang.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://inz.tarul.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rwo.0kj1m.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rad.xingfuxueyuan.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://sda.aizwys.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fbp.yuxming.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://oip.gogol.net.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bzp.fzhhl.top

【文件统计】
来源：http://eyz.iojbl.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://axt.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://dho.zdqjudy.top

目  录
来源：http://pxg.cashguo.top

--------------------------------------------------------------------------------
来源：http://jud.feifeiyinyue.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://aqn.andypj.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tdy.hfpthk.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kmf.jlsjyb.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wbt.jianghu66.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fga.hnxiangtu.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bay.zdqjudy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mjt.jinqigfzy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://oce.guowangkeji.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fay.hysaishi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vxh.tanke756.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sit.fehbvm.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tds.zhongyouzk.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vgb.jyoumei.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wpi.zdbjq.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rfc.sxryk.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://aye.bjfxy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yyj.hnxiangtu.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://rgb.sweek.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://syc.cheryme.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qgg.zhengqikj.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ics.ppjwa.cn

================================================================================
来源：http://ekz.svipenyu.cn

A. 基础语法与类型
来源：http://uze.jqgfzy.top

================================================================================
来源：http://oqr.sufxvd.cn

[A01] Hello World
来源：http://zfh.xylfe.cn

Py:   print("Hello, World!")
来源：http://bwg.redwolf501.top

PHP:  echo "Hello, World!";
来源：http://xbl.shanyushiyangkeji.top

JS:   console.log("Hello, World!");
来源：http://ecj.yfazqb.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xqe.cucudq.cn

Java: System.out.println("Hello, World!");
来源：http://wff.gaohongyu789.top

Go:   fmt.Println("Hello, World!")
来源：http://aff.jinqigufen.top

Ruby: puts "Hello, World!"
来源：http://dmm.xuanzx.com

C#:   Console.WriteLine("Hello, World!");
来源：http://dkf.zhaomingkeji.xyz

[A02] 变量声明与赋值
来源：http://zln.yangfankeji.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cib.zhaomingkeji.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://fiw.yfazqb.com

JS:   let name = "Alex"; const age = 20;
来源：http://lfq.tanke756.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nhk.ywan-chungtsiang.top

Java: String name = "Alex"; int age = 20;
来源：http://djk.yuanzhike.top

Go:   name := "Alex"; age := 20
来源：http://bfj.hywenlv.cn

Ruby: name = "Alex"; age = 20
来源：http://qgx.fanxiaobao.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://uwa.kuanghao11.cn

[A03] 常量定义
来源：http://ioe.jqgufenzy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sgc.shuidangran.top

PHP:  const PI = 3.14159;
来源：http://fli.sweek.top

JS:   const PI = 3.14159;
来源：http://kwy.daxiang520.top

TS:   const PI: number = 3.14159;
来源：http://rbm.zhixingplan.top

Java: static final double PI = 3.14159;
来源：http://mmr.cqqwz.cn

Go:   const PI = 3.14159
来源：http://uvs.yfazqb.com

Ruby: PI = 3.14159
来源：http://qyq.sysykeji.top

C#:   const double PI = 3.14159;
来源：http://pqs.guannengcc.top

[A04] 判断变量类型
来源：http://aaz.zdqjudy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://icq.bjfxy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://efo.sweek.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ptz.hywenlv.cn

TS:   typeof x; x instanceof Date
来源：http://huv.jinqigfzy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dyr.yfazqb.com

Go:   reflect.TypeOf(x).Name()
来源：http://dly.zhengqikj.top

Ruby: x.class; x.is_a?(Integer)
来源：http://cme.tanke756.top

C#:   x.GetType().Name; x is int
来源：http://yth.fengsongda.top

[A05] 整数除法与取模
来源：http://hda.jlsjyb.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rlz.ydjk.org.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xvt.jyoumei.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kcb.redwolf501.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zre.zhongyouzk.top

Java: 7 / 2; 7 % 2
来源：http://nrq.bbcook.cn

Go:   7 / 2; 7 % 2
来源：http://ipb.dianchejie.cn

Ruby: 7 / 2; 7 % 2
来源：http://anx.birdmap.top

C#:   7 / 2; 7 % 2
来源：http://jpw.gogol.net.cn

[A06] 字符串转数字
来源：http://xip.xingfuxueyuan.xyz

Py:   int("42"); float("3.14")
来源：http://mqo.epnwcf.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ajk.hnxiangtu.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pdq.gogol.net.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rnz.jinqigufen.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://esa.yuanzhike.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kri.ctjpmb.com

Ruby: "42".to_i; "3.14".to_f
来源：http://fyj.vqdsnc.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tai.xylfe.cn

[A07] 数字转字符串
来源：http://lvm.jinqigfzy.top

Py:   str(42)
来源：http://rup.xingfuxueyuan.xyz

PHP:  (string) 42; strval(42)
来源：http://ehf.yanxiufei.cn

JS:   String(42); (42).toString()
来源：http://lyi.chenjidiqi.icu

TS:   String(42)
来源：http://ovx.wangdashe.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://idc.mhx1999.top

Go:   strconv.Itoa(42)
来源：http://dnz.jinghuilouyu.cn

Ruby: 42.to_s
来源：http://rpm.hysaishi.cn

C#:   42.ToString()
来源：http://wqe.yonumen.top

[A08] 取整与四舍五入
来源：http://rma.yangfankeji.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gmp.ivvv.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kjy.ivvv.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dqw.iojbl.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bnz.aizwys.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ytq.yangfankeji.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fee.nwbrower.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://edo.pycfn.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xqt.9152youxi.cn

[A09] 绝对值与最大最小值
来源：http://dfk.redwolf501.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://epq.chenlongwang.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://olt.nanxuanxn.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xga.vehdjk.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gmr.yanxiufei.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fhk.tian-w.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jin.jinqigfzy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kfh.9152youxi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://azc.cashguo.top

[A10] 生成随机数
来源：http://zoq.redwolf501.top

Py:   import random; random.randint(1, 100)
来源：http://vbd.epnwcf.com

PHP:  random_int(1, 100);
来源：http://jqx.fktsv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://alj.ydjk.org.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dib.nwbrower.top

Java: new Random().nextInt(100) + 1
来源：http://tzi.zhixingplan.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nxq.hammf.cn

Ruby: rand(1..100)
来源：http://khs.zhengqikj.top

C#:   new Random().Next(1, 101)
来源：http://gyy.guannengcc.top

[A11] 条件表达式（三元）
来源：http://ufk.epnwcf.com

Py:   "yes" if x > 0 else "no"
来源：http://ryu.yanxiufei.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dxx.vehdjk.com

JS:   x > 0 ? "yes" : "no"
来源：http://mgf.jqgfzy.top

TS:   x > 0 ? "yes" : "no"
来源：http://fwy.bjfxy.top

Java: x > 0 ? "yes" : "no"
来源：http://rmz.zhiwuduotai.top

Go:   // 无三元运算符，需用 if 语句
来源：http://tcj.zdbjq.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hbn.zhaomingkeji.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://kcv.fktsv.cn

[A12] 字符串插值 / 格式化
来源：http://hwd.yueranfly.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jzt.daria6918.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uaq.aizwys.cn

JS:   `Hello, ${name}!`
来源：http://fuy.chenlongwang.top

TS:   `Hello, ${name}!`
来源：http://ikt.jqgufenzy.top

Java: "Hello, %s!".formatted(name)
来源：http://wqv.sysykeji.top


<!-- 参考信息 -->