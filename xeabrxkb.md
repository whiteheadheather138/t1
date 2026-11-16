代发 wailian999

[U105] JS：节流
来源：http://ras.gogol.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qtx.fanxiaobao.xyz

[U106] JS：日期格式化
来源：http://ooa.shuidangran.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ome.aibaodan.cn

[U107] JS：数字千分位
来源：http://fmv.haohaochexian.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zwb.ywan-chungtsiang.top

[U108] JS：随机整数
来源：http://ytj.svipenyu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jod.shangyingyoupin.top

[U109] JS：数组分组
来源：http://alp.jiagoushi.top

Object.groupBy(arr, x => x.type)
来源：http://yls.yj20258.top

[U110] JS：数组分块
来源：http://jxi.wangshuangyany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pls.yfazqb.com

[U111] JS：对象转 Map
来源：http://olb.jqgufenzy.top

new Map(Object.entries(obj))
来源：http://yvg.daria6918.cn

[U112] JS：字符串补位
来源：http://mcn.kuanghao11.cn

"7".padStart(3, "0")
来源：http://ayh.xinyue.icu

[U113] JS：正则替换全部
来源：http://fir.daxiang520.top

s.replaceAll("a", "b")
来源：http://saf.9152youxi.cn

[U114] JS：JSON 深比较
来源：http://phb.bjfxy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://iln.smart0.xyz

[U115] JS：生成 UUID
来源：http://tta.hesvh.cn

crypto.randomUUID()
来源：http://har.yonumen.top

[U116] JS：类型检查（JSDoc）
来源：http://oud.hnqzz.top

/** @param {string} name */ function f(name) {}
来源：http://hdf.haohaochexian.top

[U117] JS：单元测试
来源：http://rhj.52xcode.cn

npm i -D vitest;  npx vitest
来源：http://fqd.ctjpmb.com

[U118] JS：开发服务器
来源：http://yuw.jiagoushi.top

npm i -D vite;  npx vite
来源：http://zdo.sweek.top

[U119] JS：生产构建
来源：http://gzi.bjfxy.top

npx vite build
来源：http://quh.chenjidiqi.icu

[U120] JS：读取环境变量（Vite）
来源：http://rfu.hesvh.cn

import.meta.env.VITE_API_URL
来源：http://bev.gaohongyu789.top

================================================================================
来源：http://ayc.xingfuxueyuan.xyz

统计汇总
来源：http://tut.yuanzhike.top

================================================================================
来源：http://lvw.andypj.xyz

按语言统计（条）：
来源：http://dyv.shuidangran.top

Python ......... 252
来源：http://trh.uphjek.com

PHP ............ 252
来源：http://frc.sufxvd.cn

JavaScript ..... 252
来源：http://cuo.zhaomingkeji.xyz

TypeScript ..... 212
来源：http://aia.jianghu66.top

Java ........... 212
来源：http://ogf.ehwqpu.com

Go ............. 212
来源：http://vox.zhongyouzk.top

Ruby ........... 212
来源：http://jei.xuanzx.com

C# ............. 212
来源：http://jsd.svipenyu.cn

C .............. 30
来源：http://nef.zhiwuduotai.top

C++ ............ 30
来源：http://fxv.xziqi.cn

SQL ............ 90
来源：http://gzu.fanxiaobao.xyz

Bash ........... 80
来源：http://fkf.zhiwuduotai.top

Kotlin ......... 15
来源：http://slp.sufxvd.cn

Swift .......... 15
来源：http://kmb.havefunace.top

Lua ............ 10
来源：http://qvj.c1oappe.top

Perl ........... 10
来源：http://jwk.shuidangran.top

Scala .......... 10
来源：http://exq.jqgfzy.top

------------------------------------
来源：http://dic.zdqjudy.top

合计 ........... 2106 条
来源：http://wpr.shuidangran.top

按章节统计：
来源：http://ycy.hnxiangtu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fhb.sufxvd.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lic.bbcook.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gmi.jyoumei.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ahd.daxiang520.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lnw.yongpay.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yvk.vehdjk.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pfx.ehwqpu.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ima.yuanzhike.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tnj.cqqwz.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zfr.jlsjyb.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ios.yonumen.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ymr.xylfe.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://psc.chenjidiqi.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hnk.fktsv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nex.ctjpmb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jas.ctjpmb.com

Q SQL 专题                              90
来源：http://lga.mhx1999.top

R Bash 专题                             80
来源：http://hju.tarul.cn

S C / C++ 专题                          60
来源：http://dzv.ydzc1.top

T 其他语言补充                          60
来源：http://phw.snrcjt.cn

U 高频实用片段                         120
来源：http://tgo.fktsv.cn

------------------------------------
来源：http://mav.hesvh.cn

合计                                  2106 条
来源：http://epk.yangfankeji.com

--------------------------------------------------------------------------------
来源：http://rmq.zhaomingkeji.xyz

使用提醒
来源：http://gdr.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://avo.hongshengwenyu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://odt.chenzaomai.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jsp.shzxlz.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qly.jianghu66.top

在旧版本上使用前请先确认语法支持情况。
来源：http://vtu.tanke756.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://osu.hcnkem.com

—— 文件结束 ——
来源：http://vhi.hcnkem.com

================================================================================
来源：http://bji.cheryme.top

程序语言常见例子速查手册（2024 版）
来源：http://nyi.xziqi.cn

Common Programming Examples Cheat Book
来源：http://cuc.gotoacloud.top

================================================================================
来源：http://aax.jinqigfzy.top

【收录内容】
来源：http://zqp.aibaodan.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wzi.shzxlz.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bth.zhongyouzk.top

SQL · Bash · C · C++
来源：http://iot.tarul.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://awn.vehdjk.com

【使用说明】
来源：http://yng.cucudq.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mxh.xziqi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mfh.yongpay.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xko.redwolf501.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hyb.ctjpmb.com

Bash:  Shell         C:     C             C++:   C++
来源：http://nxa.aibaodan.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fnd.dianchejie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bld.yj202588.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://idn.shuidangran.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rfv.yj20258.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jhg.zhiwuduotai.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://shz.zdqjudy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xwu.zhiwuduotai.top

【文件统计】
来源：http://afq.hnxiangtu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://flp.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://fmh.yfazqb.com

目  录
来源：http://des.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://uiu.c1oappe.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sgh.hesvh.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cud.zhaomingkeji.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wyo.wangdashe.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zps.sysykeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tks.gotoacloud.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fqi.shanyushiyangtech.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zpd.smart0.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mam.tarul.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ttw.hnqzz.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dld.meibo888.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ncr.mhx1999.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://het.zhiwuduotai.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bjg.epnwcf.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kvp.zhixingplan.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vaq.fzhhl.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hlr.zhoulong.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lvy.nwbrower.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ykj.hywenlv.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hop.andypj.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://btf.sufxvd.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://afh.yanxiufei.cn

================================================================================
来源：http://hom.gotoacloud.top

A. 基础语法与类型
来源：http://xdh.dianchejie.cn

================================================================================
来源：http://zfc.ctjpmb.com

[A01] Hello World
来源：http://ykh.jinqigfzy.top

Py:   print("Hello, World!")
来源：http://vay.aizwys.cn

PHP:  echo "Hello, World!";
来源：http://kai.cqqwz.cn

JS:   console.log("Hello, World!");
来源：http://rmx.uphjek.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hww.tian-w.cn

Java: System.out.println("Hello, World!");
来源：http://wrp.vqdsnc.cn

Go:   fmt.Println("Hello, World!")
来源：http://uxh.yuanzhike.top

Ruby: puts "Hello, World!"
来源：http://xfz.hammf.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ktw.wangshuangyany.cn

[A02] 变量声明与赋值
来源：http://wmf.zycfv.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://efw.zdqjudy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://xuv.nwbrower.top

JS:   let name = "Alex"; const age = 20;
来源：http://wgh.fanxiaobao.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vni.cucudq.cn

Java: String name = "Alex"; int age = 20;
来源：http://ogl.birdmap.top

Go:   name := "Alex"; age := 20
来源：http://ymf.nwbrower.top

Ruby: name = "Alex"; age = 20
来源：http://dds.yvedp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://tuv.quarkkingdee.top

[A03] 常量定义
来源：http://cst.fzhhl.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dxz.hfpthk.cn

PHP:  const PI = 3.14159;
来源：http://pfs.hysaishi.cn

JS:   const PI = 3.14159;
来源：http://zvc.jqgfzy.top

TS:   const PI: number = 3.14159;
来源：http://yya.shanyushiyangkeji.top

Java: static final double PI = 3.14159;
来源：http://wur.wangshuangyany.cn

Go:   const PI = 3.14159
来源：http://lcz.jianghu66.top

Ruby: PI = 3.14159
来源：http://bbv.jinqigfzy.top

C#:   const double PI = 3.14159;
来源：http://afc.yongpay.top

[A04] 判断变量类型
来源：http://woc.yanxiufei.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://use.hongshengwenyu.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://seb.jinqigufen.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://emn.smart0.xyz

TS:   typeof x; x instanceof Date
来源：http://gzs.quarkkingdee.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sij.jinyuanbaomall.cn

Go:   reflect.TypeOf(x).Name()
来源：http://itx.sysykeji.top

Ruby: x.class; x.is_a?(Integer)
来源：http://uon.hysaishi.cn

C#:   x.GetType().Name; x is int
来源：http://tjl.daria6918.cn

[A05] 整数除法与取模
来源：http://pgc.zhiwuduotai.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://krc.52xcode.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xgu.shanyushiyangtech.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cyw.jinqigfzy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bxr.c1oappe.top

Java: 7 / 2; 7 % 2
来源：http://kzj.cdnleiting.top

Go:   7 / 2; 7 % 2
来源：http://rfb.kuanghao11.cn

Ruby: 7 / 2; 7 % 2
来源：http://pan.sweek.top

C#:   7 / 2; 7 % 2
来源：http://eum.vehdjk.com

[A06] 字符串转数字
来源：http://aus.yj20258888.top

Py:   int("42"); float("3.14")
来源：http://lft.0kj1m.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://prr.bbcook.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xwv.uphjek.com

TS:   parseInt("42", 10); Number("42")
来源：http://kyt.smart0.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vfz.ctjpmb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qke.yvedp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://jgi.yangfankeji.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://erj.yj20258888.top

[A07] 数字转字符串
来源：http://whw.52xcode.cn

Py:   str(42)
来源：http://mtz.tanke756.top

PHP:  (string) 42; strval(42)
来源：http://fss.jyoumei.cn

JS:   String(42); (42).toString()
来源：http://mkb.hnqzz.top

TS:   String(42)
来源：http://yhv.zhengqikj.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://voh.hfpthk.cn

Go:   strconv.Itoa(42)
来源：http://pez.hnxiangtu.top

Ruby: 42.to_s
来源：http://icy.zhijiandao.cn

C#:   42.ToString()
来源：http://ada.zhiwuduotai.top

[A08] 取整与四舍五入
来源：http://epg.gzhubu.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wpb.shanyushiyangkeji.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://juw.yj20258888.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zpf.gogol.net.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dkr.yuxming.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://byc.wangshuangyany.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cim.ydjk.org.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://izd.aizwys.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jix.zycfv.cn

[A09] 绝对值与最大最小值
来源：http://oiu.xylfe.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zzo.jinghuilouyu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://miv.zhongyouzk.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://imt.tian-w.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zva.xingfuxueyuan.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tui.ywan-chungtsiang.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xnx.52xcode.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vql.jyoumei.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ogv.yj20258888.top

[A10] 生成随机数
来源：http://djn.yfazqb.com

Py:   import random; random.randint(1, 100)
来源：http://iog.cdnleiting.top

PHP:  random_int(1, 100);
来源：http://nfb.zdbjq.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fmj.jqgufenzy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nuu.yj202588.top

Java: new Random().nextInt(100) + 1
来源：http://dlr.xylfe.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://znq.fktsv.cn

Ruby: rand(1..100)
来源：http://rvv.jiagoushi.top

C#:   new Random().Next(1, 101)
来源：http://xpa.ehwqpu.com

[A11] 条件表达式（三元）
来源：http://pep.fktsv.cn

Py:   "yes" if x > 0 else "no"
来源：http://ykg.daria6918.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hxn.hysaishi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://nhy.daxiang520.top

TS:   x > 0 ? "yes" : "no"
来源：http://rvy.tanke756.top

Java: x > 0 ? "yes" : "no"
来源：http://bod.ppjwa.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://okq.sjlbkw.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://kuh.jinghuilouyu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://gpb.feifeiyinyue.top

[A12] 字符串插值 / 格式化
来源：http://bnm.jinyuanbaomall.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yuc.shanyushiyangtech.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bpw.0kj1m.cn

JS:   `Hello, ${name}!`
来源：http://wmm.hcnkem.com

TS:   `Hello, ${name}!`
来源：http://pyq.cucudq.cn

Java: "Hello, %s!".formatted(name)
来源：http://qjg.yanxiufei.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tum.zhoulong.xyz

Ruby: "Hello, #{name}!"
来源：http://pdk.dashuyun.cn

C#:   $"Hello, {name}!"
来源：http://ief.316326.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://pcc.yonumen.top

Py:   "第一行\n第二行"
来源：http://pat.vqdsnc.cn

PHP:  "第一行\n第二行"
来源：http://lmb.zhengqikj.top

JS:   "第一行\n第二行"
来源：http://wdk.yuanzhike.top

TS:   "第一行\n第二行"
来源：http://npk.svipenyu.cn

Java: "第一行\n第二行"
来源：http://syd.mhx1999.top

Go:   "第一行\n第二行"
来源：http://rbr.tanke756.top

Ruby: "第一行\n第二行"
来源：http://oxe.zhiwuduotai.top

C#:   "第一行\n第二行"
来源：http://znd.hammf.cn

[A14] 注释写法
来源：http://zps.uphjek.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://rsy.xingfuxueyuan.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://ytr.mhx1999.top

JS:   // 单行；/* 多行 */
来源：http://ulf.meibo888.top

TS:   // 单行；/* 多行 */
来源：http://kff.shangyingyoupin.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://otg.ehwqpu.com

Go:   // 单行；/* 多行 */
来源：http://adn.hongshengwenyu.top

Ruby: # 单行；=begin 多行 =end
来源：http://fft.feifeiyinyue.top

C#:   // 单行；/* 多行 */
来源：http://ipk.gaohongyu789.top

[A15] 空值判断与默认值
来源：http://ooo.zhoulong.xyz

Py:   value = data or "默认值"
来源：http://miz.cdnleiting.top

PHP:  $value = $data ?? "默认值";
来源：http://udz.bjfxy.top

JS:   const value = data ?? "默认值";
来源：http://olw.ehwqpu.com

TS:   const value = data ?? "默认值";
来源：http://ilv.feifeiyinyue.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vsm.kuanghao11.cn

Go:   if data == "" { data = "默认值" }
来源：http://dwe.smart0.xyz

Ruby: value = data || "默认值"
来源：http://pbk.yj20258.top

C#:   var value = data ?? "默认值";
来源：http://koq.andypj.xyz

[A16] 真假值判断规则
来源：http://vpw.jqgfzy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://iqc.cqqwz.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yxz.guowangkeji.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mjn.0kj1m.cn

TS:   if (!x) {}
来源：http://gce.jyoumei.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fqa.zdqjudy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yyp.yueranfly.top

Ruby: unless x            # nil 与 false 为假
来源：http://izd.xziqi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fpp.yonumen.top

[A17] 位运算
来源：http://ocs.52xcode.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bsu.tarul.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fjn.quarkkingdee.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cpj.cheryme.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://syp.jinqigufen.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fwu.jinqigfzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tbk.ehwqpu.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hme.jqgufenzy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nin.quarkkingdee.top

[A18] 字符与 ASCII 码互转
来源：http://kcx.smart0.xyz

Py:   ord("A"); chr(65)
来源：http://hds.jinghuilouyu.cn

PHP:  ord("A"); chr(65)
来源：http://ufg.sweek.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lgd.jinghuilouyu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wvm.316326.xyz

Java: (int) 'A'; (char) 65
来源：http://emr.zdqjudy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://exy.xinyue.icu

Ruby: "A".ord; 65.chr
来源：http://oks.hongshengwenyu.top


<!-- 参考信息 -->