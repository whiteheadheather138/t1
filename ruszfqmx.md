代发 wailian999

[U89] JS：数组去重
来源：http://wak.cheryme.top

[...new Set(arr)]
来源：http://wpu.fktsv.cn

[U90] JS：数字数组排序
来源：http://jij.pycfn.com

[...arr].sort((a, b) => a - b)
来源：http://evq.vehdjk.com

[U91] JS：对象键值遍历
来源：http://xzj.cdnleiting.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ris.chenlongwang.top

[U92] JS：深拷贝
来源：http://ybx.9152youxi.cn

structuredClone(obj)
来源：http://kup.aibaodan.cn

[U93] JS：模板字符串
来源：http://ogy.shangyingyoupin.top

`共 ${n} 条`
来源：http://gpm.yongpay.top

[U94] JS：箭头函数
来源：http://wdt.daxiang520.top

const double = x => x * 2;
来源：http://gcj.0kj1m.cn

[U95] JS：Promise 包装
来源：http://wnw.jinqigufen.top

new Promise((resolve, reject) => {})
来源：http://umu.hongshengwenyu.top

[U96] JS：async/await 与异常
来源：http://vus.jianghu66.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://otn.jyoumei.cn

[U97] JS：并发请求
来源：http://pix.nanxinkj.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://hkm.ydzc1.top

[U98] JS：fetch 带 JSON
来源：http://ykj.yj202588.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ixa.yuxming.cn

[U99] JS：事件监听
来源：http://cmn.bjfxy.top

el.addEventListener("click", e => {})
来源：http://ykz.yj20258.top

[U100] JS：DOM 查询
来源：http://cxl.xuanzx.com

document.querySelector(".item")
来源：http://ksk.jqgfzy.top

[U101] JS：classList 操作
来源：http://ick.sufxvd.cn

el.classList.toggle("active")
来源：http://hub.yangfankeji.com

[U102] JS：本地存储
来源：http://naq.yj202588.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://sve.ydjk.org.cn

[U103] JS：定时器
来源：http://bsn.tarul.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zqc.haohaochexian.top

[U104] JS：防抖
来源：http://vfb.ctjpmb.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uhw.haohaochexian.top

[U105] JS：节流
来源：http://jtk.hywenlv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kby.vqdsnc.cn

[U106] JS：日期格式化
来源：http://gyq.yueranfly.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nee.iojbl.cn

[U107] JS：数字千分位
来源：http://off.uphjek.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mhe.ydjk.org.cn

[U108] JS：随机整数
来源：http://tem.svipenyu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fqi.hfpthk.cn

[U109] JS：数组分组
来源：http://edn.jinqigfzy.top

Object.groupBy(arr, x => x.type)
来源：http://vrv.hysaishi.cn

[U110] JS：数组分块
来源：http://hnv.shangyingyoupin.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tac.ybcxt.top

[U111] JS：对象转 Map
来源：http://cbi.shzxlz.cn

new Map(Object.entries(obj))
来源：http://ski.shuidangran.top

[U112] JS：字符串补位
来源：http://wsk.nanxinkj.top

"7".padStart(3, "0")
来源：http://fzc.sjlbkw.cn

[U113] JS：正则替换全部
来源：http://otx.pycfn.com

s.replaceAll("a", "b")
来源：http://exi.redwolf501.top

[U114] JS：JSON 深比较
来源：http://vyg.yvedp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ana.gogol.net.cn

[U115] JS：生成 UUID
来源：http://qsf.andypj.xyz

crypto.randomUUID()
来源：http://znc.kuanghao11.cn

[U116] JS：类型检查（JSDoc）
来源：http://ior.zycfv.cn

/** @param {string} name */ function f(name) {}
来源：http://dps.nwbrower.top

[U117] JS：单元测试
来源：http://nbr.hywenlv.cn

npm i -D vitest;  npx vitest
来源：http://umj.zhijiandao.cn

[U118] JS：开发服务器
来源：http://gwz.shuidangran.top

npm i -D vite;  npx vite
来源：http://dhr.zycfv.cn

[U119] JS：生产构建
来源：http://eir.havefunace.top

npx vite build
来源：http://jik.cashguo.top

[U120] JS：读取环境变量（Vite）
来源：http://yug.shuidangran.top

import.meta.env.VITE_API_URL
来源：http://biz.9152youxi.cn

================================================================================
来源：http://oqk.zhijiandao.cn

统计汇总
来源：http://btc.ehwqpu.com

================================================================================
来源：http://mqd.xinyue.icu

按语言统计（条）：
来源：http://pgd.shanyushiyangkeji.top

Python ......... 252
来源：http://nuq.vqdsnc.cn

PHP ............ 252
来源：http://vus.zhoulong.xyz

JavaScript ..... 252
来源：http://aqs.mhx1999.top

TypeScript ..... 212
来源：http://zjw.cucudq.cn

Java ........... 212
来源：http://sph.yangfankeji.com

Go ............. 212
来源：http://qtb.kuanghao11.cn

Ruby ........... 212
来源：http://gvg.yonumen.top

C# ............. 212
来源：http://psc.shanyushiyangtech.top

C .............. 30
来源：http://dzh.ydjk.org.cn

C++ ............ 30
来源：http://mzr.hongshengwenyu.top

SQL ............ 90
来源：http://fdf.xylfe.cn

Bash ........... 80
来源：http://whx.9152youxi.cn

Kotlin ......... 15
来源：http://cwi.wangdashe.top

Swift .......... 15
来源：http://ftu.yuanzhike.top

Lua ............ 10
来源：http://ppy.xuetiantiany.cn

Perl ........... 10
来源：http://stv.epnwcf.com

Scala .......... 10
来源：http://dch.sufxvd.cn

------------------------------------
来源：http://mzl.sufxvd.cn

合计 ........... 2106 条
来源：http://gnc.yongpay.top

按章节统计：
来源：http://rze.smart0.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qkv.cqqwz.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://orf.zhijiandao.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pvd.guannengcc.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qof.snrcjt.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yru.yj20258888.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://eeu.nanxinkj.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lkc.guannengcc.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vfe.smart0.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xya.svipenyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://are.sweek.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://agb.birdmap.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://axv.cqqwz.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ylo.cdnleiting.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://toz.mhx1999.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xqn.zycfv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rzz.yfazqb.com

Q SQL 专题                              90
来源：http://hpi.iojbl.cn

R Bash 专题                             80
来源：http://xyc.shzxlz.cn

S C / C++ 专题                          60
来源：http://zxr.jinqigfzy.top

T 其他语言补充                          60
来源：http://kfw.iojbl.cn

U 高频实用片段                         120
来源：http://efb.shzxlz.cn

------------------------------------
来源：http://gxf.ppjwa.cn

合计                                  2106 条
来源：http://ktk.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://vnc.hongshengwenyu.top

使用提醒
来源：http://dew.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://gej.cdnleiting.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://snf.ywan-chungtsiang.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ipx.gaohongyu789.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://scx.gaohongyu789.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ldf.havefunace.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cai.zhoulong.xyz

—— 文件结束 ——
来源：http://apt.chenlongwang.top

================================================================================
来源：http://xll.xziqi.cn

程序语言常见例子速查手册（2024 版）
来源：http://npb.daxiang520.top

Common Programming Examples Cheat Book
来源：http://emy.hesvh.cn

================================================================================
来源：http://vcc.chenlongwang.top

【收录内容】
来源：http://ldp.ydzc1.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://rct.hnqzz.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kgv.ywan-chungtsiang.top

SQL · Bash · C · C++
来源：http://ouu.fehbvm.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nae.cdnleiting.top

【使用说明】
来源：http://nhv.epnwcf.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://oaa.hcnkem.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xjh.zhixingplan.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bcg.fehbvm.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rba.ppjwa.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://myo.xuanzx.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wxk.snrcjt.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xle.jinqigufen.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ang.gogol.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wrr.tanke756.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gtt.guowangkeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://feg.dashuyun.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zdv.shzxlz.cn

【文件统计】
来源：http://esk.sweek.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qad.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://vbs.havefunace.top

目  录
来源：http://klc.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://vod.nanxinkj.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hxb.yueranfly.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zsw.yuanzhike.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uzu.gaohongyu789.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fcd.ctjpmb.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cin.andypj.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://eyy.ydjk.org.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xhf.pycfn.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jrh.zhijiandao.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://epy.gogol.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ofx.yj202588.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://utu.hnxiangtu.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://oat.yj202588.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qtf.pengpengdd.cyou

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://srn.nwbrower.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xyf.gzhubu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://grm.sxryk.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yzl.bbcook.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ock.xuanzx.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ump.sweek.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xru.wangshuangyany.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rxa.wangshuangyany.cn

================================================================================
来源：http://xnm.shangyingyoupin.top

A. 基础语法与类型
来源：http://uco.zhixingplan.top

================================================================================
来源：http://jcc.zhengqikj.top

[A01] Hello World
来源：http://jxy.hysaishi.cn

Py:   print("Hello, World!")
来源：http://ryq.yueranfly.top

PHP:  echo "Hello, World!";
来源：http://vyh.aibaodan.cn

JS:   console.log("Hello, World!");
来源：http://ajh.sweek.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://txc.haohaochexian.top

Java: System.out.println("Hello, World!");
来源：http://qoc.yonumen.top

Go:   fmt.Println("Hello, World!")
来源：http://gup.jqgfzy.top

Ruby: puts "Hello, World!"
来源：http://qxi.hcnkem.com

C#:   Console.WriteLine("Hello, World!");
来源：http://cov.yuanzhike.top

[A02] 变量声明与赋值
来源：http://idc.zhixingplan.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qkq.sweek.top

PHP:  $name = "Alex"; $age = 20;
来源：http://tjz.epnwcf.com

JS:   let name = "Alex"; const age = 20;
来源：http://hjw.havefunace.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://muc.9152youxi.cn

Java: String name = "Alex"; int age = 20;
来源：http://hex.hcnkem.com

Go:   name := "Alex"; age := 20
来源：http://bqb.yvedp.cn

Ruby: name = "Alex"; age = 20
来源：http://rte.wangdashe.top

C#:   string name = "Alex"; int age = 20;
来源：http://mst.tarul.cn

[A03] 常量定义
来源：http://clu.tarul.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://btp.daria6918.cn

PHP:  const PI = 3.14159;
来源：http://gii.jinqigfzy.top

JS:   const PI = 3.14159;
来源：http://pst.feifeiyinyue.top

TS:   const PI: number = 3.14159;
来源：http://uxj.yangfankeji.com

Java: static final double PI = 3.14159;
来源：http://ecu.zdbjq.cn

Go:   const PI = 3.14159
来源：http://qvy.sjlbkw.cn

Ruby: PI = 3.14159
来源：http://nnv.xuanzx.com

C#:   const double PI = 3.14159;
来源：http://zqi.bjfxy.top

[A04] 判断变量类型
来源：http://mtq.zhiwuduotai.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://bil.hywenlv.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jpc.kuanghao11.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://usq.daxiang520.top

TS:   typeof x; x instanceof Date
来源：http://jvc.chenzaomai.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dqe.redwolf501.top

Go:   reflect.TypeOf(x).Name()
来源：http://igh.yuxming.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lsk.jqgfzy.top

C#:   x.GetType().Name; x is int
来源：http://kwg.kuanghao11.cn

[A05] 整数除法与取模
来源：http://imh.sweek.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yya.ehwqpu.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://kvj.chenjidiqi.icu

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gdy.cdnleiting.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tpv.mhx1999.top

Java: 7 / 2; 7 % 2
来源：http://idq.jyoumei.cn

Go:   7 / 2; 7 % 2
来源：http://uqy.shuidangran.top

Ruby: 7 / 2; 7 % 2
来源：http://eeq.tianlin.xyz

C#:   7 / 2; 7 % 2
来源：http://dkr.quarkkingdee.top

[A06] 字符串转数字
来源：http://lhc.zycfv.cn

Py:   int("42"); float("3.14")
来源：http://rge.nanxinkj.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sjt.havefunace.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gif.hesvh.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cuf.aizwys.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mbw.jinqigfzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bbl.pycfn.com

Ruby: "42".to_i; "3.14".to_f
来源：http://aap.iojbl.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pcw.sufxvd.cn

[A07] 数字转字符串
来源：http://mdi.chenjidiqi.icu

Py:   str(42)
来源：http://lsq.haohaochexian.top

PHP:  (string) 42; strval(42)
来源：http://hum.jqgufenzy.top

JS:   String(42); (42).toString()
来源：http://bbv.nwbrower.top

TS:   String(42)
来源：http://gbt.gaohongyu789.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://jlb.hnqzz.top

Go:   strconv.Itoa(42)
来源：http://yqd.fehbvm.com

Ruby: 42.to_s
来源：http://lna.cashguo.top

C#:   42.ToString()
来源：http://pik.hesvh.cn

[A08] 取整与四舍五入
来源：http://nps.haohaochexian.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ytb.yonumen.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mgt.yuxming.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://oas.sysykeji.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xkh.zycfv.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kra.pengpengdd.cyou

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gaw.ivvv.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://fgx.vehdjk.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vcb.xuetiantiany.cn

[A09] 绝对值与最大最小值
来源：http://mnd.ydzc1.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://exj.yonumen.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://guy.sweek.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nyh.hesvh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://csk.jianghu66.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uys.iojbl.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://avy.shanyushiyangtech.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vhz.feifeiyinyue.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cdz.52xcode.cn

[A10] 生成随机数
来源：http://kxp.jiagoushi.top

Py:   import random; random.randint(1, 100)
来源：http://gfa.aibaodan.cn

PHP:  random_int(1, 100);
来源：http://udt.jlsjyb.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wwg.fzhhl.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hdo.shuidangran.top

Java: new Random().nextInt(100) + 1
来源：http://nwv.jinghuilouyu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pjp.svipenyu.cn

Ruby: rand(1..100)
来源：http://pdj.xziqi.cn

C#:   new Random().Next(1, 101)
来源：http://pgi.tianlin.xyz

[A11] 条件表达式（三元）
来源：http://sfa.shangyingyoupin.top

Py:   "yes" if x > 0 else "no"
来源：http://cgt.jiagoushi.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://kvz.havefunace.top

JS:   x > 0 ? "yes" : "no"
来源：http://zqh.c1oappe.top

TS:   x > 0 ? "yes" : "no"
来源：http://jso.svipenyu.cn

Java: x > 0 ? "yes" : "no"
来源：http://him.vehdjk.com

Go:   // 无三元运算符，需用 if 语句
来源：http://cac.guowangkeji.top

Ruby: x > 0 ? "yes" : "no"
来源：http://vmo.ctjpmb.com

C#:   x > 0 ? "yes" : "no"
来源：http://otp.316326.xyz

[A12] 字符串插值 / 格式化
来源：http://oui.jianghu66.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ain.tanke756.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jli.jqgfzy.top

JS:   `Hello, ${name}!`
来源：http://zlw.daria6918.cn

TS:   `Hello, ${name}!`
来源：http://qik.xylfe.cn

Java: "Hello, %s!".formatted(name)
来源：http://cht.pycfn.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lma.aibaodan.cn

Ruby: "Hello, #{name}!"
来源：http://bpl.52xcode.cn

C#:   $"Hello, {name}!"
来源：http://kgg.hfpthk.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xcv.hysaishi.cn

Py:   "第一行\n第二行"
来源：http://qsx.zhiwuduotai.top

PHP:  "第一行\n第二行"
来源：http://gcm.yuanzhike.top

JS:   "第一行\n第二行"
来源：http://xcx.hongshengwenyu.top

TS:   "第一行\n第二行"
来源：http://zik.tian-w.cn

Java: "第一行\n第二行"
来源：http://fvm.daxiang520.top

Go:   "第一行\n第二行"
来源：http://mag.zhixingplan.top

Ruby: "第一行\n第二行"
来源：http://ean.gotoacloud.top

C#:   "第一行\n第二行"
来源：http://rsg.wangdashe.top

[A14] 注释写法
来源：http://dwo.hywenlv.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://nzj.jinghuilouyu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rgf.chenlongwang.top

JS:   // 单行；/* 多行 */
来源：http://irx.xinyue.icu

TS:   // 单行；/* 多行 */
来源：http://ukx.ydzc1.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://thk.mhx1999.top

Go:   // 单行；/* 多行 */
来源：http://vpx.hysaishi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ecr.jlsjyb.cn

C#:   // 单行；/* 多行 */
来源：http://dlk.tanke756.top

[A15] 空值判断与默认值
来源：http://hoc.chenzaomai.com

Py:   value = data or "默认值"
来源：http://skc.yj202588.top

PHP:  $value = $data ?? "默认值";
来源：http://smt.smart0.xyz


<!-- 参考信息 -->