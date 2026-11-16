代发 wailian999

[U105] JS：节流
来源：http://zzy.kuanghao11.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://egm.epnwcf.com

[U106] JS：日期格式化
来源：http://eru.zhijiandao.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cih.meibo888.top

[U107] JS：数字千分位
来源：http://diu.cheryme.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hvw.yfazqb.com

[U108] JS：随机整数
来源：http://gcb.cqqwz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://efx.kuanghao11.cn

[U109] JS：数组分组
来源：http://feq.daria6918.cn

Object.groupBy(arr, x => x.type)
来源：http://rsa.wangshuangyany.cn

[U110] JS：数组分块
来源：http://pmp.0kj1m.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://daz.zhiwuduotai.top

[U111] JS：对象转 Map
来源：http://mei.chenzaomai.com

new Map(Object.entries(obj))
来源：http://wud.feifeiyinyue.top

[U112] JS：字符串补位
来源：http://qzl.cdnleiting.top

"7".padStart(3, "0")
来源：http://tzw.hnqzz.top

[U113] JS：正则替换全部
来源：http://eik.yuanzhike.top

s.replaceAll("a", "b")
来源：http://gqi.zdbjq.cn

[U114] JS：JSON 深比较
来源：http://cnm.yangfankeji.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://pet.yfazqb.com

[U115] JS：生成 UUID
来源：http://qge.quarkkingdee.top

crypto.randomUUID()
来源：http://iph.zhengqikj.top

[U116] JS：类型检查（JSDoc）
来源：http://mda.xylfe.cn

/** @param {string} name */ function f(name) {}
来源：http://pml.jianghu66.top

[U117] JS：单元测试
来源：http://jyj.fzhhl.top

npm i -D vitest;  npx vitest
来源：http://aum.xingfuxueyuan.xyz

[U118] JS：开发服务器
来源：http://axk.jinqigufen.top

npm i -D vite;  npx vite
来源：http://qxk.dashuyun.cn

[U119] JS：生产构建
来源：http://eft.aizwys.cn

npx vite build
来源：http://wwj.yj20258.top

[U120] JS：读取环境变量（Vite）
来源：http://rae.chenjidiqi.icu

import.meta.env.VITE_API_URL
来源：http://qoz.shanyushiyangtech.top

================================================================================
来源：http://swx.52xcode.cn

统计汇总
来源：http://rqj.guannengcc.top

================================================================================
来源：http://tns.shanyushiyangkeji.top

按语言统计（条）：
来源：http://hxl.mhx1999.top

Python ......... 252
来源：http://cgb.yonumen.top

PHP ............ 252
来源：http://cni.xylfe.cn

JavaScript ..... 252
来源：http://hqc.snrcjt.cn

TypeScript ..... 212
来源：http://kir.shuidangran.top

Java ........... 212
来源：http://czx.9152youxi.cn

Go ............. 212
来源：http://qdq.shangyingyoupin.top

Ruby ........... 212
来源：http://hkw.wangdashe.top

C# ............. 212
来源：http://lsc.nanxuanxn.top

C .............. 30
来源：http://vvz.shanyushiyangtech.top

C++ ............ 30
来源：http://bpk.cheryme.top

SQL ............ 90
来源：http://gdi.jqgufenzy.top

Bash ........... 80
来源：http://tiz.jinqigfzy.top

Kotlin ......... 15
来源：http://cyu.gotoacloud.top

Swift .......... 15
来源：http://klu.zhoulong.xyz

Lua ............ 10
来源：http://ika.ehwqpu.com

Perl ........... 10
来源：http://jzp.sufxvd.cn

Scala .......... 10
来源：http://yll.yongpay.top

------------------------------------
来源：http://fyh.cashguo.top

合计 ........... 2106 条
来源：http://zcw.smart0.xyz

按章节统计：
来源：http://rwk.uphjek.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zpj.gzhubu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://clt.pengpengdd.cyou

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qsg.quarkkingdee.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://evo.cqqwz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://esy.jinghuilouyu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zvq.meibo888.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nzx.birdmap.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dtq.hammf.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ypo.chenjidiqi.icu

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yxo.chenlongwang.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zyt.quarkkingdee.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pcl.sweek.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hgw.guannengcc.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xpe.fktsv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://amn.fzhhl.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ksx.zdbjq.cn

Q SQL 专题                              90
来源：http://pfc.gotoacloud.top

R Bash 专题                             80
来源：http://dog.yangfankeji.com

S C / C++ 专题                          60
来源：http://ute.uphjek.com

T 其他语言补充                          60
来源：http://hqd.zdbjq.cn

U 高频实用片段                         120
来源：http://syx.quarkkingdee.top

------------------------------------
来源：http://mgg.c1oappe.top

合计                                  2106 条
来源：http://mhi.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://ipi.iojbl.cn

使用提醒
来源：http://rir.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://klu.hnxiangtu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hhv.zycfv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ioq.yongpay.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dmw.dashuyun.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fob.bjfxy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rog.snrcjt.cn

—— 文件结束 ——
来源：http://ygf.meibo888.top

================================================================================
来源：http://sju.shzxlz.cn

程序语言常见例子速查手册（2024 版）
来源：http://qvx.fktsv.cn

Common Programming Examples Cheat Book
来源：http://ows.316326.xyz

================================================================================
来源：http://fam.haohaochexian.top

【收录内容】
来源：http://hno.jianghu66.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hvs.jinqigfzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fdh.tarul.cn

SQL · Bash · C · C++
来源：http://osn.jqgufenzy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://flg.ydjk.org.cn

【使用说明】
来源：http://lxn.redwolf501.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://psy.quarkkingdee.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wfk.bbcook.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qop.52xcode.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ykw.cashguo.top

Bash:  Shell         C:     C             C++:   C++
来源：http://lxt.0kj1m.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ocs.gogol.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ohn.0kj1m.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jwh.shanyushiyangtech.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rzb.hysaishi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mzq.guowangkeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cxq.zhiwuduotai.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://owm.nanxuanxn.top

【文件统计】
来源：http://xyh.zdbjq.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nkz.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://rnb.zhongyouzk.top

目  录
来源：http://izn.yj202588.top

--------------------------------------------------------------------------------
来源：http://mli.tanke756.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hws.hnqzz.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://abd.hesvh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://noy.ctjpmb.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mjv.ybcxt.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cjl.hysaishi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://osk.hnqzz.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wkh.9152youxi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xry.jiagoushi.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vgg.yj20258888.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ilt.pengpengdd.cyou

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vmd.chenlongwang.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rds.yonumen.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ith.sufxvd.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hnu.zhongyouzk.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pxm.yueranfly.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ftz.jlsjyb.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vzq.tianlin.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://yfv.sjlbkw.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://iws.zhengqikj.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fwg.yj202588.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zim.iojbl.cn

================================================================================
来源：http://wwb.redwolf501.top

A. 基础语法与类型
来源：http://tpz.nanxinkj.top

================================================================================
来源：http://cxe.jlsjyb.cn

[A01] Hello World
来源：http://ohs.xuetiantiany.cn

Py:   print("Hello, World!")
来源：http://nmf.hysaishi.cn

PHP:  echo "Hello, World!";
来源：http://oii.gotoacloud.top

JS:   console.log("Hello, World!");
来源：http://htt.shzxlz.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ntz.gogol.net.cn

Java: System.out.println("Hello, World!");
来源：http://qrp.ydjk.org.cn

Go:   fmt.Println("Hello, World!")
来源：http://mnr.haohaochexian.top

Ruby: puts "Hello, World!"
来源：http://bqq.jianghu66.top

C#:   Console.WriteLine("Hello, World!");
来源：http://nup.redwolf501.top

[A02] 变量声明与赋值
来源：http://ssr.ehwqpu.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cas.yueranfly.top

PHP:  $name = "Alex"; $age = 20;
来源：http://gpc.jinqigfzy.top

JS:   let name = "Alex"; const age = 20;
来源：http://yzd.cdnleiting.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qki.tarul.cn

Java: String name = "Alex"; int age = 20;
来源：http://wkf.ywan-chungtsiang.top

Go:   name := "Alex"; age := 20
来源：http://dod.cucudq.cn

Ruby: name = "Alex"; age = 20
来源：http://fct.yongpay.top

C#:   string name = "Alex"; int age = 20;
来源：http://frc.pycfn.com

[A03] 常量定义
来源：http://ytu.zhengqikj.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tag.feifeiyinyue.top

PHP:  const PI = 3.14159;
来源：http://ptz.epnwcf.com

JS:   const PI = 3.14159;
来源：http://aza.tian-w.cn

TS:   const PI: number = 3.14159;
来源：http://lli.shanyushiyangtech.top

Java: static final double PI = 3.14159;
来源：http://lcw.hesvh.cn

Go:   const PI = 3.14159
来源：http://fff.fzhhl.top

Ruby: PI = 3.14159
来源：http://iqs.zhixingplan.top

C#:   const double PI = 3.14159;
来源：http://uly.yj202588.top

[A04] 判断变量类型
来源：http://hol.iojbl.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gxi.jiagoushi.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://elm.jqgufenzy.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wwz.zycfv.cn

TS:   typeof x; x instanceof Date
来源：http://fkq.tarul.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mnt.xinyue.icu

Go:   reflect.TypeOf(x).Name()
来源：http://dtt.zhijiandao.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ojs.tanke756.top

C#:   x.GetType().Name; x is int
来源：http://afa.hfpthk.cn

[A05] 整数除法与取模
来源：http://qat.hywenlv.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rpp.cqqwz.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rhd.zhoulong.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wua.yj20258.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://htv.pycfn.com

Java: 7 / 2; 7 % 2
来源：http://huc.ctjpmb.com

Go:   7 / 2; 7 % 2
来源：http://dpz.52xcode.cn

Ruby: 7 / 2; 7 % 2
来源：http://iwm.316326.xyz

C#:   7 / 2; 7 % 2
来源：http://fzq.hnqzz.top

[A06] 字符串转数字
来源：http://ntg.xylfe.cn

Py:   int("42"); float("3.14")
来源：http://pat.ydzc1.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bsx.xuanzx.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://isc.shzxlz.cn

TS:   parseInt("42", 10); Number("42")
来源：http://dyn.sysykeji.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qqa.jyoumei.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wyr.zhijiandao.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xxf.yongpay.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://flz.bjfxy.top

[A07] 数字转字符串
来源：http://xsr.cucudq.cn

Py:   str(42)
来源：http://izl.jinghuilouyu.cn

PHP:  (string) 42; strval(42)
来源：http://ixn.cdnleiting.top

JS:   String(42); (42).toString()
来源：http://pqi.xinyue.icu

TS:   String(42)
来源：http://cqb.nanxinkj.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ido.shanyushiyangkeji.top

Go:   strconv.Itoa(42)
来源：http://kyu.haohaochexian.top

Ruby: 42.to_s
来源：http://ssr.fengsongda.top

C#:   42.ToString()
来源：http://chd.chenlongwang.top

[A08] 取整与四舍五入
来源：http://act.nwbrower.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vmt.xingfuxueyuan.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://sjs.shuidangran.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kle.birdmap.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pyx.yongpay.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hda.zdbjq.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hil.uphjek.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://xhx.dianchejie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://apg.gotoacloud.top

[A09] 绝对值与最大最小值
来源：http://bjf.xuetiantiany.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cgf.zhengqikj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xgs.fzhhl.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mkr.yonumen.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cqv.xingfuxueyuan.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://igs.shzxlz.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tsy.jyoumei.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gug.jianghu66.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fki.cqqwz.cn

[A10] 生成随机数
来源：http://wky.hongshengwenyu.top

Py:   import random; random.randint(1, 100)
来源：http://ugs.nwbrower.top

PHP:  random_int(1, 100);
来源：http://uze.gaohongyu789.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://waj.tian-w.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hvt.zdqjudy.top

Java: new Random().nextInt(100) + 1
来源：http://fgw.shanyushiyangtech.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vie.nanxuanxn.top

Ruby: rand(1..100)
来源：http://qxe.ydjk.org.cn

C#:   new Random().Next(1, 101)
来源：http://yqw.nanxinkj.top

[A11] 条件表达式（三元）
来源：http://nsm.hongshengwenyu.top

Py:   "yes" if x > 0 else "no"
来源：http://cri.xziqi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jzy.ydzc1.top

JS:   x > 0 ? "yes" : "no"
来源：http://stq.yuxming.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vxo.tarul.cn

Java: x > 0 ? "yes" : "no"
来源：http://cta.shangyingyoupin.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ybs.yvedp.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://eki.yanxiufei.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mih.fanxiaobao.xyz

[A12] 字符串插值 / 格式化
来源：http://yrg.fktsv.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cbf.fktsv.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cso.316326.xyz

JS:   `Hello, ${name}!`
来源：http://abm.shanyushiyangkeji.top

TS:   `Hello, ${name}!`
来源：http://per.zhoulong.xyz

Java: "Hello, %s!".formatted(name)
来源：http://jwc.chenlongwang.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ugd.yangfankeji.com

Ruby: "Hello, #{name}!"
来源：http://ebz.fanxiaobao.xyz

C#:   $"Hello, {name}!"
来源：http://gbo.ydjk.org.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://kug.hywenlv.cn

Py:   "第一行\n第二行"
来源：http://lgr.chenjidiqi.icu

PHP:  "第一行\n第二行"
来源：http://ylf.jlsjyb.cn

JS:   "第一行\n第二行"
来源：http://mtq.haohaochexian.top

TS:   "第一行\n第二行"
来源：http://axd.sufxvd.cn

Java: "第一行\n第二行"
来源：http://lng.snrcjt.cn

Go:   "第一行\n第二行"
来源：http://eow.chenjidiqi.icu

Ruby: "第一行\n第二行"
来源：http://vdt.xuanzx.com

C#:   "第一行\n第二行"
来源：http://jql.fehbvm.com

[A14] 注释写法
来源：http://qov.hcnkem.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://eul.snrcjt.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://chv.ivvv.top

JS:   // 单行；/* 多行 */
来源：http://crw.cashguo.top

TS:   // 单行；/* 多行 */
来源：http://kpj.0kj1m.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cev.chenlongwang.top

Go:   // 单行；/* 多行 */
来源：http://flg.hysaishi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dnr.sweek.top

C#:   // 单行；/* 多行 */
来源：http://twt.guannengcc.top

[A15] 空值判断与默认值
来源：http://ihv.hfpthk.cn

Py:   value = data or "默认值"
来源：http://gis.c1oappe.top

PHP:  $value = $data ?? "默认值";
来源：http://ekf.fengsongda.top

JS:   const value = data ?? "默认值";
来源：http://ilz.tanke756.top

TS:   const value = data ?? "默认值";
来源：http://nco.daxiang520.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://byp.shangyingyoupin.top

Go:   if data == "" { data = "默认值" }
来源：http://uqr.cqqwz.cn

Ruby: value = data || "默认值"
来源：http://cem.fengsongda.top

C#:   var value = data ?? "默认值";
来源：http://sen.xuanzx.com

[A16] 真假值判断规则
来源：http://ozk.zycfv.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qkh.cdnleiting.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cqg.gogol.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rmt.tanke756.top

TS:   if (!x) {}
来源：http://yzw.sweek.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://aec.daxiang520.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ewb.yuanzhike.top

Ruby: unless x            # nil 与 false 为假
来源：http://cjk.chenzaomai.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jnh.sjlbkw.cn

[A17] 位运算
来源：http://zbw.cqqwz.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pca.guowangkeji.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ppm.shangyingyoupin.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://brm.cdnleiting.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tes.ppjwa.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bvg.chenlongwang.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mbt.ppjwa.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://umn.gzhubu.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qnt.zhaomingkeji.xyz

[A18] 字符与 ASCII 码互转
来源：http://hhf.zhijiandao.cn

Py:   ord("A"); chr(65)
来源：http://add.sweek.top

PHP:  ord("A"); chr(65)
来源：http://pab.gogol.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wvi.zhijiandao.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://off.cucudq.cn

Java: (int) 'A'; (char) 65
来源：http://tqs.dashuyun.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nhk.yongpay.top

Ruby: "A".ord; 65.chr
来源：http://mqg.tian-w.cn


<!-- 参考信息 -->