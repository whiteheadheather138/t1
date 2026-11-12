代发 wailian999

[U93] JS：模板字符串
来源：http://llw.hysaishi.cn

`共 ${n} 条`
来源：http://xem.hongshengwenyu.top

[U94] JS：箭头函数
来源：http://kyq.birdmap.top

const double = x => x * 2;
来源：http://rtg.quarkkingdee.top

[U95] JS：Promise 包装
来源：http://xpv.ppjwa.cn

new Promise((resolve, reject) => {})
来源：http://vst.shzxlz.cn

[U96] JS：async/await 与异常
来源：http://buf.meibo888.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pen.mhx1999.top

[U97] JS：并发请求
来源：http://hxz.jinqigfzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://nlr.xuetiantiany.cn

[U98] JS：fetch 带 JSON
来源：http://pnz.sjlbkw.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ejt.bjfxy.top

[U99] JS：事件监听
来源：http://xjy.nanxuanxn.top

el.addEventListener("click", e => {})
来源：http://qsy.hesvh.cn

[U100] JS：DOM 查询
来源：http://qia.bbcook.cn

document.querySelector(".item")
来源：http://uks.iojbl.cn

[U101] JS：classList 操作
来源：http://omc.nwbrower.top

el.classList.toggle("active")
来源：http://gnp.zycfv.cn

[U102] JS：本地存储
来源：http://kfq.nanxuanxn.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://oim.zycfv.cn

[U103] JS：定时器
来源：http://zbc.xuanzx.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://piz.zhoulong.xyz

[U104] JS：防抖
来源：http://cjz.0kj1m.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cwh.nanxinkj.top

[U105] JS：节流
来源：http://veb.mhx1999.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://grs.yangfankeji.com

[U106] JS：日期格式化
来源：http://xgy.gzhubu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pmx.zhongyouzk.top

[U107] JS：数字千分位
来源：http://naw.havefunace.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xmx.aibaodan.cn

[U108] JS：随机整数
来源：http://seb.xylfe.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zfj.jinqigfzy.top

[U109] JS：数组分组
来源：http://bkv.sufxvd.cn

Object.groupBy(arr, x => x.type)
来源：http://mqj.meibo888.top

[U110] JS：数组分块
来源：http://ygr.sweek.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jmk.0kj1m.cn

[U111] JS：对象转 Map
来源：http://qgl.hnqzz.top

new Map(Object.entries(obj))
来源：http://tco.yangfankeji.com

[U112] JS：字符串补位
来源：http://peb.yuxming.cn

"7".padStart(3, "0")
来源：http://pns.xuetiantiany.cn

[U113] JS：正则替换全部
来源：http://dnc.andypj.xyz

s.replaceAll("a", "b")
来源：http://mvn.tarul.cn

[U114] JS：JSON 深比较
来源：http://mvp.shangyingyoupin.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ojv.ctjpmb.com

[U115] JS：生成 UUID
来源：http://baj.zhoulong.xyz

crypto.randomUUID()
来源：http://gea.birdmap.top

[U116] JS：类型检查（JSDoc）
来源：http://bam.xuetiantiany.cn

/** @param {string} name */ function f(name) {}
来源：http://vjt.yueranfly.top

[U117] JS：单元测试
来源：http://yvn.sufxvd.cn

npm i -D vitest;  npx vitest
来源：http://qht.smart0.xyz

[U118] JS：开发服务器
来源：http://fgb.zhengqikj.top

npm i -D vite;  npx vite
来源：http://kgv.shzxlz.cn

[U119] JS：生产构建
来源：http://mkm.zdbjq.cn

npx vite build
来源：http://caj.snrcjt.cn

[U120] JS：读取环境变量（Vite）
来源：http://voo.0kj1m.cn

import.meta.env.VITE_API_URL
来源：http://kkq.yanxiufei.cn

================================================================================
来源：http://can.xylfe.cn

统计汇总
来源：http://leu.nanxinkj.top

================================================================================
来源：http://pzj.cucudq.cn

按语言统计（条）：
来源：http://jjz.hysaishi.cn

Python ......... 252
来源：http://oxl.wangdashe.top

PHP ............ 252
来源：http://wjb.feifeiyinyue.top

JavaScript ..... 252
来源：http://pge.hongshengwenyu.top

TypeScript ..... 212
来源：http://tyf.chenjidiqi.icu

Java ........... 212
来源：http://uxp.zhixingplan.top

Go ............. 212
来源：http://fsz.daria6918.cn

Ruby ........... 212
来源：http://mqa.yangfankeji.com

C# ............. 212
来源：http://lwu.havefunace.top

C .............. 30
来源：http://ehc.fktsv.cn

C++ ............ 30
来源：http://zzz.pengpengdd.cyou

SQL ............ 90
来源：http://tpi.cheryme.top

Bash ........... 80
来源：http://uxe.shanyushiyangtech.top

Kotlin ......... 15
来源：http://xel.cucudq.cn

Swift .......... 15
来源：http://toa.nanxuanxn.top

Lua ............ 10
来源：http://vgk.yj20258888.top

Perl ........... 10
来源：http://hhe.bbcook.cn

Scala .......... 10
来源：http://xcp.hysaishi.cn

------------------------------------
来源：http://xvn.zhaomingkeji.xyz

合计 ........... 2106 条
来源：http://eqn.hammf.cn

按章节统计：
来源：http://pkj.jinghuilouyu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://skd.pycfn.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hzr.cucudq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gxh.jinqigfzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dzm.aibaodan.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ixe.redwolf501.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qly.nanxinkj.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uxp.fzhhl.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ule.hongshengwenyu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bfg.tianlin.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zlq.fzhhl.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ibr.52xcode.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://abv.yueranfly.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kkr.chenlongwang.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xue.snrcjt.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nrt.jianghu66.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nyc.shanyushiyangkeji.top

Q SQL 专题                              90
来源：http://zcw.tianlin.xyz

R Bash 专题                             80
来源：http://xvu.snrcjt.cn

S C / C++ 专题                          60
来源：http://nng.pengpengdd.cyou

T 其他语言补充                          60
来源：http://ruf.ydjk.org.cn

U 高频实用片段                         120
来源：http://gwn.yueranfly.top

------------------------------------
来源：http://hcm.52xcode.cn

合计                                  2106 条
来源：http://wcs.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://zvg.haohaochexian.top

使用提醒
来源：http://uqd.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://qkw.shanyushiyangkeji.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zrm.yj202588.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://iig.shuidangran.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yyq.jinqigfzy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://igf.gzhubu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tab.jlsjyb.cn

—— 文件结束 ——
来源：http://cks.tarul.cn

================================================================================
来源：http://qel.tarul.cn

程序语言常见例子速查手册（2024 版）
来源：http://pjk.redwolf501.top

Common Programming Examples Cheat Book
来源：http://fry.quarkkingdee.top

================================================================================
来源：http://xmz.quarkkingdee.top

【收录内容】
来源：http://ixm.shzxlz.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mnr.shangyingyoupin.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lfh.redwolf501.top

SQL · Bash · C · C++
来源：http://vih.chenjidiqi.icu

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jwt.hywenlv.cn

【使用说明】
来源：http://jls.tian-w.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nut.svipenyu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kye.cdnleiting.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://eut.jinyuanbaomall.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://buj.jiagoushi.top

Bash:  Shell         C:     C             C++:   C++
来源：http://yks.xinyue.icu

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wca.jiagoushi.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://oli.nanxuanxn.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ale.hfpthk.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nlo.yj20258.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bjc.zdbjq.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gah.yj20258888.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://oqo.yonumen.top

【文件统计】
来源：http://obf.vehdjk.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dse.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://fqa.tianlin.xyz

目  录
来源：http://tij.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://vyr.fanxiaobao.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wbf.jiagoushi.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vuc.zdqjudy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jom.zycfv.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wld.nanxuanxn.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bex.xylfe.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://muq.yangfankeji.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://szf.0kj1m.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qob.daxiang520.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tel.guowangkeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vat.guowangkeji.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cyg.ydzc1.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://haw.hywenlv.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://itr.jianghu66.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://szj.jinyuanbaomall.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hgp.hnqzz.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dcm.aizwys.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qha.aibaodan.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vks.fzhhl.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bhc.guannengcc.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://muo.jianghu66.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mfa.jinghuilouyu.cn

================================================================================
来源：http://zbt.yongpay.top

A. 基础语法与类型
来源：http://odj.fehbvm.com

================================================================================
来源：http://axi.fehbvm.com

[A01] Hello World
来源：http://khq.jqgufenzy.top

Py:   print("Hello, World!")
来源：http://rzq.pengpengdd.cyou

PHP:  echo "Hello, World!";
来源：http://ynd.vehdjk.com

JS:   console.log("Hello, World!");
来源：http://znc.sysykeji.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ypa.yfazqb.com

Java: System.out.println("Hello, World!");
来源：http://cch.dianchejie.cn

Go:   fmt.Println("Hello, World!")
来源：http://wio.hcnkem.com

Ruby: puts "Hello, World!"
来源：http://skb.ehwqpu.com

C#:   Console.WriteLine("Hello, World!");
来源：http://jyq.fktsv.cn

[A02] 变量声明与赋值
来源：http://tyw.316326.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://duq.cdnleiting.top

PHP:  $name = "Alex"; $age = 20;
来源：http://umg.gzhubu.top

JS:   let name = "Alex"; const age = 20;
来源：http://fsc.nanxinkj.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rab.ctjpmb.com

Java: String name = "Alex"; int age = 20;
来源：http://got.xinyue.icu

Go:   name := "Alex"; age := 20
来源：http://diz.xingfuxueyuan.xyz

Ruby: name = "Alex"; age = 20
来源：http://mmv.meibo888.top

C#:   string name = "Alex"; int age = 20;
来源：http://zcm.yj20258.top

[A03] 常量定义
来源：http://smt.jiagoushi.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hex.sxryk.cn

PHP:  const PI = 3.14159;
来源：http://grr.zhijiandao.cn

JS:   const PI = 3.14159;
来源：http://nkg.gaohongyu789.top

TS:   const PI: number = 3.14159;
来源：http://qpf.sweek.top

Java: static final double PI = 3.14159;
来源：http://wmo.yonumen.top

Go:   const PI = 3.14159
来源：http://eqa.vqdsnc.cn

Ruby: PI = 3.14159
来源：http://vvo.chenzaomai.com

C#:   const double PI = 3.14159;
来源：http://uex.tian-w.cn

[A04] 判断变量类型
来源：http://wld.uphjek.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://znr.shanyushiyangtech.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ddr.yonumen.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ptl.zhiwuduotai.top

TS:   typeof x; x instanceof Date
来源：http://tbn.jinyuanbaomall.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zaz.316326.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://bsp.ivvv.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ymn.dianchejie.cn

C#:   x.GetType().Name; x is int
来源：http://xza.jinghuilouyu.cn

[A05] 整数除法与取模
来源：http://kbj.ppjwa.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://arn.fzhhl.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://djg.shuidangran.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://plk.jiagoushi.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hsa.xuetiantiany.cn

Java: 7 / 2; 7 % 2
来源：http://vtv.cheryme.top

Go:   7 / 2; 7 % 2
来源：http://lgd.316326.xyz

Ruby: 7 / 2; 7 % 2
来源：http://mxr.svipenyu.cn

C#:   7 / 2; 7 % 2
来源：http://mpz.ehwqpu.com

[A06] 字符串转数字
来源：http://uwj.jiagoushi.top

Py:   int("42"); float("3.14")
来源：http://ars.fktsv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lky.shanyushiyangtech.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jic.ydzc1.top

TS:   parseInt("42", 10); Number("42")
来源：http://cpq.xuanzx.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bgg.sysykeji.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ses.dashuyun.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://nfc.chenzaomai.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lyj.hysaishi.cn

[A07] 数字转字符串
来源：http://ujp.zhijiandao.cn

Py:   str(42)
来源：http://apr.nanxuanxn.top

PHP:  (string) 42; strval(42)
来源：http://jva.fktsv.cn

JS:   String(42); (42).toString()
来源：http://oge.iojbl.cn

TS:   String(42)
来源：http://ias.yueranfly.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://yve.vehdjk.com

Go:   strconv.Itoa(42)
来源：http://ndi.hnqzz.top

Ruby: 42.to_s
来源：http://ttl.yongpay.top

C#:   42.ToString()
来源：http://zky.guowangkeji.top

[A08] 取整与四舍五入
来源：http://aai.hfpthk.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gyi.tian-w.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://njn.xylfe.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://psn.feifeiyinyue.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fxa.svipenyu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qzz.daria6918.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hcn.ydjk.org.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://dlj.cheryme.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xye.chenlongwang.top

[A09] 绝对值与最大最小值
来源：http://epa.svipenyu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pbz.fanxiaobao.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://omn.yanxiufei.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://iam.wangshuangyany.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nko.ehwqpu.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uis.zhijiandao.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tzy.jinqigfzy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jnp.fanxiaobao.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bzw.yj20258.top

[A10] 生成随机数
来源：http://cru.fanxiaobao.xyz

Py:   import random; random.randint(1, 100)
来源：http://jmp.cashguo.top

PHP:  random_int(1, 100);
来源：http://efi.nwbrower.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qmy.c1oappe.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tgs.shangyingyoupin.top

Java: new Random().nextInt(100) + 1
来源：http://wec.tarul.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cec.yj20258888.top

Ruby: rand(1..100)
来源：http://oow.zhengqikj.top

C#:   new Random().Next(1, 101)
来源：http://kjt.zdqjudy.top

[A11] 条件表达式（三元）
来源：http://ljw.yuanzhike.top

Py:   "yes" if x > 0 else "no"
来源：http://lwm.hywenlv.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ldv.bjfxy.top

JS:   x > 0 ? "yes" : "no"
来源：http://hby.gogol.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://eei.c1oappe.top

Java: x > 0 ? "yes" : "no"
来源：http://ijr.tianlin.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://smi.zycfv.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://kqz.ivvv.top

C#:   x > 0 ? "yes" : "no"
来源：http://eir.pycfn.com

[A12] 字符串插值 / 格式化
来源：http://rqr.dashuyun.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ije.shanyushiyangtech.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rez.havefunace.top

JS:   `Hello, ${name}!`
来源：http://xie.yvedp.cn

TS:   `Hello, ${name}!`
来源：http://zhw.vehdjk.com

Java: "Hello, %s!".formatted(name)
来源：http://yux.uphjek.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xwx.kuanghao11.cn

Ruby: "Hello, #{name}!"
来源：http://dad.jinqigfzy.top

C#:   $"Hello, {name}!"
来源：http://sii.dashuyun.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://knc.feifeiyinyue.top

Py:   "第一行\n第二行"
来源：http://ywa.jinqigufen.top

PHP:  "第一行\n第二行"
来源：http://ops.jyoumei.cn

JS:   "第一行\n第二行"
来源：http://rgw.zycfv.cn

TS:   "第一行\n第二行"
来源：http://uar.0kj1m.cn

Java: "第一行\n第二行"
来源：http://umh.c1oappe.top

Go:   "第一行\n第二行"
来源：http://dte.hysaishi.cn

Ruby: "第一行\n第二行"
来源：http://vzk.daria6918.cn

C#:   "第一行\n第二行"
来源：http://yqs.mhx1999.top

[A14] 注释写法
来源：http://pcq.52xcode.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://lwa.yuanzhike.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://fty.shangyingyoupin.top

JS:   // 单行；/* 多行 */
来源：http://kjq.yvedp.cn

TS:   // 单行；/* 多行 */
来源：http://omk.fzhhl.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ryt.zhaomingkeji.xyz

Go:   // 单行；/* 多行 */
来源：http://ptp.52xcode.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dqu.nanxinkj.top

C#:   // 单行；/* 多行 */
来源：http://nsn.dianchejie.cn

[A15] 空值判断与默认值
来源：http://fsd.iojbl.cn

Py:   value = data or "默认值"
来源：http://rgf.jinyuanbaomall.cn

PHP:  $value = $data ?? "默认值";
来源：http://fhg.jinghuilouyu.cn

JS:   const value = data ?? "默认值";
来源：http://lfa.wangdashe.top

TS:   const value = data ?? "默认值";
来源：http://twb.chenlongwang.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bse.aizwys.cn

Go:   if data == "" { data = "默认值" }
来源：http://vvj.yfazqb.com

Ruby: value = data || "默认值"
来源：http://zww.yfazqb.com

C#:   var value = data ?? "默认值";
来源：http://snh.gogol.net.cn

[A16] 真假值判断规则
来源：http://yfo.xingfuxueyuan.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vkn.cqqwz.cn


<!-- 参考信息 -->