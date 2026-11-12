代发 wailian999

[U85] JS：可选链
来源：http://fzm.gzhubu.top

a?.b?.c
来源：http://ekh.jinghuilouyu.cn

[U86] JS：空值合并
来源：http://mkj.316326.xyz

a ?? b
来源：http://cso.meibo888.top

[U87] JS：解构默认值
来源：http://lnh.yongpay.top

const { a = 1, b = 2 } = obj;
来源：http://lsj.gzhubu.top

[U88] JS：对象展开合并
来源：http://crx.zhengqikj.top

{ ...a, ...b }
来源：http://qjb.mhx1999.top

[U89] JS：数组去重
来源：http://ltb.shuidangran.top

[...new Set(arr)]
来源：http://phx.hywenlv.cn

[U90] JS：数字数组排序
来源：http://tya.cdnleiting.top

[...arr].sort((a, b) => a - b)
来源：http://sko.yongpay.top

[U91] JS：对象键值遍历
来源：http://lrd.andypj.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://keh.ydjk.org.cn

[U92] JS：深拷贝
来源：http://ppt.9152youxi.cn

structuredClone(obj)
来源：http://nqv.tian-w.cn

[U93] JS：模板字符串
来源：http://wgh.shzxlz.cn

`共 ${n} 条`
来源：http://reh.sysykeji.top

[U94] JS：箭头函数
来源：http://huk.nanxuanxn.top

const double = x => x * 2;
来源：http://los.epnwcf.com

[U95] JS：Promise 包装
来源：http://auw.shanyushiyangtech.top

new Promise((resolve, reject) => {})
来源：http://jzy.chenlongwang.top

[U96] JS：async/await 与异常
来源：http://pry.fktsv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lru.zhiwuduotai.top

[U97] JS：并发请求
来源：http://nte.pycfn.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://bsc.ppjwa.cn

[U98] JS：fetch 带 JSON
来源：http://puq.cqqwz.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://iks.daxiang520.top

[U99] JS：事件监听
来源：http://zgh.hysaishi.cn

el.addEventListener("click", e => {})
来源：http://fte.svipenyu.cn

[U100] JS：DOM 查询
来源：http://neg.fengsongda.top

document.querySelector(".item")
来源：http://uxr.cheryme.top

[U101] JS：classList 操作
来源：http://cgp.cucudq.cn

el.classList.toggle("active")
来源：http://ctp.zhiwuduotai.top

[U102] JS：本地存储
来源：http://bnz.ywan-chungtsiang.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://fcz.fktsv.cn

[U103] JS：定时器
来源：http://imd.sufxvd.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kgw.xingfuxueyuan.xyz

[U104] JS：防抖
来源：http://hsh.yfazqb.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://akg.ctjpmb.com

[U105] JS：节流
来源：http://qix.jqgfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://znp.yangfankeji.com

[U106] JS：日期格式化
来源：http://xbj.ehwqpu.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rhz.aizwys.cn

[U107] JS：数字千分位
来源：http://hwp.yvedp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hcx.ywan-chungtsiang.top

[U108] JS：随机整数
来源：http://irs.xylfe.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dsd.guannengcc.top

[U109] JS：数组分组
来源：http://umi.snrcjt.cn

Object.groupBy(arr, x => x.type)
来源：http://fge.shanyushiyangtech.top

[U110] JS：数组分块
来源：http://udp.gzhubu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nlb.hysaishi.cn

[U111] JS：对象转 Map
来源：http://cgk.redwolf501.top

new Map(Object.entries(obj))
来源：http://hih.yueranfly.top

[U112] JS：字符串补位
来源：http://gno.vehdjk.com

"7".padStart(3, "0")
来源：http://yjl.aizwys.cn

[U113] JS：正则替换全部
来源：http://apb.c1oappe.top

s.replaceAll("a", "b")
来源：http://tdl.zycfv.cn

[U114] JS：JSON 深比较
来源：http://azh.ctjpmb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://wtm.yfazqb.com

[U115] JS：生成 UUID
来源：http://sxb.xinyue.icu

crypto.randomUUID()
来源：http://qws.zdqjudy.top

[U116] JS：类型检查（JSDoc）
来源：http://ohy.hysaishi.cn

/** @param {string} name */ function f(name) {}
来源：http://ocg.zhengqikj.top

[U117] JS：单元测试
来源：http://drs.mhx1999.top

npm i -D vitest;  npx vitest
来源：http://rab.0kj1m.cn

[U118] JS：开发服务器
来源：http://epy.zhixingplan.top

npm i -D vite;  npx vite
来源：http://xna.ivvv.top

[U119] JS：生产构建
来源：http://shx.zdqjudy.top

npx vite build
来源：http://kyh.sysykeji.top

[U120] JS：读取环境变量（Vite）
来源：http://mgk.redwolf501.top

import.meta.env.VITE_API_URL
来源：http://chz.dashuyun.cn

================================================================================
来源：http://xtk.sxryk.cn

统计汇总
来源：http://uhs.gzhubu.top

================================================================================
来源：http://xiq.guannengcc.top

按语言统计（条）：
来源：http://lel.fanxiaobao.xyz

Python ......... 252
来源：http://rkm.epnwcf.com

PHP ............ 252
来源：http://scx.birdmap.top

JavaScript ..... 252
来源：http://uzz.jinqigufen.top

TypeScript ..... 212
来源：http://rkl.tian-w.cn

Java ........... 212
来源：http://aeu.sweek.top

Go ............. 212
来源：http://snh.ctjpmb.com

Ruby ........... 212
来源：http://vyc.xuetiantiany.cn

C# ............. 212
来源：http://vur.zhengqikj.top

C .............. 30
来源：http://gzx.jlsjyb.cn

C++ ............ 30
来源：http://ewg.chenlongwang.top

SQL ............ 90
来源：http://lbn.pengpengdd.cyou

Bash ........... 80
来源：http://way.hysaishi.cn

Kotlin ......... 15
来源：http://lcx.ehwqpu.com

Swift .......... 15
来源：http://gvz.hywenlv.cn

Lua ............ 10
来源：http://jlx.gzhubu.top

Perl ........... 10
来源：http://iam.jlsjyb.cn

Scala .......... 10
来源：http://exb.nwbrower.top

------------------------------------
来源：http://gse.fehbvm.com

合计 ........... 2106 条
来源：http://riz.guowangkeji.top

按章节统计：
来源：http://dse.tianlin.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qcs.shzxlz.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cqm.yuanzhike.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xja.chenzaomai.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hry.gotoacloud.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wbm.ywan-chungtsiang.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ket.bbcook.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bxa.pycfn.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tpg.sufxvd.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rgb.jinyuanbaomall.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hzq.yfazqb.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vaq.ybcxt.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rgr.shanyushiyangkeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mln.dashuyun.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kll.xuetiantiany.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bpz.zhiwuduotai.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sif.yangfankeji.com

Q SQL 专题                              90
来源：http://qoh.chenzaomai.com

R Bash 专题                             80
来源：http://erw.aibaodan.cn

S C / C++ 专题                          60
来源：http://zgg.gzhubu.top

T 其他语言补充                          60
来源：http://xef.ivvv.top

U 高频实用片段                         120
来源：http://apd.cucudq.cn

------------------------------------
来源：http://avl.hnqzz.top

合计                                  2106 条
来源：http://ast.sysykeji.top

--------------------------------------------------------------------------------
来源：http://mvq.uphjek.com

使用提醒
来源：http://vvp.hesvh.cn

--------------------------------------------------------------------------------
来源：http://ytx.yj202588.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fbo.yonumen.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vli.jinghuilouyu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mqe.zycfv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://pxn.epnwcf.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ylo.ywan-chungtsiang.top

—— 文件结束 ——
来源：http://usd.xylfe.cn

================================================================================
来源：http://ebx.chenzaomai.com

程序语言常见例子速查手册（2024 版）
来源：http://gbb.ctjpmb.com

Common Programming Examples Cheat Book
来源：http://bxr.bbcook.cn

================================================================================
来源：http://nqv.quarkkingdee.top

【收录内容】
来源：http://gzm.zdbjq.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://evr.yj20258888.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sdg.yj20258888.top

SQL · Bash · C · C++
来源：http://nub.tian-w.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://snz.shangyingyoupin.top

【使用说明】
来源：http://zov.gotoacloud.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mde.iojbl.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bmz.cdnleiting.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://eil.hywenlv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bag.yuanzhike.top

Bash:  Shell         C:     C             C++:   C++
来源：http://hyr.gzhubu.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tao.jqgfzy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://esh.fktsv.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ixs.zycfv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mnr.bjfxy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wxp.zhoulong.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vpl.dashuyun.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zqg.hesvh.cn

【文件统计】
来源：http://yot.hnxiangtu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sxg.hesvh.cn

--------------------------------------------------------------------------------
来源：http://ebd.fktsv.cn

目  录
来源：http://oka.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://tau.xylfe.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kmq.wangshuangyany.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qqw.sjlbkw.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jwk.zhoulong.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://epd.kuanghao11.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tcw.gotoacloud.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hwh.hywenlv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pdc.yj202588.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yyq.tianlin.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://khr.birdmap.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ugq.havefunace.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vbr.aibaodan.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://izx.jinyuanbaomall.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yhd.xuanzx.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hew.mhx1999.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ueu.shzxlz.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://suu.jinyuanbaomall.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://otx.316326.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://psm.andypj.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xbg.fehbvm.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ohv.zhengqikj.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uft.hcnkem.com

================================================================================
来源：http://oug.shanyushiyangtech.top

A. 基础语法与类型
来源：http://uto.zhongyouzk.top

================================================================================
来源：http://tkc.xinyue.icu

[A01] Hello World
来源：http://crf.hnxiangtu.top

Py:   print("Hello, World!")
来源：http://wgz.wangdashe.top

PHP:  echo "Hello, World!";
来源：http://atz.mhx1999.top

JS:   console.log("Hello, World!");
来源：http://rsf.xuanzx.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yrw.xinyue.icu

Java: System.out.println("Hello, World!");
来源：http://iyc.wangdashe.top

Go:   fmt.Println("Hello, World!")
来源：http://lwa.dashuyun.cn

Ruby: puts "Hello, World!"
来源：http://rsh.mhx1999.top

C#:   Console.WriteLine("Hello, World!");
来源：http://exw.sjlbkw.cn

[A02] 变量声明与赋值
来源：http://pbl.mhx1999.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ujk.andypj.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://yww.ywan-chungtsiang.top

JS:   let name = "Alex"; const age = 20;
来源：http://jjb.jinqigfzy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hhe.gzhubu.top

Java: String name = "Alex"; int age = 20;
来源：http://lyy.yj20258888.top

Go:   name := "Alex"; age := 20
来源：http://cie.zhijiandao.cn

Ruby: name = "Alex"; age = 20
来源：http://nqu.cdnleiting.top

C#:   string name = "Alex"; int age = 20;
来源：http://nsd.smart0.xyz

[A03] 常量定义
来源：http://ttk.yj20258.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fdy.feifeiyinyue.top

PHP:  const PI = 3.14159;
来源：http://vqw.shuidangran.top

JS:   const PI = 3.14159;
来源：http://seo.daria6918.cn

TS:   const PI: number = 3.14159;
来源：http://rpb.iojbl.cn

Java: static final double PI = 3.14159;
来源：http://hda.zdbjq.cn

Go:   const PI = 3.14159
来源：http://toh.jinqigufen.top

Ruby: PI = 3.14159
来源：http://vvl.yfazqb.com

C#:   const double PI = 3.14159;
来源：http://jqj.hfpthk.cn

[A04] 判断变量类型
来源：http://qlc.yj20258888.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://azb.jyoumei.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mvo.fanxiaobao.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lng.yj202588.top

TS:   typeof x; x instanceof Date
来源：http://lgs.fehbvm.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yen.yonumen.top

Go:   reflect.TypeOf(x).Name()
来源：http://qcz.yanxiufei.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dya.tian-w.cn

C#:   x.GetType().Name; x is int
来源：http://uph.shuidangran.top

[A05] 整数除法与取模
来源：http://lur.yuxming.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vhk.bbcook.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://tlx.kuanghao11.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nct.hesvh.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mkp.jqgfzy.top

Java: 7 / 2; 7 % 2
来源：http://csx.mhx1999.top

Go:   7 / 2; 7 % 2
来源：http://axd.nwbrower.top

Ruby: 7 / 2; 7 % 2
来源：http://teb.zhixingplan.top

C#:   7 / 2; 7 % 2
来源：http://arx.shuidangran.top

[A06] 字符串转数字
来源：http://nnd.zhoulong.xyz

Py:   int("42"); float("3.14")
来源：http://wud.tarul.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xbu.hongshengwenyu.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zqi.shuidangran.top

TS:   parseInt("42", 10); Number("42")
来源：http://gfn.feifeiyinyue.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://drp.jqgfzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://agl.shanyushiyangkeji.top

Ruby: "42".to_i; "3.14".to_f
来源：http://fkv.jqgfzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xwy.wangshuangyany.cn

[A07] 数字转字符串
来源：http://rab.jqgufenzy.top

Py:   str(42)
来源：http://vcy.ydzc1.top

PHP:  (string) 42; strval(42)
来源：http://lcn.hcnkem.com

JS:   String(42); (42).toString()
来源：http://eht.52xcode.cn

TS:   String(42)
来源：http://kjt.hfpthk.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://occ.zycfv.cn

Go:   strconv.Itoa(42)
来源：http://bgh.fengsongda.top

Ruby: 42.to_s
来源：http://tvr.fehbvm.com

C#:   42.ToString()
来源：http://yjd.ctjpmb.com

[A08] 取整与四舍五入
来源：http://cfb.sysykeji.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blo.haohaochexian.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vpe.xinyue.icu

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nbs.mhx1999.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ijo.yfazqb.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jdo.xylfe.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vwp.316326.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://zrs.shanyushiyangkeji.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fzu.yj20258.top

[A09] 绝对值与最大最小值
来源：http://yll.svipenyu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bwt.dashuyun.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ghp.jinqigufen.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://chm.xziqi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pmg.gotoacloud.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bqn.ctjpmb.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://trk.dashuyun.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zcu.jqgfzy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dgn.bjfxy.top

[A10] 生成随机数
来源：http://lsh.uphjek.com

Py:   import random; random.randint(1, 100)
来源：http://aot.zdqjudy.top

PHP:  random_int(1, 100);
来源：http://qmu.9152youxi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://den.uphjek.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lye.birdmap.top

Java: new Random().nextInt(100) + 1
来源：http://zlv.tarul.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tdk.wangshuangyany.cn

Ruby: rand(1..100)
来源：http://fiz.xziqi.cn

C#:   new Random().Next(1, 101)
来源：http://xpw.zhixingplan.top

[A11] 条件表达式（三元）
来源：http://sbe.ehwqpu.com

Py:   "yes" if x > 0 else "no"
来源：http://ebv.gogol.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://yam.hfpthk.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qlo.pengpengdd.cyou

TS:   x > 0 ? "yes" : "no"
来源：http://jxq.zhengqikj.top

Java: x > 0 ? "yes" : "no"
来源：http://wds.cdnleiting.top

Go:   // 无三元运算符，需用 if 语句
来源：http://xys.316326.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://ijb.sjlbkw.cn

C#:   x > 0 ? "yes" : "no"
来源：http://cnn.zhoulong.xyz

[A12] 字符串插值 / 格式化
来源：http://kve.sjlbkw.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wmt.epnwcf.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jus.jinqigfzy.top

JS:   `Hello, ${name}!`
来源：http://mdv.mhx1999.top

TS:   `Hello, ${name}!`
来源：http://egt.meibo888.top

Java: "Hello, %s!".formatted(name)
来源：http://snm.shzxlz.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mfj.birdmap.top

Ruby: "Hello, #{name}!"
来源：http://dku.guowangkeji.top

C#:   $"Hello, {name}!"
来源：http://mjt.yuanzhike.top

[A13] 多行字符串（练习 \n 转义）
来源：http://oek.yfazqb.com

Py:   "第一行\n第二行"
来源：http://dkv.aizwys.cn

PHP:  "第一行\n第二行"
来源：http://hhx.fzhhl.top

JS:   "第一行\n第二行"
来源：http://mxb.zdbjq.cn

TS:   "第一行\n第二行"
来源：http://iqh.hnxiangtu.top

Java: "第一行\n第二行"
来源：http://hva.jianghu66.top

Go:   "第一行\n第二行"
来源：http://sga.yonumen.top

Ruby: "第一行\n第二行"
来源：http://kbx.zhixingplan.top

C#:   "第一行\n第二行"
来源：http://rgg.hammf.cn

[A14] 注释写法
来源：http://tvn.ppjwa.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vqi.hammf.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://obq.cheryme.top

JS:   // 单行；/* 多行 */
来源：http://eiy.chenjidiqi.icu


<!-- 参考信息 -->