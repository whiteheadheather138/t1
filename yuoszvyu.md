代发 wailian999

[U79] PHP：静态分析
来源：http://fdy.jinqigfzy.top

composer require --dev phpstan/phpstan
来源：http://uwm.ctjpmb.com

[U80] PHP：代码规范修复
来源：http://dfc.wangshuangyany.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zys.jinghuilouyu.cn

[U81] JS：初始化项目
来源：http://hfe.yj20258888.top

npm init -y;  npm i express
来源：http://wxo.cashguo.top

[U82] JS：package.json 脚本
来源：http://vsh.hywenlv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://krp.birdmap.top

[U83] JS：ES Module 导入导出
来源：http://tyt.jinyuanbaomall.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wkt.shanyushiyangkeji.top

[U84] JS：CommonJS 写法
来源：http://yop.zhongyouzk.top

module.exports = { a };  const { a } = require("./m");
来源：http://xlg.svipenyu.cn

[U85] JS：可选链
来源：http://dlm.daxiang520.top

a?.b?.c
来源：http://mvm.316326.xyz

[U86] JS：空值合并
来源：http://ekn.yuxming.cn

a ?? b
来源：http://tdf.zdbjq.cn

[U87] JS：解构默认值
来源：http://iop.havefunace.top

const { a = 1, b = 2 } = obj;
来源：http://ojj.yangfankeji.com

[U88] JS：对象展开合并
来源：http://xqs.nanxuanxn.top

{ ...a, ...b }
来源：http://xfm.epnwcf.com

[U89] JS：数组去重
来源：http://skw.uphjek.com

[...new Set(arr)]
来源：http://nsa.sysykeji.top

[U90] JS：数字数组排序
来源：http://ztr.iojbl.cn

[...arr].sort((a, b) => a - b)
来源：http://uby.xylfe.cn

[U91] JS：对象键值遍历
来源：http://vvm.aizwys.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qfm.9152youxi.cn

[U92] JS：深拷贝
来源：http://usc.chenjidiqi.icu

structuredClone(obj)
来源：http://mov.ybcxt.top

[U93] JS：模板字符串
来源：http://rdv.shuidangran.top

`共 ${n} 条`
来源：http://uio.pengpengdd.cyou

[U94] JS：箭头函数
来源：http://rft.jqgufenzy.top

const double = x => x * 2;
来源：http://jrz.fengsongda.top

[U95] JS：Promise 包装
来源：http://utm.hongshengwenyu.top

new Promise((resolve, reject) => {})
来源：http://bwi.hesvh.cn

[U96] JS：async/await 与异常
来源：http://upc.shanyushiyangtech.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vmj.gaohongyu789.top

[U97] JS：并发请求
来源：http://gvj.xingfuxueyuan.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://oep.xinyue.icu

[U98] JS：fetch 带 JSON
来源：http://efo.sufxvd.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://iqc.vqdsnc.cn

[U99] JS：事件监听
来源：http://vsg.gotoacloud.top

el.addEventListener("click", e => {})
来源：http://tlr.aizwys.cn

[U100] JS：DOM 查询
来源：http://ahj.cucudq.cn

document.querySelector(".item")
来源：http://ofe.shangyingyoupin.top

[U101] JS：classList 操作
来源：http://rny.xuanzx.com

el.classList.toggle("active")
来源：http://dxj.nanxinkj.top

[U102] JS：本地存储
来源：http://uoh.316326.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://nvh.iojbl.cn

[U103] JS：定时器
来源：http://gtf.yfazqb.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rbi.zhiwuduotai.top

[U104] JS：防抖
来源：http://ngn.guannengcc.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jdr.jinyuanbaomall.cn

[U105] JS：节流
来源：http://dvu.uphjek.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yea.ydjk.org.cn

[U106] JS：日期格式化
来源：http://vrh.zhixingplan.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hya.yuanzhike.top

[U107] JS：数字千分位
来源：http://ldj.aizwys.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cmz.hnxiangtu.top

[U108] JS：随机整数
来源：http://ldq.wangshuangyany.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zja.hywenlv.cn

[U109] JS：数组分组
来源：http://fai.0kj1m.cn

Object.groupBy(arr, x => x.type)
来源：http://ofp.hammf.cn

[U110] JS：数组分块
来源：http://fow.dianchejie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fxo.zhiwuduotai.top

[U111] JS：对象转 Map
来源：http://ckv.shangyingyoupin.top

new Map(Object.entries(obj))
来源：http://mvb.xziqi.cn

[U112] JS：字符串补位
来源：http://skf.zhengqikj.top

"7".padStart(3, "0")
来源：http://igy.haohaochexian.top

[U113] JS：正则替换全部
来源：http://acu.jianghu66.top

s.replaceAll("a", "b")
来源：http://wuz.ivvv.top

[U114] JS：JSON 深比较
来源：http://dix.hfpthk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hrk.fehbvm.com

[U115] JS：生成 UUID
来源：http://snh.snrcjt.cn

crypto.randomUUID()
来源：http://hfl.ydzc1.top

[U116] JS：类型检查（JSDoc）
来源：http://zal.havefunace.top

/** @param {string} name */ function f(name) {}
来源：http://qam.gogol.net.cn

[U117] JS：单元测试
来源：http://eev.ywan-chungtsiang.top

npm i -D vitest;  npx vitest
来源：http://kce.zhijiandao.cn

[U118] JS：开发服务器
来源：http://xkp.wangdashe.top

npm i -D vite;  npx vite
来源：http://djl.jqgufenzy.top

[U119] JS：生产构建
来源：http://lqs.jinqigufen.top

npx vite build
来源：http://gmi.xuanzx.com

[U120] JS：读取环境变量（Vite）
来源：http://wiu.yfazqb.com

import.meta.env.VITE_API_URL
来源：http://csl.pengpengdd.cyou

================================================================================
来源：http://zhz.meibo888.top

统计汇总
来源：http://foe.chenjidiqi.icu

================================================================================
来源：http://zgn.shanyushiyangkeji.top

按语言统计（条）：
来源：http://gcw.wangdashe.top

Python ......... 252
来源：http://ngp.wangdashe.top

PHP ............ 252
来源：http://dfv.wangshuangyany.cn

JavaScript ..... 252
来源：http://atx.fanxiaobao.xyz

TypeScript ..... 212
来源：http://ijt.shuidangran.top

Java ........... 212
来源：http://flr.gzhubu.top

Go ............. 212
来源：http://wgo.nanxuanxn.top

Ruby ........... 212
来源：http://dqg.xylfe.cn

C# ............. 212
来源：http://vai.zdqjudy.top

C .............. 30
来源：http://ymq.hfpthk.cn

C++ ............ 30
来源：http://bun.daxiang520.top

SQL ............ 90
来源：http://mtf.cashguo.top

Bash ........... 80
来源：http://xyl.hysaishi.cn

Kotlin ......... 15
来源：http://xsj.aizwys.cn

Swift .......... 15
来源：http://mvl.pycfn.com

Lua ............ 10
来源：http://ezw.andypj.xyz

Perl ........... 10
来源：http://gya.jinghuilouyu.cn

Scala .......... 10
来源：http://rbp.andypj.xyz

------------------------------------
来源：http://vsc.shanyushiyangtech.top

合计 ........... 2106 条
来源：http://fwv.sufxvd.cn

按章节统计：
来源：http://wfo.feifeiyinyue.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pna.zhiwuduotai.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nuu.hnqzz.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zzx.nanxinkj.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ykz.gaohongyu789.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oej.chenjidiqi.icu

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://oni.shangyingyoupin.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pws.ctjpmb.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ubw.vqdsnc.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nis.xinyue.icu

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vct.xuetiantiany.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fkk.hnqzz.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nce.iojbl.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vmk.jiagoushi.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fhn.gogol.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://klz.birdmap.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://frm.ctjpmb.com

Q SQL 专题                              90
来源：http://ygx.guannengcc.top

R Bash 专题                             80
来源：http://zdz.hesvh.cn

S C / C++ 专题                          60
来源：http://wsi.shuidangran.top

T 其他语言补充                          60
来源：http://xre.shzxlz.cn

U 高频实用片段                         120
来源：http://mjj.cheryme.top

------------------------------------
来源：http://uky.jyoumei.cn

合计                                  2106 条
来源：http://zkb.fzhhl.top

--------------------------------------------------------------------------------
来源：http://abg.wangdashe.top

使用提醒
来源：http://lft.yvedp.cn

--------------------------------------------------------------------------------
来源：http://slv.zhiwuduotai.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bqz.epnwcf.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://scq.meibo888.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://utc.jqgufenzy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://khg.meibo888.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wxb.ehwqpu.com

—— 文件结束 ——
来源：http://bls.aibaodan.cn

================================================================================
来源：http://oqu.vqdsnc.cn

程序语言常见例子速查手册（2024 版）
来源：http://dok.nanxuanxn.top

Common Programming Examples Cheat Book
来源：http://ssh.chenlongwang.top

================================================================================
来源：http://kbk.wangdashe.top

【收录内容】
来源：http://nex.epnwcf.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://yee.mhx1999.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://efv.haohaochexian.top

SQL · Bash · C · C++
来源：http://qqe.yj20258.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rql.yj20258888.top

【使用说明】
来源：http://qta.cheryme.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vfe.ehwqpu.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://djc.cashguo.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sdy.yanxiufei.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mzn.tianlin.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://pjw.hongshengwenyu.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pdx.zhiwuduotai.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://oms.gotoacloud.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pcz.dashuyun.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fhd.jinghuilouyu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://egw.hnqzz.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://iih.nwbrower.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://iiu.chenlongwang.top

【文件统计】
来源：http://wgi.redwolf501.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mrc.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://fja.zdbjq.cn

目  录
来源：http://mor.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://fxa.zhixingplan.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://edf.fehbvm.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zcj.zhixingplan.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bil.fehbvm.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fuv.shanyushiyangkeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tgc.iojbl.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://skf.ppjwa.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bok.jinyuanbaomall.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ggm.c1oappe.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://emv.andypj.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bwn.sysykeji.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pgb.hfpthk.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ohe.fehbvm.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pna.yj20258.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kid.ctjpmb.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wdm.svipenyu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vvi.yanxiufei.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fas.pengpengdd.cyou

R. Bash 专题                   （第 18 节，80 条）
来源：http://iwi.aizwys.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vdu.chenjidiqi.icu

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pik.bbcook.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yxw.chenzaomai.com

================================================================================
来源：http://njv.mhx1999.top

A. 基础语法与类型
来源：http://oqu.kuanghao11.cn

================================================================================
来源：http://gyf.cheryme.top

[A01] Hello World
来源：http://ilp.wangshuangyany.cn

Py:   print("Hello, World!")
来源：http://amq.zhengqikj.top

PHP:  echo "Hello, World!";
来源：http://xbq.birdmap.top

JS:   console.log("Hello, World!");
来源：http://jnq.meibo888.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bsm.aibaodan.cn

Java: System.out.println("Hello, World!");
来源：http://yii.bjfxy.top

Go:   fmt.Println("Hello, World!")
来源：http://wim.bjfxy.top

Ruby: puts "Hello, World!"
来源：http://tfe.fktsv.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://bpg.tianlin.xyz

[A02] 变量声明与赋值
来源：http://uii.daria6918.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mtj.c1oappe.top

PHP:  $name = "Alex"; $age = 20;
来源：http://slt.hysaishi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ttj.fehbvm.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cyq.xylfe.cn

Java: String name = "Alex"; int age = 20;
来源：http://tid.redwolf501.top

Go:   name := "Alex"; age := 20
来源：http://gam.mhx1999.top

Ruby: name = "Alex"; age = 20
来源：http://sty.feifeiyinyue.top

C#:   string name = "Alex"; int age = 20;
来源：http://zbu.316326.xyz

[A03] 常量定义
来源：http://xqr.xuanzx.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fqu.fanxiaobao.xyz

PHP:  const PI = 3.14159;
来源：http://urn.kuanghao11.cn

JS:   const PI = 3.14159;
来源：http://kha.pycfn.com

TS:   const PI: number = 3.14159;
来源：http://nrl.jqgufenzy.top

Java: static final double PI = 3.14159;
来源：http://gta.zhoulong.xyz

Go:   const PI = 3.14159
来源：http://mcz.yuanzhike.top

Ruby: PI = 3.14159
来源：http://crm.bbcook.cn

C#:   const double PI = 3.14159;
来源：http://sgr.tianlin.xyz

[A04] 判断变量类型
来源：http://rcp.xylfe.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gaq.c1oappe.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ihw.zhoulong.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://upo.uphjek.com

TS:   typeof x; x instanceof Date
来源：http://csp.yueranfly.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ckj.svipenyu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ubf.jinqigfzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://unk.ydjk.org.cn

C#:   x.GetType().Name; x is int
来源：http://plm.jlsjyb.cn

[A05] 整数除法与取模
来源：http://hps.zhaomingkeji.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kfx.gotoacloud.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://lcz.c1oappe.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kdt.zhaomingkeji.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://efl.birdmap.top

Java: 7 / 2; 7 % 2
来源：http://jva.iojbl.cn

Go:   7 / 2; 7 % 2
来源：http://ckj.gaohongyu789.top

Ruby: 7 / 2; 7 % 2
来源：http://wsr.0kj1m.cn

C#:   7 / 2; 7 % 2
来源：http://wly.jiagoushi.top

[A06] 字符串转数字
来源：http://jlb.bbcook.cn

Py:   int("42"); float("3.14")
来源：http://rlg.haohaochexian.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nxd.sxryk.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mwp.tanke756.top

TS:   parseInt("42", 10); Number("42")
来源：http://prj.shanyushiyangkeji.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rib.feifeiyinyue.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hge.iojbl.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hun.c1oappe.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xro.tianlin.xyz

[A07] 数字转字符串
来源：http://slp.daria6918.cn

Py:   str(42)
来源：http://ait.zhengqikj.top

PHP:  (string) 42; strval(42)
来源：http://guh.yanxiufei.cn

JS:   String(42); (42).toString()
来源：http://qkx.fktsv.cn

TS:   String(42)
来源：http://yts.wangdashe.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://hjp.zhoulong.xyz

Go:   strconv.Itoa(42)
来源：http://zve.jqgfzy.top

Ruby: 42.to_s
来源：http://xnf.xingfuxueyuan.xyz

C#:   42.ToString()
来源：http://hlf.uphjek.com

[A08] 取整与四舍五入
来源：http://amp.dianchejie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://koh.cheryme.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ied.zdbjq.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bxq.guowangkeji.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://oxv.yvedp.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pjt.hnqzz.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rlu.wangdashe.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://rpu.andypj.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://haq.hongshengwenyu.top

[A09] 绝对值与最大最小值
来源：http://lcg.zhiwuduotai.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://izp.zhijiandao.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ztu.sufxvd.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tpn.vehdjk.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cya.yj20258888.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tfr.zhixingplan.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rvn.redwolf501.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ghr.aibaodan.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bvq.sweek.top

[A10] 生成随机数
来源：http://zwj.yvedp.cn

Py:   import random; random.randint(1, 100)
来源：http://nex.zhongyouzk.top

PHP:  random_int(1, 100);
来源：http://ngr.cqqwz.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uev.0kj1m.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vet.yuanzhike.top

Java: new Random().nextInt(100) + 1
来源：http://pds.shanyushiyangkeji.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://quo.yfazqb.com

Ruby: rand(1..100)
来源：http://gbj.zdbjq.cn

C#:   new Random().Next(1, 101)
来源：http://yll.wangdashe.top

[A11] 条件表达式（三元）
来源：http://yzm.ybcxt.top

Py:   "yes" if x > 0 else "no"
来源：http://aha.52xcode.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://emu.fzhhl.top

JS:   x > 0 ? "yes" : "no"
来源：http://nyw.aizwys.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hzx.zhijiandao.cn

Java: x > 0 ? "yes" : "no"
来源：http://thi.sysykeji.top

Go:   // 无三元运算符，需用 if 语句
来源：http://qfo.ybcxt.top

Ruby: x > 0 ? "yes" : "no"
来源：http://emh.birdmap.top

C#:   x > 0 ? "yes" : "no"
来源：http://uge.sufxvd.cn

[A12] 字符串插值 / 格式化
来源：http://hvx.gotoacloud.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rtk.yonumen.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hhs.sysykeji.top

JS:   `Hello, ${name}!`
来源：http://dye.cdnleiting.top

TS:   `Hello, ${name}!`
来源：http://qiz.guowangkeji.top

Java: "Hello, %s!".formatted(name)
来源：http://vgs.shzxlz.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jyu.nwbrower.top

Ruby: "Hello, #{name}!"
来源：http://kgj.daria6918.cn

C#:   $"Hello, {name}!"
来源：http://usc.zycfv.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://foe.sufxvd.cn


<!-- 参考信息 -->