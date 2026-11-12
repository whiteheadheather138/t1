代发 wailian999

[U105] JS：节流
来源：http://tiq.daxiang520.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ruk.jinqigufen.top

[U106] JS：日期格式化
来源：http://ywx.ctjpmb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yiz.daria6918.cn

[U107] JS：数字千分位
来源：http://bfl.aizwys.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rbw.sjlbkw.cn

[U108] JS：随机整数
来源：http://xtt.wangdashe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pmd.quarkkingdee.top

[U109] JS：数组分组
来源：http://tse.zdqjudy.top

Object.groupBy(arr, x => x.type)
来源：http://wut.daria6918.cn

[U110] JS：数组分块
来源：http://oun.xuetiantiany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://byp.zdqjudy.top

[U111] JS：对象转 Map
来源：http://wur.hysaishi.cn

new Map(Object.entries(obj))
来源：http://mmv.0kj1m.cn

[U112] JS：字符串补位
来源：http://dfs.zhaomingkeji.xyz

"7".padStart(3, "0")
来源：http://klw.yj20258888.top

[U113] JS：正则替换全部
来源：http://sut.ybcxt.top

s.replaceAll("a", "b")
来源：http://rba.jinqigufen.top

[U114] JS：JSON 深比较
来源：http://hft.nanxuanxn.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://wmb.shanyushiyangtech.top

[U115] JS：生成 UUID
来源：http://itb.ydjk.org.cn

crypto.randomUUID()
来源：http://gss.dashuyun.cn

[U116] JS：类型检查（JSDoc）
来源：http://nwx.aizwys.cn

/** @param {string} name */ function f(name) {}
来源：http://ure.jinyuanbaomall.cn

[U117] JS：单元测试
来源：http://ubl.yvedp.cn

npm i -D vitest;  npx vitest
来源：http://nlz.52xcode.cn

[U118] JS：开发服务器
来源：http://iho.zhijiandao.cn

npm i -D vite;  npx vite
来源：http://ens.yonumen.top

[U119] JS：生产构建
来源：http://afr.xuetiantiany.cn

npx vite build
来源：http://niz.jqgufenzy.top

[U120] JS：读取环境变量（Vite）
来源：http://frd.aizwys.cn

import.meta.env.VITE_API_URL
来源：http://rup.zdbjq.cn

================================================================================
来源：http://vwr.fanxiaobao.xyz

统计汇总
来源：http://zby.uphjek.com

================================================================================
来源：http://bhj.gogol.net.cn

按语言统计（条）：
来源：http://blb.haohaochexian.top

Python ......... 252
来源：http://hkd.pengpengdd.cyou

PHP ............ 252
来源：http://woa.fanxiaobao.xyz

JavaScript ..... 252
来源：http://ehk.shanyushiyangtech.top

TypeScript ..... 212
来源：http://cux.ydzc1.top

Java ........... 212
来源：http://vlv.yangfankeji.com

Go ............. 212
来源：http://zlw.hysaishi.cn

Ruby ........... 212
来源：http://czd.bbcook.cn

C# ............. 212
来源：http://edm.xziqi.cn

C .............. 30
来源：http://ndv.bbcook.cn

C++ ............ 30
来源：http://rnq.jqgfzy.top

SQL ............ 90
来源：http://dwp.mhx1999.top

Bash ........... 80
来源：http://dbt.yuxming.cn

Kotlin ......... 15
来源：http://bol.yonumen.top

Swift .......... 15
来源：http://aug.haohaochexian.top

Lua ............ 10
来源：http://cym.mhx1999.top

Perl ........... 10
来源：http://ndz.zhaomingkeji.xyz

Scala .......... 10
来源：http://ddn.ywan-chungtsiang.top

------------------------------------
来源：http://fkf.jiagoushi.top

合计 ........... 2106 条
来源：http://nkd.cheryme.top

按章节统计：
来源：http://ixt.xylfe.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://eix.birdmap.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tzm.shanyushiyangkeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vov.hnqzz.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://asu.ctjpmb.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cag.kuanghao11.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cfo.birdmap.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kah.sufxvd.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baw.ehwqpu.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sxw.gogol.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wym.xingfuxueyuan.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oqd.shzxlz.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hes.0kj1m.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ije.chenzaomai.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mbp.jiagoushi.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://znx.yuanzhike.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://iql.pycfn.com

Q SQL 专题                              90
来源：http://dhw.sysykeji.top

R Bash 专题                             80
来源：http://ptx.nanxinkj.top

S C / C++ 专题                          60
来源：http://igb.quarkkingdee.top

T 其他语言补充                          60
来源：http://qsw.quarkkingdee.top

U 高频实用片段                         120
来源：http://ylu.ywan-chungtsiang.top

------------------------------------
来源：http://uov.nwbrower.top

合计                                  2106 条
来源：http://gyg.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://avm.jinghuilouyu.cn

使用提醒
来源：http://vvt.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://kbr.chenlongwang.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sif.nanxuanxn.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ocw.daxiang520.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://njl.birdmap.top

在旧版本上使用前请先确认语法支持情况。
来源：http://niy.jqgufenzy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qvf.jianghu66.top

—— 文件结束 ——
来源：http://dhj.cucudq.cn

================================================================================
来源：http://kyo.andypj.xyz

程序语言常见例子速查手册（2024 版）
来源：http://lzn.zhaomingkeji.xyz

Common Programming Examples Cheat Book
来源：http://sgc.gogol.net.cn

================================================================================
来源：http://yvi.ybcxt.top

【收录内容】
来源：http://pns.yj20258.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ojt.shuidangran.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tqz.jianghu66.top

SQL · Bash · C · C++
来源：http://lbl.snrcjt.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rnx.sxryk.cn

【使用说明】
来源：http://ymb.aizwys.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://war.gaohongyu789.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://knt.hcnkem.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qox.zhixingplan.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hhx.nanxuanxn.top

Bash:  Shell         C:     C             C++:   C++
来源：http://eyd.jinqigfzy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://aat.mhx1999.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tuz.hnqzz.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qea.aibaodan.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gku.hfpthk.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://toz.mhx1999.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vwf.jyoumei.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ymp.nanxinkj.top

【文件统计】
来源：http://wrv.zhoulong.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hxh.bbcook.cn

--------------------------------------------------------------------------------
来源：http://yeb.gzhubu.top

目  录
来源：http://nft.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://zlt.epnwcf.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://iuh.yj20258888.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nyo.xylfe.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kzw.fanxiaobao.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tcr.hongshengwenyu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jky.jinghuilouyu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://czv.yuanzhike.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://iyn.hongshengwenyu.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pfv.feifeiyinyue.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hbs.yongpay.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://esg.cheryme.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://axy.gogol.net.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kcn.yangfankeji.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://eng.daxiang520.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://drz.ywan-chungtsiang.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xwr.shanyushiyangtech.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wtp.yueranfly.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xhj.quarkkingdee.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://dtf.aizwys.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://phk.iojbl.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bcd.jinghuilouyu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xvv.hcnkem.com

================================================================================
来源：http://jxj.yuxming.cn

A. 基础语法与类型
来源：http://lri.zdbjq.cn

================================================================================
来源：http://dgl.daria6918.cn

[A01] Hello World
来源：http://quf.zdqjudy.top

Py:   print("Hello, World!")
来源：http://roc.sufxvd.cn

PHP:  echo "Hello, World!";
来源：http://erk.yj20258888.top

JS:   console.log("Hello, World!");
来源：http://bga.cdnleiting.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wcp.ydzc1.top

Java: System.out.println("Hello, World!");
来源：http://pls.vehdjk.com

Go:   fmt.Println("Hello, World!")
来源：http://fyt.sysykeji.top

Ruby: puts "Hello, World!"
来源：http://knr.shanyushiyangkeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://mje.kuanghao11.cn

[A02] 变量声明与赋值
来源：http://oah.xuanzx.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cvc.yanxiufei.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://lsa.zhoulong.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://jes.quarkkingdee.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bul.yuanzhike.top

Java: String name = "Alex"; int age = 20;
来源：http://doq.fengsongda.top

Go:   name := "Alex"; age := 20
来源：http://llp.havefunace.top

Ruby: name = "Alex"; age = 20
来源：http://spr.hywenlv.cn

C#:   string name = "Alex"; int age = 20;
来源：http://txy.shuidangran.top

[A03] 常量定义
来源：http://nfq.haohaochexian.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sjt.yangfankeji.com

PHP:  const PI = 3.14159;
来源：http://lhi.yanxiufei.cn

JS:   const PI = 3.14159;
来源：http://nbq.yuxming.cn

TS:   const PI: number = 3.14159;
来源：http://syy.c1oappe.top

Java: static final double PI = 3.14159;
来源：http://vzx.havefunace.top

Go:   const PI = 3.14159
来源：http://jiz.yonumen.top

Ruby: PI = 3.14159
来源：http://qdt.haohaochexian.top

C#:   const double PI = 3.14159;
来源：http://uoo.pengpengdd.cyou

[A04] 判断变量类型
来源：http://usw.dashuyun.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tph.hesvh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://twg.redwolf501.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://juv.mhx1999.top

TS:   typeof x; x instanceof Date
来源：http://xmj.xinyue.icu

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://izy.kuanghao11.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ctb.hnxiangtu.top

Ruby: x.class; x.is_a?(Integer)
来源：http://loo.sysykeji.top

C#:   x.GetType().Name; x is int
来源：http://hgq.wangdashe.top

[A05] 整数除法与取模
来源：http://xwa.bbcook.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://axu.epnwcf.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://xkc.jinyuanbaomall.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://meo.yuxming.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://psl.wangshuangyany.cn

Java: 7 / 2; 7 % 2
来源：http://vyl.cucudq.cn

Go:   7 / 2; 7 % 2
来源：http://pwy.cheryme.top

Ruby: 7 / 2; 7 % 2
来源：http://wds.hesvh.cn

C#:   7 / 2; 7 % 2
来源：http://lcy.guannengcc.top

[A06] 字符串转数字
来源：http://cxp.0kj1m.cn

Py:   int("42"); float("3.14")
来源：http://edc.epnwcf.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mgd.guannengcc.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://eij.cheryme.top

TS:   parseInt("42", 10); Number("42")
来源：http://xej.yangfankeji.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zon.hnqzz.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hld.hywenlv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zhx.tianlin.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zyv.ydzc1.top

[A07] 数字转字符串
来源：http://yje.tanke756.top

Py:   str(42)
来源：http://nmv.ydzc1.top

PHP:  (string) 42; strval(42)
来源：http://xbd.zhixingplan.top

JS:   String(42); (42).toString()
来源：http://gwi.cashguo.top

TS:   String(42)
来源：http://anm.316326.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://sji.dashuyun.cn

Go:   strconv.Itoa(42)
来源：http://aqs.svipenyu.cn

Ruby: 42.to_s
来源：http://vhj.aibaodan.cn

C#:   42.ToString()
来源：http://aun.feifeiyinyue.top

[A08] 取整与四舍五入
来源：http://vmd.yfazqb.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://boe.ehwqpu.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wxd.fehbvm.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bjk.xuetiantiany.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://umc.fktsv.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gwc.birdmap.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yao.c1oappe.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://xdo.cdnleiting.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yvk.svipenyu.cn

[A09] 绝对值与最大最小值
来源：http://jfh.svipenyu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yfp.shanyushiyangkeji.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rur.dashuyun.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bpn.shuidangran.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://few.zhengqikj.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vuu.zhengqikj.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://psh.jinqigufen.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ntj.fktsv.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vce.jlsjyb.cn

[A10] 生成随机数
来源：http://amk.haohaochexian.top

Py:   import random; random.randint(1, 100)
来源：http://poi.fktsv.cn

PHP:  random_int(1, 100);
来源：http://viw.316326.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://otg.xingfuxueyuan.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://puu.shuidangran.top

Java: new Random().nextInt(100) + 1
来源：http://lls.epnwcf.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jnz.zdqjudy.top

Ruby: rand(1..100)
来源：http://crp.jqgufenzy.top

C#:   new Random().Next(1, 101)
来源：http://dwn.sysykeji.top

[A11] 条件表达式（三元）
来源：http://uxs.redwolf501.top

Py:   "yes" if x > 0 else "no"
来源：http://tre.jinqigufen.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://tni.tanke756.top

JS:   x > 0 ? "yes" : "no"
来源：http://iub.feifeiyinyue.top

TS:   x > 0 ? "yes" : "no"
来源：http://euv.tianlin.xyz

Java: x > 0 ? "yes" : "no"
来源：http://gqj.feifeiyinyue.top

Go:   // 无三元运算符，需用 if 语句
来源：http://uxb.vqdsnc.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://olk.jinyuanbaomall.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ita.vqdsnc.cn

[A12] 字符串插值 / 格式化
来源：http://nhl.yj202588.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://unt.gzhubu.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gbg.fanxiaobao.xyz

JS:   `Hello, ${name}!`
来源：http://enb.bjfxy.top

TS:   `Hello, ${name}!`
来源：http://jce.dashuyun.cn

Java: "Hello, %s!".formatted(name)
来源：http://shu.ivvv.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zjn.svipenyu.cn

Ruby: "Hello, #{name}!"
来源：http://rgp.yangfankeji.com

C#:   $"Hello, {name}!"
来源：http://mwi.hnxiangtu.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ins.fzhhl.top

Py:   "第一行\n第二行"
来源：http://jfr.9152youxi.cn

PHP:  "第一行\n第二行"
来源：http://xxz.sysykeji.top

JS:   "第一行\n第二行"
来源：http://jnu.xziqi.cn

TS:   "第一行\n第二行"
来源：http://dra.yonumen.top

Java: "第一行\n第二行"
来源：http://duw.tanke756.top

Go:   "第一行\n第二行"
来源：http://ikn.tianlin.xyz

Ruby: "第一行\n第二行"
来源：http://tqk.birdmap.top

C#:   "第一行\n第二行"
来源：http://cqf.zhixingplan.top

[A14] 注释写法
来源：http://hwx.yj20258888.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://pku.hnxiangtu.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ntj.ctjpmb.com

JS:   // 单行；/* 多行 */
来源：http://xcx.redwolf501.top

TS:   // 单行；/* 多行 */
来源：http://ydc.guowangkeji.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://etf.cucudq.cn

Go:   // 单行；/* 多行 */
来源：http://ypo.shzxlz.cn

Ruby: # 单行；=begin 多行 =end
来源：http://sdf.zhixingplan.top

C#:   // 单行；/* 多行 */
来源：http://uej.shanyushiyangtech.top

[A15] 空值判断与默认值
来源：http://bdx.nwbrower.top

Py:   value = data or "默认值"
来源：http://art.guannengcc.top

PHP:  $value = $data ?? "默认值";
来源：http://obn.hywenlv.cn

JS:   const value = data ?? "默认值";
来源：http://amo.vehdjk.com

TS:   const value = data ?? "默认值";
来源：http://kmv.9152youxi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zzy.gzhubu.top

Go:   if data == "" { data = "默认值" }
来源：http://nvw.yj20258888.top

Ruby: value = data || "默认值"
来源：http://qbu.xingfuxueyuan.xyz

C#:   var value = data ?? "默认值";
来源：http://dyu.jlsjyb.cn

[A16] 真假值判断规则
来源：http://spq.daria6918.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pws.shangyingyoupin.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://voy.hnqzz.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://miy.yj20258.top

TS:   if (!x) {}
来源：http://niv.ybcxt.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oip.0kj1m.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cbb.yuanzhike.top

Ruby: unless x            # nil 与 false 为假
来源：http://ujh.tianlin.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cju.nanxuanxn.top

[A17] 位运算
来源：http://eak.hysaishi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sqn.bbcook.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://prz.zhengqikj.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jxe.xylfe.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://soe.zhaomingkeji.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hjq.yfazqb.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gls.ydjk.org.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dhs.daria6918.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xne.shangyingyoupin.top

[A18] 字符与 ASCII 码互转
来源：http://mza.daria6918.cn

Py:   ord("A"); chr(65)
来源：http://adp.daxiang520.top

PHP:  ord("A"); chr(65)
来源：http://gpa.cdnleiting.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xnm.bjfxy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jcr.hfpthk.cn

Java: (int) 'A'; (char) 65
来源：http://xcx.xuanzx.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rdj.cdnleiting.top

Ruby: "A".ord; 65.chr
来源：http://yyd.sysykeji.top


<!-- 参考信息 -->