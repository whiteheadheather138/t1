代发 wailian999

[U91] JS：对象键值遍历
来源：http://oci.ydjk.org.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hie.yueranfly.top

[U92] JS：深拷贝
来源：http://rwq.xuanzx.com

structuredClone(obj)
来源：http://lzj.zhaomingkeji.xyz

[U93] JS：模板字符串
来源：http://lbu.pycfn.com

`共 ${n} 条`
来源：http://xhk.shangyingyoupin.top

[U94] JS：箭头函数
来源：http://ymi.cheryme.top

const double = x => x * 2;
来源：http://bol.zhiwuduotai.top

[U95] JS：Promise 包装
来源：http://rhd.nwbrower.top

new Promise((resolve, reject) => {})
来源：http://yzo.316326.xyz

[U96] JS：async/await 与异常
来源：http://xgb.zhiwuduotai.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hss.xziqi.cn

[U97] JS：并发请求
来源：http://mrn.sweek.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://kgg.tianlin.xyz

[U98] JS：fetch 带 JSON
来源：http://vkf.gzhubu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mjq.ppjwa.cn

[U99] JS：事件监听
来源：http://eiv.shuidangran.top

el.addEventListener("click", e => {})
来源：http://hfy.9152youxi.cn

[U100] JS：DOM 查询
来源：http://bbj.zdqjudy.top

document.querySelector(".item")
来源：http://haw.tarul.cn

[U101] JS：classList 操作
来源：http://yys.epnwcf.com

el.classList.toggle("active")
来源：http://zgs.hysaishi.cn

[U102] JS：本地存储
来源：http://peu.yuxming.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sdu.316326.xyz

[U103] JS：定时器
来源：http://ovw.chenjidiqi.icu

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jyp.xuanzx.com

[U104] JS：防抖
来源：http://ctz.svipenyu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pax.guannengcc.top

[U105] JS：节流
来源：http://gga.vqdsnc.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gnp.meibo888.top

[U106] JS：日期格式化
来源：http://czi.jyoumei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lha.feifeiyinyue.top

[U107] JS：数字千分位
来源：http://tta.ctjpmb.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://isw.yj20258.top

[U108] JS：随机整数
来源：http://aql.cheryme.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tig.ydjk.org.cn

[U109] JS：数组分组
来源：http://nia.yj20258888.top

Object.groupBy(arr, x => x.type)
来源：http://oct.tian-w.cn

[U110] JS：数组分块
来源：http://btl.jinghuilouyu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://scy.pycfn.com

[U111] JS：对象转 Map
来源：http://zso.nanxuanxn.top

new Map(Object.entries(obj))
来源：http://bhl.shanyushiyangkeji.top

[U112] JS：字符串补位
来源：http://zux.mhx1999.top

"7".padStart(3, "0")
来源：http://ejn.shangyingyoupin.top

[U113] JS：正则替换全部
来源：http://xif.ehwqpu.com

s.replaceAll("a", "b")
来源：http://gqq.shzxlz.cn

[U114] JS：JSON 深比较
来源：http://ned.hcnkem.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://quu.chenzaomai.com

[U115] JS：生成 UUID
来源：http://dmh.bjfxy.top

crypto.randomUUID()
来源：http://rrl.hnxiangtu.top

[U116] JS：类型检查（JSDoc）
来源：http://ecf.fanxiaobao.xyz

/** @param {string} name */ function f(name) {}
来源：http://uty.xylfe.cn

[U117] JS：单元测试
来源：http://nyc.pycfn.com

npm i -D vitest;  npx vitest
来源：http://mrq.yueranfly.top

[U118] JS：开发服务器
来源：http://vcq.guannengcc.top

npm i -D vite;  npx vite
来源：http://dqx.sufxvd.cn

[U119] JS：生产构建
来源：http://qai.feifeiyinyue.top

npx vite build
来源：http://xnp.andypj.xyz

[U120] JS：读取环境变量（Vite）
来源：http://hkr.zhaomingkeji.xyz

import.meta.env.VITE_API_URL
来源：http://jpb.havefunace.top

================================================================================
来源：http://xoc.zhoulong.xyz

统计汇总
来源：http://egi.vqdsnc.cn

================================================================================
来源：http://wwo.jqgufenzy.top

按语言统计（条）：
来源：http://zxh.cucudq.cn

Python ......... 252
来源：http://ckv.xziqi.cn

PHP ............ 252
来源：http://det.zhongyouzk.top

JavaScript ..... 252
来源：http://iau.yfazqb.com

TypeScript ..... 212
来源：http://ntf.yongpay.top

Java ........... 212
来源：http://mbc.shuidangran.top

Go ............. 212
来源：http://wdn.jqgufenzy.top

Ruby ........... 212
来源：http://ccs.shanyushiyangtech.top

C# ............. 212
来源：http://vyu.fanxiaobao.xyz

C .............. 30
来源：http://ykq.guannengcc.top

C++ ............ 30
来源：http://uje.hnxiangtu.top

SQL ............ 90
来源：http://aqc.ywan-chungtsiang.top

Bash ........... 80
来源：http://xxx.wangdashe.top

Kotlin ......... 15
来源：http://iyb.nwbrower.top

Swift .......... 15
来源：http://blj.yj202588.top

Lua ............ 10
来源：http://dls.zhixingplan.top

Perl ........... 10
来源：http://ffj.ctjpmb.com

Scala .......... 10
来源：http://ons.vehdjk.com

------------------------------------
来源：http://qzn.ppjwa.cn

合计 ........... 2106 条
来源：http://bvy.cheryme.top

按章节统计：
来源：http://yic.uphjek.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ums.yanxiufei.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xmo.sysykeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bak.chenlongwang.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hsk.hesvh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mct.gzhubu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vnk.jinghuilouyu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://amg.guowangkeji.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hgm.zhiwuduotai.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zxu.shzxlz.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://czs.yanxiufei.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gly.c1oappe.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ybs.epnwcf.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rom.zhoulong.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://una.hcnkem.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mff.hywenlv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rri.vqdsnc.cn

Q SQL 专题                              90
来源：http://zce.fzhhl.top

R Bash 专题                             80
来源：http://oud.yuanzhike.top

S C / C++ 专题                          60
来源：http://asl.jlsjyb.cn

T 其他语言补充                          60
来源：http://rug.xingfuxueyuan.xyz

U 高频实用片段                         120
来源：http://jhg.nwbrower.top

------------------------------------
来源：http://nlu.guowangkeji.top

合计                                  2106 条
来源：http://ddt.birdmap.top

--------------------------------------------------------------------------------
来源：http://hgo.chenzaomai.com

使用提醒
来源：http://egf.gzhubu.top

--------------------------------------------------------------------------------
来源：http://kiq.mhx1999.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ffh.hywenlv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wiv.bbcook.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ttp.feifeiyinyue.top

在旧版本上使用前请先确认语法支持情况。
来源：http://oxa.vehdjk.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wor.shuidangran.top

—— 文件结束 ——
来源：http://cdj.yj202588.top

================================================================================
来源：http://crk.shzxlz.cn

程序语言常见例子速查手册（2024 版）
来源：http://blc.yuanzhike.top

Common Programming Examples Cheat Book
来源：http://kha.epnwcf.com

================================================================================
来源：http://axs.yj20258.top

【收录内容】
来源：http://ixj.guowangkeji.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://znn.havefunace.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://skl.fanxiaobao.xyz

SQL · Bash · C · C++
来源：http://ypb.jinghuilouyu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wui.cashguo.top

【使用说明】
来源：http://lbl.hfpthk.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tsu.fanxiaobao.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://liu.jiagoushi.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xos.hfpthk.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ssx.wangdashe.top

Bash:  Shell         C:     C             C++:   C++
来源：http://pnm.jinghuilouyu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://urg.gzhubu.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jwp.jinyuanbaomall.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wqv.jinqigfzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://eod.fktsv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kcp.chenzaomai.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hsp.bbcook.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ycm.yvedp.cn

【文件统计】
来源：http://dgj.svipenyu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zgj.yuxming.cn

--------------------------------------------------------------------------------
来源：http://yux.smart0.xyz

目  录
来源：http://clz.epnwcf.com

--------------------------------------------------------------------------------
来源：http://azy.ydjk.org.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xlx.jlsjyb.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yye.snrcjt.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ous.pycfn.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wrg.wangdashe.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kzj.ivvv.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kwp.dianchejie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mxz.fengsongda.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hyg.tarul.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ccn.nanxinkj.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rrm.vqdsnc.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fuh.ivvv.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://srt.wangdashe.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jbo.jiagoushi.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kgm.fengsongda.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yla.jqgufenzy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sub.daria6918.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ank.hysaishi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gql.shuidangran.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mhs.cqqwz.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hse.zhiwuduotai.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ydr.yangfankeji.com

================================================================================
来源：http://tyb.bjfxy.top

A. 基础语法与类型
来源：http://qir.ydzc1.top

================================================================================
来源：http://tgx.zdqjudy.top

[A01] Hello World
来源：http://wgo.shanyushiyangtech.top

Py:   print("Hello, World!")
来源：http://agf.hammf.cn

PHP:  echo "Hello, World!";
来源：http://twt.quarkkingdee.top

JS:   console.log("Hello, World!");
来源：http://mlo.jiagoushi.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lvz.wangshuangyany.cn

Java: System.out.println("Hello, World!");
来源：http://vxd.iojbl.cn

Go:   fmt.Println("Hello, World!")
来源：http://lgd.hnqzz.top

Ruby: puts "Hello, World!"
来源：http://lyh.fengsongda.top

C#:   Console.WriteLine("Hello, World!");
来源：http://xzn.fehbvm.com

[A02] 变量声明与赋值
来源：http://abv.iojbl.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kie.pycfn.com

PHP:  $name = "Alex"; $age = 20;
来源：http://xbb.nanxuanxn.top

JS:   let name = "Alex"; const age = 20;
来源：http://fhl.gogol.net.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://djm.yangfankeji.com

Java: String name = "Alex"; int age = 20;
来源：http://pat.vehdjk.com

Go:   name := "Alex"; age := 20
来源：http://axf.fehbvm.com

Ruby: name = "Alex"; age = 20
来源：http://bkh.gzhubu.top

C#:   string name = "Alex"; int age = 20;
来源：http://fqq.0kj1m.cn

[A03] 常量定义
来源：http://fgu.jinyuanbaomall.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gff.tarul.cn

PHP:  const PI = 3.14159;
来源：http://pdu.nanxinkj.top

JS:   const PI = 3.14159;
来源：http://gud.ydzc1.top

TS:   const PI: number = 3.14159;
来源：http://vee.yj20258.top

Java: static final double PI = 3.14159;
来源：http://aby.feifeiyinyue.top

Go:   const PI = 3.14159
来源：http://puy.shanyushiyangkeji.top

Ruby: PI = 3.14159
来源：http://ixr.sjlbkw.cn

C#:   const double PI = 3.14159;
来源：http://hno.quarkkingdee.top

[A04] 判断变量类型
来源：http://fop.zdbjq.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tqu.ppjwa.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wfu.fanxiaobao.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nbm.jlsjyb.cn

TS:   typeof x; x instanceof Date
来源：http://rot.ydzc1.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rco.yfazqb.com

Go:   reflect.TypeOf(x).Name()
来源：http://xue.kuanghao11.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://zcw.tarul.cn

C#:   x.GetType().Name; x is int
来源：http://ifm.cdnleiting.top

[A05] 整数除法与取模
来源：http://qqm.haohaochexian.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pcs.jqgfzy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://bnn.hammf.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yny.cqqwz.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xcz.epnwcf.com

Java: 7 / 2; 7 % 2
来源：http://ocu.dianchejie.cn

Go:   7 / 2; 7 % 2
来源：http://jul.birdmap.top

Ruby: 7 / 2; 7 % 2
来源：http://yon.hfpthk.cn

C#:   7 / 2; 7 % 2
来源：http://xrq.chenzaomai.com

[A06] 字符串转数字
来源：http://qnv.guannengcc.top

Py:   int("42"); float("3.14")
来源：http://jdt.chenzaomai.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ybp.gzhubu.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vtl.xylfe.cn

TS:   parseInt("42", 10); Number("42")
来源：http://sia.daria6918.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://irj.wangshuangyany.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ado.sweek.top

Ruby: "42".to_i; "3.14".to_f
来源：http://gnp.ppjwa.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://swv.daria6918.cn

[A07] 数字转字符串
来源：http://eap.andypj.xyz

Py:   str(42)
来源：http://wbg.iojbl.cn

PHP:  (string) 42; strval(42)
来源：http://hqd.jinqigfzy.top

JS:   String(42); (42).toString()
来源：http://ilp.vehdjk.com

TS:   String(42)
来源：http://yce.ppjwa.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ohk.vehdjk.com

Go:   strconv.Itoa(42)
来源：http://yyu.ydjk.org.cn

Ruby: 42.to_s
来源：http://akg.shuidangran.top

C#:   42.ToString()
来源：http://ltp.jinqigfzy.top

[A08] 取整与四舍五入
来源：http://nyu.0kj1m.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uus.jqgfzy.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tqt.daria6918.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gbi.gotoacloud.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ymn.yueranfly.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pjh.sjlbkw.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gcs.haohaochexian.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://fzh.cheryme.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://iow.wangdashe.top

[A09] 绝对值与最大最小值
来源：http://mvl.pengpengdd.cyou

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ojm.yj20258888.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://oub.smart0.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rzx.cqqwz.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pei.zhiwuduotai.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nqn.fktsv.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://epf.cashguo.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lbb.gzhubu.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gzt.fktsv.cn

[A10] 生成随机数
来源：http://ntv.shanyushiyangtech.top

Py:   import random; random.randint(1, 100)
来源：http://pka.cashguo.top

PHP:  random_int(1, 100);
来源：http://juo.zdbjq.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qve.fktsv.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vdu.shangyingyoupin.top

Java: new Random().nextInt(100) + 1
来源：http://eta.cheryme.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hah.tianlin.xyz

Ruby: rand(1..100)
来源：http://ycc.zhijiandao.cn

C#:   new Random().Next(1, 101)
来源：http://fig.wangshuangyany.cn

[A11] 条件表达式（三元）
来源：http://nfh.hywenlv.cn

Py:   "yes" if x > 0 else "no"
来源：http://zrm.ybcxt.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://uyf.hcnkem.com

JS:   x > 0 ? "yes" : "no"
来源：http://suh.pengpengdd.cyou

TS:   x > 0 ? "yes" : "no"
来源：http://gho.zhoulong.xyz

Java: x > 0 ? "yes" : "no"
来源：http://bpd.hesvh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://pvx.jinqigfzy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://bto.xylfe.cn

C#:   x > 0 ? "yes" : "no"
来源：http://akb.shzxlz.cn

[A12] 字符串插值 / 格式化
来源：http://fls.sxryk.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vna.aibaodan.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vvo.jinghuilouyu.cn

JS:   `Hello, ${name}!`
来源：http://vbt.hesvh.cn

TS:   `Hello, ${name}!`
来源：http://slm.fanxiaobao.xyz

Java: "Hello, %s!".formatted(name)
来源：http://cgr.yuxming.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ysa.jiagoushi.top

Ruby: "Hello, #{name}!"
来源：http://mog.nanxuanxn.top

C#:   $"Hello, {name}!"
来源：http://dfp.hnqzz.top

[A13] 多行字符串（练习 \n 转义）
来源：http://tlu.ivvv.top

Py:   "第一行\n第二行"
来源：http://ppt.zycfv.cn

PHP:  "第一行\n第二行"
来源：http://zpr.52xcode.cn

JS:   "第一行\n第二行"
来源：http://rco.quarkkingdee.top

TS:   "第一行\n第二行"
来源：http://juu.c1oappe.top

Java: "第一行\n第二行"
来源：http://lyp.daxiang520.top

Go:   "第一行\n第二行"
来源：http://tet.ppjwa.cn

Ruby: "第一行\n第二行"
来源：http://iln.zhixingplan.top

C#:   "第一行\n第二行"
来源：http://vla.zdbjq.cn

[A14] 注释写法
来源：http://pqu.iojbl.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://oum.yfazqb.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://soc.chenjidiqi.icu

JS:   // 单行；/* 多行 */
来源：http://btq.xylfe.cn

TS:   // 单行；/* 多行 */
来源：http://ufg.hesvh.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ljn.sufxvd.cn

Go:   // 单行；/* 多行 */
来源：http://tjn.0kj1m.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zch.c1oappe.top

C#:   // 单行；/* 多行 */
来源：http://xaj.sjlbkw.cn

[A15] 空值判断与默认值
来源：http://esr.9152youxi.cn

Py:   value = data or "默认值"
来源：http://svm.smart0.xyz

PHP:  $value = $data ?? "默认值";
来源：http://zfq.tanke756.top

JS:   const value = data ?? "默认值";
来源：http://xiw.yfazqb.com

TS:   const value = data ?? "默认值";
来源：http://qyh.xziqi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wip.uphjek.com

Go:   if data == "" { data = "默认值" }
来源：http://lvx.sweek.top


<!-- 参考信息 -->