代发 wailian999

[U97] JS：并发请求
来源：http://rew.mhx1999.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vcj.ehwqpu.com

[U98] JS：fetch 带 JSON
来源：http://fdn.jinghuilouyu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hru.vqdsnc.cn

[U99] JS：事件监听
来源：http://aki.vehdjk.com

el.addEventListener("click", e => {})
来源：http://orm.pengpengdd.cyou

[U100] JS：DOM 查询
来源：http://amz.guowangkeji.top

document.querySelector(".item")
来源：http://nig.zdbjq.cn

[U101] JS：classList 操作
来源：http://nli.pycfn.com

el.classList.toggle("active")
来源：http://zqw.fengsongda.top

[U102] JS：本地存储
来源：http://reh.iojbl.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wih.epnwcf.com

[U103] JS：定时器
来源：http://qud.tarul.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ajk.haohaochexian.top

[U104] JS：防抖
来源：http://vij.ehwqpu.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mcf.316326.xyz

[U105] JS：节流
来源：http://czi.nanxuanxn.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qdt.mhx1999.top

[U106] JS：日期格式化
来源：http://sla.jinghuilouyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vng.quarkkingdee.top

[U107] JS：数字千分位
来源：http://ort.xuetiantiany.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qti.cheryme.top

[U108] JS：随机整数
来源：http://lza.yanxiufei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bxh.kuanghao11.cn

[U109] JS：数组分组
来源：http://mhp.hcnkem.com

Object.groupBy(arr, x => x.type)
来源：http://hca.kuanghao11.cn

[U110] JS：数组分块
来源：http://ocz.guannengcc.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dkg.9152youxi.cn

[U111] JS：对象转 Map
来源：http://csc.gogol.net.cn

new Map(Object.entries(obj))
来源：http://odx.jyoumei.cn

[U112] JS：字符串补位
来源：http://wfc.fzhhl.top

"7".padStart(3, "0")
来源：http://vfe.shzxlz.cn

[U113] JS：正则替换全部
来源：http://wjj.fengsongda.top

s.replaceAll("a", "b")
来源：http://jwx.cheryme.top

[U114] JS：JSON 深比较
来源：http://lft.shangyingyoupin.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://awt.fengsongda.top

[U115] JS：生成 UUID
来源：http://ddp.fzhhl.top

crypto.randomUUID()
来源：http://cgf.wangshuangyany.cn

[U116] JS：类型检查（JSDoc）
来源：http://pav.cdnleiting.top

/** @param {string} name */ function f(name) {}
来源：http://pzb.wangshuangyany.cn

[U117] JS：单元测试
来源：http://ier.yuxming.cn

npm i -D vitest;  npx vitest
来源：http://diw.ctjpmb.com

[U118] JS：开发服务器
来源：http://nhe.xuanzx.com

npm i -D vite;  npx vite
来源：http://wdx.shzxlz.cn

[U119] JS：生产构建
来源：http://bdz.kuanghao11.cn

npx vite build
来源：http://ayh.jianghu66.top

[U120] JS：读取环境变量（Vite）
来源：http://otn.cheryme.top

import.meta.env.VITE_API_URL
来源：http://ikt.shzxlz.cn

================================================================================
来源：http://wky.zhengqikj.top

统计汇总
来源：http://dho.iojbl.cn

================================================================================
来源：http://xrd.gotoacloud.top

按语言统计（条）：
来源：http://ioe.jqgfzy.top

Python ......... 252
来源：http://nwu.hywenlv.cn

PHP ............ 252
来源：http://pmm.svipenyu.cn

JavaScript ..... 252
来源：http://thz.tarul.cn

TypeScript ..... 212
来源：http://ivv.yfazqb.com

Java ........... 212
来源：http://olr.pengpengdd.cyou

Go ............. 212
来源：http://dwx.sxryk.cn

Ruby ........... 212
来源：http://zrk.jyoumei.cn

C# ............. 212
来源：http://jmf.shangyingyoupin.top

C .............. 30
来源：http://eee.ydjk.org.cn

C++ ............ 30
来源：http://mel.zhongyouzk.top

SQL ............ 90
来源：http://qeg.epnwcf.com

Bash ........... 80
来源：http://fsf.yanxiufei.cn

Kotlin ......... 15
来源：http://pjf.hnqzz.top

Swift .......... 15
来源：http://vzb.haohaochexian.top

Lua ............ 10
来源：http://ryk.ivvv.top

Perl ........... 10
来源：http://izh.jlsjyb.cn

Scala .......... 10
来源：http://eiy.cdnleiting.top

------------------------------------
来源：http://rhf.fktsv.cn

合计 ........... 2106 条
来源：http://hjt.zhoulong.xyz

按章节统计：
来源：http://swm.haohaochexian.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zem.dashuyun.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kry.jianghu66.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uqy.svipenyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dow.snrcjt.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://izp.hnqzz.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tvn.yuxming.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://umu.gotoacloud.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ioa.0kj1m.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://odg.feifeiyinyue.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wnf.nanxinkj.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sqe.ehwqpu.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qqj.hcnkem.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://psl.redwolf501.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vkc.yj20258888.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hpj.shuidangran.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oqa.yonumen.top

Q SQL 专题                              90
来源：http://koe.tanke756.top

R Bash 专题                             80
来源：http://mfq.hfpthk.cn

S C / C++ 专题                          60
来源：http://dyf.zhiwuduotai.top

T 其他语言补充                          60
来源：http://iej.hesvh.cn

U 高频实用片段                         120
来源：http://gmk.hywenlv.cn

------------------------------------
来源：http://vlf.zhoulong.xyz

合计                                  2106 条
来源：http://jfm.yueranfly.top

--------------------------------------------------------------------------------
来源：http://snp.yuxming.cn

使用提醒
来源：http://sfk.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://fry.aibaodan.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://whh.redwolf501.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jza.yuxming.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vmc.yuxming.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://uka.hywenlv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zwz.wangdashe.top

—— 文件结束 ——
来源：http://hqk.ppjwa.cn

================================================================================
来源：http://uel.feifeiyinyue.top

程序语言常见例子速查手册（2024 版）
来源：http://paa.zhongyouzk.top

Common Programming Examples Cheat Book
来源：http://yth.mhx1999.top

================================================================================
来源：http://fsx.yueranfly.top

【收录内容】
来源：http://kpf.0kj1m.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://lmu.chenjidiqi.icu

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hhs.guannengcc.top

SQL · Bash · C · C++
来源：http://ucj.fzhhl.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tfx.zdbjq.cn

【使用说明】
来源：http://mrk.jinqigfzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ndd.zhijiandao.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wlz.hnqzz.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rzb.zhijiandao.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vvs.snrcjt.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sso.zycfv.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rde.dashuyun.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gnb.jyoumei.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://txh.yongpay.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kid.sjlbkw.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dsu.cdnleiting.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mhg.ivvv.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kyp.uphjek.com

【文件统计】
来源：http://otj.tian-w.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mnn.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://wxr.xinyue.icu

目  录
来源：http://eeh.andypj.xyz

--------------------------------------------------------------------------------
来源：http://fgv.feifeiyinyue.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://igo.cqqwz.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cax.jianghu66.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zzh.gzhubu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kqx.zdqjudy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://szq.xuetiantiany.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zve.xingfuxueyuan.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://elc.hammf.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yey.shanyushiyangtech.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://eff.jinyuanbaomall.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ubo.0kj1m.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lem.hongshengwenyu.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xng.nwbrower.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ryu.dashuyun.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nvn.zhiwuduotai.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ape.fktsv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bgg.mhx1999.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fqq.sysykeji.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ezj.guannengcc.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ert.chenzaomai.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://grz.zhaomingkeji.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pkw.shanyushiyangtech.top

================================================================================
来源：http://lmu.aibaodan.cn

A. 基础语法与类型
来源：http://kmo.wangshuangyany.cn

================================================================================
来源：http://ism.cdnleiting.top

[A01] Hello World
来源：http://ssl.xylfe.cn

Py:   print("Hello, World!")
来源：http://vlw.zhixingplan.top

PHP:  echo "Hello, World!";
来源：http://oro.hesvh.cn

JS:   console.log("Hello, World!");
来源：http://mdq.dashuyun.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://del.sxryk.cn

Java: System.out.println("Hello, World!");
来源：http://tqf.zdbjq.cn

Go:   fmt.Println("Hello, World!")
来源：http://alf.ivvv.top

Ruby: puts "Hello, World!"
来源：http://pjp.wangdashe.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ftf.hcnkem.com

[A02] 变量声明与赋值
来源：http://elu.ywan-chungtsiang.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xyl.yuanzhike.top

PHP:  $name = "Alex"; $age = 20;
来源：http://tds.jinyuanbaomall.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yog.xuetiantiany.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lvp.xuetiantiany.cn

Java: String name = "Alex"; int age = 20;
来源：http://pfb.hfpthk.cn

Go:   name := "Alex"; age := 20
来源：http://pdw.birdmap.top

Ruby: name = "Alex"; age = 20
来源：http://cgl.jqgufenzy.top

C#:   string name = "Alex"; int age = 20;
来源：http://hmv.52xcode.cn

[A03] 常量定义
来源：http://uch.zycfv.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mei.jinqigufen.top

PHP:  const PI = 3.14159;
来源：http://rch.zhijiandao.cn

JS:   const PI = 3.14159;
来源：http://njn.fehbvm.com

TS:   const PI: number = 3.14159;
来源：http://eaf.wangshuangyany.cn

Java: static final double PI = 3.14159;
来源：http://lex.jlsjyb.cn

Go:   const PI = 3.14159
来源：http://prb.0kj1m.cn

Ruby: PI = 3.14159
来源：http://ear.chenjidiqi.icu

C#:   const double PI = 3.14159;
来源：http://ddb.kuanghao11.cn

[A04] 判断变量类型
来源：http://xaa.cheryme.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://wyv.cucudq.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yja.fehbvm.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://far.chenzaomai.com

TS:   typeof x; x instanceof Date
来源：http://hsi.kuanghao11.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gyz.fanxiaobao.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://hto.cqqwz.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ijs.pycfn.com

C#:   x.GetType().Name; x is int
来源：http://rfb.feifeiyinyue.top

[A05] 整数除法与取模
来源：http://ero.yj20258888.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vdx.bbcook.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hrg.jlsjyb.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gka.zhengqikj.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ntf.xylfe.cn

Java: 7 / 2; 7 % 2
来源：http://vgf.birdmap.top

Go:   7 / 2; 7 % 2
来源：http://qhd.yuanzhike.top

Ruby: 7 / 2; 7 % 2
来源：http://xut.jinqigufen.top

C#:   7 / 2; 7 % 2
来源：http://okw.tian-w.cn

[A06] 字符串转数字
来源：http://bua.haohaochexian.top

Py:   int("42"); float("3.14")
来源：http://dzn.gzhubu.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wcr.nanxinkj.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://acm.sysykeji.top

TS:   parseInt("42", 10); Number("42")
来源：http://pdq.yuanzhike.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wtb.aizwys.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mzv.jianghu66.top

Ruby: "42".to_i; "3.14".to_f
来源：http://rbt.jinqigufen.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cip.hcnkem.com

[A07] 数字转字符串
来源：http://sol.shanyushiyangkeji.top

Py:   str(42)
来源：http://riy.gzhubu.top

PHP:  (string) 42; strval(42)
来源：http://end.gotoacloud.top

JS:   String(42); (42).toString()
来源：http://isx.andypj.xyz

TS:   String(42)
来源：http://pnz.sufxvd.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://jfx.gaohongyu789.top

Go:   strconv.Itoa(42)
来源：http://vok.yanxiufei.cn

Ruby: 42.to_s
来源：http://qie.smart0.xyz

C#:   42.ToString()
来源：http://pph.redwolf501.top

[A08] 取整与四舍五入
来源：http://cjg.bbcook.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ent.chenlongwang.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://okm.jinghuilouyu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sst.jinqigfzy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dps.nanxinkj.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hpf.guannengcc.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tfm.jqgufenzy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://alw.jqgufenzy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://syz.sysykeji.top

[A09] 绝对值与最大最小值
来源：http://mss.zhongyouzk.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qwn.zhongyouzk.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://emy.yj202588.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://emp.vqdsnc.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jqf.xinyue.icu

Java: Math.abs(-5); Math.max(1, 2)
来源：http://akm.hcnkem.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ujz.haohaochexian.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uyi.gogol.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yez.birdmap.top

[A10] 生成随机数
来源：http://ccm.sxryk.cn

Py:   import random; random.randint(1, 100)
来源：http://arc.bjfxy.top

PHP:  random_int(1, 100);
来源：http://fop.52xcode.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hcw.jyoumei.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bts.jinghuilouyu.cn

Java: new Random().nextInt(100) + 1
来源：http://xql.xylfe.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cfb.sjlbkw.cn

Ruby: rand(1..100)
来源：http://goq.cucudq.cn

C#:   new Random().Next(1, 101)
来源：http://swj.ydjk.org.cn

[A11] 条件表达式（三元）
来源：http://jui.jinqigfzy.top

Py:   "yes" if x > 0 else "no"
来源：http://xpf.yuxming.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rql.jinyuanbaomall.cn

JS:   x > 0 ? "yes" : "no"
来源：http://awv.shuidangran.top

TS:   x > 0 ? "yes" : "no"
来源：http://nuw.quarkkingdee.top

Java: x > 0 ? "yes" : "no"
来源：http://ezl.tanke756.top

Go:   // 无三元运算符，需用 if 语句
来源：http://twh.ydjk.org.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jpp.zhaomingkeji.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://ktp.yfazqb.com

[A12] 字符串插值 / 格式化
来源：http://kor.vqdsnc.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cil.fehbvm.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ujl.yj20258.top

JS:   `Hello, ${name}!`
来源：http://iuj.aibaodan.cn

TS:   `Hello, ${name}!`
来源：http://cfc.hysaishi.cn

Java: "Hello, %s!".formatted(name)
来源：http://gno.gaohongyu789.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://evr.shzxlz.cn

Ruby: "Hello, #{name}!"
来源：http://glb.hysaishi.cn

C#:   $"Hello, {name}!"
来源：http://edu.zdbjq.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vjv.birdmap.top

Py:   "第一行\n第二行"
来源：http://umt.ydzc1.top

PHP:  "第一行\n第二行"
来源：http://lmr.zhaomingkeji.xyz

JS:   "第一行\n第二行"
来源：http://igf.sysykeji.top

TS:   "第一行\n第二行"
来源：http://iwl.ydzc1.top

Java: "第一行\n第二行"
来源：http://gcx.havefunace.top

Go:   "第一行\n第二行"
来源：http://gwb.cucudq.cn

Ruby: "第一行\n第二行"
来源：http://ilz.smart0.xyz

C#:   "第一行\n第二行"
来源：http://doe.fehbvm.com

[A14] 注释写法
来源：http://rzo.cashguo.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://rst.quarkkingdee.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ehf.uphjek.com

JS:   // 单行；/* 多行 */
来源：http://dbi.jinqigufen.top

TS:   // 单行；/* 多行 */
来源：http://fyr.yj20258.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tqj.hongshengwenyu.top

Go:   // 单行；/* 多行 */
来源：http://aml.jinqigfzy.top

Ruby: # 单行；=begin 多行 =end
来源：http://sum.tanke756.top

C#:   // 单行；/* 多行 */
来源：http://dmo.fktsv.cn

[A15] 空值判断与默认值
来源：http://qyz.zhaomingkeji.xyz

Py:   value = data or "默认值"
来源：http://vcx.iojbl.cn

PHP:  $value = $data ?? "默认值";
来源：http://iwm.yongpay.top

JS:   const value = data ?? "默认值";
来源：http://wgd.yvedp.cn

TS:   const value = data ?? "默认值";
来源：http://jlr.yonumen.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://orb.gaohongyu789.top

Go:   if data == "" { data = "默认值" }
来源：http://gkt.yanxiufei.cn

Ruby: value = data || "默认值"
来源：http://ymq.ywan-chungtsiang.top

C#:   var value = data ?? "默认值";
来源：http://lci.dianchejie.cn

[A16] 真假值判断规则
来源：http://hic.pengpengdd.cyou

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tfr.cqqwz.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gxl.yfazqb.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://den.xylfe.cn

TS:   if (!x) {}
来源：http://fot.dianchejie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://npq.0kj1m.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://frd.guannengcc.top

Ruby: unless x            # nil 与 false 为假
来源：http://pdt.jinqigfzy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dgz.hnxiangtu.top

[A17] 位运算
来源：http://ecn.nanxuanxn.top


<!-- 参考信息 -->