代发 wailian999

[U91] JS：对象键值遍历
来源：http://lzf.316326.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://avv.gotoacloud.top

[U92] JS：深拷贝
来源：http://rdv.aibaodan.cn

structuredClone(obj)
来源：http://kyt.zdbjq.cn

[U93] JS：模板字符串
来源：http://bzh.andypj.xyz

`共 ${n} 条`
来源：http://ghy.zhijiandao.cn

[U94] JS：箭头函数
来源：http://rcj.nanxinkj.top

const double = x => x * 2;
来源：http://sjg.xuetiantiany.cn

[U95] JS：Promise 包装
来源：http://emo.ivvv.top

new Promise((resolve, reject) => {})
来源：http://hnn.yj20258888.top

[U96] JS：async/await 与异常
来源：http://zni.yuxming.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dmx.jyoumei.cn

[U97] JS：并发请求
来源：http://gfk.shangyingyoupin.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://mhc.smart0.xyz

[U98] JS：fetch 带 JSON
来源：http://jwz.zhaomingkeji.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uqe.daria6918.cn

[U99] JS：事件监听
来源：http://bcq.ybcxt.top

el.addEventListener("click", e => {})
来源：http://zbq.gaohongyu789.top

[U100] JS：DOM 查询
来源：http://vsg.gzhubu.top

document.querySelector(".item")
来源：http://zos.cqqwz.cn

[U101] JS：classList 操作
来源：http://trw.jyoumei.cn

el.classList.toggle("active")
来源：http://wut.yonumen.top

[U102] JS：本地存储
来源：http://vqi.chenlongwang.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xcl.ydjk.org.cn

[U103] JS：定时器
来源：http://qdt.yanxiufei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fup.jianghu66.top

[U104] JS：防抖
来源：http://mio.tianlin.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hsq.ppjwa.cn

[U105] JS：节流
来源：http://tze.uphjek.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://whl.jyoumei.cn

[U106] JS：日期格式化
来源：http://urj.xuanzx.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ugb.iojbl.cn

[U107] JS：数字千分位
来源：http://xuq.aizwys.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hmv.yangfankeji.com

[U108] JS：随机整数
来源：http://kay.bbcook.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wxc.sweek.top

[U109] JS：数组分组
来源：http://bre.yongpay.top

Object.groupBy(arr, x => x.type)
来源：http://lfm.shanyushiyangtech.top

[U110] JS：数组分块
来源：http://ytd.cheryme.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://prt.sufxvd.cn

[U111] JS：对象转 Map
来源：http://mpp.feifeiyinyue.top

new Map(Object.entries(obj))
来源：http://lka.quarkkingdee.top

[U112] JS：字符串补位
来源：http://ezf.chenzaomai.com

"7".padStart(3, "0")
来源：http://kdv.nanxuanxn.top

[U113] JS：正则替换全部
来源：http://ngs.fktsv.cn

s.replaceAll("a", "b")
来源：http://srz.zhongyouzk.top

[U114] JS：JSON 深比较
来源：http://dle.jqgufenzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://cxi.yvedp.cn

[U115] JS：生成 UUID
来源：http://ima.0kj1m.cn

crypto.randomUUID()
来源：http://eyd.zhongyouzk.top

[U116] JS：类型检查（JSDoc）
来源：http://hwi.mhx1999.top

/** @param {string} name */ function f(name) {}
来源：http://dcb.hongshengwenyu.top

[U117] JS：单元测试
来源：http://kbz.nanxuanxn.top

npm i -D vitest;  npx vitest
来源：http://wyw.ehwqpu.com

[U118] JS：开发服务器
来源：http://mud.meibo888.top

npm i -D vite;  npx vite
来源：http://iyc.epnwcf.com

[U119] JS：生产构建
来源：http://pdh.smart0.xyz

npx vite build
来源：http://fit.zdbjq.cn

[U120] JS：读取环境变量（Vite）
来源：http://cqa.kuanghao11.cn

import.meta.env.VITE_API_URL
来源：http://fwn.ehwqpu.com

================================================================================
来源：http://lav.pycfn.com

统计汇总
来源：http://dxl.hnxiangtu.top

================================================================================
来源：http://tvo.gaohongyu789.top

按语言统计（条）：
来源：http://fbk.shzxlz.cn

Python ......... 252
来源：http://zpi.xylfe.cn

PHP ............ 252
来源：http://bvr.hongshengwenyu.top

JavaScript ..... 252
来源：http://nxc.vehdjk.com

TypeScript ..... 212
来源：http://nvz.iojbl.cn

Java ........... 212
来源：http://xib.zdqjudy.top

Go ............. 212
来源：http://kxz.svipenyu.cn

Ruby ........... 212
来源：http://oxl.svipenyu.cn

C# ............. 212
来源：http://smh.epnwcf.com

C .............. 30
来源：http://unb.yfazqb.com

C++ ............ 30
来源：http://dee.cdnleiting.top

SQL ............ 90
来源：http://sna.haohaochexian.top

Bash ........... 80
来源：http://anf.hnxiangtu.top

Kotlin ......... 15
来源：http://enm.epnwcf.com

Swift .......... 15
来源：http://zfz.chenjidiqi.icu

Lua ............ 10
来源：http://sza.shzxlz.cn

Perl ........... 10
来源：http://gll.hfpthk.cn

Scala .......... 10
来源：http://lqj.sxryk.cn

------------------------------------
来源：http://gog.fehbvm.com

合计 ........... 2106 条
来源：http://jqz.yj202588.top

按章节统计：
来源：http://rsx.daxiang520.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://aye.ybcxt.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jed.quarkkingdee.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vjh.yj202588.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gpx.redwolf501.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mku.yueranfly.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vmn.iojbl.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wxc.yvedp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gba.aibaodan.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yaw.zdbjq.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bpj.yj20258.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yvy.sjlbkw.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ekk.sxryk.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zko.nanxinkj.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://otv.xingfuxueyuan.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://byd.epnwcf.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dyd.gogol.net.cn

Q SQL 专题                              90
来源：http://eqm.fzhhl.top

R Bash 专题                             80
来源：http://ldz.uphjek.com

S C / C++ 专题                          60
来源：http://wdt.hywenlv.cn

T 其他语言补充                          60
来源：http://ato.ydzc1.top

U 高频实用片段                         120
来源：http://xii.chenlongwang.top

------------------------------------
来源：http://dcy.yanxiufei.cn

合计                                  2106 条
来源：http://fbw.cashguo.top

--------------------------------------------------------------------------------
来源：http://lwq.xuetiantiany.cn

使用提醒
来源：http://jxh.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://rvx.hammf.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kzo.zhengqikj.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sge.zhiwuduotai.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://drc.vehdjk.com

在旧版本上使用前请先确认语法支持情况。
来源：http://udw.zdqjudy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wyv.shuidangran.top

—— 文件结束 ——
来源：http://uuv.fehbvm.com

================================================================================
来源：http://lwz.xingfuxueyuan.xyz

程序语言常见例子速查手册（2024 版）
来源：http://dou.9152youxi.cn

Common Programming Examples Cheat Book
来源：http://hib.shzxlz.cn

================================================================================
来源：http://pxz.cqqwz.cn

【收录内容】
来源：http://oaw.cucudq.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ous.xylfe.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sbr.yanxiufei.cn

SQL · Bash · C · C++
来源：http://zmy.birdmap.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hoi.sjlbkw.cn

【使用说明】
来源：http://nax.hcnkem.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nvb.cqqwz.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://olw.cheryme.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://msp.mhx1999.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dxc.zdbjq.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hpm.yangfankeji.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xwu.hywenlv.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://niy.smart0.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xhr.snrcjt.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nnl.yanxiufei.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kmc.xylfe.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://flq.havefunace.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vdn.tanke756.top

【文件统计】
来源：http://xmb.chenzaomai.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://olk.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://ouk.dashuyun.cn

目  录
来源：http://ynu.316326.xyz

--------------------------------------------------------------------------------
来源：http://vvm.jinghuilouyu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dhx.sweek.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ixt.xingfuxueyuan.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nzx.vehdjk.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wzh.birdmap.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://iqr.mhx1999.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://krt.gzhubu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pik.aibaodan.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yns.ppjwa.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ycf.iojbl.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://drn.aizwys.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wmv.yvedp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://eir.xuetiantiany.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lds.chenlongwang.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pif.xylfe.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fud.cdnleiting.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jry.shanyushiyangtech.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dmm.bbcook.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gyg.zhoulong.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mby.redwolf501.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://amf.redwolf501.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dox.wangdashe.top

================================================================================
来源：http://brq.chenlongwang.top

A. 基础语法与类型
来源：http://hwf.hnqzz.top

================================================================================
来源：http://qmj.redwolf501.top

[A01] Hello World
来源：http://cki.hfpthk.cn

Py:   print("Hello, World!")
来源：http://sbl.zdqjudy.top

PHP:  echo "Hello, World!";
来源：http://wak.yuxming.cn

JS:   console.log("Hello, World!");
来源：http://jxx.tianlin.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dza.jqgfzy.top

Java: System.out.println("Hello, World!");
来源：http://dvf.jinyuanbaomall.cn

Go:   fmt.Println("Hello, World!")
来源：http://itz.cucudq.cn

Ruby: puts "Hello, World!"
来源：http://jxm.c1oappe.top

C#:   Console.WriteLine("Hello, World!");
来源：http://vuo.kuanghao11.cn

[A02] 变量声明与赋值
来源：http://wzu.aizwys.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jgp.gogol.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://akn.pycfn.com

JS:   let name = "Alex"; const age = 20;
来源：http://zrv.nwbrower.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://acu.shanyushiyangtech.top

Java: String name = "Alex"; int age = 20;
来源：http://rat.cashguo.top

Go:   name := "Alex"; age := 20
来源：http://moj.dianchejie.cn

Ruby: name = "Alex"; age = 20
来源：http://itq.jinqigfzy.top

C#:   string name = "Alex"; int age = 20;
来源：http://mwn.shangyingyoupin.top

[A03] 常量定义
来源：http://lll.yanxiufei.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xln.fzhhl.top

PHP:  const PI = 3.14159;
来源：http://qhz.ctjpmb.com

JS:   const PI = 3.14159;
来源：http://tvh.jianghu66.top

TS:   const PI: number = 3.14159;
来源：http://vyn.guowangkeji.top

Java: static final double PI = 3.14159;
来源：http://bog.zhoulong.xyz

Go:   const PI = 3.14159
来源：http://dai.tian-w.cn

Ruby: PI = 3.14159
来源：http://bsw.jqgfzy.top

C#:   const double PI = 3.14159;
来源：http://wdl.ydzc1.top

[A04] 判断变量类型
来源：http://wmk.guannengcc.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://zfr.cashguo.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nku.yueranfly.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://aes.nwbrower.top

TS:   typeof x; x instanceof Date
来源：http://ghq.dashuyun.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tay.feifeiyinyue.top

Go:   reflect.TypeOf(x).Name()
来源：http://phe.tian-w.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://zde.ydjk.org.cn

C#:   x.GetType().Name; x is int
来源：http://mco.wangdashe.top

[A05] 整数除法与取模
来源：http://nhp.xingfuxueyuan.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hrs.zhoulong.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://yii.zhijiandao.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rgv.sjlbkw.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nhr.hcnkem.com

Java: 7 / 2; 7 % 2
来源：http://qvq.mhx1999.top

Go:   7 / 2; 7 % 2
来源：http://mco.xziqi.cn

Ruby: 7 / 2; 7 % 2
来源：http://lrb.tarul.cn

C#:   7 / 2; 7 % 2
来源：http://tdg.zhengqikj.top

[A06] 字符串转数字
来源：http://atu.chenzaomai.com

Py:   int("42"); float("3.14")
来源：http://leb.zhongyouzk.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jds.hnqzz.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bhm.jianghu66.top

TS:   parseInt("42", 10); Number("42")
来源：http://jwv.feifeiyinyue.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ytm.gzhubu.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pcn.chenzaomai.com

Ruby: "42".to_i; "3.14".to_f
来源：http://qaj.xuetiantiany.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://igk.hammf.cn

[A07] 数字转字符串
来源：http://nxi.xinyue.icu

Py:   str(42)
来源：http://sep.316326.xyz

PHP:  (string) 42; strval(42)
来源：http://hna.ehwqpu.com

JS:   String(42); (42).toString()
来源：http://noa.fanxiaobao.xyz

TS:   String(42)
来源：http://xbu.bbcook.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zte.uphjek.com

Go:   strconv.Itoa(42)
来源：http://cqe.mhx1999.top

Ruby: 42.to_s
来源：http://mls.dianchejie.cn

C#:   42.ToString()
来源：http://fxj.haohaochexian.top

[A08] 取整与四舍五入
来源：http://oea.gaohongyu789.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sjg.jinyuanbaomall.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mbi.mhx1999.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rpe.zhaomingkeji.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://abz.gotoacloud.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cme.cqqwz.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://oih.cdnleiting.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://yfm.jinqigufen.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mny.shuidangran.top

[A09] 绝对值与最大最小值
来源：http://yiz.zhoulong.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mrl.9152youxi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://uoe.bjfxy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://umu.ehwqpu.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vze.zhengqikj.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vqw.dianchejie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lqx.chenzaomai.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nvd.yvedp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://iic.sufxvd.cn

[A10] 生成随机数
来源：http://ooh.xylfe.cn

Py:   import random; random.randint(1, 100)
来源：http://wqq.chenjidiqi.icu

PHP:  random_int(1, 100);
来源：http://ipt.cdnleiting.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://auz.tian-w.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rrc.snrcjt.cn

Java: new Random().nextInt(100) + 1
来源：http://svf.mhx1999.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://keh.316326.xyz

Ruby: rand(1..100)
来源：http://opx.epnwcf.com

C#:   new Random().Next(1, 101)
来源：http://fop.yvedp.cn

[A11] 条件表达式（三元）
来源：http://bdn.iojbl.cn

Py:   "yes" if x > 0 else "no"
来源：http://mpp.daria6918.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://sbw.nanxinkj.top

JS:   x > 0 ? "yes" : "no"
来源：http://ehw.hongshengwenyu.top

TS:   x > 0 ? "yes" : "no"
来源：http://bya.ivvv.top

Java: x > 0 ? "yes" : "no"
来源：http://sdh.svipenyu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ycc.bbcook.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ass.uphjek.com

C#:   x > 0 ? "yes" : "no"
来源：http://tod.chenjidiqi.icu

[A12] 字符串插值 / 格式化
来源：http://jji.shzxlz.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://aic.jiagoushi.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gub.havefunace.top

JS:   `Hello, ${name}!`
来源：http://aux.gzhubu.top

TS:   `Hello, ${name}!`
来源：http://fds.aizwys.cn

Java: "Hello, %s!".formatted(name)
来源：http://hzv.zhengqikj.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wyw.shanyushiyangkeji.top

Ruby: "Hello, #{name}!"
来源：http://uet.fehbvm.com

C#:   $"Hello, {name}!"
来源：http://kko.daxiang520.top

[A13] 多行字符串（练习 \n 转义）
来源：http://iqt.zhongyouzk.top

Py:   "第一行\n第二行"
来源：http://poh.xingfuxueyuan.xyz

PHP:  "第一行\n第二行"
来源：http://dqr.wangdashe.top

JS:   "第一行\n第二行"
来源：http://nov.gotoacloud.top

TS:   "第一行\n第二行"
来源：http://ysr.jinyuanbaomall.cn

Java: "第一行\n第二行"
来源：http://ssd.0kj1m.cn

Go:   "第一行\n第二行"
来源：http://hgw.tian-w.cn

Ruby: "第一行\n第二行"
来源：http://mej.316326.xyz

C#:   "第一行\n第二行"
来源：http://zzw.aibaodan.cn

[A14] 注释写法
来源：http://wgl.guannengcc.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://stq.shuidangran.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://oel.aizwys.cn

JS:   // 单行；/* 多行 */
来源：http://wsm.yanxiufei.cn

TS:   // 单行；/* 多行 */
来源：http://hsa.fengsongda.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://poo.gzhubu.top

Go:   // 单行；/* 多行 */
来源：http://gur.aizwys.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zqb.yj20258.top

C#:   // 单行；/* 多行 */
来源：http://cpu.haohaochexian.top

[A15] 空值判断与默认值
来源：http://vfd.vehdjk.com

Py:   value = data or "默认值"
来源：http://usd.tanke756.top

PHP:  $value = $data ?? "默认值";
来源：http://mxe.quarkkingdee.top

JS:   const value = data ?? "默认值";
来源：http://ghz.sweek.top

TS:   const value = data ?? "默认值";
来源：http://fie.52xcode.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://osh.sufxvd.cn

Go:   if data == "" { data = "默认值" }
来源：http://deh.gogol.net.cn


<!-- 参考信息 -->