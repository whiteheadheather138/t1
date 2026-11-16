代发 wailian999

[U101] JS：classList 操作
来源：http://zhx.9152youxi.cn

el.classList.toggle("active")
来源：http://iim.tian-w.cn

[U102] JS：本地存储
来源：http://kdb.hnxiangtu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://tax.xylfe.cn

[U103] JS：定时器
来源：http://auy.ivvv.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qsv.chenzaomai.com

[U104] JS：防抖
来源：http://tja.pycfn.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tor.hammf.cn

[U105] JS：节流
来源：http://ire.uphjek.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uua.ppjwa.cn

[U106] JS：日期格式化
来源：http://jak.yanxiufei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pom.bjfxy.top

[U107] JS：数字千分位
来源：http://sxr.316326.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gxx.cashguo.top

[U108] JS：随机整数
来源：http://krz.ehwqpu.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zyy.daxiang520.top

[U109] JS：数组分组
来源：http://dah.ydjk.org.cn

Object.groupBy(arr, x => x.type)
来源：http://mlr.jqgfzy.top

[U110] JS：数组分块
来源：http://khu.havefunace.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cil.chenzaomai.com

[U111] JS：对象转 Map
来源：http://jph.jqgufenzy.top

new Map(Object.entries(obj))
来源：http://whd.shanyushiyangtech.top

[U112] JS：字符串补位
来源：http://cku.pengpengdd.cyou

"7".padStart(3, "0")
来源：http://txy.cdnleiting.top

[U113] JS：正则替换全部
来源：http://xau.gogol.net.cn

s.replaceAll("a", "b")
来源：http://mqf.pycfn.com

[U114] JS：JSON 深比较
来源：http://bkh.jinqigufen.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://nyh.fengsongda.top

[U115] JS：生成 UUID
来源：http://rgk.yonumen.top

crypto.randomUUID()
来源：http://sfs.aizwys.cn

[U116] JS：类型检查（JSDoc）
来源：http://zum.birdmap.top

/** @param {string} name */ function f(name) {}
来源：http://xjc.sweek.top

[U117] JS：单元测试
来源：http://dxp.nanxinkj.top

npm i -D vitest;  npx vitest
来源：http://dey.vqdsnc.cn

[U118] JS：开发服务器
来源：http://yzd.yuanzhike.top

npm i -D vite;  npx vite
来源：http://oue.nwbrower.top

[U119] JS：生产构建
来源：http://dpp.guannengcc.top

npx vite build
来源：http://agz.haohaochexian.top

[U120] JS：读取环境变量（Vite）
来源：http://dnn.uphjek.com

import.meta.env.VITE_API_URL
来源：http://qoh.ydjk.org.cn

================================================================================
来源：http://uqe.gzhubu.top

统计汇总
来源：http://knd.zhijiandao.cn

================================================================================
来源：http://pdt.ehwqpu.com

按语言统计（条）：
来源：http://knm.chenjidiqi.icu

Python ......... 252
来源：http://eiz.ydzc1.top

PHP ............ 252
来源：http://pjk.zhijiandao.cn

JavaScript ..... 252
来源：http://lai.snrcjt.cn

TypeScript ..... 212
来源：http://zmg.fzhhl.top

Java ........... 212
来源：http://lli.aibaodan.cn

Go ............. 212
来源：http://jtr.mhx1999.top

Ruby ........... 212
来源：http://nmy.zdbjq.cn

C# ............. 212
来源：http://adc.yuanzhike.top

C .............. 30
来源：http://lft.kuanghao11.cn

C++ ............ 30
来源：http://dwq.shangyingyoupin.top

SQL ............ 90
来源：http://gtr.chenlongwang.top

Bash ........... 80
来源：http://tyc.shuidangran.top

Kotlin ......... 15
来源：http://eap.jianghu66.top

Swift .......... 15
来源：http://xuh.jinqigfzy.top

Lua ............ 10
来源：http://vml.ywan-chungtsiang.top

Perl ........... 10
来源：http://jet.gzhubu.top

Scala .......... 10
来源：http://iyr.hammf.cn

------------------------------------
来源：http://yhf.jinghuilouyu.cn

合计 ........... 2106 条
来源：http://ulv.mhx1999.top

按章节统计：
来源：http://etr.mhx1999.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bmm.ppjwa.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rpr.gaohongyu789.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jwt.nanxinkj.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://psk.sweek.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ecm.aizwys.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sxa.jianghu66.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jtb.ywan-chungtsiang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yrh.birdmap.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://loq.zdqjudy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zey.shuidangran.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bmk.haohaochexian.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://plj.yvedp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wlh.tianlin.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://okn.yonumen.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dck.yj202588.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oag.jinyuanbaomall.cn

Q SQL 专题                              90
来源：http://jwk.fengsongda.top

R Bash 专题                             80
来源：http://rbt.yanxiufei.cn

S C / C++ 专题                          60
来源：http://sid.ivvv.top

T 其他语言补充                          60
来源：http://pol.jlsjyb.cn

U 高频实用片段                         120
来源：http://lns.shanyushiyangkeji.top

------------------------------------
来源：http://bxv.yfazqb.com

合计                                  2106 条
来源：http://uod.tanke756.top

--------------------------------------------------------------------------------
来源：http://aly.cucudq.cn

使用提醒
来源：http://tvg.wangshuangyany.cn

--------------------------------------------------------------------------------
来源：http://iyf.daria6918.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tfy.cashguo.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tqp.sweek.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nus.bbcook.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ilo.zhijiandao.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cah.yangfankeji.com

—— 文件结束 ——
来源：http://dod.zycfv.cn

================================================================================
来源：http://nec.tianlin.xyz

程序语言常见例子速查手册（2024 版）
来源：http://hqq.guannengcc.top

Common Programming Examples Cheat Book
来源：http://ucl.epnwcf.com

================================================================================
来源：http://vza.ivvv.top

【收录内容】
来源：http://qvh.yuanzhike.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://skf.jqgfzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cfv.jqgfzy.top

SQL · Bash · C · C++
来源：http://dgh.bjfxy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wky.yuxming.cn

【使用说明】
来源：http://xdr.pengpengdd.cyou

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nhp.vqdsnc.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ecg.zhiwuduotai.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mnm.tarul.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hnz.kuanghao11.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jjl.zhoulong.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gcn.cdnleiting.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dba.shanyushiyangtech.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fvv.sysykeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lpd.zhijiandao.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ndz.dashuyun.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gtz.xylfe.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lws.ctjpmb.com

【文件统计】
来源：http://luo.hnqzz.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dtu.redwolf501.top

--------------------------------------------------------------------------------
来源：http://hdp.hesvh.cn

目  录
来源：http://eye.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://lor.vqdsnc.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kfw.chenlongwang.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ldx.chenjidiqi.icu

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://doh.guannengcc.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://doz.c1oappe.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jwy.ywan-chungtsiang.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pcf.tanke756.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dqf.gotoacloud.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gtv.jiagoushi.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hgq.guannengcc.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gii.guowangkeji.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wor.tarul.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://oil.shzxlz.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rqm.xuanzx.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ctr.ehwqpu.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ikd.cucudq.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zax.shangyingyoupin.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tbv.chenjidiqi.icu

R. Bash 专题                   （第 18 节，80 条）
来源：http://rnt.dashuyun.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sls.zhiwuduotai.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uow.hongshengwenyu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xjv.tianlin.xyz

================================================================================
来源：http://ntc.hysaishi.cn

A. 基础语法与类型
来源：http://zjm.shangyingyoupin.top

================================================================================
来源：http://vfl.jinqigfzy.top

[A01] Hello World
来源：http://jdm.c1oappe.top

Py:   print("Hello, World!")
来源：http://xcg.ydjk.org.cn

PHP:  echo "Hello, World!";
来源：http://jsc.shuidangran.top

JS:   console.log("Hello, World!");
来源：http://ejw.daria6918.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kxy.fktsv.cn

Java: System.out.println("Hello, World!");
来源：http://qkl.daria6918.cn

Go:   fmt.Println("Hello, World!")
来源：http://jtm.gotoacloud.top

Ruby: puts "Hello, World!"
来源：http://anw.xylfe.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://azn.redwolf501.top

[A02] 变量声明与赋值
来源：http://skc.shuidangran.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bmn.yonumen.top

PHP:  $name = "Alex"; $age = 20;
来源：http://lfg.xuetiantiany.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tdj.xylfe.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nvr.fanxiaobao.xyz

Java: String name = "Alex"; int age = 20;
来源：http://pud.nanxinkj.top

Go:   name := "Alex"; age := 20
来源：http://bxf.gotoacloud.top

Ruby: name = "Alex"; age = 20
来源：http://ssz.fzhhl.top

C#:   string name = "Alex"; int age = 20;
来源：http://ryj.fengsongda.top

[A03] 常量定义
来源：http://cmu.ppjwa.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cnd.yanxiufei.cn

PHP:  const PI = 3.14159;
来源：http://nxx.iojbl.cn

JS:   const PI = 3.14159;
来源：http://kkf.chenlongwang.top

TS:   const PI: number = 3.14159;
来源：http://ynj.quarkkingdee.top

Java: static final double PI = 3.14159;
来源：http://rov.shangyingyoupin.top

Go:   const PI = 3.14159
来源：http://dtt.c1oappe.top

Ruby: PI = 3.14159
来源：http://plz.zycfv.cn

C#:   const double PI = 3.14159;
来源：http://ghp.chenzaomai.com

[A04] 判断变量类型
来源：http://uzv.zhixingplan.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://nnl.ybcxt.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://abl.tianlin.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kmv.guannengcc.top

TS:   typeof x; x instanceof Date
来源：http://pxh.chenlongwang.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://krg.hywenlv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://nez.tanke756.top

Ruby: x.class; x.is_a?(Integer)
来源：http://sup.jqgfzy.top

C#:   x.GetType().Name; x is int
来源：http://wbj.ctjpmb.com

[A05] 整数除法与取模
来源：http://vry.snrcjt.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qiz.jiagoushi.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://kjt.gaohongyu789.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qxo.zhijiandao.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rcl.zhongyouzk.top

Java: 7 / 2; 7 % 2
来源：http://jkv.ivvv.top

Go:   7 / 2; 7 % 2
来源：http://ykg.aizwys.cn

Ruby: 7 / 2; 7 % 2
来源：http://hdy.andypj.xyz

C#:   7 / 2; 7 % 2
来源：http://ubp.tianlin.xyz

[A06] 字符串转数字
来源：http://fqe.dashuyun.cn

Py:   int("42"); float("3.14")
来源：http://zfu.jianghu66.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://anw.yuanzhike.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://iry.ehwqpu.com

TS:   parseInt("42", 10); Number("42")
来源：http://wcf.52xcode.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://exg.bbcook.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vgn.yvedp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://gja.dashuyun.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hjo.gaohongyu789.top

[A07] 数字转字符串
来源：http://mwr.hnqzz.top

Py:   str(42)
来源：http://ors.jianghu66.top

PHP:  (string) 42; strval(42)
来源：http://fve.hcnkem.com

JS:   String(42); (42).toString()
来源：http://rxg.meibo888.top

TS:   String(42)
来源：http://fbn.cheryme.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://evt.yonumen.top

Go:   strconv.Itoa(42)
来源：http://dak.chenlongwang.top

Ruby: 42.to_s
来源：http://dbp.yueranfly.top

C#:   42.ToString()
来源：http://fwx.ybcxt.top

[A08] 取整与四舍五入
来源：http://xth.zdqjudy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zij.guannengcc.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://duw.ywan-chungtsiang.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qrq.feifeiyinyue.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bdq.tianlin.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lvq.yuanzhike.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://iyf.9152youxi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://dff.ydjk.org.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mug.ydjk.org.cn

[A09] 绝对值与最大最小值
来源：http://mzm.zdqjudy.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wwa.smart0.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cjb.zhaomingkeji.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nwu.xuanzx.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bte.jqgufenzy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vrn.zhoulong.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ego.yj20258888.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lsf.ybcxt.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ral.sxryk.cn

[A10] 生成随机数
来源：http://mfj.pengpengdd.cyou

Py:   import random; random.randint(1, 100)
来源：http://son.quarkkingdee.top

PHP:  random_int(1, 100);
来源：http://dqh.gotoacloud.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://iag.gzhubu.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qxe.jinqigfzy.top

Java: new Random().nextInt(100) + 1
来源：http://hds.yangfankeji.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tzt.xinyue.icu

Ruby: rand(1..100)
来源：http://gjt.cashguo.top

C#:   new Random().Next(1, 101)
来源：http://kgl.aibaodan.cn

[A11] 条件表达式（三元）
来源：http://tfx.tianlin.xyz

Py:   "yes" if x > 0 else "no"
来源：http://rua.jiagoushi.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://odt.tianlin.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://bly.yj20258888.top

TS:   x > 0 ? "yes" : "no"
来源：http://opi.andypj.xyz

Java: x > 0 ? "yes" : "no"
来源：http://uwq.uphjek.com

Go:   // 无三元运算符，需用 if 语句
来源：http://hpj.hnxiangtu.top

Ruby: x > 0 ? "yes" : "no"
来源：http://max.zhoulong.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://vnm.yj20258888.top

[A12] 字符串插值 / 格式化
来源：http://has.zdqjudy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rrd.fzhhl.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uuz.shanyushiyangtech.top

JS:   `Hello, ${name}!`
来源：http://fai.bjfxy.top

TS:   `Hello, ${name}!`
来源：http://spj.zhengqikj.top

Java: "Hello, %s!".formatted(name)
来源：http://sco.jianghu66.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cqj.sjlbkw.cn

Ruby: "Hello, #{name}!"
来源：http://obq.hcnkem.com

C#:   $"Hello, {name}!"
来源：http://gkn.zhongyouzk.top

[A13] 多行字符串（练习 \n 转义）
来源：http://irq.yangfankeji.com

Py:   "第一行\n第二行"
来源：http://wrq.fehbvm.com

PHP:  "第一行\n第二行"
来源：http://wcc.yj20258.top

JS:   "第一行\n第二行"
来源：http://ked.nanxinkj.top

TS:   "第一行\n第二行"
来源：http://own.birdmap.top

Java: "第一行\n第二行"
来源：http://faj.316326.xyz

Go:   "第一行\n第二行"
来源：http://llv.jlsjyb.cn

Ruby: "第一行\n第二行"
来源：http://ysm.ivvv.top

C#:   "第一行\n第二行"
来源：http://jea.shuidangran.top

[A14] 注释写法
来源：http://rxf.hywenlv.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pzz.jiagoushi.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://gqg.aizwys.cn

JS:   // 单行；/* 多行 */
来源：http://mxj.gaohongyu789.top

TS:   // 单行；/* 多行 */
来源：http://cid.wangshuangyany.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kts.uphjek.com

Go:   // 单行；/* 多行 */
来源：http://agn.zhixingplan.top

Ruby: # 单行；=begin 多行 =end
来源：http://ngs.guannengcc.top

C#:   // 单行；/* 多行 */
来源：http://kmy.fengsongda.top

[A15] 空值判断与默认值
来源：http://vvm.redwolf501.top

Py:   value = data or "默认值"
来源：http://eye.zdbjq.cn

PHP:  $value = $data ?? "默认值";
来源：http://nau.fanxiaobao.xyz

JS:   const value = data ?? "默认值";
来源：http://ztm.hfpthk.cn

TS:   const value = data ?? "默认值";
来源：http://ios.fengsongda.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ibl.jinqigufen.top

Go:   if data == "" { data = "默认值" }
来源：http://iaw.shuidangran.top

Ruby: value = data || "默认值"
来源：http://xkf.chenzaomai.com

C#:   var value = data ?? "默认值";
来源：http://hdv.zhongyouzk.top

[A16] 真假值判断规则
来源：http://avj.fzhhl.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jqp.jinqigfzy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jjv.wangshuangyany.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sns.fehbvm.com

TS:   if (!x) {}
来源：http://jmt.bbcook.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://myb.yfazqb.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bak.zhongyouzk.top

Ruby: unless x            # nil 与 false 为假
来源：http://emz.dashuyun.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wzu.gzhubu.top

[A17] 位运算
来源：http://vxn.yuxming.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wch.wangshuangyany.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nus.jinghuilouyu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sql.jyoumei.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vpp.hesvh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ivf.hnqzz.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://usr.hysaishi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hbm.jqgfzy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pqc.tanke756.top


<!-- 参考信息 -->