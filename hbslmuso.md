代发 wailian999

[U89] JS：数组去重
来源：http://uce.chenzaomai.com

[...new Set(arr)]
来源：http://yix.quarkkingdee.top

[U90] JS：数字数组排序
来源：http://vsp.nanxinkj.top

[...arr].sort((a, b) => a - b)
来源：http://jky.sysykeji.top

[U91] JS：对象键值遍历
来源：http://fje.sweek.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vef.pengpengdd.cyou

[U92] JS：深拷贝
来源：http://uve.sufxvd.cn

structuredClone(obj)
来源：http://kwx.hywenlv.cn

[U93] JS：模板字符串
来源：http://woz.jiagoushi.top

`共 ${n} 条`
来源：http://uex.tarul.cn

[U94] JS：箭头函数
来源：http://fgv.xziqi.cn

const double = x => x * 2;
来源：http://zbj.jinqigufen.top

[U95] JS：Promise 包装
来源：http://etx.sweek.top

new Promise((resolve, reject) => {})
来源：http://enf.jinyuanbaomall.cn

[U96] JS：async/await 与异常
来源：http://mub.meibo888.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://naa.xziqi.cn

[U97] JS：并发请求
来源：http://pqh.daxiang520.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://rzl.shuidangran.top

[U98] JS：fetch 带 JSON
来源：http://wqt.redwolf501.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zby.birdmap.top

[U99] JS：事件监听
来源：http://qnh.c1oappe.top

el.addEventListener("click", e => {})
来源：http://inp.bjfxy.top

[U100] JS：DOM 查询
来源：http://rsz.feifeiyinyue.top

document.querySelector(".item")
来源：http://giw.cqqwz.cn

[U101] JS：classList 操作
来源：http://thi.chenzaomai.com

el.classList.toggle("active")
来源：http://gzs.yuanzhike.top

[U102] JS：本地存储
来源：http://gxl.uphjek.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://ckh.yongpay.top

[U103] JS：定时器
来源：http://wae.zhijiandao.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vik.bjfxy.top

[U104] JS：防抖
来源：http://yue.zhixingplan.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rfh.wangdashe.top

[U105] JS：节流
来源：http://kae.yanxiufei.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ynd.yj20258888.top

[U106] JS：日期格式化
来源：http://ucx.nanxinkj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bqy.cucudq.cn

[U107] JS：数字千分位
来源：http://bpp.jiagoushi.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cgc.vehdjk.com

[U108] JS：随机整数
来源：http://tmp.pycfn.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nej.svipenyu.cn

[U109] JS：数组分组
来源：http://hcu.bjfxy.top

Object.groupBy(arr, x => x.type)
来源：http://jea.hysaishi.cn

[U110] JS：数组分块
来源：http://xvi.jqgufenzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jwn.ywan-chungtsiang.top

[U111] JS：对象转 Map
来源：http://vcb.yj20258888.top

new Map(Object.entries(obj))
来源：http://luc.fzhhl.top

[U112] JS：字符串补位
来源：http://xkr.cqqwz.cn

"7".padStart(3, "0")
来源：http://vbs.zdqjudy.top

[U113] JS：正则替换全部
来源：http://jtm.cqqwz.cn

s.replaceAll("a", "b")
来源：http://bws.cdnleiting.top

[U114] JS：JSON 深比较
来源：http://ljh.zdqjudy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ewg.birdmap.top

[U115] JS：生成 UUID
来源：http://lfd.dianchejie.cn

crypto.randomUUID()
来源：http://yho.sjlbkw.cn

[U116] JS：类型检查（JSDoc）
来源：http://uaa.shanyushiyangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://tsm.guowangkeji.top

[U117] JS：单元测试
来源：http://wbu.daxiang520.top

npm i -D vitest;  npx vitest
来源：http://sgk.hnxiangtu.top

[U118] JS：开发服务器
来源：http://csz.xziqi.cn

npm i -D vite;  npx vite
来源：http://qkc.cqqwz.cn

[U119] JS：生产构建
来源：http://lsp.vehdjk.com

npx vite build
来源：http://chj.nwbrower.top

[U120] JS：读取环境变量（Vite）
来源：http://fyj.quarkkingdee.top

import.meta.env.VITE_API_URL
来源：http://whz.hnxiangtu.top

================================================================================
来源：http://jbw.yuanzhike.top

统计汇总
来源：http://pho.hesvh.cn

================================================================================
来源：http://xil.mhx1999.top

按语言统计（条）：
来源：http://evv.cheryme.top

Python ......... 252
来源：http://cyo.redwolf501.top

PHP ............ 252
来源：http://ruj.jianghu66.top

JavaScript ..... 252
来源：http://wma.cucudq.cn

TypeScript ..... 212
来源：http://zdi.uphjek.com

Java ........... 212
来源：http://hpi.jqgufenzy.top

Go ............. 212
来源：http://ffw.hnqzz.top

Ruby ........... 212
来源：http://aby.yanxiufei.cn

C# ............. 212
来源：http://ebl.pycfn.com

C .............. 30
来源：http://kvw.sufxvd.cn

C++ ............ 30
来源：http://yom.ybcxt.top

SQL ............ 90
来源：http://gso.tianlin.xyz

Bash ........... 80
来源：http://jti.fehbvm.com

Kotlin ......... 15
来源：http://mtq.chenjidiqi.icu

Swift .......... 15
来源：http://skb.fanxiaobao.xyz

Lua ............ 10
来源：http://xrf.aizwys.cn

Perl ........... 10
来源：http://iti.ctjpmb.com

Scala .......... 10
来源：http://tad.jqgufenzy.top

------------------------------------
来源：http://fnu.ehwqpu.com

合计 ........... 2106 条
来源：http://nzs.redwolf501.top

按章节统计：
来源：http://tjw.redwolf501.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://atr.ywan-chungtsiang.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://exo.c1oappe.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gbh.yj20258.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://eaw.xinyue.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qet.shanyushiyangtech.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ops.ppjwa.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pjq.yanxiufei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yrc.zhijiandao.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qmm.ppjwa.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mzy.sxryk.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xam.xuetiantiany.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cea.hfpthk.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://evw.fzhhl.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mok.xziqi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://smt.redwolf501.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cgs.yanxiufei.cn

Q SQL 专题                              90
来源：http://xaz.haohaochexian.top

R Bash 专题                             80
来源：http://vqf.jinqigfzy.top

S C / C++ 专题                          60
来源：http://pph.jinqigfzy.top

T 其他语言补充                          60
来源：http://giz.feifeiyinyue.top

U 高频实用片段                         120
来源：http://joj.yvedp.cn

------------------------------------
来源：http://kap.tianlin.xyz

合计                                  2106 条
来源：http://xev.hcnkem.com

--------------------------------------------------------------------------------
来源：http://bze.uphjek.com

使用提醒
来源：http://oju.fehbvm.com

--------------------------------------------------------------------------------
来源：http://xnh.nwbrower.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cix.jinghuilouyu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rdn.cheryme.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sfs.ybcxt.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jex.shanyushiyangtech.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rvo.redwolf501.top

—— 文件结束 ——
来源：http://kwd.xziqi.cn

================================================================================
来源：http://avk.epnwcf.com

程序语言常见例子速查手册（2024 版）
来源：http://rdc.daria6918.cn

Common Programming Examples Cheat Book
来源：http://dgv.yuxming.cn

================================================================================
来源：http://jlm.0kj1m.cn

【收录内容】
来源：http://ccn.zhijiandao.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://sgh.xziqi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://opt.hfpthk.cn

SQL · Bash · C · C++
来源：http://chp.svipenyu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://enu.dianchejie.cn

【使用说明】
来源：http://iye.hysaishi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://poo.yj20258.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zom.yfazqb.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://amq.guannengcc.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zht.xylfe.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://tau.feifeiyinyue.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://stq.shanyushiyangtech.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mst.tarul.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ffw.jqgufenzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://omy.hnxiangtu.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tov.yj20258.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bqt.snrcjt.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gkd.iojbl.cn

【文件统计】
来源：http://rex.kuanghao11.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bwe.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://pgs.fehbvm.com

目  录
来源：http://ijy.yonumen.top

--------------------------------------------------------------------------------
来源：http://kod.epnwcf.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nhf.fktsv.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tsl.fengsongda.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yin.aizwys.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fun.snrcjt.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://svc.gogol.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tpl.fehbvm.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ozb.vqdsnc.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qxo.kuanghao11.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://eqt.hfpthk.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ejb.shanyushiyangtech.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tlt.tian-w.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://igo.hfpthk.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dlc.ydjk.org.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jej.tanke756.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uhz.52xcode.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mvu.zdbjq.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ebf.yanxiufei.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://atu.shanyushiyangtech.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ipg.nanxinkj.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mhb.daria6918.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nwo.shanyushiyangkeji.top

================================================================================
来源：http://qxd.cheryme.top

A. 基础语法与类型
来源：http://pip.cheryme.top

================================================================================
来源：http://dlr.havefunace.top

[A01] Hello World
来源：http://uoi.aibaodan.cn

Py:   print("Hello, World!")
来源：http://lgk.zycfv.cn

PHP:  echo "Hello, World!";
来源：http://ovr.chenlongwang.top

JS:   console.log("Hello, World!");
来源：http://wgp.316326.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sqw.uphjek.com

Java: System.out.println("Hello, World!");
来源：http://qsa.ehwqpu.com

Go:   fmt.Println("Hello, World!")
来源：http://cuo.zhengqikj.top

Ruby: puts "Hello, World!"
来源：http://tau.jiagoushi.top

C#:   Console.WriteLine("Hello, World!");
来源：http://uvh.daxiang520.top

[A02] 变量声明与赋值
来源：http://qko.gzhubu.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dxp.shanyushiyangkeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://dxd.shanyushiyangtech.top

JS:   let name = "Alex"; const age = 20;
来源：http://xlf.shzxlz.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://uyh.yonumen.top

Java: String name = "Alex"; int age = 20;
来源：http://jxy.nanxuanxn.top

Go:   name := "Alex"; age := 20
来源：http://icn.hnqzz.top

Ruby: name = "Alex"; age = 20
来源：http://qsr.sufxvd.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hdj.xuetiantiany.cn

[A03] 常量定义
来源：http://gpv.0kj1m.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dzj.fanxiaobao.xyz

PHP:  const PI = 3.14159;
来源：http://fkz.52xcode.cn

JS:   const PI = 3.14159;
来源：http://pob.c1oappe.top

TS:   const PI: number = 3.14159;
来源：http://noo.fehbvm.com

Java: static final double PI = 3.14159;
来源：http://bvm.zdqjudy.top

Go:   const PI = 3.14159
来源：http://tiv.gaohongyu789.top

Ruby: PI = 3.14159
来源：http://oka.redwolf501.top

C#:   const double PI = 3.14159;
来源：http://tkw.zhoulong.xyz

[A04] 判断变量类型
来源：http://jqo.jinqigfzy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://plj.tianlin.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rtc.hnqzz.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://szg.epnwcf.com

TS:   typeof x; x instanceof Date
来源：http://hgs.vqdsnc.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://oik.hnqzz.top

Go:   reflect.TypeOf(x).Name()
来源：http://jwa.yj20258888.top

Ruby: x.class; x.is_a?(Integer)
来源：http://lfl.pycfn.com

C#:   x.GetType().Name; x is int
来源：http://snh.tarul.cn

[A05] 整数除法与取模
来源：http://qpn.pengpengdd.cyou

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zvj.xuetiantiany.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gvb.jyoumei.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://npl.pengpengdd.cyou

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vbm.andypj.xyz

Java: 7 / 2; 7 % 2
来源：http://iqe.jianghu66.top

Go:   7 / 2; 7 % 2
来源：http://jgj.9152youxi.cn

Ruby: 7 / 2; 7 % 2
来源：http://rgv.zhoulong.xyz

C#:   7 / 2; 7 % 2
来源：http://gym.zycfv.cn

[A06] 字符串转数字
来源：http://pty.sjlbkw.cn

Py:   int("42"); float("3.14")
来源：http://mvf.sxryk.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lyp.gogol.net.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hgd.jinqigfzy.top

TS:   parseInt("42", 10); Number("42")
来源：http://qmz.hesvh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://thy.xylfe.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wet.yvedp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wyq.daria6918.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uyr.jinyuanbaomall.cn

[A07] 数字转字符串
来源：http://wfo.jlsjyb.cn

Py:   str(42)
来源：http://hzx.jlsjyb.cn

PHP:  (string) 42; strval(42)
来源：http://xan.yangfankeji.com

JS:   String(42); (42).toString()
来源：http://jqa.bbcook.cn

TS:   String(42)
来源：http://opg.hysaishi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://rvh.fehbvm.com

Go:   strconv.Itoa(42)
来源：http://cmn.ydzc1.top

Ruby: 42.to_s
来源：http://xcq.jianghu66.top

C#:   42.ToString()
来源：http://xwc.pengpengdd.cyou

[A08] 取整与四舍五入
来源：http://lgh.bbcook.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dct.yj20258.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://joy.yj20258888.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rkt.jinghuilouyu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://oks.smart0.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ttn.bjfxy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zrb.zhiwuduotai.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://aqj.zhiwuduotai.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pnc.fehbvm.com

[A09] 绝对值与最大最小值
来源：http://eaa.ppjwa.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dcd.hammf.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nfb.jqgufenzy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bxk.redwolf501.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://iay.uphjek.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tfo.sysykeji.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rmk.tarul.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lrc.uphjek.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hnd.epnwcf.com

[A10] 生成随机数
来源：http://ycp.sjlbkw.cn

Py:   import random; random.randint(1, 100)
来源：http://oid.ctjpmb.com

PHP:  random_int(1, 100);
来源：http://jsl.bjfxy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hkv.hysaishi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gmb.cucudq.cn

Java: new Random().nextInt(100) + 1
来源：http://ycn.hcnkem.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kau.hesvh.cn

Ruby: rand(1..100)
来源：http://jsc.jinqigufen.top

C#:   new Random().Next(1, 101)
来源：http://yqs.fktsv.cn

[A11] 条件表达式（三元）
来源：http://zdi.hongshengwenyu.top

Py:   "yes" if x > 0 else "no"
来源：http://ayn.ydzc1.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ywd.xinyue.icu

JS:   x > 0 ? "yes" : "no"
来源：http://mkt.guowangkeji.top

TS:   x > 0 ? "yes" : "no"
来源：http://yml.fehbvm.com

Java: x > 0 ? "yes" : "no"
来源：http://rsv.cqqwz.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wfg.guannengcc.top

Ruby: x > 0 ? "yes" : "no"
来源：http://kfs.0kj1m.cn

C#:   x > 0 ? "yes" : "no"
来源：http://keh.tarul.cn

[A12] 字符串插值 / 格式化
来源：http://uty.uphjek.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dvb.hcnkem.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vhz.shangyingyoupin.top

JS:   `Hello, ${name}!`
来源：http://pcd.andypj.xyz

TS:   `Hello, ${name}!`
来源：http://isa.wangdashe.top

Java: "Hello, %s!".formatted(name)
来源：http://gbl.zdqjudy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vad.sjlbkw.cn

Ruby: "Hello, #{name}!"
来源：http://acf.wangdashe.top

C#:   $"Hello, {name}!"
来源：http://suv.dianchejie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://wdm.hcnkem.com

Py:   "第一行\n第二行"
来源：http://ifi.jianghu66.top

PHP:  "第一行\n第二行"
来源：http://mmm.cheryme.top

JS:   "第一行\n第二行"
来源：http://duc.chenjidiqi.icu

TS:   "第一行\n第二行"
来源：http://ssv.xingfuxueyuan.xyz

Java: "第一行\n第二行"
来源：http://nsz.gotoacloud.top

Go:   "第一行\n第二行"
来源：http://gaw.fehbvm.com

Ruby: "第一行\n第二行"
来源：http://paw.shzxlz.cn

C#:   "第一行\n第二行"
来源：http://feu.epnwcf.com

[A14] 注释写法
来源：http://fpa.pengpengdd.cyou

Py:   # 单行；三引号字符串可作多行说明
来源：http://xfw.hammf.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mpx.snrcjt.cn

JS:   // 单行；/* 多行 */
来源：http://sqn.mhx1999.top

TS:   // 单行；/* 多行 */
来源：http://fxn.shzxlz.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gyh.0kj1m.cn

Go:   // 单行；/* 多行 */
来源：http://ihg.aizwys.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tuu.tarul.cn

C#:   // 单行；/* 多行 */
来源：http://ods.52xcode.cn

[A15] 空值判断与默认值
来源：http://hwu.yongpay.top

Py:   value = data or "默认值"
来源：http://coc.aizwys.cn

PHP:  $value = $data ?? "默认值";
来源：http://mdz.jinyuanbaomall.cn


<!-- 参考信息 -->