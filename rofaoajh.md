代发 wailian999

[U99] JS：事件监听
来源：http://lix.jqgfzy.top

el.addEventListener("click", e => {})
来源：http://dri.ehwqpu.com

[U100] JS：DOM 查询
来源：http://utc.ctjpmb.com

document.querySelector(".item")
来源：http://bwa.ydzc1.top

[U101] JS：classList 操作
来源：http://gnc.chenlongwang.top

el.classList.toggle("active")
来源：http://ldt.jiagoushi.top

[U102] JS：本地存储
来源：http://imp.xylfe.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qmg.xuetiantiany.cn

[U103] JS：定时器
来源：http://idw.jlsjyb.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qin.hesvh.cn

[U104] JS：防抖
来源：http://hmo.ppjwa.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://epd.yanxiufei.cn

[U105] JS：节流
来源：http://kvs.hywenlv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gww.vehdjk.com

[U106] JS：日期格式化
来源：http://glx.epnwcf.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zzb.guowangkeji.top

[U107] JS：数字千分位
来源：http://wwx.tarul.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jwj.snrcjt.cn

[U108] JS：随机整数
来源：http://adg.yongpay.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bwn.hnqzz.top

[U109] JS：数组分组
来源：http://jas.iojbl.cn

Object.groupBy(arr, x => x.type)
来源：http://hlr.52xcode.cn

[U110] JS：数组分块
来源：http://orr.andypj.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ojc.nanxuanxn.top

[U111] JS：对象转 Map
来源：http://yls.shzxlz.cn

new Map(Object.entries(obj))
来源：http://mty.hywenlv.cn

[U112] JS：字符串补位
来源：http://ofb.hywenlv.cn

"7".padStart(3, "0")
来源：http://ffc.jinghuilouyu.cn

[U113] JS：正则替换全部
来源：http://xys.cdnleiting.top

s.replaceAll("a", "b")
来源：http://fua.0kj1m.cn

[U114] JS：JSON 深比较
来源：http://scn.wangshuangyany.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kou.hywenlv.cn

[U115] JS：生成 UUID
来源：http://gxz.ctjpmb.com

crypto.randomUUID()
来源：http://flj.ivvv.top

[U116] JS：类型检查（JSDoc）
来源：http://mel.andypj.xyz

/** @param {string} name */ function f(name) {}
来源：http://pqe.yonumen.top

[U117] JS：单元测试
来源：http://ovm.zhaomingkeji.xyz

npm i -D vitest;  npx vitest
来源：http://yfg.sjlbkw.cn

[U118] JS：开发服务器
来源：http://fqh.daxiang520.top

npm i -D vite;  npx vite
来源：http://amp.ywan-chungtsiang.top

[U119] JS：生产构建
来源：http://dbr.zdqjudy.top

npx vite build
来源：http://xmm.ehwqpu.com

[U120] JS：读取环境变量（Vite）
来源：http://omq.bjfxy.top

import.meta.env.VITE_API_URL
来源：http://haq.tarul.cn

================================================================================
来源：http://gom.gogol.net.cn

统计汇总
来源：http://pft.cucudq.cn

================================================================================
来源：http://cfa.sweek.top

按语言统计（条）：
来源：http://jav.sufxvd.cn

Python ......... 252
来源：http://ssr.wangshuangyany.cn

PHP ............ 252
来源：http://oud.vehdjk.com

JavaScript ..... 252
来源：http://sex.fzhhl.top

TypeScript ..... 212
来源：http://hvd.yj20258888.top

Java ........... 212
来源：http://xmf.xuetiantiany.cn

Go ............. 212
来源：http://ybj.hnxiangtu.top

Ruby ........... 212
来源：http://wac.daria6918.cn

C# ............. 212
来源：http://ppy.hysaishi.cn

C .............. 30
来源：http://cvi.sxryk.cn

C++ ............ 30
来源：http://ypg.fengsongda.top

SQL ............ 90
来源：http://mrs.wangdashe.top

Bash ........... 80
来源：http://emn.hcnkem.com

Kotlin ......... 15
来源：http://qik.tanke756.top

Swift .......... 15
来源：http://nhv.iojbl.cn

Lua ............ 10
来源：http://xlh.shangyingyoupin.top

Perl ........... 10
来源：http://duh.fanxiaobao.xyz

Scala .......... 10
来源：http://jyt.jqgufenzy.top

------------------------------------
来源：http://dch.fanxiaobao.xyz

合计 ........... 2106 条
来源：http://utl.jyoumei.cn

按章节统计：
来源：http://nqc.9152youxi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pog.jlsjyb.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gen.shzxlz.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jso.shuidangran.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cfi.ivvv.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tyt.shanyushiyangkeji.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pzk.zhixingplan.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wah.zdbjq.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yvm.tian-w.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nla.yonumen.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://klq.gzhubu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ush.nanxinkj.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://omc.feifeiyinyue.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qnb.tanke756.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nki.havefunace.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xea.yuanzhike.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kqx.shanyushiyangkeji.top

Q SQL 专题                              90
来源：http://luw.fehbvm.com

R Bash 专题                             80
来源：http://nnb.yanxiufei.cn

S C / C++ 专题                          60
来源：http://cpu.hesvh.cn

T 其他语言补充                          60
来源：http://rsv.haohaochexian.top

U 高频实用片段                         120
来源：http://lpf.fzhhl.top

------------------------------------
来源：http://wur.jlsjyb.cn

合计                                  2106 条
来源：http://wle.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://ttf.sxryk.cn

使用提醒
来源：http://rth.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://dvx.hammf.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fsw.fktsv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mrg.jlsjyb.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://itr.yfazqb.com

在旧版本上使用前请先确认语法支持情况。
来源：http://pgu.ydjk.org.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://eta.shanyushiyangkeji.top

—— 文件结束 ——
来源：http://pqx.havefunace.top

================================================================================
来源：http://lxt.fehbvm.com

程序语言常见例子速查手册（2024 版）
来源：http://wqf.jinqigfzy.top

Common Programming Examples Cheat Book
来源：http://yxi.zhongyouzk.top

================================================================================
来源：http://mrn.ctjpmb.com

【收录内容】
来源：http://fdo.haohaochexian.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ugo.hongshengwenyu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cld.mhx1999.top

SQL · Bash · C · C++
来源：http://icb.hcnkem.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ckq.cashguo.top

【使用说明】
来源：http://chl.jianghu66.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cuf.ydzc1.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ofu.snrcjt.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xhf.guannengcc.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mwr.yj20258.top

Bash:  Shell         C:     C             C++:   C++
来源：http://vkj.xuetiantiany.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vnt.dashuyun.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rtq.shanyushiyangkeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://eby.iojbl.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vvk.snrcjt.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://utf.tian-w.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://uxe.ybcxt.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mym.snrcjt.cn

【文件统计】
来源：http://ojs.hfpthk.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rhn.cucudq.cn

--------------------------------------------------------------------------------
来源：http://izt.cucudq.cn

目  录
来源：http://paq.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://xxo.nwbrower.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qvr.yfazqb.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qiy.wangdashe.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ban.nanxinkj.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rzw.yuxming.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kqi.fehbvm.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xpz.nanxuanxn.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ghn.zdbjq.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mbb.sufxvd.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bkb.havefunace.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nrh.c1oappe.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://avb.jlsjyb.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lrp.zhixingplan.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jyp.zhaomingkeji.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://eir.chenjidiqi.icu

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bfp.epnwcf.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ydf.hnqzz.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tup.gaohongyu789.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://xcr.zhoulong.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://caj.yfazqb.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rlo.nwbrower.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fdp.xylfe.cn

================================================================================
来源：http://drc.jianghu66.top

A. 基础语法与类型
来源：http://xat.cdnleiting.top

================================================================================
来源：http://yin.yuanzhike.top

[A01] Hello World
来源：http://iiv.cqqwz.cn

Py:   print("Hello, World!")
来源：http://qcz.hywenlv.cn

PHP:  echo "Hello, World!";
来源：http://gux.jinghuilouyu.cn

JS:   console.log("Hello, World!");
来源：http://qrk.sjlbkw.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://atf.shuidangran.top

Java: System.out.println("Hello, World!");
来源：http://ynl.meibo888.top

Go:   fmt.Println("Hello, World!")
来源：http://fww.cqqwz.cn

Ruby: puts "Hello, World!"
来源：http://kgb.sysykeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://etg.yj202588.top

[A02] 变量声明与赋值
来源：http://tla.ywan-chungtsiang.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://agt.c1oappe.top

PHP:  $name = "Alex"; $age = 20;
来源：http://gsj.ivvv.top

JS:   let name = "Alex"; const age = 20;
来源：http://wxk.snrcjt.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://knd.hnqzz.top

Java: String name = "Alex"; int age = 20;
来源：http://ksi.sufxvd.cn

Go:   name := "Alex"; age := 20
来源：http://rrn.bbcook.cn

Ruby: name = "Alex"; age = 20
来源：http://sff.316326.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://rkr.tanke756.top

[A03] 常量定义
来源：http://xrj.cucudq.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://goy.ppjwa.cn

PHP:  const PI = 3.14159;
来源：http://ksf.hywenlv.cn

JS:   const PI = 3.14159;
来源：http://pbq.yfazqb.com

TS:   const PI: number = 3.14159;
来源：http://jzc.aizwys.cn

Java: static final double PI = 3.14159;
来源：http://cjw.hcnkem.com

Go:   const PI = 3.14159
来源：http://glu.nanxuanxn.top

Ruby: PI = 3.14159
来源：http://sal.smart0.xyz

C#:   const double PI = 3.14159;
来源：http://hvn.shangyingyoupin.top

[A04] 判断变量类型
来源：http://trr.yuxming.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gmg.hywenlv.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kpw.zhijiandao.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://uon.zhengqikj.top

TS:   typeof x; x instanceof Date
来源：http://tpd.jiagoushi.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dnu.yj20258.top

Go:   reflect.TypeOf(x).Name()
来源：http://hxd.ydjk.org.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qjs.fehbvm.com

C#:   x.GetType().Name; x is int
来源：http://ibk.yongpay.top

[A05] 整数除法与取模
来源：http://wfj.cashguo.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dpd.daxiang520.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://fkk.hongshengwenyu.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ozi.wangdashe.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ayq.tianlin.xyz

Java: 7 / 2; 7 % 2
来源：http://vmr.shanyushiyangtech.top

Go:   7 / 2; 7 % 2
来源：http://yny.xuanzx.com

Ruby: 7 / 2; 7 % 2
来源：http://rrn.yanxiufei.cn

C#:   7 / 2; 7 % 2
来源：http://xlo.aibaodan.cn

[A06] 字符串转数字
来源：http://nnn.snrcjt.cn

Py:   int("42"); float("3.14")
来源：http://asm.xuetiantiany.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://twg.chenzaomai.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wbk.c1oappe.top

TS:   parseInt("42", 10); Number("42")
来源：http://pzf.bjfxy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vru.yongpay.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mli.kuanghao11.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://htw.yj202588.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://slq.iojbl.cn

[A07] 数字转字符串
来源：http://mho.jinqigfzy.top

Py:   str(42)
来源：http://vob.svipenyu.cn

PHP:  (string) 42; strval(42)
来源：http://nuz.gzhubu.top

JS:   String(42); (42).toString()
来源：http://sts.hongshengwenyu.top

TS:   String(42)
来源：http://vcz.zhongyouzk.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://qmd.xingfuxueyuan.xyz

Go:   strconv.Itoa(42)
来源：http://wtd.zhengqikj.top

Ruby: 42.to_s
来源：http://wty.aibaodan.cn

C#:   42.ToString()
来源：http://ocu.sxryk.cn

[A08] 取整与四舍五入
来源：http://kax.ybcxt.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://urc.jiagoushi.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://upu.chenlongwang.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bfa.jianghu66.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kyk.bbcook.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://umh.dashuyun.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://end.vqdsnc.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://rxv.ppjwa.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qny.guowangkeji.top

[A09] 绝对值与最大最小值
来源：http://ffs.sweek.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lev.zhengqikj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mjj.jqgufenzy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zhd.yj20258888.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ibt.xylfe.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tpe.tian-w.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wyl.yfazqb.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qwv.ydzc1.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xbs.xingfuxueyuan.xyz

[A10] 生成随机数
来源：http://pgl.hysaishi.cn

Py:   import random; random.randint(1, 100)
来源：http://zfa.xylfe.cn

PHP:  random_int(1, 100);
来源：http://xcx.ivvv.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ozk.cashguo.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xcy.haohaochexian.top

Java: new Random().nextInt(100) + 1
来源：http://brt.sxryk.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nad.ybcxt.top

Ruby: rand(1..100)
来源：http://hpj.hysaishi.cn

C#:   new Random().Next(1, 101)
来源：http://fzr.nwbrower.top

[A11] 条件表达式（三元）
来源：http://nwa.zdbjq.cn

Py:   "yes" if x > 0 else "no"
来源：http://smf.fktsv.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://uoj.kuanghao11.cn

JS:   x > 0 ? "yes" : "no"
来源：http://tbg.sjlbkw.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vur.uphjek.com

Java: x > 0 ? "yes" : "no"
来源：http://jla.yuxming.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xbx.smart0.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://eya.ywan-chungtsiang.top

C#:   x > 0 ? "yes" : "no"
来源：http://ske.bjfxy.top

[A12] 字符串插值 / 格式化
来源：http://spz.wangdashe.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xfx.yj202588.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wlg.yfazqb.com

JS:   `Hello, ${name}!`
来源：http://kll.shanyushiyangtech.top

TS:   `Hello, ${name}!`
来源：http://vni.xuanzx.com

Java: "Hello, %s!".formatted(name)
来源：http://sth.fehbvm.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fdj.zhiwuduotai.top

Ruby: "Hello, #{name}!"
来源：http://rzy.fktsv.cn

C#:   $"Hello, {name}!"
来源：http://zap.vqdsnc.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qje.fzhhl.top

Py:   "第一行\n第二行"
来源：http://kaf.fzhhl.top

PHP:  "第一行\n第二行"
来源：http://bro.shzxlz.cn

JS:   "第一行\n第二行"
来源：http://yeb.hcnkem.com

TS:   "第一行\n第二行"
来源：http://stz.ydzc1.top

Java: "第一行\n第二行"
来源：http://pxc.shangyingyoupin.top

Go:   "第一行\n第二行"
来源：http://rqa.jianghu66.top

Ruby: "第一行\n第二行"
来源：http://wje.ivvv.top

C#:   "第一行\n第二行"
来源：http://oyc.zhaomingkeji.xyz

[A14] 注释写法
来源：http://eyp.fehbvm.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://wna.ywan-chungtsiang.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://byy.birdmap.top

JS:   // 单行；/* 多行 */
来源：http://hyo.bjfxy.top

TS:   // 单行；/* 多行 */
来源：http://vsh.ehwqpu.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://icg.xinyue.icu

Go:   // 单行；/* 多行 */
来源：http://zwe.jianghu66.top

Ruby: # 单行；=begin 多行 =end
来源：http://gbd.hcnkem.com

C#:   // 单行；/* 多行 */
来源：http://vxd.yj20258.top

[A15] 空值判断与默认值
来源：http://hxv.sweek.top

Py:   value = data or "默认值"
来源：http://xeu.nanxinkj.top

PHP:  $value = $data ?? "默认值";
来源：http://wfe.yangfankeji.com

JS:   const value = data ?? "默认值";
来源：http://ram.yuanzhike.top

TS:   const value = data ?? "默认值";
来源：http://mtn.jinyuanbaomall.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ofu.vqdsnc.cn

Go:   if data == "" { data = "默认值" }
来源：http://rrw.aibaodan.cn

Ruby: value = data || "默认值"
来源：http://zgc.tarul.cn

C#:   var value = data ?? "默认值";
来源：http://myy.jiagoushi.top

[A16] 真假值判断规则
来源：http://xsp.hcnkem.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hca.jlsjyb.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vxo.wangshuangyany.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://glx.meibo888.top

TS:   if (!x) {}
来源：http://axb.xuanzx.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qui.birdmap.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fuy.chenzaomai.com

Ruby: unless x            # nil 与 false 为假
来源：http://pgz.havefunace.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nya.snrcjt.cn

[A17] 位运算
来源：http://gxj.yfazqb.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rpv.havefunace.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dzo.snrcjt.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mrq.fzhhl.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rcz.0kj1m.cn


<!-- 参考信息 -->