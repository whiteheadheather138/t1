代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://zyb.redwolf501.top

export const a = 1;  import { a } from "./m.js";
来源：http://jjy.jinqigufen.top

[U84] JS：CommonJS 写法
来源：http://fgh.shuidangran.top

module.exports = { a };  const { a } = require("./m");
来源：http://xix.hammf.cn

[U85] JS：可选链
来源：http://vnk.shangyingyoupin.top

a?.b?.c
来源：http://jeu.shuidangran.top

[U86] JS：空值合并
来源：http://skn.daxiang520.top

a ?? b
来源：http://srq.wangdashe.top

[U87] JS：解构默认值
来源：http://viq.hongshengwenyu.top

const { a = 1, b = 2 } = obj;
来源：http://ybo.guowangkeji.top

[U88] JS：对象展开合并
来源：http://ucb.yangfankeji.com

{ ...a, ...b }
来源：http://zpc.ybcxt.top

[U89] JS：数组去重
来源：http://jkp.c1oappe.top

[...new Set(arr)]
来源：http://ofu.hnxiangtu.top

[U90] JS：数字数组排序
来源：http://ydh.gogol.net.cn

[...arr].sort((a, b) => a - b)
来源：http://hij.yuanzhike.top

[U91] JS：对象键值遍历
来源：http://pdp.gaohongyu789.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zpt.yfazqb.com

[U92] JS：深拷贝
来源：http://mxm.shanyushiyangkeji.top

structuredClone(obj)
来源：http://wfd.yanxiufei.cn

[U93] JS：模板字符串
来源：http://zji.shuidangran.top

`共 ${n} 条`
来源：http://wsm.bjfxy.top

[U94] JS：箭头函数
来源：http://mbx.xinyue.icu

const double = x => x * 2;
来源：http://lvm.birdmap.top

[U95] JS：Promise 包装
来源：http://mhu.bbcook.cn

new Promise((resolve, reject) => {})
来源：http://tzg.shanyushiyangtech.top

[U96] JS：async/await 与异常
来源：http://jaz.guannengcc.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dau.shangyingyoupin.top

[U97] JS：并发请求
来源：http://yyn.birdmap.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://idz.tian-w.cn

[U98] JS：fetch 带 JSON
来源：http://qvc.daria6918.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nig.tarul.cn

[U99] JS：事件监听
来源：http://thd.shanyushiyangkeji.top

el.addEventListener("click", e => {})
来源：http://tru.zhongyouzk.top

[U100] JS：DOM 查询
来源：http://yrs.cqqwz.cn

document.querySelector(".item")
来源：http://aky.epnwcf.com

[U101] JS：classList 操作
来源：http://cvz.shuidangran.top

el.classList.toggle("active")
来源：http://fnm.316326.xyz

[U102] JS：本地存储
来源：http://bcl.shanyushiyangkeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://twf.fktsv.cn

[U103] JS：定时器
来源：http://zbe.wangshuangyany.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uff.hcnkem.com

[U104] JS：防抖
来源：http://vsy.fehbvm.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lxt.shzxlz.cn

[U105] JS：节流
来源：http://kur.ivvv.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://riq.meibo888.top

[U106] JS：日期格式化
来源：http://eyq.chenjidiqi.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xui.fzhhl.top

[U107] JS：数字千分位
来源：http://uoo.c1oappe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kfw.xziqi.cn

[U108] JS：随机整数
来源：http://uux.ydzc1.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hxh.vqdsnc.cn

[U109] JS：数组分组
来源：http://tqj.gaohongyu789.top

Object.groupBy(arr, x => x.type)
来源：http://nmb.jinghuilouyu.cn

[U110] JS：数组分块
来源：http://udt.shzxlz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oix.wangdashe.top

[U111] JS：对象转 Map
来源：http://pst.chenlongwang.top

new Map(Object.entries(obj))
来源：http://ynd.zhixingplan.top

[U112] JS：字符串补位
来源：http://ewc.zhoulong.xyz

"7".padStart(3, "0")
来源：http://hhf.tian-w.cn

[U113] JS：正则替换全部
来源：http://qsa.ehwqpu.com

s.replaceAll("a", "b")
来源：http://osc.shangyingyoupin.top

[U114] JS：JSON 深比较
来源：http://qcf.cheryme.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hpt.shuidangran.top

[U115] JS：生成 UUID
来源：http://zmw.guowangkeji.top

crypto.randomUUID()
来源：http://dbk.zhixingplan.top

[U116] JS：类型检查（JSDoc）
来源：http://ooe.feifeiyinyue.top

/** @param {string} name */ function f(name) {}
来源：http://twt.yangfankeji.com

[U117] JS：单元测试
来源：http://dpz.xuanzx.com

npm i -D vitest;  npx vitest
来源：http://zyi.yj20258888.top

[U118] JS：开发服务器
来源：http://xno.gogol.net.cn

npm i -D vite;  npx vite
来源：http://yuo.yj20258.top

[U119] JS：生产构建
来源：http://knb.tarul.cn

npx vite build
来源：http://ijm.gogol.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://eqr.redwolf501.top

import.meta.env.VITE_API_URL
来源：http://lkv.c1oappe.top

================================================================================
来源：http://rdi.chenzaomai.com

统计汇总
来源：http://leg.chenlongwang.top

================================================================================
来源：http://odd.xuanzx.com

按语言统计（条）：
来源：http://mfv.sweek.top

Python ......... 252
来源：http://zal.zhoulong.xyz

PHP ............ 252
来源：http://oma.yj20258888.top

JavaScript ..... 252
来源：http://nnj.aizwys.cn

TypeScript ..... 212
来源：http://ank.birdmap.top

Java ........... 212
来源：http://iia.bbcook.cn

Go ............. 212
来源：http://xoi.sufxvd.cn

Ruby ........... 212
来源：http://hkf.jinghuilouyu.cn

C# ............. 212
来源：http://fem.yj20258888.top

C .............. 30
来源：http://ldo.ydjk.org.cn

C++ ............ 30
来源：http://rew.kuanghao11.cn

SQL ............ 90
来源：http://kdd.ydzc1.top

Bash ........... 80
来源：http://gts.aizwys.cn

Kotlin ......... 15
来源：http://pwp.yanxiufei.cn

Swift .......... 15
来源：http://jir.xingfuxueyuan.xyz

Lua ............ 10
来源：http://jzc.hongshengwenyu.top

Perl ........... 10
来源：http://drq.hfpthk.cn

Scala .......... 10
来源：http://qos.yueranfly.top

------------------------------------
来源：http://xgs.jinqigufen.top

合计 ........... 2106 条
来源：http://pzu.hammf.cn

按章节统计：
来源：http://xnf.tarul.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fkb.zhixingplan.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wkd.jiagoushi.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ljc.zhiwuduotai.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jfg.zycfv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://doa.jqgfzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gpy.vehdjk.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wuu.jyoumei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gtd.jqgufenzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://whv.yuanzhike.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yqr.shzxlz.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kfu.tianlin.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nee.jinqigfzy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://glr.hysaishi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yer.fanxiaobao.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gdb.mhx1999.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wgx.ydjk.org.cn

Q SQL 专题                              90
来源：http://niy.yuanzhike.top

R Bash 专题                             80
来源：http://eda.aizwys.cn

S C / C++ 专题                          60
来源：http://hri.fzhhl.top

T 其他语言补充                          60
来源：http://dlg.aibaodan.cn

U 高频实用片段                         120
来源：http://yxf.guannengcc.top

------------------------------------
来源：http://kzq.quarkkingdee.top

合计                                  2106 条
来源：http://rlg.cheryme.top

--------------------------------------------------------------------------------
来源：http://oyy.andypj.xyz

使用提醒
来源：http://ysf.tian-w.cn

--------------------------------------------------------------------------------
来源：http://hsh.yj20258888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qkg.gotoacloud.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vcy.chenlongwang.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jpq.redwolf501.top

在旧版本上使用前请先确认语法支持情况。
来源：http://xam.gaohongyu789.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://uig.ivvv.top

—— 文件结束 ——
来源：http://qnx.havefunace.top

================================================================================
来源：http://kli.hywenlv.cn

程序语言常见例子速查手册（2024 版）
来源：http://uog.jinyuanbaomall.cn

Common Programming Examples Cheat Book
来源：http://but.wangshuangyany.cn

================================================================================
来源：http://qbj.guannengcc.top

【收录内容】
来源：http://hav.yangfankeji.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://mza.sxryk.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nxz.jianghu66.top

SQL · Bash · C · C++
来源：http://nwm.yj20258.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://iho.xuanzx.com

【使用说明】
来源：http://dku.gzhubu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qkg.tarul.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ugf.shuidangran.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ire.hesvh.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gnu.bjfxy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://wbi.jinyuanbaomall.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gvi.hesvh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wtl.jyoumei.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://opt.cheryme.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yip.zhiwuduotai.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lps.havefunace.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zmb.0kj1m.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zqe.ehwqpu.com

【文件统计】
来源：http://mfv.pycfn.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dcg.tanke756.top

--------------------------------------------------------------------------------
来源：http://clm.316326.xyz

目  录
来源：http://jcd.xylfe.cn

--------------------------------------------------------------------------------
来源：http://jdq.wangdashe.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bbw.jlsjyb.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wpu.bbcook.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bnw.pengpengdd.cyou

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xpm.meibo888.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ozq.guannengcc.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hof.xylfe.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zzl.jinqigufen.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yli.aibaodan.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ghj.jqgfzy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wcd.aibaodan.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dnj.yueranfly.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uzl.jqgufenzy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://iav.hnxiangtu.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://uvt.xziqi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pkv.hfpthk.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bdk.daria6918.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kns.shzxlz.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bot.chenzaomai.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bjx.fehbvm.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ckx.wangdashe.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ujp.zhixingplan.top

================================================================================
来源：http://fbs.andypj.xyz

A. 基础语法与类型
来源：http://ppj.yanxiufei.cn

================================================================================
来源：http://shu.zhixingplan.top

[A01] Hello World
来源：http://lmc.pycfn.com

Py:   print("Hello, World!")
来源：http://wqr.tarul.cn

PHP:  echo "Hello, World!";
来源：http://nmr.shanyushiyangtech.top

JS:   console.log("Hello, World!");
来源：http://uwg.cqqwz.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mzs.cashguo.top

Java: System.out.println("Hello, World!");
来源：http://amn.wangshuangyany.cn

Go:   fmt.Println("Hello, World!")
来源：http://kuz.vehdjk.com

Ruby: puts "Hello, World!"
来源：http://qjg.xinyue.icu

C#:   Console.WriteLine("Hello, World!");
来源：http://utt.xinyue.icu

[A02] 变量声明与赋值
来源：http://znq.sysykeji.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kxx.fktsv.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bwo.fehbvm.com

JS:   let name = "Alex"; const age = 20;
来源：http://chu.zhijiandao.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qtb.chenlongwang.top

Java: String name = "Alex"; int age = 20;
来源：http://hbo.gzhubu.top

Go:   name := "Alex"; age := 20
来源：http://bfc.xziqi.cn

Ruby: name = "Alex"; age = 20
来源：http://bhb.zdbjq.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rwj.ivvv.top

[A03] 常量定义
来源：http://fjt.zhixingplan.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zrt.jinyuanbaomall.cn

PHP:  const PI = 3.14159;
来源：http://fqy.chenzaomai.com

JS:   const PI = 3.14159;
来源：http://pbp.haohaochexian.top

TS:   const PI: number = 3.14159;
来源：http://cks.iojbl.cn

Java: static final double PI = 3.14159;
来源：http://njd.yj202588.top

Go:   const PI = 3.14159
来源：http://adb.hywenlv.cn

Ruby: PI = 3.14159
来源：http://gry.yuanzhike.top

C#:   const double PI = 3.14159;
来源：http://hns.fktsv.cn

[A04] 判断变量类型
来源：http://wlj.guannengcc.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://bqt.pycfn.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xzf.ivvv.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://eed.haohaochexian.top

TS:   typeof x; x instanceof Date
来源：http://aad.fktsv.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://txn.tian-w.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rom.haohaochexian.top

Ruby: x.class; x.is_a?(Integer)
来源：http://hvt.kuanghao11.cn

C#:   x.GetType().Name; x is int
来源：http://ftr.fanxiaobao.xyz

[A05] 整数除法与取模
来源：http://hnf.zdqjudy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ydw.zhijiandao.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://yvu.hnqzz.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gco.feifeiyinyue.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qgg.svipenyu.cn

Java: 7 / 2; 7 % 2
来源：http://bbi.xziqi.cn

Go:   7 / 2; 7 % 2
来源：http://tth.snrcjt.cn

Ruby: 7 / 2; 7 % 2
来源：http://zgb.fehbvm.com

C#:   7 / 2; 7 % 2
来源：http://wjt.iojbl.cn

[A06] 字符串转数字
来源：http://sga.shangyingyoupin.top

Py:   int("42"); float("3.14")
来源：http://ksa.dianchejie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gfv.pengpengdd.cyou

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fme.tarul.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kit.sjlbkw.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lgv.yonumen.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://eac.jinyuanbaomall.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://uwc.chenjidiqi.icu

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mbn.ppjwa.cn

[A07] 数字转字符串
来源：http://glz.yuxming.cn

Py:   str(42)
来源：http://als.xuetiantiany.cn

PHP:  (string) 42; strval(42)
来源：http://oio.gzhubu.top

JS:   String(42); (42).toString()
来源：http://agc.redwolf501.top

TS:   String(42)
来源：http://hmv.xuetiantiany.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fkr.316326.xyz

Go:   strconv.Itoa(42)
来源：http://fmw.mhx1999.top

Ruby: 42.to_s
来源：http://tgt.zhiwuduotai.top

C#:   42.ToString()
来源：http://qrl.cheryme.top

[A08] 取整与四舍五入
来源：http://huv.fktsv.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ptb.zhoulong.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cny.yongpay.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://evm.fzhhl.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://izh.hcnkem.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ldn.jiagoushi.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xwr.xingfuxueyuan.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://xgq.xylfe.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xjb.9152youxi.cn

[A09] 绝对值与最大最小值
来源：http://caa.epnwcf.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ipj.nanxuanxn.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://egj.sysykeji.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://iay.zhixingplan.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fyk.hcnkem.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://usx.shzxlz.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gex.gzhubu.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tua.meibo888.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zve.yuanzhike.top

[A10] 生成随机数
来源：http://dza.hongshengwenyu.top

Py:   import random; random.randint(1, 100)
来源：http://xbe.zhiwuduotai.top

PHP:  random_int(1, 100);
来源：http://fhc.guowangkeji.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wxx.nanxinkj.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uoz.cashguo.top

Java: new Random().nextInt(100) + 1
来源：http://rmj.cqqwz.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lhy.guowangkeji.top

Ruby: rand(1..100)
来源：http://oft.ppjwa.cn

C#:   new Random().Next(1, 101)
来源：http://ubv.xuanzx.com

[A11] 条件表达式（三元）
来源：http://zzh.xuanzx.com

Py:   "yes" if x > 0 else "no"
来源：http://qro.pengpengdd.cyou

PHP:  $x > 0 ? "yes" : "no"
来源：http://vqy.yanxiufei.cn

JS:   x > 0 ? "yes" : "no"
来源：http://lvm.jianghu66.top

TS:   x > 0 ? "yes" : "no"
来源：http://udb.ehwqpu.com

Java: x > 0 ? "yes" : "no"
来源：http://omx.0kj1m.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://lqr.fehbvm.com

Ruby: x > 0 ? "yes" : "no"
来源：http://tob.redwolf501.top

C#:   x > 0 ? "yes" : "no"
来源：http://tqs.hesvh.cn

[A12] 字符串插值 / 格式化
来源：http://ncn.zhengqikj.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lnt.gzhubu.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cba.gogol.net.cn

JS:   `Hello, ${name}!`
来源：http://gwo.sysykeji.top

TS:   `Hello, ${name}!`
来源：http://wmg.jqgfzy.top

Java: "Hello, %s!".formatted(name)
来源：http://wey.ywan-chungtsiang.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://oke.dianchejie.cn

Ruby: "Hello, #{name}!"
来源：http://tgw.zhengqikj.top

C#:   $"Hello, {name}!"
来源：http://wrp.nanxinkj.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ild.daxiang520.top

Py:   "第一行\n第二行"
来源：http://rpe.jinghuilouyu.cn

PHP:  "第一行\n第二行"
来源：http://nix.yj202588.top

JS:   "第一行\n第二行"
来源：http://jtx.birdmap.top

TS:   "第一行\n第二行"
来源：http://fiy.guowangkeji.top

Java: "第一行\n第二行"
来源：http://ueg.havefunace.top

Go:   "第一行\n第二行"
来源：http://syy.tarul.cn

Ruby: "第一行\n第二行"
来源：http://lbc.tanke756.top

C#:   "第一行\n第二行"
来源：http://pba.yangfankeji.com


<!-- 参考信息 -->