代发 wailian999

[U103] JS：定时器
来源：http://jjk.daxiang520.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pjp.xingfuxueyuan.xyz

[U104] JS：防抖
来源：http://hiy.jqgfzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uba.nwbrower.top

[U105] JS：节流
来源：http://usc.epnwcf.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qvt.kuanghao11.cn

[U106] JS：日期格式化
来源：http://tpe.gzhubu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kwu.uphjek.com

[U107] JS：数字千分位
来源：http://kvo.yueranfly.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mwf.fktsv.cn

[U108] JS：随机整数
来源：http://kyk.cucudq.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pxs.52xcode.cn

[U109] JS：数组分组
来源：http://bkl.tarul.cn

Object.groupBy(arr, x => x.type)
来源：http://fwb.hywenlv.cn

[U110] JS：数组分块
来源：http://pek.xylfe.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zpz.yvedp.cn

[U111] JS：对象转 Map
来源：http://qux.cheryme.top

new Map(Object.entries(obj))
来源：http://mln.yanxiufei.cn

[U112] JS：字符串补位
来源：http://svd.zhengqikj.top

"7".padStart(3, "0")
来源：http://bql.zdqjudy.top

[U113] JS：正则替换全部
来源：http://vgw.yuxming.cn

s.replaceAll("a", "b")
来源：http://ihe.svipenyu.cn

[U114] JS：JSON 深比较
来源：http://pis.ydzc1.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://soh.sxryk.cn

[U115] JS：生成 UUID
来源：http://mjj.jinyuanbaomall.cn

crypto.randomUUID()
来源：http://auo.hnxiangtu.top

[U116] JS：类型检查（JSDoc）
来源：http://iog.sxryk.cn

/** @param {string} name */ function f(name) {}
来源：http://klf.dianchejie.cn

[U117] JS：单元测试
来源：http://glk.nanxuanxn.top

npm i -D vitest;  npx vitest
来源：http://opl.wangdashe.top

[U118] JS：开发服务器
来源：http://qtu.gotoacloud.top

npm i -D vite;  npx vite
来源：http://fyk.iojbl.cn

[U119] JS：生产构建
来源：http://xcw.hcnkem.com

npx vite build
来源：http://clt.yfazqb.com

[U120] JS：读取环境变量（Vite）
来源：http://onf.gogol.net.cn

import.meta.env.VITE_API_URL
来源：http://dfx.ehwqpu.com

================================================================================
来源：http://hvm.jinghuilouyu.cn

统计汇总
来源：http://bpn.yuxming.cn

================================================================================
来源：http://qqz.shanyushiyangtech.top

按语言统计（条）：
来源：http://vlq.svipenyu.cn

Python ......... 252
来源：http://xzr.chenzaomai.com

PHP ............ 252
来源：http://lmf.zhengqikj.top

JavaScript ..... 252
来源：http://fdr.xylfe.cn

TypeScript ..... 212
来源：http://abo.svipenyu.cn

Java ........... 212
来源：http://hjq.chenjidiqi.icu

Go ............. 212
来源：http://ofc.jinyuanbaomall.cn

Ruby ........... 212
来源：http://kvm.bbcook.cn

C# ............. 212
来源：http://wxx.ivvv.top

C .............. 30
来源：http://mje.zhoulong.xyz

C++ ............ 30
来源：http://epw.tianlin.xyz

SQL ............ 90
来源：http://rfs.yanxiufei.cn

Bash ........... 80
来源：http://lbo.chenzaomai.com

Kotlin ......... 15
来源：http://acf.ywan-chungtsiang.top

Swift .......... 15
来源：http://jrd.ywan-chungtsiang.top

Lua ............ 10
来源：http://ndl.yuanzhike.top

Perl ........... 10
来源：http://nff.zhaomingkeji.xyz

Scala .......... 10
来源：http://gdx.chenzaomai.com

------------------------------------
来源：http://pam.jinqigufen.top

合计 ........... 2106 条
来源：http://txb.hongshengwenyu.top

按章节统计：
来源：http://buj.iojbl.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ibk.nwbrower.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xrf.dashuyun.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qhh.cdnleiting.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lrx.wangshuangyany.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://esa.tarul.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tuk.shanyushiyangtech.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xgu.jinqigfzy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fsm.cheryme.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tqy.jqgfzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jua.tarul.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oyd.shuidangran.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://etg.0kj1m.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fxg.nanxinkj.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jus.chenjidiqi.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cxz.ydjk.org.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ypf.fktsv.cn

Q SQL 专题                              90
来源：http://jqn.yonumen.top

R Bash 专题                             80
来源：http://rbc.xziqi.cn

S C / C++ 专题                          60
来源：http://dak.ppjwa.cn

T 其他语言补充                          60
来源：http://abo.cheryme.top

U 高频实用片段                         120
来源：http://xab.yj20258888.top

------------------------------------
来源：http://sec.hywenlv.cn

合计                                  2106 条
来源：http://tzp.hnqzz.top

--------------------------------------------------------------------------------
来源：http://ggf.hcnkem.com

使用提醒
来源：http://nnm.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://yql.jqgufenzy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tzn.52xcode.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tkg.birdmap.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dyl.fanxiaobao.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://kus.yueranfly.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tms.pengpengdd.cyou

—— 文件结束 ——
来源：http://hav.wangshuangyany.cn

================================================================================
来源：http://eoi.chenlongwang.top

程序语言常见例子速查手册（2024 版）
来源：http://lwx.jqgufenzy.top

Common Programming Examples Cheat Book
来源：http://ltu.jinyuanbaomall.cn

================================================================================
来源：http://yju.cucudq.cn

【收录内容】
来源：http://mas.9152youxi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nze.hfpthk.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yub.jinqigufen.top

SQL · Bash · C · C++
来源：http://uwy.nwbrower.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rny.haohaochexian.top

【使用说明】
来源：http://glr.feifeiyinyue.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sjm.jyoumei.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hvj.jiagoushi.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qqb.sxryk.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://grc.daxiang520.top

Bash:  Shell         C:     C             C++:   C++
来源：http://fhw.hcnkem.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jso.jiagoushi.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pku.zhoulong.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ogm.jinqigfzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lps.chenjidiqi.icu

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yut.xuetiantiany.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qsg.nanxinkj.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kgx.mhx1999.top

【文件统计】
来源：http://vjb.cucudq.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://omv.yongpay.top

--------------------------------------------------------------------------------
来源：http://wgv.sxryk.cn

目  录
来源：http://ych.tanke756.top

--------------------------------------------------------------------------------
来源：http://bcn.meibo888.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://upw.ctjpmb.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kmp.jinghuilouyu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://swm.hnqzz.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vxc.svipenyu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dtj.chenzaomai.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://iox.snrcjt.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fzf.yangfankeji.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dgh.vehdjk.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qmp.hfpthk.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lbq.tianlin.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jfh.jianghu66.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xxy.0kj1m.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ewr.ehwqpu.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zug.havefunace.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qxl.9152youxi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vun.vehdjk.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xoi.havefunace.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ivn.ywan-chungtsiang.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://daa.jqgufenzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cat.shzxlz.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qzd.dashuyun.cn

================================================================================
来源：http://snu.gzhubu.top

A. 基础语法与类型
来源：http://xcn.jqgufenzy.top

================================================================================
来源：http://yjo.sweek.top

[A01] Hello World
来源：http://wfm.hnxiangtu.top

Py:   print("Hello, World!")
来源：http://jxt.jiagoushi.top

PHP:  echo "Hello, World!";
来源：http://ief.ywan-chungtsiang.top

JS:   console.log("Hello, World!");
来源：http://neo.52xcode.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://spa.zhiwuduotai.top

Java: System.out.println("Hello, World!");
来源：http://ijt.316326.xyz

Go:   fmt.Println("Hello, World!")
来源：http://hul.yonumen.top

Ruby: puts "Hello, World!"
来源：http://zji.fanxiaobao.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://ztx.zdbjq.cn

[A02] 变量声明与赋值
来源：http://kic.zhoulong.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ggf.yj20258.top

PHP:  $name = "Alex"; $age = 20;
来源：http://grz.aibaodan.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yku.yfazqb.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://iyx.hnqzz.top

Java: String name = "Alex"; int age = 20;
来源：http://nul.fktsv.cn

Go:   name := "Alex"; age := 20
来源：http://ilw.smart0.xyz

Ruby: name = "Alex"; age = 20
来源：http://zac.quarkkingdee.top

C#:   string name = "Alex"; int age = 20;
来源：http://oen.zhiwuduotai.top

[A03] 常量定义
来源：http://tcb.jinyuanbaomall.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jmd.chenzaomai.com

PHP:  const PI = 3.14159;
来源：http://vmp.bjfxy.top

JS:   const PI = 3.14159;
来源：http://ckq.ivvv.top

TS:   const PI: number = 3.14159;
来源：http://nis.quarkkingdee.top

Java: static final double PI = 3.14159;
来源：http://hpa.c1oappe.top

Go:   const PI = 3.14159
来源：http://lqy.yongpay.top

Ruby: PI = 3.14159
来源：http://msp.shanyushiyangtech.top

C#:   const double PI = 3.14159;
来源：http://txx.hammf.cn

[A04] 判断变量类型
来源：http://qzz.hysaishi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://aif.epnwcf.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wbx.jinyuanbaomall.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kwd.jinyuanbaomall.cn

TS:   typeof x; x instanceof Date
来源：http://ngh.yfazqb.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pdy.gaohongyu789.top

Go:   reflect.TypeOf(x).Name()
来源：http://ypa.yuanzhike.top

Ruby: x.class; x.is_a?(Integer)
来源：http://cvm.aibaodan.cn

C#:   x.GetType().Name; x is int
来源：http://gzn.jinghuilouyu.cn

[A05] 整数除法与取模
来源：http://biz.hongshengwenyu.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dib.xylfe.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xmr.jinyuanbaomall.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zrf.hcnkem.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bhj.cdnleiting.top

Java: 7 / 2; 7 % 2
来源：http://pbe.yvedp.cn

Go:   7 / 2; 7 % 2
来源：http://xna.chenjidiqi.icu

Ruby: 7 / 2; 7 % 2
来源：http://ftd.sysykeji.top

C#:   7 / 2; 7 % 2
来源：http://qhl.zycfv.cn

[A06] 字符串转数字
来源：http://drw.jinqigufen.top

Py:   int("42"); float("3.14")
来源：http://mxw.meibo888.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xcx.andypj.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xpa.meibo888.top

TS:   parseInt("42", 10); Number("42")
来源：http://vyn.iojbl.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pmr.yongpay.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hlf.yj20258.top

Ruby: "42".to_i; "3.14".to_f
来源：http://fat.zdbjq.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pis.shanyushiyangkeji.top

[A07] 数字转字符串
来源：http://ycq.jyoumei.cn

Py:   str(42)
来源：http://vra.shangyingyoupin.top

PHP:  (string) 42; strval(42)
来源：http://szo.cdnleiting.top

JS:   String(42); (42).toString()
来源：http://zhn.dashuyun.cn

TS:   String(42)
来源：http://kii.zdbjq.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://jxa.cqqwz.cn

Go:   strconv.Itoa(42)
来源：http://gxj.xuetiantiany.cn

Ruby: 42.to_s
来源：http://ocj.yueranfly.top

C#:   42.ToString()
来源：http://asg.sweek.top

[A08] 取整与四舍五入
来源：http://ock.ppjwa.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://srf.hnxiangtu.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jht.andypj.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://avt.ydzc1.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ejo.hnqzz.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://szz.cheryme.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gkz.nwbrower.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://gtw.hnxiangtu.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dud.fzhhl.top

[A09] 绝对值与最大最小值
来源：http://iqy.birdmap.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dnl.bjfxy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vxc.havefunace.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cpn.xylfe.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ojy.epnwcf.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sre.fehbvm.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ixs.nanxinkj.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://omt.jinyuanbaomall.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dbw.jinqigfzy.top

[A10] 生成随机数
来源：http://dmx.aizwys.cn

Py:   import random; random.randint(1, 100)
来源：http://sjz.pengpengdd.cyou

PHP:  random_int(1, 100);
来源：http://vcv.cucudq.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kjm.zhengqikj.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yms.jinqigufen.top

Java: new Random().nextInt(100) + 1
来源：http://uoy.zdbjq.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hzr.yfazqb.com

Ruby: rand(1..100)
来源：http://bou.zhixingplan.top

C#:   new Random().Next(1, 101)
来源：http://txo.9152youxi.cn

[A11] 条件表达式（三元）
来源：http://qhx.nanxinkj.top

Py:   "yes" if x > 0 else "no"
来源：http://xwe.shangyingyoupin.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ium.chenlongwang.top

JS:   x > 0 ? "yes" : "no"
来源：http://djj.pycfn.com

TS:   x > 0 ? "yes" : "no"
来源：http://qop.ydjk.org.cn

Java: x > 0 ? "yes" : "no"
来源：http://aer.guowangkeji.top

Go:   // 无三元运算符，需用 if 语句
来源：http://fjn.gotoacloud.top

Ruby: x > 0 ? "yes" : "no"
来源：http://gys.ydjk.org.cn

C#:   x > 0 ? "yes" : "no"
来源：http://isu.c1oappe.top

[A12] 字符串插值 / 格式化
来源：http://wzh.zdbjq.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fbi.jinyuanbaomall.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hls.yueranfly.top

JS:   `Hello, ${name}!`
来源：http://ewy.shangyingyoupin.top

TS:   `Hello, ${name}!`
来源：http://cqn.meibo888.top

Java: "Hello, %s!".formatted(name)
来源：http://bbf.jianghu66.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://swp.0kj1m.cn

Ruby: "Hello, #{name}!"
来源：http://yvt.zdbjq.cn

C#:   $"Hello, {name}!"
来源：http://ajz.hammf.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ibs.cqqwz.cn

Py:   "第一行\n第二行"
来源：http://azk.uphjek.com

PHP:  "第一行\n第二行"
来源：http://ris.yonumen.top

JS:   "第一行\n第二行"
来源：http://pye.meibo888.top

TS:   "第一行\n第二行"
来源：http://dll.yuxming.cn

Java: "第一行\n第二行"
来源：http://otw.zhiwuduotai.top

Go:   "第一行\n第二行"
来源：http://biq.xuanzx.com

Ruby: "第一行\n第二行"
来源：http://sfc.zhiwuduotai.top

C#:   "第一行\n第二行"
来源：http://cky.c1oappe.top

[A14] 注释写法
来源：http://bmy.ydjk.org.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cpe.shuidangran.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ubx.sysykeji.top

JS:   // 单行；/* 多行 */
来源：http://vao.ivvv.top

TS:   // 单行；/* 多行 */
来源：http://ytx.hysaishi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vio.ywan-chungtsiang.top

Go:   // 单行；/* 多行 */
来源：http://tce.aizwys.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fcg.xuanzx.com

C#:   // 单行；/* 多行 */
来源：http://vpl.havefunace.top

[A15] 空值判断与默认值
来源：http://glk.xuetiantiany.cn

Py:   value = data or "默认值"
来源：http://uir.ydjk.org.cn

PHP:  $value = $data ?? "默认值";
来源：http://zeb.birdmap.top

JS:   const value = data ?? "默认值";
来源：http://xvo.jinghuilouyu.cn

TS:   const value = data ?? "默认值";
来源：http://bwu.yangfankeji.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xir.daxiang520.top

Go:   if data == "" { data = "默认值" }
来源：http://zwz.jinqigfzy.top

Ruby: value = data || "默认值"
来源：http://sto.smart0.xyz

C#:   var value = data ?? "默认值";
来源：http://yde.nwbrower.top

[A16] 真假值判断规则
来源：http://rbv.yj202588.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://frl.sjlbkw.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xos.smart0.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lxz.uphjek.com

TS:   if (!x) {}
来源：http://atq.svipenyu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zaf.zhengqikj.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qea.chenlongwang.top

Ruby: unless x            # nil 与 false 为假
来源：http://ggt.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nss.meibo888.top

[A17] 位运算
来源：http://glp.zhiwuduotai.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ipx.hcnkem.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uzi.snrcjt.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://slg.cashguo.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xro.aibaodan.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cyc.zdbjq.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nas.shuidangran.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ind.hnxiangtu.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://htm.jinyuanbaomall.cn

[A18] 字符与 ASCII 码互转
来源：http://mvn.nwbrower.top

Py:   ord("A"); chr(65)
来源：http://pym.wangdashe.top

PHP:  ord("A"); chr(65)
来源：http://vsj.cucudq.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://owx.hfpthk.cn


<!-- 参考信息 -->