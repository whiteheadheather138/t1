代发 wailian999

[U79] PHP：静态分析
来源：http://ibp.yj20258.top

composer require --dev phpstan/phpstan
来源：http://uqq.yueranfly.top

[U80] PHP：代码规范修复
来源：http://ved.gzhubu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://uyl.vqdsnc.cn

[U81] JS：初始化项目
来源：http://gpj.shzxlz.cn

npm init -y;  npm i express
来源：http://hny.jinqigufen.top

[U82] JS：package.json 脚本
来源：http://tdh.jinqigufen.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://enp.nanxinkj.top

[U83] JS：ES Module 导入导出
来源：http://rbd.hammf.cn

export const a = 1;  import { a } from "./m.js";
来源：http://znn.zhixingplan.top

[U84] JS：CommonJS 写法
来源：http://mcs.ydjk.org.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pxs.xuetiantiany.cn

[U85] JS：可选链
来源：http://vfe.c1oappe.top

a?.b?.c
来源：http://npu.birdmap.top

[U86] JS：空值合并
来源：http://uyd.vehdjk.com

a ?? b
来源：http://qfd.yvedp.cn

[U87] JS：解构默认值
来源：http://yzw.yangfankeji.com

const { a = 1, b = 2 } = obj;
来源：http://pdm.xingfuxueyuan.xyz

[U88] JS：对象展开合并
来源：http://vht.0kj1m.cn

{ ...a, ...b }
来源：http://ktm.fzhhl.top

[U89] JS：数组去重
来源：http://vwh.aibaodan.cn

[...new Set(arr)]
来源：http://apm.bbcook.cn

[U90] JS：数字数组排序
来源：http://mhu.316326.xyz

[...arr].sort((a, b) => a - b)
来源：http://zga.meibo888.top

[U91] JS：对象键值遍历
来源：http://jnl.hfpthk.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ycs.nanxinkj.top

[U92] JS：深拷贝
来源：http://apa.zhaomingkeji.xyz

structuredClone(obj)
来源：http://jfw.sysykeji.top

[U93] JS：模板字符串
来源：http://vtp.zycfv.cn

`共 ${n} 条`
来源：http://lna.yfazqb.com

[U94] JS：箭头函数
来源：http://hgg.ywan-chungtsiang.top

const double = x => x * 2;
来源：http://sul.shanyushiyangkeji.top

[U95] JS：Promise 包装
来源：http://mjf.gotoacloud.top

new Promise((resolve, reject) => {})
来源：http://wlx.pengpengdd.cyou

[U96] JS：async/await 与异常
来源：http://nrd.andypj.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xsk.zhijiandao.cn

[U97] JS：并发请求
来源：http://koy.hnxiangtu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://eqs.zhixingplan.top

[U98] JS：fetch 带 JSON
来源：http://tpk.feifeiyinyue.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dgd.epnwcf.com

[U99] JS：事件监听
来源：http://but.iojbl.cn

el.addEventListener("click", e => {})
来源：http://wmg.shuidangran.top

[U100] JS：DOM 查询
来源：http://uir.shuidangran.top

document.querySelector(".item")
来源：http://oym.hammf.cn

[U101] JS：classList 操作
来源：http://rst.daria6918.cn

el.classList.toggle("active")
来源：http://bem.zhixingplan.top

[U102] JS：本地存储
来源：http://ftz.hammf.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ype.sysykeji.top

[U103] JS：定时器
来源：http://iih.xuanzx.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nnq.zhaomingkeji.xyz

[U104] JS：防抖
来源：http://kvd.hesvh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://avz.yj202588.top

[U105] JS：节流
来源：http://pwn.zhengqikj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oky.316326.xyz

[U106] JS：日期格式化
来源：http://gbl.jinqigufen.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fvk.feifeiyinyue.top

[U107] JS：数字千分位
来源：http://xcn.zhoulong.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ado.zhengqikj.top

[U108] JS：随机整数
来源：http://czh.yj20258888.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kby.yongpay.top

[U109] JS：数组分组
来源：http://tch.uphjek.com

Object.groupBy(arr, x => x.type)
来源：http://jwg.ydjk.org.cn

[U110] JS：数组分块
来源：http://tkd.yfazqb.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ygv.hywenlv.cn

[U111] JS：对象转 Map
来源：http://elh.cqqwz.cn

new Map(Object.entries(obj))
来源：http://cnj.xingfuxueyuan.xyz

[U112] JS：字符串补位
来源：http://ptv.yj20258888.top

"7".padStart(3, "0")
来源：http://klr.pengpengdd.cyou

[U113] JS：正则替换全部
来源：http://juw.iojbl.cn

s.replaceAll("a", "b")
来源：http://jhk.xuanzx.com

[U114] JS：JSON 深比较
来源：http://syl.havefunace.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://vsw.ppjwa.cn

[U115] JS：生成 UUID
来源：http://ouo.iojbl.cn

crypto.randomUUID()
来源：http://unc.ctjpmb.com

[U116] JS：类型检查（JSDoc）
来源：http://iin.aizwys.cn

/** @param {string} name */ function f(name) {}
来源：http://rmi.yonumen.top

[U117] JS：单元测试
来源：http://twj.shangyingyoupin.top

npm i -D vitest;  npx vitest
来源：http://yhw.birdmap.top

[U118] JS：开发服务器
来源：http://xsk.ydjk.org.cn

npm i -D vite;  npx vite
来源：http://pjh.meibo888.top

[U119] JS：生产构建
来源：http://ovh.svipenyu.cn

npx vite build
来源：http://xix.yj20258.top

[U120] JS：读取环境变量（Vite）
来源：http://jbp.zycfv.cn

import.meta.env.VITE_API_URL
来源：http://ecd.epnwcf.com

================================================================================
来源：http://cjm.fzhhl.top

统计汇总
来源：http://ocl.hcnkem.com

================================================================================
来源：http://bkh.aibaodan.cn

按语言统计（条）：
来源：http://zse.aizwys.cn

Python ......... 252
来源：http://vhg.guowangkeji.top

PHP ............ 252
来源：http://guv.quarkkingdee.top

JavaScript ..... 252
来源：http://hru.redwolf501.top

TypeScript ..... 212
来源：http://bmf.dianchejie.cn

Java ........... 212
来源：http://chq.pycfn.com

Go ............. 212
来源：http://txq.guowangkeji.top

Ruby ........... 212
来源：http://hhx.jinghuilouyu.cn

C# ............. 212
来源：http://spb.havefunace.top

C .............. 30
来源：http://agk.yuxming.cn

C++ ............ 30
来源：http://giw.epnwcf.com

SQL ............ 90
来源：http://doy.yvedp.cn

Bash ........... 80
来源：http://glc.zhijiandao.cn

Kotlin ......... 15
来源：http://rtf.dianchejie.cn

Swift .......... 15
来源：http://rzk.ybcxt.top

Lua ............ 10
来源：http://bue.dashuyun.cn

Perl ........... 10
来源：http://hfm.cucudq.cn

Scala .......... 10
来源：http://jty.shanyushiyangkeji.top

------------------------------------
来源：http://hdm.xuetiantiany.cn

合计 ........... 2106 条
来源：http://xmo.hcnkem.com

按章节统计：
来源：http://ehn.vehdjk.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yqk.zhixingplan.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bxr.dashuyun.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oal.316326.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fif.chenjidiqi.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vze.jiagoushi.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jtl.wangdashe.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yze.yueranfly.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pph.gotoacloud.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jzx.ivvv.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gam.sxryk.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hdx.ywan-chungtsiang.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qaq.pycfn.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ikc.vehdjk.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://eep.xinyue.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lbb.yj20258.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ycw.jianghu66.top

Q SQL 专题                              90
来源：http://oca.fengsongda.top

R Bash 专题                             80
来源：http://pxo.cdnleiting.top

S C / C++ 专题                          60
来源：http://jjv.316326.xyz

T 其他语言补充                          60
来源：http://fxp.shanyushiyangkeji.top

U 高频实用片段                         120
来源：http://xeg.xingfuxueyuan.xyz

------------------------------------
来源：http://nrw.yj20258.top

合计                                  2106 条
来源：http://wld.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://qed.wangshuangyany.cn

使用提醒
来源：http://ufe.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://giz.hcnkem.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mls.chenzaomai.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sgl.zhijiandao.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://euc.iojbl.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wen.ybcxt.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pvx.shanyushiyangkeji.top

—— 文件结束 ——
来源：http://snx.xuanzx.com

================================================================================
来源：http://qaa.gzhubu.top

程序语言常见例子速查手册（2024 版）
来源：http://eao.chenlongwang.top

Common Programming Examples Cheat Book
来源：http://tud.gaohongyu789.top

================================================================================
来源：http://xxp.gaohongyu789.top

【收录内容】
来源：http://ivr.fehbvm.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://edj.haohaochexian.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qwl.tanke756.top

SQL · Bash · C · C++
来源：http://gkl.wangshuangyany.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://eqw.ctjpmb.com

【使用说明】
来源：http://ale.hcnkem.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bef.yj20258888.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nor.chenlongwang.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hdq.shanyushiyangkeji.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://die.xylfe.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://emh.uphjek.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tsr.tarul.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qqo.shanyushiyangkeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qec.shuidangran.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lly.andypj.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ohl.fanxiaobao.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zic.hongshengwenyu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vuq.sweek.top

【文件统计】
来源：http://thk.fzhhl.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://but.hesvh.cn

--------------------------------------------------------------------------------
来源：http://zow.pycfn.com

目  录
来源：http://sdu.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://lqv.c1oappe.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xdr.ybcxt.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xiu.shangyingyoupin.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ubj.yanxiufei.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ytr.jlsjyb.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://snm.mhx1999.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://abg.zhixingplan.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://skm.guowangkeji.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wtl.sjlbkw.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://llw.daxiang520.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://psl.sxryk.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://oyc.sxryk.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ioq.xingfuxueyuan.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pvx.andypj.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kem.sweek.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rlr.nanxinkj.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bsz.ehwqpu.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ypu.guannengcc.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://dnl.xylfe.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bvs.ybcxt.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bft.havefunace.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wzg.snrcjt.cn

================================================================================
来源：http://qiw.pengpengdd.cyou

A. 基础语法与类型
来源：http://kcc.yvedp.cn

================================================================================
来源：http://zgr.ybcxt.top

[A01] Hello World
来源：http://ruq.hywenlv.cn

Py:   print("Hello, World!")
来源：http://rsl.yj202588.top

PHP:  echo "Hello, World!";
来源：http://yrs.gotoacloud.top

JS:   console.log("Hello, World!");
来源：http://pou.xuanzx.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pxx.tianlin.xyz

Java: System.out.println("Hello, World!");
来源：http://oza.gaohongyu789.top

Go:   fmt.Println("Hello, World!")
来源：http://dty.tianlin.xyz

Ruby: puts "Hello, World!"
来源：http://giq.svipenyu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://dxc.fehbvm.com

[A02] 变量声明与赋值
来源：http://ziq.hywenlv.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ifb.jlsjyb.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://llq.xuetiantiany.cn

JS:   let name = "Alex"; const age = 20;
来源：http://kkb.zycfv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kyj.xuanzx.com

Java: String name = "Alex"; int age = 20;
来源：http://rch.daxiang520.top

Go:   name := "Alex"; age := 20
来源：http://otn.fehbvm.com

Ruby: name = "Alex"; age = 20
来源：http://skn.yonumen.top

C#:   string name = "Alex"; int age = 20;
来源：http://rrm.guannengcc.top

[A03] 常量定义
来源：http://dhs.smart0.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://iil.daria6918.cn

PHP:  const PI = 3.14159;
来源：http://dtr.kuanghao11.cn

JS:   const PI = 3.14159;
来源：http://hra.jinyuanbaomall.cn

TS:   const PI: number = 3.14159;
来源：http://ggn.daxiang520.top

Java: static final double PI = 3.14159;
来源：http://kdh.xziqi.cn

Go:   const PI = 3.14159
来源：http://zfs.sjlbkw.cn

Ruby: PI = 3.14159
来源：http://fyi.chenjidiqi.icu

C#:   const double PI = 3.14159;
来源：http://pan.jlsjyb.cn

[A04] 判断变量类型
来源：http://euk.hongshengwenyu.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://fbz.gogol.net.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tpp.ppjwa.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yfp.yanxiufei.cn

TS:   typeof x; x instanceof Date
来源：http://nmz.ydjk.org.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kyk.zhoulong.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://zgm.ydjk.org.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lgm.jyoumei.cn

C#:   x.GetType().Name; x is int
来源：http://vbd.sufxvd.cn

[A05] 整数除法与取模
来源：http://qmj.fengsongda.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hsm.jyoumei.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://nal.tian-w.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bac.guannengcc.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qrf.xuetiantiany.cn

Java: 7 / 2; 7 % 2
来源：http://ilx.nanxinkj.top

Go:   7 / 2; 7 % 2
来源：http://itf.nanxinkj.top

Ruby: 7 / 2; 7 % 2
来源：http://tax.yj202588.top

C#:   7 / 2; 7 % 2
来源：http://hdn.cashguo.top

[A06] 字符串转数字
来源：http://xvj.xziqi.cn

Py:   int("42"); float("3.14")
来源：http://rjb.iojbl.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hfu.jqgfzy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ngb.zhoulong.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://uer.kuanghao11.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://etf.vehdjk.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tqd.pycfn.com

Ruby: "42".to_i; "3.14".to_f
来源：http://ruz.fzhhl.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mkp.hnqzz.top

[A07] 数字转字符串
来源：http://pqg.hywenlv.cn

Py:   str(42)
来源：http://pds.yangfankeji.com

PHP:  (string) 42; strval(42)
来源：http://ihu.aibaodan.cn

JS:   String(42); (42).toString()
来源：http://tph.birdmap.top

TS:   String(42)
来源：http://rbs.fzhhl.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://jac.haohaochexian.top

Go:   strconv.Itoa(42)
来源：http://qcc.chenjidiqi.icu

Ruby: 42.to_s
来源：http://fgg.yueranfly.top

C#:   42.ToString()
来源：http://hij.gzhubu.top

[A08] 取整与四舍五入
来源：http://flq.hammf.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hrk.0kj1m.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nou.cashguo.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vdy.tian-w.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hhu.cheryme.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pen.ydzc1.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zdx.jqgfzy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://zmd.zhijiandao.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cev.chenjidiqi.icu

[A09] 绝对值与最大最小值
来源：http://ddo.ehwqpu.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://sxq.pycfn.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://imm.aizwys.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://iwk.tianlin.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ijg.jinqigfzy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nui.9152youxi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zqz.ppjwa.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bas.xylfe.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fyi.xingfuxueyuan.xyz

[A10] 生成随机数
来源：http://fgy.yonumen.top

Py:   import random; random.randint(1, 100)
来源：http://thw.chenjidiqi.icu

PHP:  random_int(1, 100);
来源：http://ctu.yangfankeji.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ytt.gzhubu.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bxg.smart0.xyz

Java: new Random().nextInt(100) + 1
来源：http://gta.yangfankeji.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wni.wangshuangyany.cn

Ruby: rand(1..100)
来源：http://ziq.xziqi.cn

C#:   new Random().Next(1, 101)
来源：http://tyu.smart0.xyz

[A11] 条件表达式（三元）
来源：http://awm.chenjidiqi.icu

Py:   "yes" if x > 0 else "no"
来源：http://css.zhaomingkeji.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://fqx.guowangkeji.top

JS:   x > 0 ? "yes" : "no"
来源：http://sxf.feifeiyinyue.top

TS:   x > 0 ? "yes" : "no"
来源：http://rnd.yonumen.top

Java: x > 0 ? "yes" : "no"
来源：http://osn.pengpengdd.cyou

Go:   // 无三元运算符，需用 if 语句
来源：http://eof.iojbl.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hud.shanyushiyangtech.top

C#:   x > 0 ? "yes" : "no"
来源：http://btq.hongshengwenyu.top

[A12] 字符串插值 / 格式化
来源：http://xpw.wangdashe.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jom.wangdashe.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ovz.daria6918.cn

JS:   `Hello, ${name}!`
来源：http://tvm.fktsv.cn

TS:   `Hello, ${name}!`
来源：http://vsj.xinyue.icu

Java: "Hello, %s!".formatted(name)
来源：http://qze.mhx1999.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ajw.kuanghao11.cn

Ruby: "Hello, #{name}!"
来源：http://wif.wangdashe.top

C#:   $"Hello, {name}!"
来源：http://oxn.9152youxi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://iqx.bjfxy.top


<!-- 参考信息 -->