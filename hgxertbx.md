代发 wailian999

[U85] JS：可选链
来源：http://dzl.ivvv.top

a?.b?.c
来源：http://zmb.hammf.cn

[U86] JS：空值合并
来源：http://ajl.nwbrower.top

a ?? b
来源：http://vrf.yj20258.top

[U87] JS：解构默认值
来源：http://sma.gaohongyu789.top

const { a = 1, b = 2 } = obj;
来源：http://dfw.haohaochexian.top

[U88] JS：对象展开合并
来源：http://qac.jianghu66.top

{ ...a, ...b }
来源：http://jcx.iojbl.cn

[U89] JS：数组去重
来源：http://vhq.ywan-chungtsiang.top

[...new Set(arr)]
来源：http://ahi.ctjpmb.com

[U90] JS：数字数组排序
来源：http://hyz.mhx1999.top

[...arr].sort((a, b) => a - b)
来源：http://hya.fehbvm.com

[U91] JS：对象键值遍历
来源：http://qul.daria6918.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://aiv.yvedp.cn

[U92] JS：深拷贝
来源：http://jmg.gotoacloud.top

structuredClone(obj)
来源：http://nmf.xziqi.cn

[U93] JS：模板字符串
来源：http://zhn.xuanzx.com

`共 ${n} 条`
来源：http://fau.bjfxy.top

[U94] JS：箭头函数
来源：http://jcy.andypj.xyz

const double = x => x * 2;
来源：http://pne.jqgufenzy.top

[U95] JS：Promise 包装
来源：http://ivu.zhijiandao.cn

new Promise((resolve, reject) => {})
来源：http://emp.yueranfly.top

[U96] JS：async/await 与异常
来源：http://kdt.xingfuxueyuan.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://upn.jianghu66.top

[U97] JS：并发请求
来源：http://vpa.yj20258.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://pzx.hongshengwenyu.top

[U98] JS：fetch 带 JSON
来源：http://prl.fzhhl.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://agn.9152youxi.cn

[U99] JS：事件监听
来源：http://unq.aibaodan.cn

el.addEventListener("click", e => {})
来源：http://gvm.aibaodan.cn

[U100] JS：DOM 查询
来源：http://neq.pycfn.com

document.querySelector(".item")
来源：http://tkv.hysaishi.cn

[U101] JS：classList 操作
来源：http://zrt.jinqigufen.top

el.classList.toggle("active")
来源：http://gog.jiagoushi.top

[U102] JS：本地存储
来源：http://uxv.xylfe.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wad.zhongyouzk.top

[U103] JS：定时器
来源：http://rom.smart0.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pvc.hywenlv.cn

[U104] JS：防抖
来源：http://nae.nanxuanxn.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qok.daria6918.cn

[U105] JS：节流
来源：http://aks.cqqwz.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ita.yongpay.top

[U106] JS：日期格式化
来源：http://vrl.jiagoushi.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cxk.fehbvm.com

[U107] JS：数字千分位
来源：http://abq.ivvv.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qcc.gaohongyu789.top

[U108] JS：随机整数
来源：http://kvt.9152youxi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://muf.cheryme.top

[U109] JS：数组分组
来源：http://blk.vehdjk.com

Object.groupBy(arr, x => x.type)
来源：http://tyj.birdmap.top

[U110] JS：数组分块
来源：http://ksu.iojbl.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oxr.havefunace.top

[U111] JS：对象转 Map
来源：http://hqh.ywan-chungtsiang.top

new Map(Object.entries(obj))
来源：http://dni.tarul.cn

[U112] JS：字符串补位
来源：http://dry.yvedp.cn

"7".padStart(3, "0")
来源：http://mhs.tian-w.cn

[U113] JS：正则替换全部
来源：http://fdh.snrcjt.cn

s.replaceAll("a", "b")
来源：http://ddh.jinqigfzy.top

[U114] JS：JSON 深比较
来源：http://qxx.shzxlz.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zng.yongpay.top

[U115] JS：生成 UUID
来源：http://wow.sweek.top

crypto.randomUUID()
来源：http://aol.chenzaomai.com

[U116] JS：类型检查（JSDoc）
来源：http://rpz.gotoacloud.top

/** @param {string} name */ function f(name) {}
来源：http://xfj.shzxlz.cn

[U117] JS：单元测试
来源：http://xkl.tarul.cn

npm i -D vitest;  npx vitest
来源：http://ibl.kuanghao11.cn

[U118] JS：开发服务器
来源：http://qdo.hammf.cn

npm i -D vite;  npx vite
来源：http://fmk.cdnleiting.top

[U119] JS：生产构建
来源：http://liw.jinyuanbaomall.cn

npx vite build
来源：http://rll.yj202588.top

[U120] JS：读取环境变量（Vite）
来源：http://abn.gzhubu.top

import.meta.env.VITE_API_URL
来源：http://yaz.ivvv.top

================================================================================
来源：http://smd.vehdjk.com

统计汇总
来源：http://vac.9152youxi.cn

================================================================================
来源：http://aym.sjlbkw.cn

按语言统计（条）：
来源：http://jny.fzhhl.top

Python ......... 252
来源：http://hud.sxryk.cn

PHP ............ 252
来源：http://pgq.xuetiantiany.cn

JavaScript ..... 252
来源：http://yeb.cheryme.top

TypeScript ..... 212
来源：http://tfl.pycfn.com

Java ........... 212
来源：http://goo.fehbvm.com

Go ............. 212
来源：http://ifl.wangshuangyany.cn

Ruby ........... 212
来源：http://huq.iojbl.cn

C# ............. 212
来源：http://lij.xuetiantiany.cn

C .............. 30
来源：http://ttp.zhongyouzk.top

C++ ............ 30
来源：http://fso.ydjk.org.cn

SQL ............ 90
来源：http://fgy.quarkkingdee.top

Bash ........... 80
来源：http://ygs.daria6918.cn

Kotlin ......... 15
来源：http://ocy.ehwqpu.com

Swift .......... 15
来源：http://fqk.fehbvm.com

Lua ............ 10
来源：http://cko.zycfv.cn

Perl ........... 10
来源：http://des.gogol.net.cn

Scala .......... 10
来源：http://mtf.hnxiangtu.top

------------------------------------
来源：http://osd.hesvh.cn

合计 ........... 2106 条
来源：http://use.hesvh.cn

按章节统计：
来源：http://tcq.epnwcf.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dty.ydjk.org.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cms.zhijiandao.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kbd.yonumen.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lsb.quarkkingdee.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nid.jqgfzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://num.yuxming.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dvf.zhiwuduotai.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://koz.hesvh.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ezo.birdmap.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ayk.mhx1999.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fno.xinyue.icu

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ela.redwolf501.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://igw.guowangkeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://elj.nanxuanxn.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://igh.ydjk.org.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xjl.daria6918.cn

Q SQL 专题                              90
来源：http://kdh.haohaochexian.top

R Bash 专题                             80
来源：http://oxt.jyoumei.cn

S C / C++ 专题                          60
来源：http://vvs.cqqwz.cn

T 其他语言补充                          60
来源：http://kou.zhoulong.xyz

U 高频实用片段                         120
来源：http://zkl.dianchejie.cn

------------------------------------
来源：http://lms.cashguo.top

合计                                  2106 条
来源：http://qmv.zycfv.cn

--------------------------------------------------------------------------------
来源：http://hph.guowangkeji.top

使用提醒
来源：http://fpd.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://obc.yj20258888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ohp.zdqjudy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tbl.guowangkeji.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://chd.ydzc1.top

在旧版本上使用前请先确认语法支持情况。
来源：http://chj.ctjpmb.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rma.quarkkingdee.top

—— 文件结束 ——
来源：http://taz.hfpthk.cn

================================================================================
来源：http://yuq.epnwcf.com

程序语言常见例子速查手册（2024 版）
来源：http://ylu.guannengcc.top

Common Programming Examples Cheat Book
来源：http://phe.chenzaomai.com

================================================================================
来源：http://hgs.dianchejie.cn

【收录内容】
来源：http://oub.tanke756.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://owo.yfazqb.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ttg.ctjpmb.com

SQL · Bash · C · C++
来源：http://bql.yj20258.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ofh.gaohongyu789.top

【使用说明】
来源：http://ysu.hnxiangtu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://myt.nanxuanxn.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://luy.sxryk.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jsa.shzxlz.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pyn.yuxming.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://vjy.zhengqikj.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dod.fengsongda.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mwg.tian-w.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mpr.pycfn.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lgx.redwolf501.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wls.fehbvm.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ktv.hnxiangtu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://trz.jinqigfzy.top

【文件统计】
来源：http://mce.birdmap.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fxj.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://rkr.sweek.top

目  录
来源：http://jif.yj20258.top

--------------------------------------------------------------------------------
来源：http://aac.shangyingyoupin.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zqd.haohaochexian.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ipf.chenlongwang.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uja.fehbvm.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vkw.yongpay.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bfg.yonumen.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://obs.fktsv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cqo.yuanzhike.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bex.jinqigfzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://eoo.aibaodan.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sni.cdnleiting.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mri.ehwqpu.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tvs.zdqjudy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cne.yfazqb.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lxk.hongshengwenyu.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kos.dianchejie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fks.chenjidiqi.icu

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sij.sjlbkw.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xmk.vehdjk.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ood.xingfuxueyuan.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yiv.mhx1999.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ohg.jinghuilouyu.cn

================================================================================
来源：http://daj.gzhubu.top

A. 基础语法与类型
来源：http://bvu.zhixingplan.top

================================================================================
来源：http://wfk.shanyushiyangkeji.top

[A01] Hello World
来源：http://efp.hcnkem.com

Py:   print("Hello, World!")
来源：http://mdb.nanxuanxn.top

PHP:  echo "Hello, World!";
来源：http://djz.aibaodan.cn

JS:   console.log("Hello, World!");
来源：http://vjo.0kj1m.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ube.yongpay.top

Java: System.out.println("Hello, World!");
来源：http://qwq.shzxlz.cn

Go:   fmt.Println("Hello, World!")
来源：http://nnr.wangdashe.top

Ruby: puts "Hello, World!"
来源：http://kht.ybcxt.top

C#:   Console.WriteLine("Hello, World!");
来源：http://avr.0kj1m.cn

[A02] 变量声明与赋值
来源：http://drv.jqgfzy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pnb.snrcjt.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qqs.pycfn.com

JS:   let name = "Alex"; const age = 20;
来源：http://wou.cheryme.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vgd.vqdsnc.cn

Java: String name = "Alex"; int age = 20;
来源：http://hyw.snrcjt.cn

Go:   name := "Alex"; age := 20
来源：http://syb.316326.xyz

Ruby: name = "Alex"; age = 20
来源：http://xga.52xcode.cn

C#:   string name = "Alex"; int age = 20;
来源：http://oyk.hesvh.cn

[A03] 常量定义
来源：http://bzu.ydzc1.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kmc.shuidangran.top

PHP:  const PI = 3.14159;
来源：http://gmz.jlsjyb.cn

JS:   const PI = 3.14159;
来源：http://tad.dianchejie.cn

TS:   const PI: number = 3.14159;
来源：http://yzy.jqgfzy.top

Java: static final double PI = 3.14159;
来源：http://qyl.gotoacloud.top

Go:   const PI = 3.14159
来源：http://oyh.havefunace.top

Ruby: PI = 3.14159
来源：http://rhw.ydjk.org.cn

C#:   const double PI = 3.14159;
来源：http://cbx.haohaochexian.top

[A04] 判断变量类型
来源：http://vgj.zdbjq.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://equ.chenzaomai.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wzc.aizwys.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zmp.aizwys.cn

TS:   typeof x; x instanceof Date
来源：http://hmo.feifeiyinyue.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vyg.xuanzx.com

Go:   reflect.TypeOf(x).Name()
来源：http://evj.yj20258.top

Ruby: x.class; x.is_a?(Integer)
来源：http://wma.zdqjudy.top

C#:   x.GetType().Name; x is int
来源：http://nnt.jlsjyb.cn

[A05] 整数除法与取模
来源：http://thx.ppjwa.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://czo.hcnkem.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://sqt.feifeiyinyue.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://otp.yj20258888.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bis.svipenyu.cn

Java: 7 / 2; 7 % 2
来源：http://kyq.zhiwuduotai.top

Go:   7 / 2; 7 % 2
来源：http://esq.sysykeji.top

Ruby: 7 / 2; 7 % 2
来源：http://vte.ywan-chungtsiang.top

C#:   7 / 2; 7 % 2
来源：http://odd.kuanghao11.cn

[A06] 字符串转数字
来源：http://zpe.daxiang520.top

Py:   int("42"); float("3.14")
来源：http://oqe.c1oappe.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qks.nanxinkj.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gem.tian-w.cn

TS:   parseInt("42", 10); Number("42")
来源：http://zzt.yj202588.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://obn.c1oappe.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://two.quarkkingdee.top

Ruby: "42".to_i; "3.14".to_f
来源：http://vwe.epnwcf.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pft.316326.xyz

[A07] 数字转字符串
来源：http://qzz.xinyue.icu

Py:   str(42)
来源：http://waw.nanxuanxn.top

PHP:  (string) 42; strval(42)
来源：http://gef.yueranfly.top

JS:   String(42); (42).toString()
来源：http://onp.chenjidiqi.icu

TS:   String(42)
来源：http://jnk.chenlongwang.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://cax.sufxvd.cn

Go:   strconv.Itoa(42)
来源：http://vcl.xuetiantiany.cn

Ruby: 42.to_s
来源：http://pho.jyoumei.cn

C#:   42.ToString()
来源：http://ltv.sweek.top

[A08] 取整与四舍五入
来源：http://ked.hesvh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://umy.zhaomingkeji.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kwy.zhaomingkeji.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nlz.tian-w.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://meg.tian-w.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qqq.havefunace.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ana.shangyingyoupin.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ear.cashguo.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wmu.xuanzx.com

[A09] 绝对值与最大最小值
来源：http://lmo.yvedp.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hme.svipenyu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yhw.sysykeji.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vui.shanyushiyangkeji.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lts.ctjpmb.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jkz.daxiang520.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://eou.gaohongyu789.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fxn.hcnkem.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wrx.zhengqikj.top

[A10] 生成随机数
来源：http://mzu.cucudq.cn

Py:   import random; random.randint(1, 100)
来源：http://rol.redwolf501.top

PHP:  random_int(1, 100);
来源：http://ziq.nanxinkj.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kpc.tianlin.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fyd.ivvv.top

Java: new Random().nextInt(100) + 1
来源：http://vnp.zycfv.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tue.sjlbkw.cn

Ruby: rand(1..100)
来源：http://exo.zdbjq.cn

C#:   new Random().Next(1, 101)
来源：http://esn.snrcjt.cn

[A11] 条件表达式（三元）
来源：http://tos.zdqjudy.top

Py:   "yes" if x > 0 else "no"
来源：http://yxw.yj20258888.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://djs.meibo888.top

JS:   x > 0 ? "yes" : "no"
来源：http://vlr.zdbjq.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vhe.shanyushiyangtech.top

Java: x > 0 ? "yes" : "no"
来源：http://zwf.jlsjyb.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vts.vehdjk.com

Ruby: x > 0 ? "yes" : "no"
来源：http://xhs.haohaochexian.top

C#:   x > 0 ? "yes" : "no"
来源：http://isa.kuanghao11.cn

[A12] 字符串插值 / 格式化
来源：http://xov.chenzaomai.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://awh.yueranfly.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://euj.gaohongyu789.top

JS:   `Hello, ${name}!`
来源：http://wwf.iojbl.cn

TS:   `Hello, ${name}!`
来源：http://lyp.xuanzx.com

Java: "Hello, %s!".formatted(name)
来源：http://ssy.dashuyun.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ojo.bjfxy.top

Ruby: "Hello, #{name}!"
来源：http://mra.quarkkingdee.top

C#:   $"Hello, {name}!"
来源：http://cwp.sjlbkw.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ddu.yonumen.top

Py:   "第一行\n第二行"
来源：http://myi.ydjk.org.cn

PHP:  "第一行\n第二行"
来源：http://vky.shzxlz.cn

JS:   "第一行\n第二行"
来源：http://mhl.yongpay.top

TS:   "第一行\n第二行"
来源：http://fvs.cqqwz.cn

Java: "第一行\n第二行"
来源：http://bpk.zhengqikj.top

Go:   "第一行\n第二行"
来源：http://zxn.0kj1m.cn

Ruby: "第一行\n第二行"
来源：http://fnq.hammf.cn

C#:   "第一行\n第二行"
来源：http://fis.dianchejie.cn

[A14] 注释写法
来源：http://peu.yvedp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wet.jlsjyb.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://nbk.nanxuanxn.top

JS:   // 单行；/* 多行 */
来源：http://hyg.shuidangran.top


<!-- 参考信息 -->