代发 wailian999

[U89] JS：数组去重
来源：http://gwq.birdmap.top

[...new Set(arr)]
来源：http://gjt.jiagoushi.top

[U90] JS：数字数组排序
来源：http://xtl.vehdjk.com

[...arr].sort((a, b) => a - b)
来源：http://kuv.yfazqb.com

[U91] JS：对象键值遍历
来源：http://qxs.jqgufenzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://txf.jqgufenzy.top

[U92] JS：深拷贝
来源：http://nfe.zdqjudy.top

structuredClone(obj)
来源：http://qhh.zhengqikj.top

[U93] JS：模板字符串
来源：http://nqp.feifeiyinyue.top

`共 ${n} 条`
来源：http://ryq.sjlbkw.cn

[U94] JS：箭头函数
来源：http://rts.ppjwa.cn

const double = x => x * 2;
来源：http://eab.sufxvd.cn

[U95] JS：Promise 包装
来源：http://imu.tanke756.top

new Promise((resolve, reject) => {})
来源：http://ivc.meibo888.top

[U96] JS：async/await 与异常
来源：http://hnf.xylfe.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fxl.xingfuxueyuan.xyz

[U97] JS：并发请求
来源：http://ekd.xziqi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cau.xziqi.cn

[U98] JS：fetch 带 JSON
来源：http://mca.epnwcf.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://noa.jianghu66.top

[U99] JS：事件监听
来源：http://xqd.redwolf501.top

el.addEventListener("click", e => {})
来源：http://hpq.cqqwz.cn

[U100] JS：DOM 查询
来源：http://wpe.sxryk.cn

document.querySelector(".item")
来源：http://dnl.cqqwz.cn

[U101] JS：classList 操作
来源：http://zgq.ywan-chungtsiang.top

el.classList.toggle("active")
来源：http://cqe.jqgufenzy.top

[U102] JS：本地存储
来源：http://xak.pycfn.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://rsw.aizwys.cn

[U103] JS：定时器
来源：http://skw.yanxiufei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uln.chenjidiqi.icu

[U104] JS：防抖
来源：http://iri.316326.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wmh.feifeiyinyue.top

[U105] JS：节流
来源：http://iqe.aibaodan.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wzj.zhongyouzk.top

[U106] JS：日期格式化
来源：http://ybt.yueranfly.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zbo.shanyushiyangtech.top

[U107] JS：数字千分位
来源：http://tci.cdnleiting.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vry.jiagoushi.top

[U108] JS：随机整数
来源：http://fvq.tian-w.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hkv.zhengqikj.top

[U109] JS：数组分组
来源：http://wkt.cdnleiting.top

Object.groupBy(arr, x => x.type)
来源：http://wjg.pengpengdd.cyou

[U110] JS：数组分块
来源：http://whm.zycfv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ydm.ivvv.top

[U111] JS：对象转 Map
来源：http://wkl.c1oappe.top

new Map(Object.entries(obj))
来源：http://hxl.52xcode.cn

[U112] JS：字符串补位
来源：http://pwk.ywan-chungtsiang.top

"7".padStart(3, "0")
来源：http://wui.yanxiufei.cn

[U113] JS：正则替换全部
来源：http://fvg.52xcode.cn

s.replaceAll("a", "b")
来源：http://dey.zhixingplan.top

[U114] JS：JSON 深比较
来源：http://gzv.nanxuanxn.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://kwu.xuanzx.com

[U115] JS：生成 UUID
来源：http://pbe.vqdsnc.cn

crypto.randomUUID()
来源：http://hie.wangdashe.top

[U116] JS：类型检查（JSDoc）
来源：http://gnv.hesvh.cn

/** @param {string} name */ function f(name) {}
来源：http://iri.ydjk.org.cn

[U117] JS：单元测试
来源：http://vri.shanyushiyangkeji.top

npm i -D vitest;  npx vitest
来源：http://upg.gaohongyu789.top

[U118] JS：开发服务器
来源：http://iqe.ywan-chungtsiang.top

npm i -D vite;  npx vite
来源：http://cvg.xziqi.cn

[U119] JS：生产构建
来源：http://sad.xuanzx.com

npx vite build
来源：http://vlx.jinqigfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://yvr.zhiwuduotai.top

import.meta.env.VITE_API_URL
来源：http://zvn.chenlongwang.top

================================================================================
来源：http://agd.ywan-chungtsiang.top

统计汇总
来源：http://kfn.c1oappe.top

================================================================================
来源：http://uyz.shangyingyoupin.top

按语言统计（条）：
来源：http://tzk.snrcjt.cn

Python ......... 252
来源：http://smb.redwolf501.top

PHP ............ 252
来源：http://rbw.feifeiyinyue.top

JavaScript ..... 252
来源：http://syx.jqgufenzy.top

TypeScript ..... 212
来源：http://gft.hywenlv.cn

Java ........... 212
来源：http://lcw.fzhhl.top

Go ............. 212
来源：http://els.hongshengwenyu.top

Ruby ........... 212
来源：http://cxu.aibaodan.cn

C# ............. 212
来源：http://irp.gotoacloud.top

C .............. 30
来源：http://tpm.ybcxt.top

C++ ............ 30
来源：http://vaq.xuanzx.com

SQL ............ 90
来源：http://mgy.tarul.cn

Bash ........... 80
来源：http://sey.hongshengwenyu.top

Kotlin ......... 15
来源：http://qdn.yangfankeji.com

Swift .......... 15
来源：http://bpo.zhijiandao.cn

Lua ............ 10
来源：http://ouv.pengpengdd.cyou

Perl ........... 10
来源：http://dgv.zhoulong.xyz

Scala .......... 10
来源：http://vvl.xuetiantiany.cn

------------------------------------
来源：http://keo.hnqzz.top

合计 ........... 2106 条
来源：http://ktv.xingfuxueyuan.xyz

按章节统计：
来源：http://qnv.ehwqpu.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uxs.fehbvm.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rzf.cheryme.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kir.fanxiaobao.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dzv.xuanzx.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://eyg.jinqigufen.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vdr.dianchejie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tnr.xuetiantiany.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://slq.hywenlv.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xli.ydzc1.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://plo.meibo888.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tcy.cdnleiting.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://eaw.yj202588.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://myp.cheryme.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://szo.hnxiangtu.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pbu.cheryme.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ern.smart0.xyz

Q SQL 专题                              90
来源：http://ict.cucudq.cn

R Bash 专题                             80
来源：http://cwb.jinqigfzy.top

S C / C++ 专题                          60
来源：http://cin.chenlongwang.top

T 其他语言补充                          60
来源：http://uxd.sjlbkw.cn

U 高频实用片段                         120
来源：http://plx.hnxiangtu.top

------------------------------------
来源：http://ufm.tianlin.xyz

合计                                  2106 条
来源：http://wdf.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://lwz.zhiwuduotai.top

使用提醒
来源：http://pfh.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://bvj.hcnkem.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ngt.shanyushiyangtech.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mfi.yonumen.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yov.yuxming.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://pvd.zdbjq.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://uru.316326.xyz

—— 文件结束 ——
来源：http://dtv.xuetiantiany.cn

================================================================================
来源：http://aum.hesvh.cn

程序语言常见例子速查手册（2024 版）
来源：http://hvr.zhaomingkeji.xyz

Common Programming Examples Cheat Book
来源：http://vpo.cqqwz.cn

================================================================================
来源：http://oab.shuidangran.top

【收录内容】
来源：http://sgh.xziqi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://spj.jinyuanbaomall.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ces.vqdsnc.cn

SQL · Bash · C · C++
来源：http://thq.mhx1999.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sms.zhaomingkeji.xyz

【使用说明】
来源：http://tss.hcnkem.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zsv.ydzc1.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://czq.zhixingplan.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qcm.wangdashe.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ges.hongshengwenyu.top

Bash:  Shell         C:     C             C++:   C++
来源：http://obb.xinyue.icu

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hai.xziqi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wlv.iojbl.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xck.yvedp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cty.fengsongda.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kqp.fzhhl.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lkh.yuanzhike.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fwc.svipenyu.cn

【文件统计】
来源：http://eob.gogol.net.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ppr.daxiang520.top

--------------------------------------------------------------------------------
来源：http://fru.andypj.xyz

目  录
来源：http://hgs.bbcook.cn

--------------------------------------------------------------------------------
来源：http://nfa.sysykeji.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://smq.shanyushiyangkeji.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dcw.cheryme.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nur.jqgfzy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://oap.jyoumei.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lte.tarul.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lrt.shanyushiyangkeji.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tin.316326.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xkw.yj202588.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zlp.hammf.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zal.hysaishi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vlx.ppjwa.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rya.jinqigfzy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xxt.vehdjk.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://roo.zdqjudy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ywz.yj20258888.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yrf.feifeiyinyue.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dct.sufxvd.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://myr.jinyuanbaomall.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hzc.yvedp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ria.9152youxi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bvt.haohaochexian.top

================================================================================
来源：http://ayz.nanxinkj.top

A. 基础语法与类型
来源：http://vyq.pengpengdd.cyou

================================================================================
来源：http://fkj.wangdashe.top

[A01] Hello World
来源：http://wrz.fehbvm.com

Py:   print("Hello, World!")
来源：http://zck.jinqigfzy.top

PHP:  echo "Hello, World!";
来源：http://ebj.zycfv.cn

JS:   console.log("Hello, World!");
来源：http://use.uphjek.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pyi.jqgfzy.top

Java: System.out.println("Hello, World!");
来源：http://wta.dashuyun.cn

Go:   fmt.Println("Hello, World!")
来源：http://fau.hcnkem.com

Ruby: puts "Hello, World!"
来源：http://bep.cqqwz.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hub.ehwqpu.com

[A02] 变量声明与赋值
来源：http://qvs.yj20258888.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gge.yvedp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://cwo.ehwqpu.com

JS:   let name = "Alex"; const age = 20;
来源：http://kcj.jiagoushi.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://efp.wangshuangyany.cn

Java: String name = "Alex"; int age = 20;
来源：http://egy.hesvh.cn

Go:   name := "Alex"; age := 20
来源：http://iwm.nanxinkj.top

Ruby: name = "Alex"; age = 20
来源：http://dyn.ehwqpu.com

C#:   string name = "Alex"; int age = 20;
来源：http://qsw.guannengcc.top

[A03] 常量定义
来源：http://ymt.smart0.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tqc.shanyushiyangkeji.top

PHP:  const PI = 3.14159;
来源：http://svd.nwbrower.top

JS:   const PI = 3.14159;
来源：http://wgk.chenzaomai.com

TS:   const PI: number = 3.14159;
来源：http://zxg.jinqigfzy.top

Java: static final double PI = 3.14159;
来源：http://wwv.c1oappe.top

Go:   const PI = 3.14159
来源：http://qxz.xuanzx.com

Ruby: PI = 3.14159
来源：http://rnp.fktsv.cn

C#:   const double PI = 3.14159;
来源：http://lwn.sysykeji.top

[A04] 判断变量类型
来源：http://kit.zhoulong.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://bap.uphjek.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vio.nanxuanxn.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://izn.dashuyun.cn

TS:   typeof x; x instanceof Date
来源：http://wnr.guannengcc.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://czr.yj20258888.top

Go:   reflect.TypeOf(x).Name()
来源：http://ioq.nanxuanxn.top

Ruby: x.class; x.is_a?(Integer)
来源：http://egh.chenjidiqi.icu

C#:   x.GetType().Name; x is int
来源：http://spg.gogol.net.cn

[A05] 整数除法与取模
来源：http://jrn.shuidangran.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dju.aibaodan.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jwz.fanxiaobao.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yel.nanxuanxn.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kee.cashguo.top

Java: 7 / 2; 7 % 2
来源：http://gls.zhengqikj.top

Go:   7 / 2; 7 % 2
来源：http://hkt.wangdashe.top

Ruby: 7 / 2; 7 % 2
来源：http://vwh.daxiang520.top

C#:   7 / 2; 7 % 2
来源：http://faz.52xcode.cn

[A06] 字符串转数字
来源：http://flx.zhongyouzk.top

Py:   int("42"); float("3.14")
来源：http://ajh.ydzc1.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://aut.yfazqb.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wsa.quarkkingdee.top

TS:   parseInt("42", 10); Number("42")
来源：http://gms.cqqwz.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zda.fanxiaobao.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kex.zhaomingkeji.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://igg.yueranfly.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ghh.guowangkeji.top

[A07] 数字转字符串
来源：http://qvh.hnqzz.top

Py:   str(42)
来源：http://ssk.yj20258888.top

PHP:  (string) 42; strval(42)
来源：http://qeu.chenlongwang.top

JS:   String(42); (42).toString()
来源：http://yed.wangdashe.top

TS:   String(42)
来源：http://qhe.xylfe.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://blz.aizwys.cn

Go:   strconv.Itoa(42)
来源：http://tdw.fanxiaobao.xyz

Ruby: 42.to_s
来源：http://hfy.haohaochexian.top

C#:   42.ToString()
来源：http://yyo.daria6918.cn

[A08] 取整与四舍五入
来源：http://ytq.0kj1m.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wfm.birdmap.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rrw.zhijiandao.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://yof.ppjwa.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zny.zycfv.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://csf.fktsv.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rtc.shzxlz.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lvt.52xcode.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://uhx.yfazqb.com

[A09] 绝对值与最大最小值
来源：http://egk.cdnleiting.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wmp.ehwqpu.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mxi.zhengqikj.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yil.bbcook.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uju.hfpthk.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://abb.chenlongwang.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jby.aizwys.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://eoc.wangdashe.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bmo.chenzaomai.com

[A10] 生成随机数
来源：http://lmy.shzxlz.cn

Py:   import random; random.randint(1, 100)
来源：http://tnh.zhongyouzk.top

PHP:  random_int(1, 100);
来源：http://wfu.snrcjt.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jbc.tanke756.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://laj.gotoacloud.top

Java: new Random().nextInt(100) + 1
来源：http://gvm.nanxinkj.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vaq.gzhubu.top

Ruby: rand(1..100)
来源：http://icl.nanxuanxn.top

C#:   new Random().Next(1, 101)
来源：http://ztr.nwbrower.top

[A11] 条件表达式（三元）
来源：http://ddo.yueranfly.top

Py:   "yes" if x > 0 else "no"
来源：http://qvf.chenlongwang.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://dme.feifeiyinyue.top

JS:   x > 0 ? "yes" : "no"
来源：http://tsm.fengsongda.top

TS:   x > 0 ? "yes" : "no"
来源：http://bki.jinqigfzy.top

Java: x > 0 ? "yes" : "no"
来源：http://mfp.zdbjq.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xod.hfpthk.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ilv.dianchejie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zob.birdmap.top

[A12] 字符串插值 / 格式化
来源：http://mco.andypj.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bjn.jinyuanbaomall.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tvn.dianchejie.cn

JS:   `Hello, ${name}!`
来源：http://nrg.kuanghao11.cn

TS:   `Hello, ${name}!`
来源：http://oxx.sysykeji.top

Java: "Hello, %s!".formatted(name)
来源：http://jyp.zhijiandao.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qyl.bjfxy.top

Ruby: "Hello, #{name}!"
来源：http://adw.c1oappe.top

C#:   $"Hello, {name}!"
来源：http://oqx.andypj.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://qvo.haohaochexian.top

Py:   "第一行\n第二行"
来源：http://vos.tian-w.cn

PHP:  "第一行\n第二行"
来源：http://wfn.ywan-chungtsiang.top

JS:   "第一行\n第二行"
来源：http://jtb.aizwys.cn

TS:   "第一行\n第二行"
来源：http://daj.sxryk.cn

Java: "第一行\n第二行"
来源：http://ckd.fktsv.cn

Go:   "第一行\n第二行"
来源：http://alb.yj20258888.top

Ruby: "第一行\n第二行"
来源：http://ttb.fktsv.cn

C#:   "第一行\n第二行"
来源：http://yhs.aizwys.cn

[A14] 注释写法
来源：http://onh.yvedp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://usn.jianghu66.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://xxx.snrcjt.cn

JS:   // 单行；/* 多行 */
来源：http://whp.yfazqb.com

TS:   // 单行；/* 多行 */
来源：http://giw.hysaishi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://euf.zdbjq.cn

Go:   // 单行；/* 多行 */
来源：http://jcb.52xcode.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xeg.dashuyun.cn

C#:   // 单行；/* 多行 */
来源：http://lqx.meibo888.top

[A15] 空值判断与默认值
来源：http://xsl.kuanghao11.cn

Py:   value = data or "默认值"
来源：http://wwi.nanxinkj.top

PHP:  $value = $data ?? "默认值";
来源：http://xdl.yueranfly.top


<!-- 参考信息 -->