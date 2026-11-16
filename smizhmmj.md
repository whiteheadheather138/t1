代发 wailian999

[U87] JS：解构默认值
来源：http://tuq.xziqi.cn

const { a = 1, b = 2 } = obj;
来源：http://bck.jinghuilouyu.cn

[U88] JS：对象展开合并
来源：http://hcr.yj20258.top

{ ...a, ...b }
来源：http://pqo.gotoacloud.top

[U89] JS：数组去重
来源：http://ieb.nanxinkj.top

[...new Set(arr)]
来源：http://vaq.pycfn.com

[U90] JS：数字数组排序
来源：http://rpy.yangfankeji.com

[...arr].sort((a, b) => a - b)
来源：http://lez.gzhubu.top

[U91] JS：对象键值遍历
来源：http://zpx.zdqjudy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lgk.haohaochexian.top

[U92] JS：深拷贝
来源：http://yaf.vehdjk.com

structuredClone(obj)
来源：http://kgi.gaohongyu789.top

[U93] JS：模板字符串
来源：http://bqj.vehdjk.com

`共 ${n} 条`
来源：http://dwz.sjlbkw.cn

[U94] JS：箭头函数
来源：http://qkh.zycfv.cn

const double = x => x * 2;
来源：http://msh.zhongyouzk.top

[U95] JS：Promise 包装
来源：http://sem.cucudq.cn

new Promise((resolve, reject) => {})
来源：http://dju.jinqigufen.top

[U96] JS：async/await 与异常
来源：http://ynz.xuetiantiany.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hbb.shangyingyoupin.top

[U97] JS：并发请求
来源：http://gib.xinyue.icu

await Promise.all(urls.map(u => fetch(u)))
来源：http://fsr.guowangkeji.top

[U98] JS：fetch 带 JSON
来源：http://axk.kuanghao11.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zbg.pengpengdd.cyou

[U99] JS：事件监听
来源：http://vya.wangdashe.top

el.addEventListener("click", e => {})
来源：http://urw.pycfn.com

[U100] JS：DOM 查询
来源：http://nen.52xcode.cn

document.querySelector(".item")
来源：http://gmx.tian-w.cn

[U101] JS：classList 操作
来源：http://bkv.tanke756.top

el.classList.toggle("active")
来源：http://ous.hongshengwenyu.top

[U102] JS：本地存储
来源：http://lxu.wangdashe.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://geb.nanxinkj.top

[U103] JS：定时器
来源：http://pxe.sysykeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://scc.sysykeji.top

[U104] JS：防抖
来源：http://net.yfazqb.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hcm.jiagoushi.top

[U105] JS：节流
来源：http://rnu.gotoacloud.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zss.haohaochexian.top

[U106] JS：日期格式化
来源：http://prf.snrcjt.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kzr.chenlongwang.top

[U107] JS：数字千分位
来源：http://imk.uphjek.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vab.zycfv.cn

[U108] JS：随机整数
来源：http://oay.fehbvm.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cka.shzxlz.cn

[U109] JS：数组分组
来源：http://aec.jqgufenzy.top

Object.groupBy(arr, x => x.type)
来源：http://dly.xuetiantiany.cn

[U110] JS：数组分块
来源：http://bas.yj20258888.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jcs.guannengcc.top

[U111] JS：对象转 Map
来源：http://pop.meibo888.top

new Map(Object.entries(obj))
来源：http://ner.yvedp.cn

[U112] JS：字符串补位
来源：http://xla.jqgfzy.top

"7".padStart(3, "0")
来源：http://xtt.cashguo.top

[U113] JS：正则替换全部
来源：http://wtf.zhongyouzk.top

s.replaceAll("a", "b")
来源：http://gfa.gzhubu.top

[U114] JS：JSON 深比较
来源：http://zci.hammf.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://aiw.uphjek.com

[U115] JS：生成 UUID
来源：http://wfg.dashuyun.cn

crypto.randomUUID()
来源：http://fee.sxryk.cn

[U116] JS：类型检查（JSDoc）
来源：http://bzp.ydjk.org.cn

/** @param {string} name */ function f(name) {}
来源：http://fwx.ydzc1.top

[U117] JS：单元测试
来源：http://hkh.fanxiaobao.xyz

npm i -D vitest;  npx vitest
来源：http://bdm.zhijiandao.cn

[U118] JS：开发服务器
来源：http://xvf.gogol.net.cn

npm i -D vite;  npx vite
来源：http://xlh.ydjk.org.cn

[U119] JS：生产构建
来源：http://xod.xinyue.icu

npx vite build
来源：http://krx.kuanghao11.cn

[U120] JS：读取环境变量（Vite）
来源：http://qvt.jinyuanbaomall.cn

import.meta.env.VITE_API_URL
来源：http://epv.ydzc1.top

================================================================================
来源：http://xtz.shanyushiyangkeji.top

统计汇总
来源：http://bqa.jinyuanbaomall.cn

================================================================================
来源：http://ome.pycfn.com

按语言统计（条）：
来源：http://siw.hesvh.cn

Python ......... 252
来源：http://bju.havefunace.top

PHP ............ 252
来源：http://wuz.yonumen.top

JavaScript ..... 252
来源：http://sqn.shanyushiyangtech.top

TypeScript ..... 212
来源：http://uja.hnqzz.top

Java ........... 212
来源：http://zux.kuanghao11.cn

Go ............. 212
来源：http://hfn.uphjek.com

Ruby ........... 212
来源：http://ixr.bbcook.cn

C# ............. 212
来源：http://wdo.wangshuangyany.cn

C .............. 30
来源：http://nsr.pycfn.com

C++ ............ 30
来源：http://izq.52xcode.cn

SQL ............ 90
来源：http://tao.yanxiufei.cn

Bash ........... 80
来源：http://ycm.hnxiangtu.top

Kotlin ......... 15
来源：http://gdy.meibo888.top

Swift .......... 15
来源：http://vbe.ppjwa.cn

Lua ............ 10
来源：http://szx.jinqigfzy.top

Perl ........... 10
来源：http://qzf.fehbvm.com

Scala .......... 10
来源：http://nwv.cucudq.cn

------------------------------------
来源：http://wcy.aibaodan.cn

合计 ........... 2106 条
来源：http://qvv.shanyushiyangtech.top

按章节统计：
来源：http://wbi.ydzc1.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zci.cucudq.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uxu.zhijiandao.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ufx.chenzaomai.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lzc.shzxlz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rsh.sysykeji.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://imw.cucudq.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dmk.52xcode.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qhb.xuanzx.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wsf.fktsv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ysl.fanxiaobao.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dqa.jinghuilouyu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vny.cdnleiting.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dln.svipenyu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jbb.zycfv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yta.yonumen.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bim.ywan-chungtsiang.top

Q SQL 专题                              90
来源：http://opc.cucudq.cn

R Bash 专题                             80
来源：http://shp.tanke756.top

S C / C++ 专题                          60
来源：http://mcd.fktsv.cn

T 其他语言补充                          60
来源：http://wpa.ivvv.top

U 高频实用片段                         120
来源：http://ciw.snrcjt.cn

------------------------------------
来源：http://lsu.yfazqb.com

合计                                  2106 条
来源：http://xad.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://wei.tian-w.cn

使用提醒
来源：http://nks.hcnkem.com

--------------------------------------------------------------------------------
来源：http://mtj.jinyuanbaomall.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gqw.ivvv.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bip.sjlbkw.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dpe.sysykeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://zgq.havefunace.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bmb.jinqigfzy.top

—— 文件结束 ——
来源：http://xob.chenlongwang.top

================================================================================
来源：http://cgd.gotoacloud.top

程序语言常见例子速查手册（2024 版）
来源：http://egq.xinyue.icu

Common Programming Examples Cheat Book
来源：http://yoe.meibo888.top

================================================================================
来源：http://btf.yfazqb.com

【收录内容】
来源：http://fnw.shanyushiyangtech.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ods.chenlongwang.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://trj.nanxuanxn.top

SQL · Bash · C · C++
来源：http://eqd.zdbjq.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ahm.andypj.xyz

【使用说明】
来源：http://tvg.shanyushiyangtech.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rpy.yueranfly.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wbj.andypj.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ucu.cucudq.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://poz.ppjwa.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://job.yonumen.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wpa.epnwcf.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ged.yongpay.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gja.dashuyun.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://aii.yj202588.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://alx.ctjpmb.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fzs.zhixingplan.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gaf.daria6918.cn

【文件统计】
来源：http://ofp.feifeiyinyue.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zxb.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://wjf.fengsongda.top

目  录
来源：http://fbd.tanke756.top

--------------------------------------------------------------------------------
来源：http://qgk.nwbrower.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jvj.shanyushiyangkeji.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xne.fehbvm.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ihi.hnxiangtu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kzo.ctjpmb.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ebs.iojbl.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ops.fktsv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qdo.meibo888.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zvj.epnwcf.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://aey.tian-w.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tgq.sysykeji.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://odg.cashguo.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ogz.hysaishi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ohn.yj20258.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yqh.hnqzz.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jhg.zycfv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nyp.nanxinkj.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rmt.cucudq.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xeo.c1oappe.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qxz.hnxiangtu.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://utt.chenjidiqi.icu

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zma.zhiwuduotai.top

================================================================================
来源：http://djw.c1oappe.top

A. 基础语法与类型
来源：http://gga.zhixingplan.top

================================================================================
来源：http://seh.mhx1999.top

[A01] Hello World
来源：http://xbu.hysaishi.cn

Py:   print("Hello, World!")
来源：http://vaa.aizwys.cn

PHP:  echo "Hello, World!";
来源：http://ird.daria6918.cn

JS:   console.log("Hello, World!");
来源：http://dep.jyoumei.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zlw.yuxming.cn

Java: System.out.println("Hello, World!");
来源：http://cgq.zdqjudy.top

Go:   fmt.Println("Hello, World!")
来源：http://nsg.yuxming.cn

Ruby: puts "Hello, World!"
来源：http://fxo.xziqi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://baj.hongshengwenyu.top

[A02] 变量声明与赋值
来源：http://clu.zhongyouzk.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gkq.fengsongda.top

PHP:  $name = "Alex"; $age = 20;
来源：http://cms.jinqigufen.top

JS:   let name = "Alex"; const age = 20;
来源：http://gvv.cqqwz.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ijh.jianghu66.top

Java: String name = "Alex"; int age = 20;
来源：http://tje.jinqigufen.top

Go:   name := "Alex"; age := 20
来源：http://lia.yongpay.top

Ruby: name = "Alex"; age = 20
来源：http://zem.ybcxt.top

C#:   string name = "Alex"; int age = 20;
来源：http://nsn.fengsongda.top

[A03] 常量定义
来源：http://qja.feifeiyinyue.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hyf.redwolf501.top

PHP:  const PI = 3.14159;
来源：http://kfm.yfazqb.com

JS:   const PI = 3.14159;
来源：http://icy.aizwys.cn

TS:   const PI: number = 3.14159;
来源：http://jqo.zhiwuduotai.top

Java: static final double PI = 3.14159;
来源：http://khd.tarul.cn

Go:   const PI = 3.14159
来源：http://exc.cqqwz.cn

Ruby: PI = 3.14159
来源：http://pte.aizwys.cn

C#:   const double PI = 3.14159;
来源：http://fgd.daxiang520.top

[A04] 判断变量类型
来源：http://ehu.jinqigufen.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ubm.hongshengwenyu.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pba.xziqi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zmk.zhongyouzk.top

TS:   typeof x; x instanceof Date
来源：http://ecp.zhengqikj.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yhs.yj20258888.top

Go:   reflect.TypeOf(x).Name()
来源：http://mfq.hfpthk.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ujv.fehbvm.com

C#:   x.GetType().Name; x is int
来源：http://yoq.haohaochexian.top

[A05] 整数除法与取模
来源：http://cqj.zhijiandao.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mql.xinyue.icu

PHP:  intdiv(7, 2); 7 % 2
来源：http://sde.xingfuxueyuan.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ptm.yuanzhike.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fim.gogol.net.cn

Java: 7 / 2; 7 % 2
来源：http://npv.zycfv.cn

Go:   7 / 2; 7 % 2
来源：http://zyw.ivvv.top

Ruby: 7 / 2; 7 % 2
来源：http://wug.fzhhl.top

C#:   7 / 2; 7 % 2
来源：http://wox.smart0.xyz

[A06] 字符串转数字
来源：http://pkf.jianghu66.top

Py:   int("42"); float("3.14")
来源：http://xmc.ydjk.org.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zxq.xuanzx.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wgi.kuanghao11.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fry.sufxvd.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jrl.nwbrower.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ned.cdnleiting.top

Ruby: "42".to_i; "3.14".to_f
来源：http://xcp.c1oappe.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qpp.gaohongyu789.top

[A07] 数字转字符串
来源：http://new.sufxvd.cn

Py:   str(42)
来源：http://tav.havefunace.top

PHP:  (string) 42; strval(42)
来源：http://qwf.fehbvm.com

JS:   String(42); (42).toString()
来源：http://oni.316326.xyz

TS:   String(42)
来源：http://uzk.xuanzx.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://htc.daxiang520.top

Go:   strconv.Itoa(42)
来源：http://pid.gogol.net.cn

Ruby: 42.to_s
来源：http://jmy.shanyushiyangkeji.top

C#:   42.ToString()
来源：http://ctx.gzhubu.top

[A08] 取整与四舍五入
来源：http://voo.hcnkem.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uzv.sufxvd.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://unq.yj202588.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lxr.sxryk.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cse.cucudq.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mae.cashguo.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://axb.fanxiaobao.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://wou.daxiang520.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rmu.andypj.xyz

[A09] 绝对值与最大最小值
来源：http://tid.nanxuanxn.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jac.cqqwz.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dog.yonumen.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://epa.jinqigfzy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ikg.nwbrower.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mdu.ybcxt.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fur.iojbl.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fpl.wangshuangyany.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qmv.aizwys.cn

[A10] 生成随机数
来源：http://wtc.chenjidiqi.icu

Py:   import random; random.randint(1, 100)
来源：http://nmw.jqgufenzy.top

PHP:  random_int(1, 100);
来源：http://dpb.hnqzz.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ivd.xinyue.icu

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nwb.fzhhl.top

Java: new Random().nextInt(100) + 1
来源：http://tsk.epnwcf.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cgr.ivvv.top

Ruby: rand(1..100)
来源：http://ipw.ivvv.top

C#:   new Random().Next(1, 101)
来源：http://hyj.sufxvd.cn

[A11] 条件表达式（三元）
来源：http://znm.0kj1m.cn

Py:   "yes" if x > 0 else "no"
来源：http://olf.sxryk.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rmz.yj20258888.top

JS:   x > 0 ? "yes" : "no"
来源：http://jci.hongshengwenyu.top

TS:   x > 0 ? "yes" : "no"
来源：http://vxr.ctjpmb.com

Java: x > 0 ? "yes" : "no"
来源：http://tuu.snrcjt.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://lno.jqgufenzy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://epr.tianlin.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://kat.redwolf501.top

[A12] 字符串插值 / 格式化
来源：http://nxx.xziqi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fhs.kuanghao11.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://aaj.andypj.xyz

JS:   `Hello, ${name}!`
来源：http://jfh.xingfuxueyuan.xyz

TS:   `Hello, ${name}!`
来源：http://rpf.ivvv.top

Java: "Hello, %s!".formatted(name)
来源：http://sps.ppjwa.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gsb.ydjk.org.cn

Ruby: "Hello, #{name}!"
来源：http://sty.jinqigufen.top

C#:   $"Hello, {name}!"
来源：http://cva.yueranfly.top

[A13] 多行字符串（练习 \n 转义）
来源：http://gne.zhaomingkeji.xyz

Py:   "第一行\n第二行"
来源：http://lrg.jinqigfzy.top

PHP:  "第一行\n第二行"
来源：http://kpb.yonumen.top

JS:   "第一行\n第二行"
来源：http://psk.dashuyun.cn

TS:   "第一行\n第二行"
来源：http://rev.redwolf501.top

Java: "第一行\n第二行"
来源：http://uwf.cqqwz.cn

Go:   "第一行\n第二行"
来源：http://jez.sweek.top

Ruby: "第一行\n第二行"
来源：http://azb.yonumen.top

C#:   "第一行\n第二行"
来源：http://lsu.sweek.top

[A14] 注释写法
来源：http://rsx.dashuyun.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zhz.ybcxt.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://csd.ydzc1.top

JS:   // 单行；/* 多行 */
来源：http://idz.gaohongyu789.top

TS:   // 单行；/* 多行 */
来源：http://ajt.zhixingplan.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kla.zhengqikj.top

Go:   // 单行；/* 多行 */
来源：http://isr.zhaomingkeji.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://bdy.sweek.top


<!-- 参考信息 -->