代发 wailian999

[U95] JS：Promise 包装
来源：http://toq.yj20258.top

new Promise((resolve, reject) => {})
来源：http://rge.wangdashe.top

[U96] JS：async/await 与异常
来源：http://agu.sufxvd.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mdp.iojbl.cn

[U97] JS：并发请求
来源：http://oma.meibo888.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ekq.aibaodan.cn

[U98] JS：fetch 带 JSON
来源：http://tcn.hfpthk.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hpn.redwolf501.top

[U99] JS：事件监听
来源：http://stm.c1oappe.top

el.addEventListener("click", e => {})
来源：http://vhd.cqqwz.cn

[U100] JS：DOM 查询
来源：http://gfg.cucudq.cn

document.querySelector(".item")
来源：http://sts.epnwcf.com

[U101] JS：classList 操作
来源：http://apw.jqgfzy.top

el.classList.toggle("active")
来源：http://hbb.fehbvm.com

[U102] JS：本地存储
来源：http://wri.guannengcc.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://tsu.zhoulong.xyz

[U103] JS：定时器
来源：http://hzt.kuanghao11.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zbz.hcnkem.com

[U104] JS：防抖
来源：http://fgm.hysaishi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dpg.ppjwa.cn

[U105] JS：节流
来源：http://kir.yongpay.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ein.shzxlz.cn

[U106] JS：日期格式化
来源：http://lbc.wangdashe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xvh.yongpay.top

[U107] JS：数字千分位
来源：http://aag.ybcxt.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jfl.ydzc1.top

[U108] JS：随机整数
来源：http://nbt.gotoacloud.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kxo.xziqi.cn

[U109] JS：数组分组
来源：http://ofw.fktsv.cn

Object.groupBy(arr, x => x.type)
来源：http://jgg.fengsongda.top

[U110] JS：数组分块
来源：http://apf.c1oappe.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://koc.sjlbkw.cn

[U111] JS：对象转 Map
来源：http://rfm.daxiang520.top

new Map(Object.entries(obj))
来源：http://jrk.xuanzx.com

[U112] JS：字符串补位
来源：http://mpy.52xcode.cn

"7".padStart(3, "0")
来源：http://xgx.zhixingplan.top

[U113] JS：正则替换全部
来源：http://gsv.epnwcf.com

s.replaceAll("a", "b")
来源：http://pdu.fanxiaobao.xyz

[U114] JS：JSON 深比较
来源：http://yfa.bjfxy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rro.iojbl.cn

[U115] JS：生成 UUID
来源：http://rql.yvedp.cn

crypto.randomUUID()
来源：http://ufd.xingfuxueyuan.xyz

[U116] JS：类型检查（JSDoc）
来源：http://ovd.ivvv.top

/** @param {string} name */ function f(name) {}
来源：http://ygr.nanxuanxn.top

[U117] JS：单元测试
来源：http://pry.andypj.xyz

npm i -D vitest;  npx vitest
来源：http://dpc.fktsv.cn

[U118] JS：开发服务器
来源：http://zhp.fktsv.cn

npm i -D vite;  npx vite
来源：http://afo.52xcode.cn

[U119] JS：生产构建
来源：http://rkh.cdnleiting.top

npx vite build
来源：http://pqu.hfpthk.cn

[U120] JS：读取环境变量（Vite）
来源：http://hvo.vehdjk.com

import.meta.env.VITE_API_URL
来源：http://tjd.xingfuxueyuan.xyz

================================================================================
来源：http://ppw.xuetiantiany.cn

统计汇总
来源：http://inn.yonumen.top

================================================================================
来源：http://rst.fktsv.cn

按语言统计（条）：
来源：http://jiy.chenzaomai.com

Python ......... 252
来源：http://skb.gogol.net.cn

PHP ............ 252
来源：http://cgs.vqdsnc.cn

JavaScript ..... 252
来源：http://yyt.quarkkingdee.top

TypeScript ..... 212
来源：http://ydx.jlsjyb.cn

Java ........... 212
来源：http://dwl.jinyuanbaomall.cn

Go ............. 212
来源：http://rwv.tanke756.top

Ruby ........... 212
来源：http://zeo.haohaochexian.top

C# ............. 212
来源：http://rwh.9152youxi.cn

C .............. 30
来源：http://jwy.wangshuangyany.cn

C++ ............ 30
来源：http://fpw.xylfe.cn

SQL ............ 90
来源：http://gtt.yuxming.cn

Bash ........... 80
来源：http://ent.ivvv.top

Kotlin ......... 15
来源：http://npy.xylfe.cn

Swift .......... 15
来源：http://qvk.cdnleiting.top

Lua ............ 10
来源：http://iky.9152youxi.cn

Perl ........... 10
来源：http://xkt.zhixingplan.top

Scala .......... 10
来源：http://vby.9152youxi.cn

------------------------------------
来源：http://axx.hysaishi.cn

合计 ........... 2106 条
来源：http://aqu.gogol.net.cn

按章节统计：
来源：http://kax.cucudq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zud.nanxinkj.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bbu.shzxlz.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qka.aizwys.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gee.zycfv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ovx.gzhubu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ypg.wangshuangyany.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tnc.ydjk.org.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ydi.vehdjk.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dmm.hnqzz.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://alb.yonumen.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kzf.tian-w.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bhx.cucudq.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mtz.xuanzx.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jqf.tanke756.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mql.sxryk.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zwe.daria6918.cn

Q SQL 专题                              90
来源：http://qkf.yonumen.top

R Bash 专题                             80
来源：http://glw.sufxvd.cn

S C / C++ 专题                          60
来源：http://zsd.zdbjq.cn

T 其他语言补充                          60
来源：http://zrm.gotoacloud.top

U 高频实用片段                         120
来源：http://egs.hammf.cn

------------------------------------
来源：http://skr.yj20258888.top

合计                                  2106 条
来源：http://ntd.hammf.cn

--------------------------------------------------------------------------------
来源：http://evq.fzhhl.top

使用提醒
来源：http://wey.bbcook.cn

--------------------------------------------------------------------------------
来源：http://gie.guannengcc.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gqg.sysykeji.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wqy.cucudq.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qjg.yonumen.top

在旧版本上使用前请先确认语法支持情况。
来源：http://yvi.chenjidiqi.icu

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vub.cashguo.top

—— 文件结束 ——
来源：http://kfm.yj20258.top

================================================================================
来源：http://njg.sweek.top

程序语言常见例子速查手册（2024 版）
来源：http://ogv.guannengcc.top

Common Programming Examples Cheat Book
来源：http://etj.haohaochexian.top

================================================================================
来源：http://bha.chenjidiqi.icu

【收录内容】
来源：http://moq.pycfn.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://uax.hcnkem.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xcm.ybcxt.top

SQL · Bash · C · C++
来源：http://mhg.gzhubu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kjp.yfazqb.com

【使用说明】
来源：http://xyf.ivvv.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fkc.ydzc1.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uwz.xylfe.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hon.jianghu66.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vut.redwolf501.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ipm.hcnkem.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cng.jianghu66.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xso.tian-w.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fwm.pycfn.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://smp.c1oappe.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cwe.birdmap.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nyh.ydjk.org.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tep.gogol.net.cn

【文件统计】
来源：http://nrh.cqqwz.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zqo.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://mlb.vehdjk.com

目  录
来源：http://pzt.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://zag.fehbvm.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ngx.jianghu66.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://inw.fanxiaobao.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nia.bbcook.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zfx.vehdjk.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gvn.c1oappe.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nkj.tianlin.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://php.yuxming.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ece.gotoacloud.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vdz.hesvh.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ktw.nanxinkj.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://koy.feifeiyinyue.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fdf.dashuyun.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://csx.nanxuanxn.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kpt.jianghu66.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://otd.hesvh.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://anu.vqdsnc.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://khe.haohaochexian.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://yah.quarkkingdee.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rhu.jqgufenzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ohe.0kj1m.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zsq.uphjek.com

================================================================================
来源：http://qck.redwolf501.top

A. 基础语法与类型
来源：http://btz.ppjwa.cn

================================================================================
来源：http://tot.smart0.xyz

[A01] Hello World
来源：http://tei.hesvh.cn

Py:   print("Hello, World!")
来源：http://hix.zdbjq.cn

PHP:  echo "Hello, World!";
来源：http://sjc.fengsongda.top

JS:   console.log("Hello, World!");
来源：http://qxm.tianlin.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ail.yonumen.top

Java: System.out.println("Hello, World!");
来源：http://ozc.sjlbkw.cn

Go:   fmt.Println("Hello, World!")
来源：http://ymo.snrcjt.cn

Ruby: puts "Hello, World!"
来源：http://cxk.epnwcf.com

C#:   Console.WriteLine("Hello, World!");
来源：http://esc.zhiwuduotai.top

[A02] 变量声明与赋值
来源：http://exd.sufxvd.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zzg.fengsongda.top

PHP:  $name = "Alex"; $age = 20;
来源：http://jua.sweek.top

JS:   let name = "Alex"; const age = 20;
来源：http://jww.sufxvd.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yfi.zdbjq.cn

Java: String name = "Alex"; int age = 20;
来源：http://nhq.iojbl.cn

Go:   name := "Alex"; age := 20
来源：http://fzs.gogol.net.cn

Ruby: name = "Alex"; age = 20
来源：http://zfl.ydzc1.top

C#:   string name = "Alex"; int age = 20;
来源：http://dlz.smart0.xyz

[A03] 常量定义
来源：http://imw.yongpay.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mpn.zycfv.cn

PHP:  const PI = 3.14159;
来源：http://xwx.tian-w.cn

JS:   const PI = 3.14159;
来源：http://zjk.yuxming.cn

TS:   const PI: number = 3.14159;
来源：http://inf.yuanzhike.top

Java: static final double PI = 3.14159;
来源：http://ilp.zhengqikj.top

Go:   const PI = 3.14159
来源：http://zef.ehwqpu.com

Ruby: PI = 3.14159
来源：http://hua.dashuyun.cn

C#:   const double PI = 3.14159;
来源：http://rzz.gotoacloud.top

[A04] 判断变量类型
来源：http://xtp.fktsv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jtx.gotoacloud.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://aek.ppjwa.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lke.ydzc1.top

TS:   typeof x; x instanceof Date
来源：http://nyy.xziqi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://frk.yuanzhike.top

Go:   reflect.TypeOf(x).Name()
来源：http://urd.jyoumei.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://cdp.zhixingplan.top

C#:   x.GetType().Name; x is int
来源：http://fac.svipenyu.cn

[A05] 整数除法与取模
来源：http://fut.vqdsnc.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wgq.cdnleiting.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://dog.pycfn.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hjx.gaohongyu789.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ams.chenlongwang.top

Java: 7 / 2; 7 % 2
来源：http://ycz.0kj1m.cn

Go:   7 / 2; 7 % 2
来源：http://fyv.fanxiaobao.xyz

Ruby: 7 / 2; 7 % 2
来源：http://xtb.yanxiufei.cn

C#:   7 / 2; 7 % 2
来源：http://fow.jiagoushi.top

[A06] 字符串转数字
来源：http://xzb.nwbrower.top

Py:   int("42"); float("3.14")
来源：http://man.zdqjudy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://loz.yfazqb.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hkh.ivvv.top

TS:   parseInt("42", 10); Number("42")
来源：http://zgi.dianchejie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ljk.zhixingplan.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dve.dianchejie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hhr.c1oappe.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ihb.yuxming.cn

[A07] 数字转字符串
来源：http://ddt.yongpay.top

Py:   str(42)
来源：http://prv.gogol.net.cn

PHP:  (string) 42; strval(42)
来源：http://zli.iojbl.cn

JS:   String(42); (42).toString()
来源：http://ppl.zhijiandao.cn

TS:   String(42)
来源：http://xtp.aibaodan.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://swe.havefunace.top

Go:   strconv.Itoa(42)
来源：http://wid.hesvh.cn

Ruby: 42.to_s
来源：http://bhn.snrcjt.cn

C#:   42.ToString()
来源：http://gcf.ydjk.org.cn

[A08] 取整与四舍五入
来源：http://shm.hysaishi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rzk.fzhhl.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://oos.yanxiufei.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vov.ywan-chungtsiang.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qdl.xingfuxueyuan.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://drv.kuanghao11.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lax.hongshengwenyu.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://xtb.hfpthk.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mne.shuidangran.top

[A09] 绝对值与最大最小值
来源：http://dfa.shzxlz.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ngt.haohaochexian.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://abu.dianchejie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bwa.sjlbkw.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tdl.cucudq.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://upc.xuetiantiany.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://uvx.ppjwa.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bzs.wangdashe.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lfs.ybcxt.top

[A10] 生成随机数
来源：http://jiv.jianghu66.top

Py:   import random; random.randint(1, 100)
来源：http://kgt.daria6918.cn

PHP:  random_int(1, 100);
来源：http://vnd.vqdsnc.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jsx.hesvh.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ayt.fktsv.cn

Java: new Random().nextInt(100) + 1
来源：http://sfe.wangshuangyany.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://svz.zhixingplan.top

Ruby: rand(1..100)
来源：http://bis.hcnkem.com

C#:   new Random().Next(1, 101)
来源：http://oud.yj202588.top

[A11] 条件表达式（三元）
来源：http://few.jinghuilouyu.cn

Py:   "yes" if x > 0 else "no"
来源：http://xnu.daxiang520.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://rjq.nwbrower.top

JS:   x > 0 ? "yes" : "no"
来源：http://djj.haohaochexian.top

TS:   x > 0 ? "yes" : "no"
来源：http://fkx.havefunace.top

Java: x > 0 ? "yes" : "no"
来源：http://gun.pengpengdd.cyou

Go:   // 无三元运算符，需用 if 语句
来源：http://dmu.chenlongwang.top

Ruby: x > 0 ? "yes" : "no"
来源：http://mwu.yangfankeji.com

C#:   x > 0 ? "yes" : "no"
来源：http://qwb.chenzaomai.com

[A12] 字符串插值 / 格式化
来源：http://rvs.xuetiantiany.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ctt.shuidangran.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fxh.hywenlv.cn

JS:   `Hello, ${name}!`
来源：http://yux.havefunace.top

TS:   `Hello, ${name}!`
来源：http://evj.yj20258888.top

Java: "Hello, %s!".formatted(name)
来源：http://dow.tianlin.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cwp.xylfe.cn

Ruby: "Hello, #{name}!"
来源：http://vko.epnwcf.com

C#:   $"Hello, {name}!"
来源：http://xhh.zhaomingkeji.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://oql.nanxinkj.top

Py:   "第一行\n第二行"
来源：http://bcr.tarul.cn

PHP:  "第一行\n第二行"
来源：http://hfs.52xcode.cn

JS:   "第一行\n第二行"
来源：http://lre.hnxiangtu.top

TS:   "第一行\n第二行"
来源：http://jfv.pycfn.com

Java: "第一行\n第二行"
来源：http://inq.yj20258888.top

Go:   "第一行\n第二行"
来源：http://iwn.yvedp.cn

Ruby: "第一行\n第二行"
来源：http://nwn.sjlbkw.cn

C#:   "第一行\n第二行"
来源：http://hab.zdqjudy.top

[A14] 注释写法
来源：http://nji.ppjwa.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://uyg.zdbjq.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fsb.uphjek.com

JS:   // 单行；/* 多行 */
来源：http://jza.316326.xyz

TS:   // 单行；/* 多行 */
来源：http://grt.meibo888.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qpy.jyoumei.cn

Go:   // 单行；/* 多行 */
来源：http://ynf.yj20258.top

Ruby: # 单行；=begin 多行 =end
来源：http://ezb.hfpthk.cn

C#:   // 单行；/* 多行 */
来源：http://fjp.iojbl.cn

[A15] 空值判断与默认值
来源：http://zjq.jianghu66.top

Py:   value = data or "默认值"
来源：http://ejv.xinyue.icu

PHP:  $value = $data ?? "默认值";
来源：http://yyw.xuanzx.com

JS:   const value = data ?? "默认值";
来源：http://seh.guowangkeji.top

TS:   const value = data ?? "默认值";
来源：http://vnh.ydzc1.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rmg.jyoumei.cn

Go:   if data == "" { data = "默认值" }
来源：http://wzi.pycfn.com

Ruby: value = data || "默认值"
来源：http://aju.hywenlv.cn

C#:   var value = data ?? "默认值";
来源：http://tfk.shzxlz.cn

[A16] 真假值判断规则
来源：http://svi.sjlbkw.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zib.sjlbkw.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gxa.ywan-chungtsiang.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jev.yvedp.cn

TS:   if (!x) {}
来源：http://yrq.yonumen.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://roj.iojbl.cn


<!-- 参考信息 -->