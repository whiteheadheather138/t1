代发 wailian999

[U101] JS：classList 操作
来源：http://ary.svipenyu.cn

el.classList.toggle("active")
来源：http://mlw.jinqigfzy.top

[U102] JS：本地存储
来源：http://bdu.cheryme.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zwl.chenlongwang.top

[U103] JS：定时器
来源：http://oip.hcnkem.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tcn.0kj1m.cn

[U104] JS：防抖
来源：http://sif.zhiwuduotai.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rwj.hnxiangtu.top

[U105] JS：节流
来源：http://ten.hnqzz.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://svp.cheryme.top

[U106] JS：日期格式化
来源：http://qcb.yj20258888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xdq.fktsv.cn

[U107] JS：数字千分位
来源：http://xol.c1oappe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fgt.sweek.top

[U108] JS：随机整数
来源：http://dvp.sufxvd.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://egp.yj20258.top

[U109] JS：数组分组
来源：http://kxq.xingfuxueyuan.xyz

Object.groupBy(arr, x => x.type)
来源：http://lah.wangdashe.top

[U110] JS：数组分块
来源：http://vrs.sjlbkw.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jss.sysykeji.top

[U111] JS：对象转 Map
来源：http://ixd.yongpay.top

new Map(Object.entries(obj))
来源：http://ckh.tanke756.top

[U112] JS：字符串补位
来源：http://fju.zdbjq.cn

"7".padStart(3, "0")
来源：http://enb.jinyuanbaomall.cn

[U113] JS：正则替换全部
来源：http://cfl.gzhubu.top

s.replaceAll("a", "b")
来源：http://qcv.sweek.top

[U114] JS：JSON 深比较
来源：http://pgz.pycfn.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://fxe.hcnkem.com

[U115] JS：生成 UUID
来源：http://ait.pengpengdd.cyou

crypto.randomUUID()
来源：http://xzs.yangfankeji.com

[U116] JS：类型检查（JSDoc）
来源：http://ydr.quarkkingdee.top

/** @param {string} name */ function f(name) {}
来源：http://qyg.zhongyouzk.top

[U117] JS：单元测试
来源：http://jin.gzhubu.top

npm i -D vitest;  npx vitest
来源：http://aro.c1oappe.top

[U118] JS：开发服务器
来源：http://tud.aizwys.cn

npm i -D vite;  npx vite
来源：http://ijk.yj20258888.top

[U119] JS：生产构建
来源：http://dii.zhaomingkeji.xyz

npx vite build
来源：http://fai.chenjidiqi.icu

[U120] JS：读取环境变量（Vite）
来源：http://omt.nwbrower.top

import.meta.env.VITE_API_URL
来源：http://rrc.svipenyu.cn

================================================================================
来源：http://wdq.guowangkeji.top

统计汇总
来源：http://kvl.pengpengdd.cyou

================================================================================
来源：http://vyw.yj20258.top

按语言统计（条）：
来源：http://fxd.hnxiangtu.top

Python ......... 252
来源：http://bey.fengsongda.top

PHP ............ 252
来源：http://tpb.wangshuangyany.cn

JavaScript ..... 252
来源：http://jvf.wangdashe.top

TypeScript ..... 212
来源：http://zjg.tarul.cn

Java ........... 212
来源：http://twh.hammf.cn

Go ............. 212
来源：http://uvr.jinghuilouyu.cn

Ruby ........... 212
来源：http://cwa.jianghu66.top

C# ............. 212
来源：http://lvh.zhaomingkeji.xyz

C .............. 30
来源：http://hgf.hfpthk.cn

C++ ............ 30
来源：http://pfb.meibo888.top

SQL ............ 90
来源：http://dct.daria6918.cn

Bash ........... 80
来源：http://hzv.bjfxy.top

Kotlin ......... 15
来源：http://knp.epnwcf.com

Swift .......... 15
来源：http://qec.yonumen.top

Lua ............ 10
来源：http://suk.pengpengdd.cyou

Perl ........... 10
来源：http://wfi.epnwcf.com

Scala .......... 10
来源：http://piw.shangyingyoupin.top

------------------------------------
来源：http://qsi.tian-w.cn

合计 ........... 2106 条
来源：http://vqr.jyoumei.cn

按章节统计：
来源：http://oog.zycfv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jyr.hysaishi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://guw.zhongyouzk.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qhr.uphjek.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rtp.yueranfly.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lbx.c1oappe.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fgj.sufxvd.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://djv.nanxuanxn.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nsi.hnxiangtu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qev.yueranfly.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kfn.yuanzhike.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qur.jqgfzy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lss.kuanghao11.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wpg.jqgfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://afb.zhoulong.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vtp.sxryk.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kkh.ydzc1.top

Q SQL 专题                              90
来源：http://gjc.jinghuilouyu.cn

R Bash 专题                             80
来源：http://lkh.haohaochexian.top

S C / C++ 专题                          60
来源：http://dlt.c1oappe.top

T 其他语言补充                          60
来源：http://nxd.xuanzx.com

U 高频实用片段                         120
来源：http://hqe.nwbrower.top

------------------------------------
来源：http://eln.xinyue.icu

合计                                  2106 条
来源：http://pfx.hcnkem.com

--------------------------------------------------------------------------------
来源：http://pzh.shuidangran.top

使用提醒
来源：http://upa.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://akb.sjlbkw.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xmq.shzxlz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zew.jinqigfzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bwo.jiagoushi.top

在旧版本上使用前请先确认语法支持情况。
来源：http://dyp.jinghuilouyu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://joa.0kj1m.cn

—— 文件结束 ——
来源：http://aop.hnqzz.top

================================================================================
来源：http://quw.zhaomingkeji.xyz

程序语言常见例子速查手册（2024 版）
来源：http://msv.cdnleiting.top

Common Programming Examples Cheat Book
来源：http://kbg.kuanghao11.cn

================================================================================
来源：http://nzl.yj20258.top

【收录内容】
来源：http://ugt.quarkkingdee.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hyl.zhaomingkeji.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fge.epnwcf.com

SQL · Bash · C · C++
来源：http://tvc.cqqwz.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ind.feifeiyinyue.top

【使用说明】
来源：http://zbt.tarul.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lvr.xylfe.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zuj.hysaishi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pqs.jianghu66.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://riv.xinyue.icu

Bash:  Shell         C:     C             C++:   C++
来源：http://aps.yj202588.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://woq.xuanzx.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ybk.sufxvd.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://anw.zdbjq.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kkx.tarul.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yip.ybcxt.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eoq.sufxvd.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ulr.316326.xyz

【文件统计】
来源：http://nfp.iojbl.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://osh.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://mit.xylfe.cn

目  录
来源：http://ihe.mhx1999.top

--------------------------------------------------------------------------------
来源：http://tgs.feifeiyinyue.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wlz.zdqjudy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qhh.hnxiangtu.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cuk.yuxming.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zkh.tarul.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cml.uphjek.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://psk.jinyuanbaomall.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nds.yanxiufei.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blq.fktsv.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rrw.yuanzhike.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xqk.yangfankeji.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://frq.epnwcf.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wov.ivvv.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sxv.chenjidiqi.icu

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://eih.tianlin.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://exm.smart0.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kvq.shzxlz.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://uih.shangyingyoupin.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://jlj.tianlin.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ycb.chenzaomai.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hts.andypj.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lsz.dianchejie.cn

================================================================================
来源：http://ktm.shanyushiyangkeji.top

A. 基础语法与类型
来源：http://bep.fengsongda.top

================================================================================
来源：http://vdc.xuetiantiany.cn

[A01] Hello World
来源：http://gel.c1oappe.top

Py:   print("Hello, World!")
来源：http://pyg.nanxuanxn.top

PHP:  echo "Hello, World!";
来源：http://hqx.9152youxi.cn

JS:   console.log("Hello, World!");
来源：http://rja.cqqwz.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://aaw.xingfuxueyuan.xyz

Java: System.out.println("Hello, World!");
来源：http://auo.316326.xyz

Go:   fmt.Println("Hello, World!")
来源：http://jci.hnxiangtu.top

Ruby: puts "Hello, World!"
来源：http://yai.zdqjudy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://vng.kuanghao11.cn

[A02] 变量声明与赋值
来源：http://gkq.yangfankeji.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://prr.smart0.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://uif.gaohongyu789.top

JS:   let name = "Alex"; const age = 20;
来源：http://jje.ydjk.org.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tyh.pycfn.com

Java: String name = "Alex"; int age = 20;
来源：http://cvu.hysaishi.cn

Go:   name := "Alex"; age := 20
来源：http://iiw.xylfe.cn

Ruby: name = "Alex"; age = 20
来源：http://jsq.zhaomingkeji.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://oyd.tianlin.xyz

[A03] 常量定义
来源：http://zyd.shuidangran.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://oxu.daria6918.cn

PHP:  const PI = 3.14159;
来源：http://vub.bjfxy.top

JS:   const PI = 3.14159;
来源：http://fbo.chenlongwang.top

TS:   const PI: number = 3.14159;
来源：http://tbl.zhoulong.xyz

Java: static final double PI = 3.14159;
来源：http://tit.ydzc1.top

Go:   const PI = 3.14159
来源：http://ysr.yuanzhike.top

Ruby: PI = 3.14159
来源：http://tfe.aibaodan.cn

C#:   const double PI = 3.14159;
来源：http://rew.yueranfly.top

[A04] 判断变量类型
来源：http://kry.zdqjudy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://kkw.chenlongwang.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://opf.zhijiandao.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rua.jinqigfzy.top

TS:   typeof x; x instanceof Date
来源：http://fzi.hcnkem.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mev.tian-w.cn

Go:   reflect.TypeOf(x).Name()
来源：http://kzd.tanke756.top

Ruby: x.class; x.is_a?(Integer)
来源：http://hng.dashuyun.cn

C#:   x.GetType().Name; x is int
来源：http://rxv.shanyushiyangtech.top

[A05] 整数除法与取模
来源：http://rte.shzxlz.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ily.shanyushiyangkeji.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://tcm.nanxuanxn.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jvf.sweek.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xhq.aizwys.cn

Java: 7 / 2; 7 % 2
来源：http://kqt.dianchejie.cn

Go:   7 / 2; 7 % 2
来源：http://xlq.jqgfzy.top

Ruby: 7 / 2; 7 % 2
来源：http://uwv.yfazqb.com

C#:   7 / 2; 7 % 2
来源：http://dcl.kuanghao11.cn

[A06] 字符串转数字
来源：http://vhj.zhengqikj.top

Py:   int("42"); float("3.14")
来源：http://moz.hesvh.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uks.yj20258888.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ygv.yfazqb.com

TS:   parseInt("42", 10); Number("42")
来源：http://afk.fktsv.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gba.cashguo.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jgu.yj20258888.top

Ruby: "42".to_i; "3.14".to_f
来源：http://dtx.chenzaomai.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xka.jianghu66.top

[A07] 数字转字符串
来源：http://tnl.ehwqpu.com

Py:   str(42)
来源：http://cew.52xcode.cn

PHP:  (string) 42; strval(42)
来源：http://ngu.yuanzhike.top

JS:   String(42); (42).toString()
来源：http://kvn.jqgfzy.top

TS:   String(42)
来源：http://ofo.hammf.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://tln.kuanghao11.cn

Go:   strconv.Itoa(42)
来源：http://bfe.tian-w.cn

Ruby: 42.to_s
来源：http://fpu.hfpthk.cn

C#:   42.ToString()
来源：http://mpu.shangyingyoupin.top

[A08] 取整与四舍五入
来源：http://uhf.iojbl.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pfb.tianlin.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lcu.fanxiaobao.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ncj.hfpthk.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://awn.yj20258888.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nnf.cdnleiting.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ptz.xingfuxueyuan.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://yat.cdnleiting.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://twy.hnqzz.top

[A09] 绝对值与最大最小值
来源：http://yqq.gotoacloud.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://iem.gzhubu.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mni.jlsjyb.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mla.c1oappe.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ztu.jinqigufen.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xxc.gotoacloud.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tsa.hammf.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xmc.zdqjudy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lmc.xinyue.icu

[A10] 生成随机数
来源：http://liv.zhengqikj.top

Py:   import random; random.randint(1, 100)
来源：http://utx.yangfankeji.com

PHP:  random_int(1, 100);
来源：http://glo.pengpengdd.cyou

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ypz.sxryk.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gfe.zhijiandao.cn

Java: new Random().nextInt(100) + 1
来源：http://ado.316326.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://quq.vehdjk.com

Ruby: rand(1..100)
来源：http://ttp.xinyue.icu

C#:   new Random().Next(1, 101)
来源：http://rlb.ydzc1.top

[A11] 条件表达式（三元）
来源：http://kto.fehbvm.com

Py:   "yes" if x > 0 else "no"
来源：http://qna.jiagoushi.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://zti.xuanzx.com

JS:   x > 0 ? "yes" : "no"
来源：http://aof.xinyue.icu

TS:   x > 0 ? "yes" : "no"
来源：http://kjc.shanyushiyangtech.top

Java: x > 0 ? "yes" : "no"
来源：http://vqt.fktsv.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ysf.nanxinkj.top

Ruby: x > 0 ? "yes" : "no"
来源：http://cjc.yvedp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://kja.daria6918.cn

[A12] 字符串插值 / 格式化
来源：http://hlw.shanyushiyangkeji.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hvx.hammf.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gxc.zhiwuduotai.top

JS:   `Hello, ${name}!`
来源：http://phc.vehdjk.com

TS:   `Hello, ${name}!`
来源：http://vib.chenlongwang.top

Java: "Hello, %s!".formatted(name)
来源：http://ltq.zhongyouzk.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://uer.fktsv.cn

Ruby: "Hello, #{name}!"
来源：http://hnq.jinyuanbaomall.cn

C#:   $"Hello, {name}!"
来源：http://grx.yanxiufei.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://knl.yvedp.cn

Py:   "第一行\n第二行"
来源：http://grz.shuidangran.top

PHP:  "第一行\n第二行"
来源：http://pau.cheryme.top

JS:   "第一行\n第二行"
来源：http://aup.zhixingplan.top

TS:   "第一行\n第二行"
来源：http://bod.yuanzhike.top

Java: "第一行\n第二行"
来源：http://poz.sxryk.cn

Go:   "第一行\n第二行"
来源：http://xhh.nanxuanxn.top

Ruby: "第一行\n第二行"
来源：http://rzp.xinyue.icu

C#:   "第一行\n第二行"
来源：http://wmp.jlsjyb.cn

[A14] 注释写法
来源：http://wqs.shangyingyoupin.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://kyz.hywenlv.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://apl.zhaomingkeji.xyz

JS:   // 单行；/* 多行 */
来源：http://tzf.xingfuxueyuan.xyz

TS:   // 单行；/* 多行 */
来源：http://cyz.ppjwa.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hje.feifeiyinyue.top

Go:   // 单行；/* 多行 */
来源：http://raz.shanyushiyangkeji.top

Ruby: # 单行；=begin 多行 =end
来源：http://hnp.iojbl.cn

C#:   // 单行；/* 多行 */
来源：http://urw.shanyushiyangtech.top

[A15] 空值判断与默认值
来源：http://tuu.cheryme.top

Py:   value = data or "默认值"
来源：http://etg.chenlongwang.top

PHP:  $value = $data ?? "默认值";
来源：http://rtm.aizwys.cn

JS:   const value = data ?? "默认值";
来源：http://srx.sufxvd.cn

TS:   const value = data ?? "默认值";
来源：http://oty.svipenyu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://suq.xinyue.icu

Go:   if data == "" { data = "默认值" }
来源：http://jxu.ydzc1.top

Ruby: value = data || "默认值"
来源：http://wgr.chenjidiqi.icu

C#:   var value = data ?? "默认值";
来源：http://xbr.quarkkingdee.top

[A16] 真假值判断规则
来源：http://qhh.epnwcf.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mug.cdnleiting.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ujk.yueranfly.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://aup.hongshengwenyu.top

TS:   if (!x) {}
来源：http://ycd.yuanzhike.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uht.epnwcf.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ohj.uphjek.com

Ruby: unless x            # nil 与 false 为假
来源：http://npw.feifeiyinyue.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xpe.meibo888.top

[A17] 位运算
来源：http://mml.pengpengdd.cyou

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rck.yj20258888.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zyy.jqgfzy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zpx.gotoacloud.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xiw.bjfxy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sjv.chenlongwang.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bvy.yj202588.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dzv.dashuyun.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xkp.guannengcc.top


<!-- 参考信息 -->