代发 wailian999

[U89] JS：数组去重
来源：http://qta.andypj.xyz

[...new Set(arr)]
来源：http://tyz.yuanzhike.top

[U90] JS：数字数组排序
来源：http://ehd.snrcjt.cn

[...arr].sort((a, b) => a - b)
来源：http://rfc.vqdsnc.cn

[U91] JS：对象键值遍历
来源：http://rmp.tianlin.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zst.chenlongwang.top

[U92] JS：深拷贝
来源：http://otr.xuetiantiany.cn

structuredClone(obj)
来源：http://cag.cucudq.cn

[U93] JS：模板字符串
来源：http://abb.gaohongyu789.top

`共 ${n} 条`
来源：http://ubc.hongshengwenyu.top

[U94] JS：箭头函数
来源：http://and.vehdjk.com

const double = x => x * 2;
来源：http://kge.9152youxi.cn

[U95] JS：Promise 包装
来源：http://vjq.cqqwz.cn

new Promise((resolve, reject) => {})
来源：http://qap.meibo888.top

[U96] JS：async/await 与异常
来源：http://ayo.xylfe.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cgc.zdbjq.cn

[U97] JS：并发请求
来源：http://ljx.aibaodan.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dse.tanke756.top

[U98] JS：fetch 带 JSON
来源：http://wdp.sysykeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ylz.xingfuxueyuan.xyz

[U99] JS：事件监听
来源：http://gut.guannengcc.top

el.addEventListener("click", e => {})
来源：http://bwu.fengsongda.top

[U100] JS：DOM 查询
来源：http://rdf.yongpay.top

document.querySelector(".item")
来源：http://kqs.chenjidiqi.icu

[U101] JS：classList 操作
来源：http://jgc.cheryme.top

el.classList.toggle("active")
来源：http://fkl.9152youxi.cn

[U102] JS：本地存储
来源：http://uah.yuanzhike.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://euq.birdmap.top

[U103] JS：定时器
来源：http://uoj.hfpthk.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fnk.tian-w.cn

[U104] JS：防抖
来源：http://ooh.daria6918.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oqq.cucudq.cn

[U105] JS：节流
来源：http://ebk.9152youxi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mgq.tian-w.cn

[U106] JS：日期格式化
来源：http://byj.hongshengwenyu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pcx.nanxuanxn.top

[U107] JS：数字千分位
来源：http://yxd.zhoulong.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gkl.yj20258.top

[U108] JS：随机整数
来源：http://iga.xinyue.icu

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gom.zhengqikj.top

[U109] JS：数组分组
来源：http://ygv.yj20258888.top

Object.groupBy(arr, x => x.type)
来源：http://whp.jianghu66.top

[U110] JS：数组分块
来源：http://xob.fengsongda.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qml.smart0.xyz

[U111] JS：对象转 Map
来源：http://nuj.shangyingyoupin.top

new Map(Object.entries(obj))
来源：http://ydb.dashuyun.cn

[U112] JS：字符串补位
来源：http://nkw.zhijiandao.cn

"7".padStart(3, "0")
来源：http://emg.cucudq.cn

[U113] JS：正则替换全部
来源：http://yms.xuanzx.com

s.replaceAll("a", "b")
来源：http://goj.jlsjyb.cn

[U114] JS：JSON 深比较
来源：http://cib.yueranfly.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hsc.hcnkem.com

[U115] JS：生成 UUID
来源：http://vui.yonumen.top

crypto.randomUUID()
来源：http://eag.cheryme.top

[U116] JS：类型检查（JSDoc）
来源：http://lxe.daria6918.cn

/** @param {string} name */ function f(name) {}
来源：http://jkz.jianghu66.top

[U117] JS：单元测试
来源：http://rrg.jyoumei.cn

npm i -D vitest;  npx vitest
来源：http://rpf.ydzc1.top

[U118] JS：开发服务器
来源：http://vgj.bjfxy.top

npm i -D vite;  npx vite
来源：http://dun.wangshuangyany.cn

[U119] JS：生产构建
来源：http://gtd.jinghuilouyu.cn

npx vite build
来源：http://axs.tarul.cn

[U120] JS：读取环境变量（Vite）
来源：http://onv.svipenyu.cn

import.meta.env.VITE_API_URL
来源：http://xld.jinyuanbaomall.cn

================================================================================
来源：http://joq.tian-w.cn

统计汇总
来源：http://agt.yuxming.cn

================================================================================
来源：http://atv.zhijiandao.cn

按语言统计（条）：
来源：http://obx.jqgfzy.top

Python ......... 252
来源：http://hrw.ppjwa.cn

PHP ............ 252
来源：http://wex.haohaochexian.top

JavaScript ..... 252
来源：http://uql.pengpengdd.cyou

TypeScript ..... 212
来源：http://oor.snrcjt.cn

Java ........... 212
来源：http://ukb.yuxming.cn

Go ............. 212
来源：http://aal.fengsongda.top

Ruby ........... 212
来源：http://ezw.ybcxt.top

C# ............. 212
来源：http://hpl.xylfe.cn

C .............. 30
来源：http://tkh.pengpengdd.cyou

C++ ............ 30
来源：http://yyz.yuanzhike.top

SQL ............ 90
来源：http://hrk.zhiwuduotai.top

Bash ........... 80
来源：http://laa.yj202588.top

Kotlin ......... 15
来源：http://efe.yanxiufei.cn

Swift .......... 15
来源：http://aah.ybcxt.top

Lua ............ 10
来源：http://qzl.yj202588.top

Perl ........... 10
来源：http://wlw.hcnkem.com

Scala .......... 10
来源：http://rdm.sufxvd.cn

------------------------------------
来源：http://omu.pycfn.com

合计 ........... 2106 条
来源：http://hvx.jinyuanbaomall.cn

按章节统计：
来源：http://fte.ybcxt.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://atw.zdbjq.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://llk.daria6918.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rsq.chenjidiqi.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://axe.jinqigufen.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gql.ivvv.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://roo.feifeiyinyue.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tdp.dianchejie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wca.meibo888.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jyg.ywan-chungtsiang.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://moq.xuanzx.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vpc.meibo888.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://prn.daria6918.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://daq.cucudq.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fxo.gzhubu.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://spw.jinqigfzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lez.xingfuxueyuan.xyz

Q SQL 专题                              90
来源：http://usj.shuidangran.top

R Bash 专题                             80
来源：http://zmo.aibaodan.cn

S C / C++ 专题                          60
来源：http://biv.sjlbkw.cn

T 其他语言补充                          60
来源：http://njl.cucudq.cn

U 高频实用片段                         120
来源：http://bzn.redwolf501.top

------------------------------------
来源：http://tue.chenzaomai.com

合计                                  2106 条
来源：http://pyf.yuxming.cn

--------------------------------------------------------------------------------
来源：http://scw.gzhubu.top

使用提醒
来源：http://irs.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://gvc.guannengcc.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tbl.ybcxt.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lsh.jianghu66.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pzp.tarul.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fox.hywenlv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dzp.yj20258.top

—— 文件结束 ——
来源：http://cns.gaohongyu789.top

================================================================================
来源：http://pmp.wangdashe.top

程序语言常见例子速查手册（2024 版）
来源：http://lmv.chenjidiqi.icu

Common Programming Examples Cheat Book
来源：http://vlk.xinyue.icu

================================================================================
来源：http://gkj.sxryk.cn

【收录内容】
来源：http://maa.quarkkingdee.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://wcb.vqdsnc.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://see.gaohongyu789.top

SQL · Bash · C · C++
来源：http://nmu.jianghu66.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jdd.jqgufenzy.top

【使用说明】
来源：http://axd.hysaishi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qrg.epnwcf.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wyz.dashuyun.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zde.xylfe.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ukj.vqdsnc.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cjw.sweek.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jdz.hesvh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ekz.ppjwa.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jbe.shanyushiyangtech.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://aph.haohaochexian.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fmx.haohaochexian.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://foi.bjfxy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xgv.aizwys.cn

【文件统计】
来源：http://fzp.bbcook.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lgu.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://kny.jlsjyb.cn

目  录
来源：http://vrt.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://smh.uphjek.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jmw.jinghuilouyu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cxg.guowangkeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xki.zdbjq.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jda.yuxming.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ndt.hywenlv.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://weq.jianghu66.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bnl.fengsongda.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rfg.jianghu66.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vsh.hnxiangtu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gvv.cucudq.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mld.xylfe.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://khe.feifeiyinyue.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hfk.gzhubu.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://oek.gogol.net.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xvr.xuanzx.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gsm.ywan-chungtsiang.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hei.gzhubu.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://rgq.zdbjq.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://buy.nanxinkj.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://web.cashguo.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yot.kuanghao11.cn

================================================================================
来源：http://rhn.hammf.cn

A. 基础语法与类型
来源：http://kyy.ivvv.top

================================================================================
来源：http://rqe.yj20258888.top

[A01] Hello World
来源：http://tbg.aibaodan.cn

Py:   print("Hello, World!")
来源：http://lyf.jinqigufen.top

PHP:  echo "Hello, World!";
来源：http://nun.zhoulong.xyz

JS:   console.log("Hello, World!");
来源：http://hsg.yfazqb.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gyk.fzhhl.top

Java: System.out.println("Hello, World!");
来源：http://nrs.c1oappe.top

Go:   fmt.Println("Hello, World!")
来源：http://orx.ybcxt.top

Ruby: puts "Hello, World!"
来源：http://uhf.shanyushiyangkeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://icu.jqgfzy.top

[A02] 变量声明与赋值
来源：http://nft.guannengcc.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hlt.shanyushiyangkeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://emg.xziqi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hmo.jlsjyb.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://aak.epnwcf.com

Java: String name = "Alex"; int age = 20;
来源：http://tyh.redwolf501.top

Go:   name := "Alex"; age := 20
来源：http://wym.zycfv.cn

Ruby: name = "Alex"; age = 20
来源：http://qpy.chenzaomai.com

C#:   string name = "Alex"; int age = 20;
来源：http://pui.sufxvd.cn

[A03] 常量定义
来源：http://fcu.316326.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://moi.hywenlv.cn

PHP:  const PI = 3.14159;
来源：http://oys.shuidangran.top

JS:   const PI = 3.14159;
来源：http://vef.yanxiufei.cn

TS:   const PI: number = 3.14159;
来源：http://ddo.sjlbkw.cn

Java: static final double PI = 3.14159;
来源：http://sqz.hywenlv.cn

Go:   const PI = 3.14159
来源：http://hhh.quarkkingdee.top

Ruby: PI = 3.14159
来源：http://ckx.vqdsnc.cn

C#:   const double PI = 3.14159;
来源：http://ucr.havefunace.top

[A04] 判断变量类型
来源：http://wsc.0kj1m.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xut.jinghuilouyu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://znq.iojbl.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ptz.tian-w.cn

TS:   typeof x; x instanceof Date
来源：http://kjw.nanxuanxn.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nqx.uphjek.com

Go:   reflect.TypeOf(x).Name()
来源：http://cbi.fengsongda.top

Ruby: x.class; x.is_a?(Integer)
来源：http://hbb.yj20258888.top

C#:   x.GetType().Name; x is int
来源：http://qpz.jinyuanbaomall.cn

[A05] 整数除法与取模
来源：http://nzt.sysykeji.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mwv.xinyue.icu

PHP:  intdiv(7, 2); 7 % 2
来源：http://psf.tarul.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xsg.yj202588.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tia.fanxiaobao.xyz

Java: 7 / 2; 7 % 2
来源：http://dij.yj20258.top

Go:   7 / 2; 7 % 2
来源：http://pya.yueranfly.top

Ruby: 7 / 2; 7 % 2
来源：http://sxo.zhoulong.xyz

C#:   7 / 2; 7 % 2
来源：http://kms.hysaishi.cn

[A06] 字符串转数字
来源：http://syh.cheryme.top

Py:   int("42"); float("3.14")
来源：http://cqs.pycfn.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qoe.chenzaomai.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lwq.meibo888.top

TS:   parseInt("42", 10); Number("42")
来源：http://zxh.cashguo.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bbn.316326.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://apc.epnwcf.com

Ruby: "42".to_i; "3.14".to_f
来源：http://nvy.jiagoushi.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nsh.tanke756.top

[A07] 数字转字符串
来源：http://uvm.xylfe.cn

Py:   str(42)
来源：http://air.yj202588.top

PHP:  (string) 42; strval(42)
来源：http://glt.jinqigufen.top

JS:   String(42); (42).toString()
来源：http://umh.cashguo.top

TS:   String(42)
来源：http://jty.0kj1m.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://lkb.yangfankeji.com

Go:   strconv.Itoa(42)
来源：http://kbg.sjlbkw.cn

Ruby: 42.to_s
来源：http://gub.quarkkingdee.top

C#:   42.ToString()
来源：http://xji.sweek.top

[A08] 取整与四舍五入
来源：http://nsa.ivvv.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://eiz.mhx1999.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qpd.shanyushiyangkeji.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vec.snrcjt.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rod.yj20258.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yvi.pycfn.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cnj.yueranfly.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://bfu.hfpthk.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sla.shzxlz.cn

[A09] 绝对值与最大最小值
来源：http://twc.yueranfly.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mor.zhijiandao.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pap.andypj.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gie.zycfv.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hkd.tianlin.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://txu.jinqigfzy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://eah.ivvv.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pse.chenjidiqi.icu

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qyg.yanxiufei.cn

[A10] 生成随机数
来源：http://zof.guowangkeji.top

Py:   import random; random.randint(1, 100)
来源：http://fbk.xuanzx.com

PHP:  random_int(1, 100);
来源：http://mtl.xylfe.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zah.jqgfzy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dps.zhijiandao.cn

Java: new Random().nextInt(100) + 1
来源：http://iwq.xuetiantiany.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cnj.zhongyouzk.top

Ruby: rand(1..100)
来源：http://yji.zhongyouzk.top

C#:   new Random().Next(1, 101)
来源：http://qxn.dianchejie.cn

[A11] 条件表达式（三元）
来源：http://ufy.tian-w.cn

Py:   "yes" if x > 0 else "no"
来源：http://tay.ivvv.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://nyi.ydjk.org.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xtn.yfazqb.com

TS:   x > 0 ? "yes" : "no"
来源：http://yxg.yuanzhike.top

Java: x > 0 ? "yes" : "no"
来源：http://zhi.zhiwuduotai.top

Go:   // 无三元运算符，需用 if 语句
来源：http://poz.haohaochexian.top

Ruby: x > 0 ? "yes" : "no"
来源：http://xks.zycfv.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fjd.zdqjudy.top

[A12] 字符串插值 / 格式化
来源：http://dfk.fehbvm.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://csb.jqgufenzy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fpu.ydzc1.top

JS:   `Hello, ${name}!`
来源：http://roa.birdmap.top

TS:   `Hello, ${name}!`
来源：http://cfr.xingfuxueyuan.xyz

Java: "Hello, %s!".formatted(name)
来源：http://fjp.xylfe.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://loz.yanxiufei.cn

Ruby: "Hello, #{name}!"
来源：http://coc.xinyue.icu

C#:   $"Hello, {name}!"
来源：http://smv.pengpengdd.cyou

[A13] 多行字符串（练习 \n 转义）
来源：http://uin.yanxiufei.cn

Py:   "第一行\n第二行"
来源：http://ykx.sjlbkw.cn

PHP:  "第一行\n第二行"
来源：http://egm.jlsjyb.cn

JS:   "第一行\n第二行"
来源：http://goa.shanyushiyangtech.top

TS:   "第一行\n第二行"
来源：http://zbr.snrcjt.cn

Java: "第一行\n第二行"
来源：http://swe.chenlongwang.top

Go:   "第一行\n第二行"
来源：http://mxq.jinqigfzy.top

Ruby: "第一行\n第二行"
来源：http://act.hongshengwenyu.top

C#:   "第一行\n第二行"
来源：http://zqt.hcnkem.com

[A14] 注释写法
来源：http://ynr.birdmap.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://hca.sysykeji.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://jov.bbcook.cn

JS:   // 单行；/* 多行 */
来源：http://vps.ydzc1.top

TS:   // 单行；/* 多行 */
来源：http://ait.hfpthk.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://feq.yj20258.top

Go:   // 单行；/* 多行 */
来源：http://ppx.shuidangran.top

Ruby: # 单行；=begin 多行 =end
来源：http://bep.ivvv.top

C#:   // 单行；/* 多行 */
来源：http://hkm.iojbl.cn

[A15] 空值判断与默认值
来源：http://ede.jqgfzy.top

Py:   value = data or "默认值"
来源：http://hog.xingfuxueyuan.xyz

PHP:  $value = $data ?? "默认值";
来源：http://qzz.jqgfzy.top


<!-- 参考信息 -->