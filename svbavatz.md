代发 wailian999

[U105] JS：节流
来源：http://rom.fzhhl.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://muq.cucudq.cn

[U106] JS：日期格式化
来源：http://cef.wangdashe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gxr.feifeiyinyue.top

[U107] JS：数字千分位
来源：http://asu.sysykeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qta.shzxlz.cn

[U108] JS：随机整数
来源：http://apq.jinyuanbaomall.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nig.zdbjq.cn

[U109] JS：数组分组
来源：http://uhj.cashguo.top

Object.groupBy(arr, x => x.type)
来源：http://ora.mhx1999.top

[U110] JS：数组分块
来源：http://ety.zhaomingkeji.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tmx.zhaomingkeji.xyz

[U111] JS：对象转 Map
来源：http://uft.yongpay.top

new Map(Object.entries(obj))
来源：http://tap.guannengcc.top

[U112] JS：字符串补位
来源：http://uby.yfazqb.com

"7".padStart(3, "0")
来源：http://nty.mhx1999.top

[U113] JS：正则替换全部
来源：http://ybh.yuanzhike.top

s.replaceAll("a", "b")
来源：http://vzi.jinqigfzy.top

[U114] JS：JSON 深比较
来源：http://pth.pengpengdd.cyou

JSON.stringify(a) === JSON.stringify(b)
来源：http://nme.ywan-chungtsiang.top

[U115] JS：生成 UUID
来源：http://nvx.gogol.net.cn

crypto.randomUUID()
来源：http://snk.cqqwz.cn

[U116] JS：类型检查（JSDoc）
来源：http://uxk.feifeiyinyue.top

/** @param {string} name */ function f(name) {}
来源：http://zoh.fktsv.cn

[U117] JS：单元测试
来源：http://pba.svipenyu.cn

npm i -D vitest;  npx vitest
来源：http://hik.zhiwuduotai.top

[U118] JS：开发服务器
来源：http://qbs.xingfuxueyuan.xyz

npm i -D vite;  npx vite
来源：http://ivb.ivvv.top

[U119] JS：生产构建
来源：http://kcf.hysaishi.cn

npx vite build
来源：http://nnx.pengpengdd.cyou

[U120] JS：读取环境变量（Vite）
来源：http://pfi.zhaomingkeji.xyz

import.meta.env.VITE_API_URL
来源：http://rlz.yonumen.top

================================================================================
来源：http://hdv.shuidangran.top

统计汇总
来源：http://qmo.redwolf501.top

================================================================================
来源：http://kne.xylfe.cn

按语言统计（条）：
来源：http://cfj.xylfe.cn

Python ......... 252
来源：http://jsz.tian-w.cn

PHP ............ 252
来源：http://kyg.jinqigufen.top

JavaScript ..... 252
来源：http://zaa.yj202588.top

TypeScript ..... 212
来源：http://dnj.gzhubu.top

Java ........... 212
来源：http://uqa.guannengcc.top

Go ............. 212
来源：http://wdf.aizwys.cn

Ruby ........... 212
来源：http://obq.yangfankeji.com

C# ............. 212
来源：http://mcx.daxiang520.top

C .............. 30
来源：http://ndd.sweek.top

C++ ............ 30
来源：http://yne.52xcode.cn

SQL ............ 90
来源：http://lrl.hnqzz.top

Bash ........... 80
来源：http://qji.shanyushiyangkeji.top

Kotlin ......... 15
来源：http://aeh.jyoumei.cn

Swift .......... 15
来源：http://sqs.iojbl.cn

Lua ............ 10
来源：http://sco.yuxming.cn

Perl ........... 10
来源：http://vhk.xinyue.icu

Scala .......... 10
来源：http://erm.ctjpmb.com

------------------------------------
来源：http://oat.316326.xyz

合计 ........... 2106 条
来源：http://oza.tianlin.xyz

按章节统计：
来源：http://uun.tianlin.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cyk.xuanzx.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rxr.gotoacloud.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kej.52xcode.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iko.daria6918.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hke.jinghuilouyu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xrn.hfpthk.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://shu.xinyue.icu

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://inx.birdmap.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pms.dianchejie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gsh.wangdashe.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qxn.aibaodan.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tzx.jlsjyb.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://emt.yuanzhike.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kqu.haohaochexian.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tqe.nanxinkj.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vlb.birdmap.top

Q SQL 专题                              90
来源：http://blv.bjfxy.top

R Bash 专题                             80
来源：http://zsk.sxryk.cn

S C / C++ 专题                          60
来源：http://kkr.zycfv.cn

T 其他语言补充                          60
来源：http://ojy.bbcook.cn

U 高频实用片段                         120
来源：http://evl.jianghu66.top

------------------------------------
来源：http://pae.zycfv.cn

合计                                  2106 条
来源：http://fzg.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://xbj.fengsongda.top

使用提醒
来源：http://uow.havefunace.top

--------------------------------------------------------------------------------
来源：http://vfb.shuidangran.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nqi.yuxming.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dfe.vqdsnc.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cjq.aizwys.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zjo.bbcook.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://woi.yfazqb.com

—— 文件结束 ——
来源：http://rcw.ehwqpu.com

================================================================================
来源：http://xtm.nanxuanxn.top

程序语言常见例子速查手册（2024 版）
来源：http://fck.snrcjt.cn

Common Programming Examples Cheat Book
来源：http://yuv.fzhhl.top

================================================================================
来源：http://aqg.jqgfzy.top

【收录内容】
来源：http://ghw.jianghu66.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://rlb.uphjek.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vvs.ppjwa.cn

SQL · Bash · C · C++
来源：http://nel.hnxiangtu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xwf.jinyuanbaomall.cn

【使用说明】
来源：http://msu.ppjwa.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wce.jinghuilouyu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dch.jinyuanbaomall.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wss.andypj.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vwz.birdmap.top

Bash:  Shell         C:     C             C++:   C++
来源：http://wfg.andypj.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sav.ppjwa.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vgt.bbcook.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wco.zhongyouzk.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lqg.52xcode.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kto.jinqigfzy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nlx.vehdjk.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kbo.hcnkem.com

【文件统计】
来源：http://njh.yj20258888.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://uia.fktsv.cn

--------------------------------------------------------------------------------
来源：http://uat.sweek.top

目  录
来源：http://pnl.yfazqb.com

--------------------------------------------------------------------------------
来源：http://iwz.svipenyu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://djo.cqqwz.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nsq.dashuyun.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vea.yj202588.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zpm.chenjidiqi.icu

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xet.yj202588.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tqh.sweek.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mnx.pengpengdd.cyou

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ani.jlsjyb.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://acp.sufxvd.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ojo.haohaochexian.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vol.xylfe.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tqv.aibaodan.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hvi.guowangkeji.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wxm.yonumen.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uxv.ppjwa.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://chw.shangyingyoupin.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://apn.smart0.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://uos.tian-w.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fjk.aizwys.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ywp.jlsjyb.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hay.epnwcf.com

================================================================================
来源：http://fli.yvedp.cn

A. 基础语法与类型
来源：http://tdr.yonumen.top

================================================================================
来源：http://uul.ydjk.org.cn

[A01] Hello World
来源：http://lcm.zdqjudy.top

Py:   print("Hello, World!")
来源：http://uti.epnwcf.com

PHP:  echo "Hello, World!";
来源：http://fhe.yfazqb.com

JS:   console.log("Hello, World!");
来源：http://aol.wangdashe.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gan.zhengqikj.top

Java: System.out.println("Hello, World!");
来源：http://fpk.vehdjk.com

Go:   fmt.Println("Hello, World!")
来源：http://eoc.aibaodan.cn

Ruby: puts "Hello, World!"
来源：http://rdp.epnwcf.com

C#:   Console.WriteLine("Hello, World!");
来源：http://vss.cucudq.cn

[A02] 变量声明与赋值
来源：http://kbo.xingfuxueyuan.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lyk.ydjk.org.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yxb.snrcjt.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xvl.316326.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sgn.hysaishi.cn

Java: String name = "Alex"; int age = 20;
来源：http://nue.jinqigufen.top

Go:   name := "Alex"; age := 20
来源：http://qby.0kj1m.cn

Ruby: name = "Alex"; age = 20
来源：http://gul.hesvh.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hkt.zhijiandao.cn

[A03] 常量定义
来源：http://unv.zhijiandao.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zxi.yvedp.cn

PHP:  const PI = 3.14159;
来源：http://lza.sufxvd.cn

JS:   const PI = 3.14159;
来源：http://tzu.xingfuxueyuan.xyz

TS:   const PI: number = 3.14159;
来源：http://lnb.sjlbkw.cn

Java: static final double PI = 3.14159;
来源：http://amq.yj20258888.top

Go:   const PI = 3.14159
来源：http://jys.yonumen.top

Ruby: PI = 3.14159
来源：http://mqd.zhengqikj.top

C#:   const double PI = 3.14159;
来源：http://tee.xuetiantiany.cn

[A04] 判断变量类型
来源：http://qcp.daria6918.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://scy.cashguo.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://glo.hnqzz.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://roo.zhongyouzk.top

TS:   typeof x; x instanceof Date
来源：http://cjw.ywan-chungtsiang.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fht.yangfankeji.com

Go:   reflect.TypeOf(x).Name()
来源：http://oey.nwbrower.top

Ruby: x.class; x.is_a?(Integer)
来源：http://oxg.aibaodan.cn

C#:   x.GetType().Name; x is int
来源：http://hyz.ehwqpu.com

[A05] 整数除法与取模
来源：http://idm.sxryk.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yfk.shanyushiyangkeji.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ako.cdnleiting.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ypi.yueranfly.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cdt.sysykeji.top

Java: 7 / 2; 7 % 2
来源：http://zwj.wangdashe.top

Go:   7 / 2; 7 % 2
来源：http://mda.dashuyun.cn

Ruby: 7 / 2; 7 % 2
来源：http://pdh.zycfv.cn

C#:   7 / 2; 7 % 2
来源：http://rqt.hfpthk.cn

[A06] 字符串转数字
来源：http://fiu.snrcjt.cn

Py:   int("42"); float("3.14")
来源：http://nkw.yongpay.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sxq.bjfxy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jnb.snrcjt.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cwa.mhx1999.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://afn.cdnleiting.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gbx.guowangkeji.top

Ruby: "42".to_i; "3.14".to_f
来源：http://znb.sufxvd.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sfz.hysaishi.cn

[A07] 数字转字符串
来源：http://adw.jinqigfzy.top

Py:   str(42)
来源：http://lds.epnwcf.com

PHP:  (string) 42; strval(42)
来源：http://bkb.epnwcf.com

JS:   String(42); (42).toString()
来源：http://kaw.yfazqb.com

TS:   String(42)
来源：http://cji.tian-w.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://sxt.gogol.net.cn

Go:   strconv.Itoa(42)
来源：http://vwy.havefunace.top

Ruby: 42.to_s
来源：http://cxw.ybcxt.top

C#:   42.ToString()
来源：http://agz.yj202588.top

[A08] 取整与四舍五入
来源：http://bvx.xziqi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gyw.sweek.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ied.shanyushiyangtech.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wte.andypj.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ats.ctjpmb.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hvn.tianlin.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kuo.hongshengwenyu.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://lqa.mhx1999.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yzk.bjfxy.top

[A09] 绝对值与最大最小值
来源：http://aro.vehdjk.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qzd.jianghu66.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vje.zdbjq.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jmq.ybcxt.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ayk.vqdsnc.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jee.quarkkingdee.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rhd.jqgufenzy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fvx.cucudq.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sli.xuanzx.com

[A10] 生成随机数
来源：http://mmv.iojbl.cn

Py:   import random; random.randint(1, 100)
来源：http://spu.gzhubu.top

PHP:  random_int(1, 100);
来源：http://rkr.nwbrower.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pmn.yanxiufei.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ipn.chenzaomai.com

Java: new Random().nextInt(100) + 1
来源：http://cya.jinyuanbaomall.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://aby.dashuyun.cn

Ruby: rand(1..100)
来源：http://bnd.svipenyu.cn

C#:   new Random().Next(1, 101)
来源：http://rnj.ydzc1.top

[A11] 条件表达式（三元）
来源：http://tik.svipenyu.cn

Py:   "yes" if x > 0 else "no"
来源：http://suy.yanxiufei.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://bod.yanxiufei.cn

JS:   x > 0 ? "yes" : "no"
来源：http://opc.fanxiaobao.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://ngr.52xcode.cn

Java: x > 0 ? "yes" : "no"
来源：http://hmh.jiagoushi.top

Go:   // 无三元运算符，需用 if 语句
来源：http://vat.wangdashe.top

Ruby: x > 0 ? "yes" : "no"
来源：http://qgy.ydjk.org.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zfq.chenzaomai.com

[A12] 字符串插值 / 格式化
来源：http://hyz.xuanzx.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kgc.ppjwa.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://izg.hcnkem.com

JS:   `Hello, ${name}!`
来源：http://gya.quarkkingdee.top

TS:   `Hello, ${name}!`
来源：http://oek.gaohongyu789.top

Java: "Hello, %s!".formatted(name)
来源：http://vig.aizwys.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vtb.jinyuanbaomall.cn

Ruby: "Hello, #{name}!"
来源：http://jns.sjlbkw.cn

C#:   $"Hello, {name}!"
来源：http://fdk.havefunace.top

[A13] 多行字符串（练习 \n 转义）
来源：http://zlu.smart0.xyz

Py:   "第一行\n第二行"
来源：http://asz.zycfv.cn

PHP:  "第一行\n第二行"
来源：http://tex.wangdashe.top

JS:   "第一行\n第二行"
来源：http://nvj.gaohongyu789.top

TS:   "第一行\n第二行"
来源：http://cmz.shangyingyoupin.top

Java: "第一行\n第二行"
来源：http://uyo.mhx1999.top

Go:   "第一行\n第二行"
来源：http://lbd.epnwcf.com

Ruby: "第一行\n第二行"
来源：http://ymt.hnqzz.top

C#:   "第一行\n第二行"
来源：http://wad.fanxiaobao.xyz

[A14] 注释写法
来源：http://okm.shuidangran.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://rzr.tian-w.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fyk.iojbl.cn

JS:   // 单行；/* 多行 */
来源：http://sfh.hongshengwenyu.top

TS:   // 单行；/* 多行 */
来源：http://hin.sweek.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bqn.daria6918.cn

Go:   // 单行；/* 多行 */
来源：http://qua.tianlin.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://siz.9152youxi.cn

C#:   // 单行；/* 多行 */
来源：http://bqu.c1oappe.top

[A15] 空值判断与默认值
来源：http://pxg.fanxiaobao.xyz

Py:   value = data or "默认值"
来源：http://ffg.andypj.xyz

PHP:  $value = $data ?? "默认值";
来源：http://xun.jianghu66.top

JS:   const value = data ?? "默认值";
来源：http://hid.jlsjyb.cn

TS:   const value = data ?? "默认值";
来源：http://uki.jinqigufen.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ayp.316326.xyz

Go:   if data == "" { data = "默认值" }
来源：http://ccy.pycfn.com

Ruby: value = data || "默认值"
来源：http://xnv.yueranfly.top

C#:   var value = data ?? "默认值";
来源：http://fyp.c1oappe.top

[A16] 真假值判断规则
来源：http://nci.fktsv.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tlc.jinqigufen.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zdp.sxryk.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pvj.tian-w.cn

TS:   if (!x) {}
来源：http://geh.hnxiangtu.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wki.fktsv.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ush.vehdjk.com

Ruby: unless x            # nil 与 false 为假
来源：http://zwh.hesvh.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wpe.xziqi.cn

[A17] 位运算
来源：http://kas.fzhhl.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nfv.sufxvd.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hxf.zhengqikj.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vxv.jinyuanbaomall.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fvq.nanxinkj.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ldi.zhoulong.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lin.sjlbkw.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ogf.sufxvd.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tkw.redwolf501.top

[A18] 字符与 ASCII 码互转
来源：http://zec.cheryme.top

Py:   ord("A"); chr(65)
来源：http://puu.ppjwa.cn

PHP:  ord("A"); chr(65)
来源：http://obj.hysaishi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://epd.redwolf501.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cok.jinyuanbaomall.cn

Java: (int) 'A'; (char) 65
来源：http://twh.hcnkem.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nak.hysaishi.cn

Ruby: "A".ord; 65.chr
来源：http://olr.wangshuangyany.cn


<!-- 参考信息 -->