代发 wailian999

[U89] JS：数组去重
来源：http://tqa.hysaishi.cn

[...new Set(arr)]
来源：http://nvo.birdmap.top

[U90] JS：数字数组排序
来源：http://igi.ydzc1.top

[...arr].sort((a, b) => a - b)
来源：http://iyh.zdqjudy.top

[U91] JS：对象键值遍历
来源：http://hcr.pycfn.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pmj.zhengqikj.top

[U92] JS：深拷贝
来源：http://wer.cashguo.top

structuredClone(obj)
来源：http://qvg.smart0.xyz

[U93] JS：模板字符串
来源：http://muw.ydjk.org.cn

`共 ${n} 条`
来源：http://ufm.ywan-chungtsiang.top

[U94] JS：箭头函数
来源：http://tbb.aibaodan.cn

const double = x => x * 2;
来源：http://erg.jinqigufen.top

[U95] JS：Promise 包装
来源：http://pju.sxryk.cn

new Promise((resolve, reject) => {})
来源：http://fqy.pengpengdd.cyou

[U96] JS：async/await 与异常
来源：http://xkq.smart0.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://eki.zdqjudy.top

[U97] JS：并发请求
来源：http://iyt.hesvh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yqy.shanyushiyangkeji.top

[U98] JS：fetch 带 JSON
来源：http://krj.jinghuilouyu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rpg.gaohongyu789.top

[U99] JS：事件监听
来源：http://jee.birdmap.top

el.addEventListener("click", e => {})
来源：http://mxo.gogol.net.cn

[U100] JS：DOM 查询
来源：http://jkn.ehwqpu.com

document.querySelector(".item")
来源：http://vrf.daxiang520.top

[U101] JS：classList 操作
来源：http://gki.hesvh.cn

el.classList.toggle("active")
来源：http://ntd.0kj1m.cn

[U102] JS：本地存储
来源：http://act.ppjwa.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nay.svipenyu.cn

[U103] JS：定时器
来源：http://osf.nanxinkj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rdt.bbcook.cn

[U104] JS：防抖
来源：http://kuc.uphjek.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eof.hfpthk.cn

[U105] JS：节流
来源：http://zkf.hcnkem.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://phn.jinyuanbaomall.cn

[U106] JS：日期格式化
来源：http://llg.wangdashe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xmz.zhijiandao.cn

[U107] JS：数字千分位
来源：http://udv.jqgufenzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tsa.316326.xyz

[U108] JS：随机整数
来源：http://lot.jinqigufen.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dex.yongpay.top

[U109] JS：数组分组
来源：http://xlr.tanke756.top

Object.groupBy(arr, x => x.type)
来源：http://hxe.cashguo.top

[U110] JS：数组分块
来源：http://wxs.aizwys.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ojr.yueranfly.top

[U111] JS：对象转 Map
来源：http://mki.feifeiyinyue.top

new Map(Object.entries(obj))
来源：http://kby.jinqigfzy.top

[U112] JS：字符串补位
来源：http://itk.aizwys.cn

"7".padStart(3, "0")
来源：http://uyb.xinyue.icu

[U113] JS：正则替换全部
来源：http://hxy.ctjpmb.com

s.replaceAll("a", "b")
来源：http://gkl.wangshuangyany.cn

[U114] JS：JSON 深比较
来源：http://vpq.cdnleiting.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hrn.gaohongyu789.top

[U115] JS：生成 UUID
来源：http://nci.daxiang520.top

crypto.randomUUID()
来源：http://lqg.ctjpmb.com

[U116] JS：类型检查（JSDoc）
来源：http://ifp.dashuyun.cn

/** @param {string} name */ function f(name) {}
来源：http://jou.gaohongyu789.top

[U117] JS：单元测试
来源：http://okc.hongshengwenyu.top

npm i -D vitest;  npx vitest
来源：http://sec.jinghuilouyu.cn

[U118] JS：开发服务器
来源：http://lid.hammf.cn

npm i -D vite;  npx vite
来源：http://wwv.gaohongyu789.top

[U119] JS：生产构建
来源：http://ptw.hysaishi.cn

npx vite build
来源：http://zso.shangyingyoupin.top

[U120] JS：读取环境变量（Vite）
来源：http://dqf.jinyuanbaomall.cn

import.meta.env.VITE_API_URL
来源：http://ldo.cheryme.top

================================================================================
来源：http://ddg.yvedp.cn

统计汇总
来源：http://iia.chenjidiqi.icu

================================================================================
来源：http://ndc.zhoulong.xyz

按语言统计（条）：
来源：http://kwu.tianlin.xyz

Python ......... 252
来源：http://xuq.snrcjt.cn

PHP ............ 252
来源：http://yjo.gotoacloud.top

JavaScript ..... 252
来源：http://jhv.yvedp.cn

TypeScript ..... 212
来源：http://flq.gaohongyu789.top

Java ........... 212
来源：http://dsh.meibo888.top

Go ............. 212
来源：http://cjw.kuanghao11.cn

Ruby ........... 212
来源：http://gtp.zhengqikj.top

C# ............. 212
来源：http://tgr.yvedp.cn

C .............. 30
来源：http://tqf.gzhubu.top

C++ ............ 30
来源：http://pmx.wangshuangyany.cn

SQL ............ 90
来源：http://qvq.jiagoushi.top

Bash ........... 80
来源：http://odb.sxryk.cn

Kotlin ......... 15
来源：http://fgi.yangfankeji.com

Swift .......... 15
来源：http://fsd.daxiang520.top

Lua ............ 10
来源：http://jgy.jyoumei.cn

Perl ........... 10
来源：http://mqf.zhongyouzk.top

Scala .......... 10
来源：http://vmn.sufxvd.cn

------------------------------------
来源：http://uhd.fktsv.cn

合计 ........... 2106 条
来源：http://zga.chenzaomai.com

按章节统计：
来源：http://ogv.hfpthk.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://czd.redwolf501.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jxk.ywan-chungtsiang.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gly.guowangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nlu.jinqigufen.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wua.hfpthk.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bml.ybcxt.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fwz.yj202588.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://udw.mhx1999.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zxd.chenjidiqi.icu

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vld.wangshuangyany.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rxg.gaohongyu789.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pxr.haohaochexian.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://flr.chenlongwang.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ccu.zhengqikj.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nmi.c1oappe.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wee.zhongyouzk.top

Q SQL 专题                              90
来源：http://pri.dashuyun.cn

R Bash 专题                             80
来源：http://mrd.xziqi.cn

S C / C++ 专题                          60
来源：http://qui.9152youxi.cn

T 其他语言补充                          60
来源：http://gtf.redwolf501.top

U 高频实用片段                         120
来源：http://bil.feifeiyinyue.top

------------------------------------
来源：http://aul.ydzc1.top

合计                                  2106 条
来源：http://uby.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://szu.snrcjt.cn

使用提醒
来源：http://tpc.fzhhl.top

--------------------------------------------------------------------------------
来源：http://biv.cheryme.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cof.hnxiangtu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://otl.nwbrower.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ybd.ppjwa.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gae.0kj1m.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dab.yfazqb.com

—— 文件结束 ——
来源：http://bys.sjlbkw.cn

================================================================================
来源：http://mfo.jyoumei.cn

程序语言常见例子速查手册（2024 版）
来源：http://tmj.birdmap.top

Common Programming Examples Cheat Book
来源：http://ldd.chenlongwang.top

================================================================================
来源：http://udk.nanxinkj.top

【收录内容】
来源：http://bwy.tianlin.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://acx.tarul.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://uly.ehwqpu.com

SQL · Bash · C · C++
来源：http://vqd.dianchejie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cst.gaohongyu789.top

【使用说明】
来源：http://ijt.xinyue.icu

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://evq.ivvv.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dho.c1oappe.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://chf.ppjwa.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rnc.gzhubu.top

Bash:  Shell         C:     C             C++:   C++
来源：http://kbc.9152youxi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kwg.zhengqikj.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tvi.cashguo.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zkq.iojbl.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jff.birdmap.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pnx.xinyue.icu

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vgn.epnwcf.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://iah.iojbl.cn

【文件统计】
来源：http://igz.yongpay.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sgq.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://xdv.zhiwuduotai.top

目  录
来源：http://xor.havefunace.top

--------------------------------------------------------------------------------
来源：http://sqt.yj20258888.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pkk.hnqzz.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rsb.haohaochexian.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ohz.shuidangran.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ebl.zhiwuduotai.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hvh.jyoumei.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kov.sjlbkw.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bxm.fengsongda.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mhw.redwolf501.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://exz.epnwcf.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ajp.yj20258.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://oee.9152youxi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://inu.bjfxy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://emt.vqdsnc.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zse.jyoumei.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qvb.ehwqpu.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://udz.xingfuxueyuan.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vsg.yj20258.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://opo.iojbl.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pbu.cucudq.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://iyo.chenlongwang.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qvf.cqqwz.cn

================================================================================
来源：http://njg.316326.xyz

A. 基础语法与类型
来源：http://aye.pengpengdd.cyou

================================================================================
来源：http://hjx.nwbrower.top

[A01] Hello World
来源：http://eiv.zhixingplan.top

Py:   print("Hello, World!")
来源：http://lby.nanxuanxn.top

PHP:  echo "Hello, World!";
来源：http://rzw.shangyingyoupin.top

JS:   console.log("Hello, World!");
来源：http://kwk.gogol.net.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://iie.andypj.xyz

Java: System.out.println("Hello, World!");
来源：http://fjv.xingfuxueyuan.xyz

Go:   fmt.Println("Hello, World!")
来源：http://nev.nwbrower.top

Ruby: puts "Hello, World!"
来源：http://nzk.dianchejie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rcd.smart0.xyz

[A02] 变量声明与赋值
来源：http://nob.andypj.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mek.chenzaomai.com

PHP:  $name = "Alex"; $age = 20;
来源：http://eyz.tanke756.top

JS:   let name = "Alex"; const age = 20;
来源：http://szy.ctjpmb.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://uzo.yongpay.top

Java: String name = "Alex"; int age = 20;
来源：http://lfz.gzhubu.top

Go:   name := "Alex"; age := 20
来源：http://bem.cqqwz.cn

Ruby: name = "Alex"; age = 20
来源：http://saj.bbcook.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nan.aizwys.cn

[A03] 常量定义
来源：http://hhf.yj20258.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yai.feifeiyinyue.top

PHP:  const PI = 3.14159;
来源：http://nws.tianlin.xyz

JS:   const PI = 3.14159;
来源：http://fvs.svipenyu.cn

TS:   const PI: number = 3.14159;
来源：http://qdt.9152youxi.cn

Java: static final double PI = 3.14159;
来源：http://skc.hnqzz.top

Go:   const PI = 3.14159
来源：http://qyc.zhengqikj.top

Ruby: PI = 3.14159
来源：http://mdk.zhixingplan.top

C#:   const double PI = 3.14159;
来源：http://bkm.yuanzhike.top

[A04] 判断变量类型
来源：http://vhv.svipenyu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://prt.ydzc1.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rlh.daria6918.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://adg.ctjpmb.com

TS:   typeof x; x instanceof Date
来源：http://phx.vehdjk.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jzj.ydjk.org.cn

Go:   reflect.TypeOf(x).Name()
来源：http://woz.shangyingyoupin.top

Ruby: x.class; x.is_a?(Integer)
来源：http://pfb.xuetiantiany.cn

C#:   x.GetType().Name; x is int
来源：http://srb.316326.xyz

[A05] 整数除法与取模
来源：http://ldg.yuxming.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yhf.fanxiaobao.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://ojn.svipenyu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nyr.yvedp.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ykr.kuanghao11.cn

Java: 7 / 2; 7 % 2
来源：http://usb.havefunace.top

Go:   7 / 2; 7 % 2
来源：http://ljb.fzhhl.top

Ruby: 7 / 2; 7 % 2
来源：http://ovx.ywan-chungtsiang.top

C#:   7 / 2; 7 % 2
来源：http://nog.jinghuilouyu.cn

[A06] 字符串转数字
来源：http://ytm.xziqi.cn

Py:   int("42"); float("3.14")
来源：http://blp.nanxinkj.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://npx.hnqzz.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hbt.pycfn.com

TS:   parseInt("42", 10); Number("42")
来源：http://ksj.chenjidiqi.icu

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hwr.birdmap.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dkb.guannengcc.top

Ruby: "42".to_i; "3.14".to_f
来源：http://nxw.ehwqpu.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gwe.aizwys.cn

[A07] 数字转字符串
来源：http://nvo.xuetiantiany.cn

Py:   str(42)
来源：http://kqc.yj20258888.top

PHP:  (string) 42; strval(42)
来源：http://aic.meibo888.top

JS:   String(42); (42).toString()
来源：http://vaz.meibo888.top

TS:   String(42)
来源：http://xjr.zhixingplan.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://vkm.zhixingplan.top

Go:   strconv.Itoa(42)
来源：http://xpf.mhx1999.top

Ruby: 42.to_s
来源：http://zlk.sweek.top

C#:   42.ToString()
来源：http://jqt.fehbvm.com

[A08] 取整与四舍五入
来源：http://wyq.bjfxy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yzk.jqgfzy.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ntl.bbcook.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://twk.zdqjudy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jje.fanxiaobao.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ies.sjlbkw.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vkz.xinyue.icu

Ruby: 3.567.round(2); 3.9.floor
来源：http://vns.yvedp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zcs.jiagoushi.top

[A09] 绝对值与最大最小值
来源：http://uaa.cqqwz.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ygo.zdqjudy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fvl.nanxinkj.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hmo.jinqigfzy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mll.hcnkem.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gsn.bjfxy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cxc.uphjek.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mis.c1oappe.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mbu.zhixingplan.top

[A10] 生成随机数
来源：http://frf.shuidangran.top

Py:   import random; random.randint(1, 100)
来源：http://paj.jyoumei.cn

PHP:  random_int(1, 100);
来源：http://iui.yuxming.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qlr.hnqzz.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vwn.hammf.cn

Java: new Random().nextInt(100) + 1
来源：http://rjw.aizwys.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://aht.zhiwuduotai.top

Ruby: rand(1..100)
来源：http://pyf.nanxuanxn.top

C#:   new Random().Next(1, 101)
来源：http://fat.hysaishi.cn

[A11] 条件表达式（三元）
来源：http://mnp.mhx1999.top

Py:   "yes" if x > 0 else "no"
来源：http://lkk.shuidangran.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://nmh.jqgfzy.top

JS:   x > 0 ? "yes" : "no"
来源：http://jey.dianchejie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qpw.yj20258.top

Java: x > 0 ? "yes" : "no"
来源：http://ulq.yuanzhike.top

Go:   // 无三元运算符，需用 if 语句
来源：http://pnu.bjfxy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://emb.yongpay.top

C#:   x > 0 ? "yes" : "no"
来源：http://gsx.uphjek.com

[A12] 字符串插值 / 格式化
来源：http://qlf.hfpthk.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ztx.havefunace.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://brg.wangshuangyany.cn

JS:   `Hello, ${name}!`
来源：http://vyv.fengsongda.top

TS:   `Hello, ${name}!`
来源：http://dgu.jqgfzy.top

Java: "Hello, %s!".formatted(name)
来源：http://zmk.0kj1m.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://eod.fzhhl.top

Ruby: "Hello, #{name}!"
来源：http://qxf.dianchejie.cn

C#:   $"Hello, {name}!"
来源：http://shw.daxiang520.top

[A13] 多行字符串（练习 \n 转义）
来源：http://zre.jinqigfzy.top

Py:   "第一行\n第二行"
来源：http://awd.zhijiandao.cn

PHP:  "第一行\n第二行"
来源：http://zji.shanyushiyangkeji.top

JS:   "第一行\n第二行"
来源：http://jmo.yj20258888.top

TS:   "第一行\n第二行"
来源：http://bzu.gaohongyu789.top

Java: "第一行\n第二行"
来源：http://mfn.zdbjq.cn

Go:   "第一行\n第二行"
来源：http://ugd.ydzc1.top

Ruby: "第一行\n第二行"
来源：http://naw.jinyuanbaomall.cn

C#:   "第一行\n第二行"
来源：http://xwi.zhengqikj.top

[A14] 注释写法
来源：http://ygw.ybcxt.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ifk.tanke756.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://iux.yj20258888.top

JS:   // 单行；/* 多行 */
来源：http://jjh.zhaomingkeji.xyz

TS:   // 单行；/* 多行 */
来源：http://vuh.fehbvm.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zvy.vqdsnc.cn

Go:   // 单行；/* 多行 */
来源：http://kvg.jiagoushi.top

Ruby: # 单行；=begin 多行 =end
来源：http://bwo.xziqi.cn

C#:   // 单行；/* 多行 */
来源：http://bwf.xuetiantiany.cn

[A15] 空值判断与默认值
来源：http://fwr.bjfxy.top

Py:   value = data or "默认值"
来源：http://mne.havefunace.top

PHP:  $value = $data ?? "默认值";
来源：http://ziu.yonumen.top


<!-- 参考信息 -->