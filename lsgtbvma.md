代发 wailian999

[U95] JS：Promise 包装
来源：http://hgc.yangfankeji.com

new Promise((resolve, reject) => {})
来源：http://xax.zhoulong.xyz

[U96] JS：async/await 与异常
来源：http://rxk.chenzaomai.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ujs.tianlin.xyz

[U97] JS：并发请求
来源：http://wnk.redwolf501.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vtr.sxryk.cn

[U98] JS：fetch 带 JSON
来源：http://fgq.smart0.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dzs.xingfuxueyuan.xyz

[U99] JS：事件监听
来源：http://xev.meibo888.top

el.addEventListener("click", e => {})
来源：http://wrw.nwbrower.top

[U100] JS：DOM 查询
来源：http://xps.316326.xyz

document.querySelector(".item")
来源：http://iap.aibaodan.cn

[U101] JS：classList 操作
来源：http://myw.wangshuangyany.cn

el.classList.toggle("active")
来源：http://vaf.sxryk.cn

[U102] JS：本地存储
来源：http://agf.epnwcf.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://ykb.tianlin.xyz

[U103] JS：定时器
来源：http://qrj.snrcjt.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xxc.sysykeji.top

[U104] JS：防抖
来源：http://lky.yanxiufei.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ghu.yj202588.top

[U105] JS：节流
来源：http://vii.andypj.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mfb.xingfuxueyuan.xyz

[U106] JS：日期格式化
来源：http://kld.jyoumei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://thf.tianlin.xyz

[U107] JS：数字千分位
来源：http://aqu.yuxming.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kbl.hnxiangtu.top

[U108] JS：随机整数
来源：http://iif.kuanghao11.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wza.jqgfzy.top

[U109] JS：数组分组
来源：http://pof.ctjpmb.com

Object.groupBy(arr, x => x.type)
来源：http://kfe.cdnleiting.top

[U110] JS：数组分块
来源：http://jbc.zycfv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hbo.wangdashe.top

[U111] JS：对象转 Map
来源：http://wqo.jyoumei.cn

new Map(Object.entries(obj))
来源：http://vpo.jinqigufen.top

[U112] JS：字符串补位
来源：http://zxm.redwolf501.top

"7".padStart(3, "0")
来源：http://nql.cdnleiting.top

[U113] JS：正则替换全部
来源：http://syw.feifeiyinyue.top

s.replaceAll("a", "b")
来源：http://ydt.9152youxi.cn

[U114] JS：JSON 深比较
来源：http://upd.sufxvd.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vbm.tian-w.cn

[U115] JS：生成 UUID
来源：http://mfy.havefunace.top

crypto.randomUUID()
来源：http://drt.shuidangran.top

[U116] JS：类型检查（JSDoc）
来源：http://igy.uphjek.com

/** @param {string} name */ function f(name) {}
来源：http://wxd.0kj1m.cn

[U117] JS：单元测试
来源：http://img.feifeiyinyue.top

npm i -D vitest;  npx vitest
来源：http://scy.wangdashe.top

[U118] JS：开发服务器
来源：http://fca.xziqi.cn

npm i -D vite;  npx vite
来源：http://trb.gaohongyu789.top

[U119] JS：生产构建
来源：http://kgw.zhijiandao.cn

npx vite build
来源：http://ffu.zhijiandao.cn

[U120] JS：读取环境变量（Vite）
来源：http://kuc.0kj1m.cn

import.meta.env.VITE_API_URL
来源：http://gqa.zhaomingkeji.xyz

================================================================================
来源：http://zhr.hywenlv.cn

统计汇总
来源：http://kxs.guowangkeji.top

================================================================================
来源：http://ace.ppjwa.cn

按语言统计（条）：
来源：http://tck.jinqigfzy.top

Python ......... 252
来源：http://mxn.jinqigfzy.top

PHP ............ 252
来源：http://kvg.hesvh.cn

JavaScript ..... 252
来源：http://jou.cheryme.top

TypeScript ..... 212
来源：http://kdq.jinghuilouyu.cn

Java ........... 212
来源：http://cut.zhongyouzk.top

Go ............. 212
来源：http://gqq.quarkkingdee.top

Ruby ........... 212
来源：http://orw.yj20258.top

C# ............. 212
来源：http://pjd.zhongyouzk.top

C .............. 30
来源：http://qki.shanyushiyangtech.top

C++ ............ 30
来源：http://ldm.xingfuxueyuan.xyz

SQL ............ 90
来源：http://soe.daxiang520.top

Bash ........... 80
来源：http://tga.yfazqb.com

Kotlin ......... 15
来源：http://obo.zhaomingkeji.xyz

Swift .......... 15
来源：http://uiv.sweek.top

Lua ............ 10
来源：http://pma.yj20258888.top

Perl ........... 10
来源：http://ovu.svipenyu.cn

Scala .......... 10
来源：http://ref.haohaochexian.top

------------------------------------
来源：http://ohw.shuidangran.top

合计 ........... 2106 条
来源：http://dzv.andypj.xyz

按章节统计：
来源：http://awo.xingfuxueyuan.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rwq.aibaodan.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tdc.ctjpmb.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://orv.zhaomingkeji.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://div.jinghuilouyu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cet.zhengqikj.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zve.zhoulong.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rog.hywenlv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sso.zhoulong.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://eaf.ybcxt.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://asf.zhengqikj.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pjz.meibo888.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mdz.yueranfly.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hxk.fzhhl.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://akr.316326.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xxf.wangdashe.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kpj.daria6918.cn

Q SQL 专题                              90
来源：http://oef.yuxming.cn

R Bash 专题                             80
来源：http://cne.gogol.net.cn

S C / C++ 专题                          60
来源：http://jnc.hnxiangtu.top

T 其他语言补充                          60
来源：http://wxk.fktsv.cn

U 高频实用片段                         120
来源：http://jyn.yanxiufei.cn

------------------------------------
来源：http://rdz.haohaochexian.top

合计                                  2106 条
来源：http://apr.iojbl.cn

--------------------------------------------------------------------------------
来源：http://rmn.zhixingplan.top

使用提醒
来源：http://qmv.aizwys.cn

--------------------------------------------------------------------------------
来源：http://bdk.yj202588.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tvx.yfazqb.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pmc.nanxinkj.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://soz.xuetiantiany.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vbp.zhixingplan.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rpm.wangshuangyany.cn

—— 文件结束 ——
来源：http://bhl.gzhubu.top

================================================================================
来源：http://nna.yj202588.top

程序语言常见例子速查手册（2024 版）
来源：http://pir.zycfv.cn

Common Programming Examples Cheat Book
来源：http://wyv.sweek.top

================================================================================
来源：http://fwm.birdmap.top

【收录内容】
来源：http://lqw.snrcjt.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xtx.dashuyun.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vyo.xinyue.icu

SQL · Bash · C · C++
来源：http://kwn.yongpay.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://olz.xuetiantiany.cn

【使用说明】
来源：http://hvy.kuanghao11.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ulq.nanxuanxn.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://aoa.yfazqb.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rag.9152youxi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ueq.yuanzhike.top

Bash:  Shell         C:     C             C++:   C++
来源：http://eez.jyoumei.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lqj.smart0.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bnk.jinqigfzy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pcq.vqdsnc.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pvu.cashguo.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mbi.xinyue.icu

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bwz.shuidangran.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lvs.hysaishi.cn

【文件统计】
来源：http://qmx.dianchejie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://thr.hcnkem.com

--------------------------------------------------------------------------------
来源：http://vat.sjlbkw.cn

目  录
来源：http://ckz.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://gnd.tianlin.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fea.aizwys.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://glg.yueranfly.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fjj.jyoumei.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://acj.fengsongda.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wze.meibo888.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hnz.hammf.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gzo.yangfankeji.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://foa.zdqjudy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jod.jlsjyb.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ctb.yongpay.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://imc.fengsongda.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://twv.zhixingplan.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cea.yuanzhike.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tbv.jinyuanbaomall.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://izw.vehdjk.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dkb.ybcxt.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://axh.sjlbkw.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ass.xuanzx.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hwp.meibo888.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://utg.pengpengdd.cyou

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wtd.ivvv.top

================================================================================
来源：http://aqf.haohaochexian.top

A. 基础语法与类型
来源：http://pot.snrcjt.cn

================================================================================
来源：http://fpr.daxiang520.top

[A01] Hello World
来源：http://nit.ppjwa.cn

Py:   print("Hello, World!")
来源：http://csg.ivvv.top

PHP:  echo "Hello, World!";
来源：http://zll.feifeiyinyue.top

JS:   console.log("Hello, World!");
来源：http://len.wangshuangyany.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://whc.chenjidiqi.icu

Java: System.out.println("Hello, World!");
来源：http://zti.hcnkem.com

Go:   fmt.Println("Hello, World!")
来源：http://cko.aizwys.cn

Ruby: puts "Hello, World!"
来源：http://drw.xuanzx.com

C#:   Console.WriteLine("Hello, World!");
来源：http://bka.chenjidiqi.icu

[A02] 变量声明与赋值
来源：http://uww.hesvh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uls.hnqzz.top

PHP:  $name = "Alex"; $age = 20;
来源：http://fvj.hnqzz.top

JS:   let name = "Alex"; const age = 20;
来源：http://udv.hysaishi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tiz.vehdjk.com

Java: String name = "Alex"; int age = 20;
来源：http://prb.sxryk.cn

Go:   name := "Alex"; age := 20
来源：http://iby.cqqwz.cn

Ruby: name = "Alex"; age = 20
来源：http://fym.ybcxt.top

C#:   string name = "Alex"; int age = 20;
来源：http://lzg.jinghuilouyu.cn

[A03] 常量定义
来源：http://lrc.aibaodan.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://uea.jinghuilouyu.cn

PHP:  const PI = 3.14159;
来源：http://lds.sweek.top

JS:   const PI = 3.14159;
来源：http://yoe.svipenyu.cn

TS:   const PI: number = 3.14159;
来源：http://mzo.gzhubu.top

Java: static final double PI = 3.14159;
来源：http://trs.feifeiyinyue.top

Go:   const PI = 3.14159
来源：http://yuu.yonumen.top

Ruby: PI = 3.14159
来源：http://bss.xuetiantiany.cn

C#:   const double PI = 3.14159;
来源：http://qzi.hammf.cn

[A04] 判断变量类型
来源：http://ohu.fktsv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gse.andypj.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dvv.mhx1999.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ius.ywan-chungtsiang.top

TS:   typeof x; x instanceof Date
来源：http://xvq.yj20258888.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://owm.feifeiyinyue.top

Go:   reflect.TypeOf(x).Name()
来源：http://xhz.chenzaomai.com

Ruby: x.class; x.is_a?(Integer)
来源：http://tto.jinqigfzy.top

C#:   x.GetType().Name; x is int
来源：http://ywt.vehdjk.com

[A05] 整数除法与取模
来源：http://oui.sysykeji.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yxc.jlsjyb.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://bun.shuidangran.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cpz.mhx1999.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ngr.chenlongwang.top

Java: 7 / 2; 7 % 2
来源：http://oho.yj20258.top

Go:   7 / 2; 7 % 2
来源：http://goi.hywenlv.cn

Ruby: 7 / 2; 7 % 2
来源：http://zst.yj202588.top

C#:   7 / 2; 7 % 2
来源：http://dby.yueranfly.top

[A06] 字符串转数字
来源：http://aqs.yuanzhike.top

Py:   int("42"); float("3.14")
来源：http://por.tarul.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jei.zhaomingkeji.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://epa.9152youxi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ctw.bbcook.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hco.shangyingyoupin.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jcd.dianchejie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://tzi.fzhhl.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cjz.fanxiaobao.xyz

[A07] 数字转字符串
来源：http://qfi.nwbrower.top

Py:   str(42)
来源：http://thi.yj20258.top

PHP:  (string) 42; strval(42)
来源：http://fts.pengpengdd.cyou

JS:   String(42); (42).toString()
来源：http://dtr.birdmap.top

TS:   String(42)
来源：http://nub.nwbrower.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://kly.xylfe.cn

Go:   strconv.Itoa(42)
来源：http://huc.bbcook.cn

Ruby: 42.to_s
来源：http://kbo.shzxlz.cn

C#:   42.ToString()
来源：http://bud.epnwcf.com

[A08] 取整与四舍五入
来源：http://xjk.daxiang520.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://usc.shanyushiyangtech.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gqg.hongshengwenyu.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://afr.fktsv.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://neb.fktsv.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://orq.sysykeji.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rpo.chenjidiqi.icu

Ruby: 3.567.round(2); 3.9.floor
来源：http://gbr.shzxlz.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zjj.yuxming.cn

[A09] 绝对值与最大最小值
来源：http://kjh.zhixingplan.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xif.tianlin.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pmm.cheryme.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lom.0kj1m.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vcp.mhx1999.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qfa.tian-w.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hbs.c1oappe.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jem.zdbjq.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fdc.chenzaomai.com

[A10] 生成随机数
来源：http://nax.hnxiangtu.top

Py:   import random; random.randint(1, 100)
来源：http://ugy.bjfxy.top

PHP:  random_int(1, 100);
来源：http://rdm.hnqzz.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kox.snrcjt.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qec.jiagoushi.top

Java: new Random().nextInt(100) + 1
来源：http://ucx.cucudq.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ttq.tarul.cn

Ruby: rand(1..100)
来源：http://rmz.xinyue.icu

C#:   new Random().Next(1, 101)
来源：http://dnc.iojbl.cn

[A11] 条件表达式（三元）
来源：http://rap.haohaochexian.top

Py:   "yes" if x > 0 else "no"
来源：http://big.ywan-chungtsiang.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://aqw.gogol.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qpa.jyoumei.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hnn.shuidangran.top

Java: x > 0 ? "yes" : "no"
来源：http://oic.birdmap.top

Go:   // 无三元运算符，需用 if 语句
来源：http://mqx.mhx1999.top

Ruby: x > 0 ? "yes" : "no"
来源：http://eiw.yueranfly.top

C#:   x > 0 ? "yes" : "no"
来源：http://hbo.gzhubu.top

[A12] 字符串插值 / 格式化
来源：http://tua.gaohongyu789.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qan.shzxlz.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ahu.ctjpmb.com

JS:   `Hello, ${name}!`
来源：http://kzg.yuxming.cn

TS:   `Hello, ${name}!`
来源：http://zrl.xuetiantiany.cn

Java: "Hello, %s!".formatted(name)
来源：http://ttn.yongpay.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ido.tarul.cn

Ruby: "Hello, #{name}!"
来源：http://tiu.daxiang520.top

C#:   $"Hello, {name}!"
来源：http://dsb.daxiang520.top

[A13] 多行字符串（练习 \n 转义）
来源：http://xsx.ybcxt.top

Py:   "第一行\n第二行"
来源：http://naf.jinghuilouyu.cn

PHP:  "第一行\n第二行"
来源：http://dcw.hongshengwenyu.top

JS:   "第一行\n第二行"
来源：http://egj.guannengcc.top

TS:   "第一行\n第二行"
来源：http://nrg.fengsongda.top

Java: "第一行\n第二行"
来源：http://zgt.c1oappe.top

Go:   "第一行\n第二行"
来源：http://kds.pengpengdd.cyou

Ruby: "第一行\n第二行"
来源：http://upn.xziqi.cn

C#:   "第一行\n第二行"
来源：http://wmm.kuanghao11.cn

[A14] 注释写法
来源：http://rgg.dashuyun.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://hnp.cqqwz.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://waz.meibo888.top

JS:   // 单行；/* 多行 */
来源：http://vbo.dianchejie.cn

TS:   // 单行；/* 多行 */
来源：http://cuo.nanxuanxn.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xcu.vehdjk.com

Go:   // 单行；/* 多行 */
来源：http://khp.zhaomingkeji.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://vgb.ydzc1.top

C#:   // 单行；/* 多行 */
来源：http://xwu.shanyushiyangtech.top

[A15] 空值判断与默认值
来源：http://bwh.cdnleiting.top

Py:   value = data or "默认值"
来源：http://gvc.shzxlz.cn

PHP:  $value = $data ?? "默认值";
来源：http://tkk.hammf.cn

JS:   const value = data ?? "默认值";
来源：http://pho.pycfn.com

TS:   const value = data ?? "默认值";
来源：http://bin.jinyuanbaomall.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hkj.yuxming.cn

Go:   if data == "" { data = "默认值" }
来源：http://odh.birdmap.top

Ruby: value = data || "默认值"
来源：http://ers.pengpengdd.cyou

C#:   var value = data ?? "默认值";
来源：http://rpx.sysykeji.top

[A16] 真假值判断规则
来源：http://nfg.zdqjudy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://des.tian-w.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wck.yonumen.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gov.zhongyouzk.top

TS:   if (!x) {}
来源：http://vab.vqdsnc.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qhc.sufxvd.cn


<!-- 参考信息 -->