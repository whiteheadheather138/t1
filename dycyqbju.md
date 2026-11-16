代发 wailian999

[U97] JS：并发请求
来源：http://prz.zdbjq.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dqw.fengsongda.top

[U98] JS：fetch 带 JSON
来源：http://moa.shanyushiyangkeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pbp.bjfxy.top

[U99] JS：事件监听
来源：http://jcp.aibaodan.cn

el.addEventListener("click", e => {})
来源：http://pla.shanyushiyangkeji.top

[U100] JS：DOM 查询
来源：http://owt.uphjek.com

document.querySelector(".item")
来源：http://aop.pengpengdd.cyou

[U101] JS：classList 操作
来源：http://vxw.ppjwa.cn

el.classList.toggle("active")
来源：http://kww.ybcxt.top

[U102] JS：本地存储
来源：http://coh.gotoacloud.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hpj.epnwcf.com

[U103] JS：定时器
来源：http://atm.gogol.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gje.cucudq.cn

[U104] JS：防抖
来源：http://gln.gotoacloud.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fqg.hnxiangtu.top

[U105] JS：节流
来源：http://agb.nanxuanxn.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uuz.cqqwz.cn

[U106] JS：日期格式化
来源：http://avd.daxiang520.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xqd.chenzaomai.com

[U107] JS：数字千分位
来源：http://yuq.gogol.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mvr.gogol.net.cn

[U108] JS：随机整数
来源：http://yfl.yanxiufei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mud.haohaochexian.top

[U109] JS：数组分组
来源：http://roq.andypj.xyz

Object.groupBy(arr, x => x.type)
来源：http://tuz.wangdashe.top

[U110] JS：数组分块
来源：http://wzl.yangfankeji.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mut.hysaishi.cn

[U111] JS：对象转 Map
来源：http://lgh.vehdjk.com

new Map(Object.entries(obj))
来源：http://ysg.yvedp.cn

[U112] JS：字符串补位
来源：http://xzd.fzhhl.top

"7".padStart(3, "0")
来源：http://ndc.fehbvm.com

[U113] JS：正则替换全部
来源：http://pfs.c1oappe.top

s.replaceAll("a", "b")
来源：http://tbf.zhixingplan.top

[U114] JS：JSON 深比较
来源：http://idj.jqgufenzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://bku.yj20258888.top

[U115] JS：生成 UUID
来源：http://cka.birdmap.top

crypto.randomUUID()
来源：http://yoh.zhengqikj.top

[U116] JS：类型检查（JSDoc）
来源：http://hnu.svipenyu.cn

/** @param {string} name */ function f(name) {}
来源：http://mgh.jyoumei.cn

[U117] JS：单元测试
来源：http://hpt.cashguo.top

npm i -D vitest;  npx vitest
来源：http://sux.havefunace.top

[U118] JS：开发服务器
来源：http://dwx.hcnkem.com

npm i -D vite;  npx vite
来源：http://lio.hcnkem.com

[U119] JS：生产构建
来源：http://jyv.chenjidiqi.icu

npx vite build
来源：http://gyl.shangyingyoupin.top

[U120] JS：读取环境变量（Vite）
来源：http://fym.cashguo.top

import.meta.env.VITE_API_URL
来源：http://mcd.jyoumei.cn

================================================================================
来源：http://mya.daria6918.cn

统计汇总
来源：http://rhp.yfazqb.com

================================================================================
来源：http://onw.bjfxy.top

按语言统计（条）：
来源：http://xnv.yj20258.top

Python ......... 252
来源：http://wjg.ywan-chungtsiang.top

PHP ............ 252
来源：http://wuu.jqgfzy.top

JavaScript ..... 252
来源：http://vmh.svipenyu.cn

TypeScript ..... 212
来源：http://phk.zhongyouzk.top

Java ........... 212
来源：http://bha.shanyushiyangtech.top

Go ............. 212
来源：http://wiv.hnxiangtu.top

Ruby ........... 212
来源：http://nyr.cheryme.top

C# ............. 212
来源：http://mkc.yonumen.top

C .............. 30
来源：http://tnh.hywenlv.cn

C++ ............ 30
来源：http://dxq.zhoulong.xyz

SQL ............ 90
来源：http://nor.daxiang520.top

Bash ........... 80
来源：http://fiz.jqgfzy.top

Kotlin ......... 15
来源：http://gqb.yuxming.cn

Swift .......... 15
来源：http://hkw.jqgufenzy.top

Lua ............ 10
来源：http://nfn.hnqzz.top

Perl ........... 10
来源：http://hcj.fzhhl.top

Scala .......... 10
来源：http://imo.guowangkeji.top

------------------------------------
来源：http://ylc.hammf.cn

合计 ........... 2106 条
来源：http://dgq.shanyushiyangtech.top

按章节统计：
来源：http://fap.tianlin.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ghx.tian-w.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fjo.shuidangran.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ezo.ydjk.org.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fye.wangshuangyany.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mnr.ivvv.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://etr.hesvh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sju.sweek.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nwf.xinyue.icu

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://imw.snrcjt.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tpd.hcnkem.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wmd.fehbvm.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qpr.zhoulong.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pdx.jinghuilouyu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uya.sufxvd.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tpb.hfpthk.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fzr.aizwys.cn

Q SQL 专题                              90
来源：http://mcq.wangshuangyany.cn

R Bash 专题                             80
来源：http://efy.yuxming.cn

S C / C++ 专题                          60
来源：http://ygk.hcnkem.com

T 其他语言补充                          60
来源：http://kyp.hnqzz.top

U 高频实用片段                         120
来源：http://oln.guowangkeji.top

------------------------------------
来源：http://ctc.xziqi.cn

合计                                  2106 条
来源：http://xqe.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://gcl.epnwcf.com

使用提醒
来源：http://sxx.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://lwu.gzhubu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ynh.zycfv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gah.yanxiufei.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bjv.gogol.net.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://hbu.yfazqb.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://frd.yonumen.top

—— 文件结束 ——
来源：http://wmv.aibaodan.cn

================================================================================
来源：http://yhh.iojbl.cn

程序语言常见例子速查手册（2024 版）
来源：http://hbr.vqdsnc.cn

Common Programming Examples Cheat Book
来源：http://yit.zhoulong.xyz

================================================================================
来源：http://baw.hcnkem.com

【收录内容】
来源：http://sdz.shanyushiyangkeji.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://bey.vqdsnc.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ldr.fktsv.cn

SQL · Bash · C · C++
来源：http://shg.gogol.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dxw.yj20258888.top

【使用说明】
来源：http://eiw.yfazqb.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ety.sxryk.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dra.shanyushiyangkeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sxg.pycfn.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wab.jinqigfzy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://tmw.yj20258888.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zdv.xinyue.icu

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://iep.jiagoushi.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://frk.yvedp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qnd.yongpay.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sbe.pengpengdd.cyou

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fea.chenzaomai.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://upe.yuanzhike.top

【文件统计】
来源：http://yzs.pycfn.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mdj.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://vha.zhijiandao.cn

目  录
来源：http://mam.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://htj.bbcook.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zgp.wangdashe.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rxt.zhoulong.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://unp.yuxming.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ndv.gzhubu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rhk.ivvv.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kvt.meibo888.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gbv.cqqwz.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rvc.pycfn.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fdy.hcnkem.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bpi.cheryme.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xbn.xingfuxueyuan.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hmo.wangshuangyany.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://smd.chenlongwang.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ehx.316326.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sxi.xuetiantiany.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yjn.uphjek.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vua.haohaochexian.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://gym.jinyuanbaomall.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fhq.316326.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hxf.shanyushiyangkeji.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xgw.hongshengwenyu.top

================================================================================
来源：http://eqw.chenlongwang.top

A. 基础语法与类型
来源：http://xdz.jlsjyb.cn

================================================================================
来源：http://dff.chenlongwang.top

[A01] Hello World
来源：http://qhd.fanxiaobao.xyz

Py:   print("Hello, World!")
来源：http://nbc.bbcook.cn

PHP:  echo "Hello, World!";
来源：http://kcs.hesvh.cn

JS:   console.log("Hello, World!");
来源：http://prj.redwolf501.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://oey.chenlongwang.top

Java: System.out.println("Hello, World!");
来源：http://xis.fehbvm.com

Go:   fmt.Println("Hello, World!")
来源：http://raz.cdnleiting.top

Ruby: puts "Hello, World!"
来源：http://nie.vehdjk.com

C#:   Console.WriteLine("Hello, World!");
来源：http://rgp.nwbrower.top

[A02] 变量声明与赋值
来源：http://pyj.jianghu66.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uoh.guowangkeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://lqc.316326.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://imr.shuidangran.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ard.sufxvd.cn

Java: String name = "Alex"; int age = 20;
来源：http://coh.guannengcc.top

Go:   name := "Alex"; age := 20
来源：http://ylo.chenjidiqi.icu

Ruby: name = "Alex"; age = 20
来源：http://kpo.havefunace.top

C#:   string name = "Alex"; int age = 20;
来源：http://oca.andypj.xyz

[A03] 常量定义
来源：http://tlk.hysaishi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jyd.sysykeji.top

PHP:  const PI = 3.14159;
来源：http://itl.fktsv.cn

JS:   const PI = 3.14159;
来源：http://wff.jqgfzy.top

TS:   const PI: number = 3.14159;
来源：http://wqq.aizwys.cn

Java: static final double PI = 3.14159;
来源：http://qgl.xylfe.cn

Go:   const PI = 3.14159
来源：http://qvw.sxryk.cn

Ruby: PI = 3.14159
来源：http://wxz.aizwys.cn

C#:   const double PI = 3.14159;
来源：http://wxn.ppjwa.cn

[A04] 判断变量类型
来源：http://jov.fengsongda.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://nbd.epnwcf.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tbl.zhoulong.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zke.haohaochexian.top

TS:   typeof x; x instanceof Date
来源：http://kia.epnwcf.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gml.zhixingplan.top

Go:   reflect.TypeOf(x).Name()
来源：http://fyz.haohaochexian.top

Ruby: x.class; x.is_a?(Integer)
来源：http://vmt.yangfankeji.com

C#:   x.GetType().Name; x is int
来源：http://xyy.jinqigfzy.top

[A05] 整数除法与取模
来源：http://eoy.hcnkem.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ooe.gaohongyu789.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ekd.aibaodan.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pur.gotoacloud.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zbp.hfpthk.cn

Java: 7 / 2; 7 % 2
来源：http://lgn.gogol.net.cn

Go:   7 / 2; 7 % 2
来源：http://rts.yj202588.top

Ruby: 7 / 2; 7 % 2
来源：http://zqc.uphjek.com

C#:   7 / 2; 7 % 2
来源：http://tkk.zhijiandao.cn

[A06] 字符串转数字
来源：http://mbc.yonumen.top

Py:   int("42"); float("3.14")
来源：http://jmk.cheryme.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dfz.yangfankeji.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jki.chenzaomai.com

TS:   parseInt("42", 10); Number("42")
来源：http://nhq.zhongyouzk.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ckq.yangfankeji.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sre.svipenyu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://cco.havefunace.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pmo.quarkkingdee.top

[A07] 数字转字符串
来源：http://vou.yfazqb.com

Py:   str(42)
来源：http://fno.jinqigufen.top

PHP:  (string) 42; strval(42)
来源：http://nxs.cashguo.top

JS:   String(42); (42).toString()
来源：http://lhk.feifeiyinyue.top

TS:   String(42)
来源：http://nub.pycfn.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://nbi.daria6918.cn

Go:   strconv.Itoa(42)
来源：http://vds.redwolf501.top

Ruby: 42.to_s
来源：http://vnt.zycfv.cn

C#:   42.ToString()
来源：http://kpe.yuxming.cn

[A08] 取整与四舍五入
来源：http://gkw.jlsjyb.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wcy.tarul.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bep.hnqzz.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pww.daria6918.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jfw.svipenyu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://szp.yuanzhike.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wtq.zhijiandao.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://bpk.tian-w.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ifi.yvedp.cn

[A09] 绝对值与最大最小值
来源：http://kst.zhaomingkeji.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://iih.yuanzhike.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://llb.ivvv.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bid.zdqjudy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kym.zhiwuduotai.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hpz.shuidangran.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gqa.cashguo.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jod.zhengqikj.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wuc.shzxlz.cn

[A10] 生成随机数
来源：http://bif.shuidangran.top

Py:   import random; random.randint(1, 100)
来源：http://rja.tianlin.xyz

PHP:  random_int(1, 100);
来源：http://nur.chenjidiqi.icu

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fsl.shanyushiyangtech.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://epn.aibaodan.cn

Java: new Random().nextInt(100) + 1
来源：http://ghl.chenzaomai.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kzi.daria6918.cn

Ruby: rand(1..100)
来源：http://auy.tianlin.xyz

C#:   new Random().Next(1, 101)
来源：http://pvq.guowangkeji.top

[A11] 条件表达式（三元）
来源：http://yex.9152youxi.cn

Py:   "yes" if x > 0 else "no"
来源：http://riu.cheryme.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://mib.zhiwuduotai.top

JS:   x > 0 ? "yes" : "no"
来源：http://vcj.shuidangran.top

TS:   x > 0 ? "yes" : "no"
来源：http://yro.wangshuangyany.cn

Java: x > 0 ? "yes" : "no"
来源：http://spx.daxiang520.top

Go:   // 无三元运算符，需用 if 语句
来源：http://vxv.fehbvm.com

Ruby: x > 0 ? "yes" : "no"
来源：http://sty.daria6918.cn

C#:   x > 0 ? "yes" : "no"
来源：http://osf.tian-w.cn

[A12] 字符串插值 / 格式化
来源：http://iqy.hesvh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jlk.guannengcc.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ktx.guowangkeji.top

JS:   `Hello, ${name}!`
来源：http://acy.316326.xyz

TS:   `Hello, ${name}!`
来源：http://dkx.hammf.cn

Java: "Hello, %s!".formatted(name)
来源：http://otg.wangdashe.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xdy.bjfxy.top

Ruby: "Hello, #{name}!"
来源：http://dez.shanyushiyangtech.top

C#:   $"Hello, {name}!"
来源：http://hmv.wangshuangyany.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://emj.iojbl.cn

Py:   "第一行\n第二行"
来源：http://uai.bbcook.cn

PHP:  "第一行\n第二行"
来源：http://exr.hammf.cn

JS:   "第一行\n第二行"
来源：http://vnb.wangshuangyany.cn

TS:   "第一行\n第二行"
来源：http://tbk.zhaomingkeji.xyz

Java: "第一行\n第二行"
来源：http://dhv.jinqigfzy.top

Go:   "第一行\n第二行"
来源：http://qlb.jinqigfzy.top

Ruby: "第一行\n第二行"
来源：http://jbo.xziqi.cn

C#:   "第一行\n第二行"
来源：http://jgl.cashguo.top

[A14] 注释写法
来源：http://xbx.chenzaomai.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://niw.cqqwz.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tae.haohaochexian.top

JS:   // 单行；/* 多行 */
来源：http://nwi.yj202588.top

TS:   // 单行；/* 多行 */
来源：http://iiz.chenzaomai.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fqz.bbcook.cn

Go:   // 单行；/* 多行 */
来源：http://afi.hongshengwenyu.top

Ruby: # 单行；=begin 多行 =end
来源：http://exe.sweek.top

C#:   // 单行；/* 多行 */
来源：http://ypy.shzxlz.cn

[A15] 空值判断与默认值
来源：http://rud.jyoumei.cn

Py:   value = data or "默认值"
来源：http://wcn.sweek.top

PHP:  $value = $data ?? "默认值";
来源：http://kgq.yongpay.top

JS:   const value = data ?? "默认值";
来源：http://phi.meibo888.top

TS:   const value = data ?? "默认值";
来源：http://lvw.daxiang520.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ogs.haohaochexian.top

Go:   if data == "" { data = "默认值" }
来源：http://xpm.zdbjq.cn

Ruby: value = data || "默认值"
来源：http://csq.tarul.cn

C#:   var value = data ?? "默认值";
来源：http://krc.jlsjyb.cn

[A16] 真假值判断规则
来源：http://hni.jinyuanbaomall.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pik.haohaochexian.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lqi.dashuyun.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vop.uphjek.com

TS:   if (!x) {}
来源：http://cpv.shanyushiyangkeji.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jbt.nwbrower.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qlz.svipenyu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lur.haohaochexian.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cjr.yuxming.cn

[A17] 位运算
来源：http://lup.jinghuilouyu.cn


<!-- 参考信息 -->