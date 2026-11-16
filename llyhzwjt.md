代发 wailian999

[U95] JS：Promise 包装
来源：http://vob.pycfn.com

new Promise((resolve, reject) => {})
来源：http://cfw.jyoumei.cn

[U96] JS：async/await 与异常
来源：http://foe.chenlongwang.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qfc.xingfuxueyuan.xyz

[U97] JS：并发请求
来源：http://tsf.gzhubu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://sgh.hnxiangtu.top

[U98] JS：fetch 带 JSON
来源：http://ufg.nanxinkj.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://slf.pengpengdd.cyou

[U99] JS：事件监听
来源：http://use.nanxuanxn.top

el.addEventListener("click", e => {})
来源：http://pkn.jianghu66.top

[U100] JS：DOM 查询
来源：http://ahv.redwolf501.top

document.querySelector(".item")
来源：http://vst.fktsv.cn

[U101] JS：classList 操作
来源：http://hvy.redwolf501.top

el.classList.toggle("active")
来源：http://inp.fengsongda.top

[U102] JS：本地存储
来源：http://zdo.hywenlv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pfg.yanxiufei.cn

[U103] JS：定时器
来源：http://nkj.nanxuanxn.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ucp.zhixingplan.top

[U104] JS：防抖
来源：http://pwv.daria6918.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://srf.fanxiaobao.xyz

[U105] JS：节流
来源：http://fhp.xingfuxueyuan.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xab.xylfe.cn

[U106] JS：日期格式化
来源：http://tan.52xcode.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://szj.tarul.cn

[U107] JS：数字千分位
来源：http://lmb.xinyue.icu

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wvs.zhiwuduotai.top

[U108] JS：随机整数
来源：http://atk.svipenyu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bzs.hywenlv.cn

[U109] JS：数组分组
来源：http://scq.chenlongwang.top

Object.groupBy(arr, x => x.type)
来源：http://msc.ydzc1.top

[U110] JS：数组分块
来源：http://kjd.gzhubu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wro.xuanzx.com

[U111] JS：对象转 Map
来源：http://omq.fanxiaobao.xyz

new Map(Object.entries(obj))
来源：http://ndj.sufxvd.cn

[U112] JS：字符串补位
来源：http://gfd.yanxiufei.cn

"7".padStart(3, "0")
来源：http://tpw.gzhubu.top

[U113] JS：正则替换全部
来源：http://ydx.snrcjt.cn

s.replaceAll("a", "b")
来源：http://trv.aibaodan.cn

[U114] JS：JSON 深比较
来源：http://kon.vehdjk.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://vhs.hesvh.cn

[U115] JS：生成 UUID
来源：http://eiv.guannengcc.top

crypto.randomUUID()
来源：http://vqb.ywan-chungtsiang.top

[U116] JS：类型检查（JSDoc）
来源：http://crs.guowangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://eji.meibo888.top

[U117] JS：单元测试
来源：http://olp.hongshengwenyu.top

npm i -D vitest;  npx vitest
来源：http://uwl.epnwcf.com

[U118] JS：开发服务器
来源：http://lml.haohaochexian.top

npm i -D vite;  npx vite
来源：http://zca.c1oappe.top

[U119] JS：生产构建
来源：http://zby.yanxiufei.cn

npx vite build
来源：http://jxz.cdnleiting.top

[U120] JS：读取环境变量（Vite）
来源：http://knh.zhixingplan.top

import.meta.env.VITE_API_URL
来源：http://hox.ydzc1.top

================================================================================
来源：http://ixu.gzhubu.top

统计汇总
来源：http://fjy.hcnkem.com

================================================================================
来源：http://zcx.hnxiangtu.top

按语言统计（条）：
来源：http://mfs.tian-w.cn

Python ......... 252
来源：http://ana.dashuyun.cn

PHP ............ 252
来源：http://fxx.xingfuxueyuan.xyz

JavaScript ..... 252
来源：http://rfo.vehdjk.com

TypeScript ..... 212
来源：http://ccw.0kj1m.cn

Java ........... 212
来源：http://uck.zhixingplan.top

Go ............. 212
来源：http://guu.xingfuxueyuan.xyz

Ruby ........... 212
来源：http://dre.zhongyouzk.top

C# ............. 212
来源：http://glb.zhixingplan.top

C .............. 30
来源：http://mzc.xuanzx.com

C++ ............ 30
来源：http://ltk.andypj.xyz

SQL ............ 90
来源：http://swj.hysaishi.cn

Bash ........... 80
来源：http://juv.jqgfzy.top

Kotlin ......... 15
来源：http://mee.cashguo.top

Swift .......... 15
来源：http://chc.zhengqikj.top

Lua ............ 10
来源：http://cki.gaohongyu789.top

Perl ........... 10
来源：http://clp.jiagoushi.top

Scala .......... 10
来源：http://nfn.ehwqpu.com

------------------------------------
来源：http://rmc.daria6918.cn

合计 ........... 2106 条
来源：http://oeo.hesvh.cn

按章节统计：
来源：http://axg.aizwys.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zzi.zhongyouzk.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jop.zhaomingkeji.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vwq.c1oappe.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pgu.meibo888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qwu.ppjwa.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dbm.gogol.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rvv.yuanzhike.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pfj.xziqi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lmc.birdmap.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ker.shzxlz.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mip.yfazqb.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cgj.wangshuangyany.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vfp.yj202588.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qpl.epnwcf.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mgh.xingfuxueyuan.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eiv.yj20258.top

Q SQL 专题                              90
来源：http://gue.yvedp.cn

R Bash 专题                             80
来源：http://ikl.c1oappe.top

S C / C++ 专题                          60
来源：http://rdb.vqdsnc.cn

T 其他语言补充                          60
来源：http://kcr.jiagoushi.top

U 高频实用片段                         120
来源：http://aih.dianchejie.cn

------------------------------------
来源：http://zlt.jinyuanbaomall.cn

合计                                  2106 条
来源：http://ndk.epnwcf.com

--------------------------------------------------------------------------------
来源：http://nph.cdnleiting.top

使用提醒
来源：http://dxz.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://kcw.gogol.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ouv.nanxinkj.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fhb.xuetiantiany.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://abg.zhongyouzk.top

在旧版本上使用前请先确认语法支持情况。
来源：http://lgc.hcnkem.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rms.jinghuilouyu.cn

—— 文件结束 ——
来源：http://rxu.tanke756.top

================================================================================
来源：http://ggz.andypj.xyz

程序语言常见例子速查手册（2024 版）
来源：http://wqy.cheryme.top

Common Programming Examples Cheat Book
来源：http://gqa.jiagoushi.top

================================================================================
来源：http://tug.daxiang520.top

【收录内容】
来源：http://trq.bbcook.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://iwy.guowangkeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jvr.jianghu66.top

SQL · Bash · C · C++
来源：http://sdd.bbcook.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ubs.yongpay.top

【使用说明】
来源：http://yqy.shuidangran.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ssq.fehbvm.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jfe.yuanzhike.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://toy.fanxiaobao.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://frv.smart0.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://vmx.cqqwz.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://drb.smart0.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://oxm.ydzc1.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vpo.nanxuanxn.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ejb.0kj1m.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dwr.wangshuangyany.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hgy.epnwcf.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sbk.vqdsnc.cn

【文件统计】
来源：http://etr.nanxuanxn.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jnk.yj20258888.top

--------------------------------------------------------------------------------
来源：http://ydz.bjfxy.top

目  录
来源：http://kec.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://rzb.jiagoushi.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xuv.yueranfly.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://iqz.fzhhl.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tbn.ctjpmb.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://caj.ybcxt.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hnn.vehdjk.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://edv.yuanzhike.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ssm.havefunace.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zaj.sxryk.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hto.gzhubu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fqd.hammf.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://van.quarkkingdee.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://krz.shangyingyoupin.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xku.feifeiyinyue.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://uli.chenlongwang.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qnz.birdmap.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://oxy.wangdashe.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tjf.xylfe.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://qik.jinqigfzy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gdy.jinqigufen.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bcd.vehdjk.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xwr.tian-w.cn

================================================================================
来源：http://amd.tian-w.cn

A. 基础语法与类型
来源：http://cij.yfazqb.com

================================================================================
来源：http://pit.zhongyouzk.top

[A01] Hello World
来源：http://vdw.hcnkem.com

Py:   print("Hello, World!")
来源：http://jox.jiagoushi.top

PHP:  echo "Hello, World!";
来源：http://cbb.sysykeji.top

JS:   console.log("Hello, World!");
来源：http://ggf.yongpay.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ufw.sweek.top

Java: System.out.println("Hello, World!");
来源：http://jej.xylfe.cn

Go:   fmt.Println("Hello, World!")
来源：http://raw.bjfxy.top

Ruby: puts "Hello, World!"
来源：http://osy.316326.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://hut.zhixingplan.top

[A02] 变量声明与赋值
来源：http://uox.cdnleiting.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bpv.yueranfly.top

PHP:  $name = "Alex"; $age = 20;
来源：http://uwx.kuanghao11.cn

JS:   let name = "Alex"; const age = 20;
来源：http://eqp.redwolf501.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ayd.haohaochexian.top

Java: String name = "Alex"; int age = 20;
来源：http://dpm.yj20258888.top

Go:   name := "Alex"; age := 20
来源：http://mvk.zhengqikj.top

Ruby: name = "Alex"; age = 20
来源：http://pgf.nwbrower.top

C#:   string name = "Alex"; int age = 20;
来源：http://dqf.pengpengdd.cyou

[A03] 常量定义
来源：http://nov.xuetiantiany.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jwu.zhaomingkeji.xyz

PHP:  const PI = 3.14159;
来源：http://nqx.jqgufenzy.top

JS:   const PI = 3.14159;
来源：http://age.cdnleiting.top

TS:   const PI: number = 3.14159;
来源：http://fam.sxryk.cn

Java: static final double PI = 3.14159;
来源：http://hrh.zdbjq.cn

Go:   const PI = 3.14159
来源：http://tuc.hongshengwenyu.top

Ruby: PI = 3.14159
来源：http://gpu.hnqzz.top

C#:   const double PI = 3.14159;
来源：http://vkg.yvedp.cn

[A04] 判断变量类型
来源：http://nnx.yanxiufei.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://sno.aibaodan.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jze.daria6918.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fym.cheryme.top

TS:   typeof x; x instanceof Date
来源：http://toa.kuanghao11.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kax.xinyue.icu

Go:   reflect.TypeOf(x).Name()
来源：http://asd.hcnkem.com

Ruby: x.class; x.is_a?(Integer)
来源：http://kgm.vehdjk.com

C#:   x.GetType().Name; x is int
来源：http://ind.fehbvm.com

[A05] 整数除法与取模
来源：http://lrg.haohaochexian.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qsy.birdmap.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://oad.jlsjyb.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wca.ybcxt.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lpl.ybcxt.top

Java: 7 / 2; 7 % 2
来源：http://enl.yj202588.top

Go:   7 / 2; 7 % 2
来源：http://wmt.iojbl.cn

Ruby: 7 / 2; 7 % 2
来源：http://xst.chenjidiqi.icu

C#:   7 / 2; 7 % 2
来源：http://usg.fktsv.cn

[A06] 字符串转数字
来源：http://ixs.cucudq.cn

Py:   int("42"); float("3.14")
来源：http://iso.nwbrower.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jmx.pycfn.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lbj.bjfxy.top

TS:   parseInt("42", 10); Number("42")
来源：http://cid.xziqi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ils.yj202588.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://iun.gogol.net.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://evq.kuanghao11.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nki.ctjpmb.com

[A07] 数字转字符串
来源：http://nkm.shzxlz.cn

Py:   str(42)
来源：http://ztr.hnxiangtu.top

PHP:  (string) 42; strval(42)
来源：http://uaj.yvedp.cn

JS:   String(42); (42).toString()
来源：http://wag.zdqjudy.top

TS:   String(42)
来源：http://mkb.xingfuxueyuan.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://fxp.cucudq.cn

Go:   strconv.Itoa(42)
来源：http://aqt.uphjek.com

Ruby: 42.to_s
来源：http://fhw.ivvv.top

C#:   42.ToString()
来源：http://rvi.xingfuxueyuan.xyz

[A08] 取整与四舍五入
来源：http://jcg.zhoulong.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://skm.zycfv.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://and.jinqigfzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blu.jlsjyb.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wqz.dashuyun.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jtq.zhaomingkeji.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nhf.jinqigfzy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://pvc.sxryk.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gvu.shangyingyoupin.top

[A09] 绝对值与最大最小值
来源：http://ppx.c1oappe.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hvy.zhixingplan.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xwp.yuxming.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ihk.haohaochexian.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pee.wangshuangyany.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://eoo.gogol.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://noi.vehdjk.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://apd.shuidangran.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hvn.dianchejie.cn

[A10] 生成随机数
来源：http://rjs.jlsjyb.cn

Py:   import random; random.randint(1, 100)
来源：http://izl.hywenlv.cn

PHP:  random_int(1, 100);
来源：http://smm.aizwys.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dco.yangfankeji.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dcy.zhijiandao.cn

Java: new Random().nextInt(100) + 1
来源：http://gec.wangdashe.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kqo.cucudq.cn

Ruby: rand(1..100)
来源：http://fcm.tanke756.top

C#:   new Random().Next(1, 101)
来源：http://xey.yvedp.cn

[A11] 条件表达式（三元）
来源：http://kxg.zycfv.cn

Py:   "yes" if x > 0 else "no"
来源：http://akq.cdnleiting.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://hsv.chenlongwang.top

JS:   x > 0 ? "yes" : "no"
来源：http://sol.shzxlz.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ngm.shangyingyoupin.top

Java: x > 0 ? "yes" : "no"
来源：http://sgx.c1oappe.top

Go:   // 无三元运算符，需用 if 语句
来源：http://zlh.quarkkingdee.top

Ruby: x > 0 ? "yes" : "no"
来源：http://axx.cashguo.top

C#:   x > 0 ? "yes" : "no"
来源：http://jyz.dashuyun.cn

[A12] 字符串插值 / 格式化
来源：http://cvl.shanyushiyangtech.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bgl.meibo888.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uha.jyoumei.cn

JS:   `Hello, ${name}!`
来源：http://pho.zdbjq.cn

TS:   `Hello, ${name}!`
来源：http://gli.zdqjudy.top

Java: "Hello, %s!".formatted(name)
来源：http://uts.epnwcf.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nqi.shzxlz.cn

Ruby: "Hello, #{name}!"
来源：http://csg.zhijiandao.cn

C#:   $"Hello, {name}!"
来源：http://yse.shzxlz.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pwg.xziqi.cn

Py:   "第一行\n第二行"
来源：http://lwk.daxiang520.top

PHP:  "第一行\n第二行"
来源：http://rzh.zhiwuduotai.top

JS:   "第一行\n第二行"
来源：http://yzk.redwolf501.top

TS:   "第一行\n第二行"
来源：http://ecn.jiagoushi.top

Java: "第一行\n第二行"
来源：http://cau.zhixingplan.top

Go:   "第一行\n第二行"
来源：http://wrm.yangfankeji.com

Ruby: "第一行\n第二行"
来源：http://ctl.redwolf501.top

C#:   "第一行\n第二行"
来源：http://jeu.c1oappe.top

[A14] 注释写法
来源：http://wqc.fktsv.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xjw.iojbl.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mmz.vehdjk.com

JS:   // 单行；/* 多行 */
来源：http://yxp.jlsjyb.cn

TS:   // 单行；/* 多行 */
来源：http://svj.hysaishi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://aoo.cdnleiting.top

Go:   // 单行；/* 多行 */
来源：http://uyv.kuanghao11.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rom.yanxiufei.cn

C#:   // 单行；/* 多行 */
来源：http://lxc.tian-w.cn

[A15] 空值判断与默认值
来源：http://bpy.kuanghao11.cn

Py:   value = data or "默认值"
来源：http://cyl.shangyingyoupin.top

PHP:  $value = $data ?? "默认值";
来源：http://zwv.jinyuanbaomall.cn

JS:   const value = data ?? "默认值";
来源：http://pyq.gotoacloud.top

TS:   const value = data ?? "默认值";
来源：http://bfh.9152youxi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://auo.andypj.xyz

Go:   if data == "" { data = "默认值" }
来源：http://nus.aibaodan.cn

Ruby: value = data || "默认值"
来源：http://ypo.hysaishi.cn

C#:   var value = data ?? "默认值";
来源：http://knr.jyoumei.cn

[A16] 真假值判断规则
来源：http://apz.yj20258888.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wca.nwbrower.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sqx.gotoacloud.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://eda.yj20258888.top

TS:   if (!x) {}
来源：http://ufo.aizwys.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jsg.xinyue.icu


<!-- 参考信息 -->