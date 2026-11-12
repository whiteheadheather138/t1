代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://heg.epnwcf.com

export const a = 1;  import { a } from "./m.js";
来源：http://dhr.daxiang520.top

[U84] JS：CommonJS 写法
来源：http://wgf.fengsongda.top

module.exports = { a };  const { a } = require("./m");
来源：http://czw.xylfe.cn

[U85] JS：可选链
来源：http://pqu.yfazqb.com

a?.b?.c
来源：http://cgd.sufxvd.cn

[U86] JS：空值合并
来源：http://sri.bjfxy.top

a ?? b
来源：http://fdz.jqgfzy.top

[U87] JS：解构默认值
来源：http://tyh.fktsv.cn

const { a = 1, b = 2 } = obj;
来源：http://vcc.meibo888.top

[U88] JS：对象展开合并
来源：http://wsb.svipenyu.cn

{ ...a, ...b }
来源：http://wev.xylfe.cn

[U89] JS：数组去重
来源：http://qhg.shanyushiyangkeji.top

[...new Set(arr)]
来源：http://cvg.xylfe.cn

[U90] JS：数字数组排序
来源：http://tkr.yueranfly.top

[...arr].sort((a, b) => a - b)
来源：http://qtz.tarul.cn

[U91] JS：对象键值遍历
来源：http://xap.316326.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bgw.hnqzz.top

[U92] JS：深拷贝
来源：http://jjp.xuetiantiany.cn

structuredClone(obj)
来源：http://dsk.hongshengwenyu.top

[U93] JS：模板字符串
来源：http://jji.andypj.xyz

`共 ${n} 条`
来源：http://avt.yj20258888.top

[U94] JS：箭头函数
来源：http://mhn.yongpay.top

const double = x => x * 2;
来源：http://xcy.gotoacloud.top

[U95] JS：Promise 包装
来源：http://mgb.bjfxy.top

new Promise((resolve, reject) => {})
来源：http://gfw.pengpengdd.cyou

[U96] JS：async/await 与异常
来源：http://alz.hongshengwenyu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sub.haohaochexian.top

[U97] JS：并发请求
来源：http://ofn.cqqwz.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vxy.nwbrower.top

[U98] JS：fetch 带 JSON
来源：http://xom.haohaochexian.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xbf.uphjek.com

[U99] JS：事件监听
来源：http://yhh.shanyushiyangtech.top

el.addEventListener("click", e => {})
来源：http://twg.guannengcc.top

[U100] JS：DOM 查询
来源：http://wrc.quarkkingdee.top

document.querySelector(".item")
来源：http://ube.birdmap.top

[U101] JS：classList 操作
来源：http://qxn.fehbvm.com

el.classList.toggle("active")
来源：http://jvw.pycfn.com

[U102] JS：本地存储
来源：http://uat.havefunace.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://yet.yuxming.cn

[U103] JS：定时器
来源：http://cop.shzxlz.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xiv.xylfe.cn

[U104] JS：防抖
来源：http://niz.iojbl.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nre.fktsv.cn

[U105] JS：节流
来源：http://bhl.nanxuanxn.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://urt.hcnkem.com

[U106] JS：日期格式化
来源：http://xzb.dashuyun.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nqs.fehbvm.com

[U107] JS：数字千分位
来源：http://mwx.aibaodan.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nuh.hcnkem.com

[U108] JS：随机整数
来源：http://lmg.ywan-chungtsiang.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vnl.ivvv.top

[U109] JS：数组分组
来源：http://tcp.sjlbkw.cn

Object.groupBy(arr, x => x.type)
来源：http://mbm.chenzaomai.com

[U110] JS：数组分块
来源：http://mer.hnqzz.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qrj.jiagoushi.top

[U111] JS：对象转 Map
来源：http://oxi.tianlin.xyz

new Map(Object.entries(obj))
来源：http://hco.yueranfly.top

[U112] JS：字符串补位
来源：http://bdj.guowangkeji.top

"7".padStart(3, "0")
来源：http://ibk.zycfv.cn

[U113] JS：正则替换全部
来源：http://ntw.snrcjt.cn

s.replaceAll("a", "b")
来源：http://elx.daria6918.cn

[U114] JS：JSON 深比较
来源：http://ynn.c1oappe.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ynw.cheryme.top

[U115] JS：生成 UUID
来源：http://blc.kuanghao11.cn

crypto.randomUUID()
来源：http://fqt.xinyue.icu

[U116] JS：类型检查（JSDoc）
来源：http://vsc.kuanghao11.cn

/** @param {string} name */ function f(name) {}
来源：http://jdd.xuetiantiany.cn

[U117] JS：单元测试
来源：http://mtn.ydzc1.top

npm i -D vitest;  npx vitest
来源：http://fnw.dianchejie.cn

[U118] JS：开发服务器
来源：http://dgr.shanyushiyangkeji.top

npm i -D vite;  npx vite
来源：http://fky.wangshuangyany.cn

[U119] JS：生产构建
来源：http://nkv.zycfv.cn

npx vite build
来源：http://zhr.xziqi.cn

[U120] JS：读取环境变量（Vite）
来源：http://ern.cheryme.top

import.meta.env.VITE_API_URL
来源：http://pmp.ydzc1.top

================================================================================
来源：http://ync.zhengqikj.top

统计汇总
来源：http://uoa.ehwqpu.com

================================================================================
来源：http://vdq.0kj1m.cn

按语言统计（条）：
来源：http://hxh.chenjidiqi.icu

Python ......... 252
来源：http://chk.fzhhl.top

PHP ............ 252
来源：http://dyg.ctjpmb.com

JavaScript ..... 252
来源：http://tdf.ppjwa.cn

TypeScript ..... 212
来源：http://vtq.zhijiandao.cn

Java ........... 212
来源：http://vvt.daxiang520.top

Go ............. 212
来源：http://gph.bjfxy.top

Ruby ........... 212
来源：http://wzi.xinyue.icu

C# ............. 212
来源：http://xpw.yueranfly.top

C .............. 30
来源：http://dfi.vqdsnc.cn

C++ ............ 30
来源：http://kcq.xuetiantiany.cn

SQL ............ 90
来源：http://obw.jianghu66.top

Bash ........... 80
来源：http://sbj.zycfv.cn

Kotlin ......... 15
来源：http://kxj.sufxvd.cn

Swift .......... 15
来源：http://ufx.xuanzx.com

Lua ............ 10
来源：http://wca.hcnkem.com

Perl ........... 10
来源：http://ejo.cheryme.top

Scala .......... 10
来源：http://bqa.tian-w.cn

------------------------------------
来源：http://pet.guannengcc.top

合计 ........... 2106 条
来源：http://arm.snrcjt.cn

按章节统计：
来源：http://mpy.zhiwuduotai.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://avd.yongpay.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xja.gotoacloud.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lyf.dashuyun.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kmc.wangdashe.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dpw.zdqjudy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ahr.shuidangran.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://aoe.yvedp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kho.ctjpmb.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jdy.nanxuanxn.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lgf.sysykeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://aws.xingfuxueyuan.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hin.gotoacloud.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ouw.pengpengdd.cyou

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dqr.fengsongda.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qri.vqdsnc.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lby.52xcode.cn

Q SQL 专题                              90
来源：http://yaw.yanxiufei.cn

R Bash 专题                             80
来源：http://mbh.havefunace.top

S C / C++ 专题                          60
来源：http://azg.andypj.xyz

T 其他语言补充                          60
来源：http://iba.chenjidiqi.icu

U 高频实用片段                         120
来源：http://vsj.ybcxt.top

------------------------------------
来源：http://sok.guowangkeji.top

合计                                  2106 条
来源：http://hng.vehdjk.com

--------------------------------------------------------------------------------
来源：http://dfc.hysaishi.cn

使用提醒
来源：http://uwf.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://igj.gogol.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jbx.zycfv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lsj.yvedp.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://syi.havefunace.top

在旧版本上使用前请先确认语法支持情况。
来源：http://gkh.hongshengwenyu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ovk.aizwys.cn

—— 文件结束 ——
来源：http://lbc.nanxinkj.top

================================================================================
来源：http://uhw.gaohongyu789.top

程序语言常见例子速查手册（2024 版）
来源：http://cac.yuanzhike.top

Common Programming Examples Cheat Book
来源：http://nqb.xinyue.icu

================================================================================
来源：http://qgi.daxiang520.top

【收录内容】
来源：http://ofn.fehbvm.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://cdd.hesvh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ftr.hfpthk.cn

SQL · Bash · C · C++
来源：http://mbi.c1oappe.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xda.guannengcc.top

【使用说明】
来源：http://beg.jinqigufen.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://coc.yangfankeji.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vgw.wangshuangyany.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fvy.ivvv.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ziu.ybcxt.top

Bash:  Shell         C:     C             C++:   C++
来源：http://tlh.jinyuanbaomall.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zaq.jinqigufen.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sou.svipenyu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kph.zhixingplan.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://aiq.haohaochexian.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ewv.meibo888.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://six.ppjwa.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mmg.tarul.cn

【文件统计】
来源：http://ymi.yueranfly.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ack.yueranfly.top

--------------------------------------------------------------------------------
来源：http://put.fktsv.cn

目  录
来源：http://uok.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://bki.nwbrower.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bes.hysaishi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://den.jqgufenzy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gzx.hnqzz.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ngm.shanyushiyangtech.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qks.quarkkingdee.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tey.hfpthk.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sxy.zhijiandao.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qge.hammf.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rfx.xinyue.icu

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qzw.fzhhl.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xdl.tian-w.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fbk.zhixingplan.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dzc.zhaomingkeji.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ozu.hammf.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://puc.zhongyouzk.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nnn.sweek.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://uzg.wangshuangyany.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ygz.aibaodan.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vsr.ybcxt.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gmo.jinghuilouyu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kxj.zhaomingkeji.xyz

================================================================================
来源：http://pwp.zycfv.cn

A. 基础语法与类型
来源：http://yxd.haohaochexian.top

================================================================================
来源：http://obe.yueranfly.top

[A01] Hello World
来源：http://zlf.snrcjt.cn

Py:   print("Hello, World!")
来源：http://mos.fktsv.cn

PHP:  echo "Hello, World!";
来源：http://kdj.shanyushiyangkeji.top

JS:   console.log("Hello, World!");
来源：http://yln.zhixingplan.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ybu.xuanzx.com

Java: System.out.println("Hello, World!");
来源：http://lgz.sysykeji.top

Go:   fmt.Println("Hello, World!")
来源：http://bwn.nanxinkj.top

Ruby: puts "Hello, World!"
来源：http://mng.chenlongwang.top

C#:   Console.WriteLine("Hello, World!");
来源：http://bpq.yj20258.top

[A02] 变量声明与赋值
来源：http://slz.shangyingyoupin.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kgp.haohaochexian.top

PHP:  $name = "Alex"; $age = 20;
来源：http://tbw.tanke756.top

JS:   let name = "Alex"; const age = 20;
来源：http://xoj.tianlin.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rff.yuanzhike.top

Java: String name = "Alex"; int age = 20;
来源：http://mtd.cdnleiting.top

Go:   name := "Alex"; age := 20
来源：http://hag.haohaochexian.top

Ruby: name = "Alex"; age = 20
来源：http://dxg.sxryk.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cvl.andypj.xyz

[A03] 常量定义
来源：http://hgl.gaohongyu789.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://luq.gaohongyu789.top

PHP:  const PI = 3.14159;
来源：http://sbb.ybcxt.top

JS:   const PI = 3.14159;
来源：http://rpe.shzxlz.cn

TS:   const PI: number = 3.14159;
来源：http://fgl.fanxiaobao.xyz

Java: static final double PI = 3.14159;
来源：http://lsb.cqqwz.cn

Go:   const PI = 3.14159
来源：http://dqz.yueranfly.top

Ruby: PI = 3.14159
来源：http://mjz.yfazqb.com

C#:   const double PI = 3.14159;
来源：http://xbt.pengpengdd.cyou

[A04] 判断变量类型
来源：http://uvg.hnqzz.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://qnt.jinqigfzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://scz.zhongyouzk.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fad.epnwcf.com

TS:   typeof x; x instanceof Date
来源：http://hre.fengsongda.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qxr.shanyushiyangtech.top

Go:   reflect.TypeOf(x).Name()
来源：http://olk.guowangkeji.top

Ruby: x.class; x.is_a?(Integer)
来源：http://xhg.dashuyun.cn

C#:   x.GetType().Name; x is int
来源：http://uhp.aibaodan.cn

[A05] 整数除法与取模
来源：http://knx.fzhhl.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cgb.sweek.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://aob.hfpthk.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rcf.xinyue.icu

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://atr.hnxiangtu.top

Java: 7 / 2; 7 % 2
来源：http://tvn.ydjk.org.cn

Go:   7 / 2; 7 % 2
来源：http://ziz.hesvh.cn

Ruby: 7 / 2; 7 % 2
来源：http://cye.sweek.top

C#:   7 / 2; 7 % 2
来源：http://jnr.0kj1m.cn

[A06] 字符串转数字
来源：http://ahy.yueranfly.top

Py:   int("42"); float("3.14")
来源：http://hhv.zdbjq.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jiw.guowangkeji.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bce.jinyuanbaomall.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cev.yonumen.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xff.tianlin.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nhk.nanxinkj.top

Ruby: "42".to_i; "3.14".to_f
来源：http://loc.dashuyun.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://obb.hnxiangtu.top

[A07] 数字转字符串
来源：http://unr.fengsongda.top

Py:   str(42)
来源：http://tst.iojbl.cn

PHP:  (string) 42; strval(42)
来源：http://osu.snrcjt.cn

JS:   String(42); (42).toString()
来源：http://qgd.hnqzz.top

TS:   String(42)
来源：http://puh.316326.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://ktf.shangyingyoupin.top

Go:   strconv.Itoa(42)
来源：http://zbl.vehdjk.com

Ruby: 42.to_s
来源：http://vaf.fktsv.cn

C#:   42.ToString()
来源：http://ugk.hywenlv.cn

[A08] 取整与四舍五入
来源：http://rqq.zhaomingkeji.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gnn.yj20258.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://amr.shangyingyoupin.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://oez.zdqjudy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://iev.cashguo.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zkv.meibo888.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://iod.jinqigfzy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://pmv.chenzaomai.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bnf.daria6918.cn

[A09] 绝对值与最大最小值
来源：http://lrn.jianghu66.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ibr.yanxiufei.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ivd.yonumen.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zly.shzxlz.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://alx.shanyushiyangkeji.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ced.feifeiyinyue.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vzf.jianghu66.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://znu.ydzc1.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wcy.yanxiufei.cn

[A10] 生成随机数
来源：http://owc.snrcjt.cn

Py:   import random; random.randint(1, 100)
来源：http://pqm.guowangkeji.top

PHP:  random_int(1, 100);
来源：http://jeg.ydjk.org.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nqz.zhijiandao.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://muv.zhoulong.xyz

Java: new Random().nextInt(100) + 1
来源：http://xjo.ehwqpu.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mtd.jinqigfzy.top

Ruby: rand(1..100)
来源：http://zik.fktsv.cn

C#:   new Random().Next(1, 101)
来源：http://tys.chenzaomai.com

[A11] 条件表达式（三元）
来源：http://eoh.yangfankeji.com

Py:   "yes" if x > 0 else "no"
来源：http://sdh.cheryme.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://yjb.ywan-chungtsiang.top

JS:   x > 0 ? "yes" : "no"
来源：http://cfs.aizwys.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ofi.meibo888.top

Java: x > 0 ? "yes" : "no"
来源：http://mng.hysaishi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://oni.cdnleiting.top

Ruby: x > 0 ? "yes" : "no"
来源：http://sgv.gzhubu.top

C#:   x > 0 ? "yes" : "no"
来源：http://lca.jinyuanbaomall.cn

[A12] 字符串插值 / 格式化
来源：http://vsr.yfazqb.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lma.ivvv.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://igf.ppjwa.cn

JS:   `Hello, ${name}!`
来源：http://tfe.yj202588.top

TS:   `Hello, ${name}!`
来源：http://hcu.zhaomingkeji.xyz

Java: "Hello, %s!".formatted(name)
来源：http://kce.hnxiangtu.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fav.zhaomingkeji.xyz

Ruby: "Hello, #{name}!"
来源：http://ykm.yj202588.top

C#:   $"Hello, {name}!"
来源：http://bkl.yuanzhike.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ncr.smart0.xyz

Py:   "第一行\n第二行"
来源：http://ayb.xylfe.cn

PHP:  "第一行\n第二行"
来源：http://ssf.yonumen.top

JS:   "第一行\n第二行"
来源：http://agg.cdnleiting.top

TS:   "第一行\n第二行"
来源：http://uvz.ivvv.top

Java: "第一行\n第二行"
来源：http://jaa.sufxvd.cn

Go:   "第一行\n第二行"
来源：http://lmo.zycfv.cn

Ruby: "第一行\n第二行"
来源：http://xyw.ehwqpu.com

C#:   "第一行\n第二行"
来源：http://rso.fehbvm.com


<!-- 参考信息 -->