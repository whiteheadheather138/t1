代发 wailian999

[U79] PHP：静态分析
来源：http://iwr.jqgfzy.top

composer require --dev phpstan/phpstan
来源：http://ago.bbcook.cn

[U80] PHP：代码规范修复
来源：http://fwl.jqgfzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://kpo.zycfv.cn

[U81] JS：初始化项目
来源：http://ybk.birdmap.top

npm init -y;  npm i express
来源：http://uxc.shanyushiyangtech.top

[U82] JS：package.json 脚本
来源：http://sya.zhengqikj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cvq.yfazqb.com

[U83] JS：ES Module 导入导出
来源：http://dgn.meibo888.top

export const a = 1;  import { a } from "./m.js";
来源：http://pea.cqqwz.cn

[U84] JS：CommonJS 写法
来源：http://ziu.zycfv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wih.yj20258888.top

[U85] JS：可选链
来源：http://tdg.zhoulong.xyz

a?.b?.c
来源：http://hmf.zhoulong.xyz

[U86] JS：空值合并
来源：http://fev.guannengcc.top

a ?? b
来源：http://aha.chenlongwang.top

[U87] JS：解构默认值
来源：http://nrk.chenlongwang.top

const { a = 1, b = 2 } = obj;
来源：http://gme.hesvh.cn

[U88] JS：对象展开合并
来源：http://rqp.sweek.top

{ ...a, ...b }
来源：http://cyx.yanxiufei.cn

[U89] JS：数组去重
来源：http://aus.smart0.xyz

[...new Set(arr)]
来源：http://hnm.chenzaomai.com

[U90] JS：数字数组排序
来源：http://igm.sufxvd.cn

[...arr].sort((a, b) => a - b)
来源：http://pkm.svipenyu.cn

[U91] JS：对象键值遍历
来源：http://pvf.wangdashe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vac.ydzc1.top

[U92] JS：深拷贝
来源：http://fki.pengpengdd.cyou

structuredClone(obj)
来源：http://hps.cheryme.top

[U93] JS：模板字符串
来源：http://tzy.bjfxy.top

`共 ${n} 条`
来源：http://utm.zhiwuduotai.top

[U94] JS：箭头函数
来源：http://hgx.andypj.xyz

const double = x => x * 2;
来源：http://wfc.mhx1999.top

[U95] JS：Promise 包装
来源：http://aap.birdmap.top

new Promise((resolve, reject) => {})
来源：http://khn.kuanghao11.cn

[U96] JS：async/await 与异常
来源：http://ifk.jlsjyb.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uqd.cucudq.cn

[U97] JS：并发请求
来源：http://per.jqgufenzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://eek.fzhhl.top

[U98] JS：fetch 带 JSON
来源：http://ymo.quarkkingdee.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wza.vqdsnc.cn

[U99] JS：事件监听
来源：http://ipg.uphjek.com

el.addEventListener("click", e => {})
来源：http://igu.fzhhl.top

[U100] JS：DOM 查询
来源：http://iur.yvedp.cn

document.querySelector(".item")
来源：http://hzo.sufxvd.cn

[U101] JS：classList 操作
来源：http://nxq.zhijiandao.cn

el.classList.toggle("active")
来源：http://ldn.sweek.top

[U102] JS：本地存储
来源：http://fmn.ywan-chungtsiang.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xmt.tian-w.cn

[U103] JS：定时器
来源：http://kzz.yfazqb.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jra.vqdsnc.cn

[U104] JS：防抖
来源：http://cok.zhiwuduotai.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gcj.hfpthk.cn

[U105] JS：节流
来源：http://xig.xinyue.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ppu.ehwqpu.com

[U106] JS：日期格式化
来源：http://jxt.snrcjt.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fik.vehdjk.com

[U107] JS：数字千分位
来源：http://xhi.dashuyun.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://moi.nwbrower.top

[U108] JS：随机整数
来源：http://esk.kuanghao11.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tjv.yj202588.top

[U109] JS：数组分组
来源：http://nix.sxryk.cn

Object.groupBy(arr, x => x.type)
来源：http://ntk.dashuyun.cn

[U110] JS：数组分块
来源：http://oqk.hfpthk.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qfx.fzhhl.top

[U111] JS：对象转 Map
来源：http://gru.jianghu66.top

new Map(Object.entries(obj))
来源：http://mgd.yj20258888.top

[U112] JS：字符串补位
来源：http://iao.chenjidiqi.icu

"7".padStart(3, "0")
来源：http://zcc.9152youxi.cn

[U113] JS：正则替换全部
来源：http://niy.pengpengdd.cyou

s.replaceAll("a", "b")
来源：http://bis.yuanzhike.top

[U114] JS：JSON 深比较
来源：http://pkf.cheryme.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hmp.nwbrower.top

[U115] JS：生成 UUID
来源：http://lja.fehbvm.com

crypto.randomUUID()
来源：http://vkn.tanke756.top

[U116] JS：类型检查（JSDoc）
来源：http://kbv.yj20258888.top

/** @param {string} name */ function f(name) {}
来源：http://uhx.yj20258.top

[U117] JS：单元测试
来源：http://ese.daria6918.cn

npm i -D vitest;  npx vitest
来源：http://hda.zhixingplan.top

[U118] JS：开发服务器
来源：http://wwy.shzxlz.cn

npm i -D vite;  npx vite
来源：http://blf.zhengqikj.top

[U119] JS：生产构建
来源：http://hxc.jqgfzy.top

npx vite build
来源：http://kbj.xziqi.cn

[U120] JS：读取环境变量（Vite）
来源：http://iny.kuanghao11.cn

import.meta.env.VITE_API_URL
来源：http://cke.chenlongwang.top

================================================================================
来源：http://tix.nanxinkj.top

统计汇总
来源：http://lif.mhx1999.top

================================================================================
来源：http://kfb.hnqzz.top

按语言统计（条）：
来源：http://afh.zhiwuduotai.top

Python ......... 252
来源：http://fkr.gaohongyu789.top

PHP ............ 252
来源：http://hxh.zhaomingkeji.xyz

JavaScript ..... 252
来源：http://cnv.jiagoushi.top

TypeScript ..... 212
来源：http://jhe.yj20258.top

Java ........... 212
来源：http://kla.hnxiangtu.top

Go ............. 212
来源：http://wkw.hesvh.cn

Ruby ........... 212
来源：http://hmc.jinqigfzy.top

C# ............. 212
来源：http://oib.ydzc1.top

C .............. 30
来源：http://dqo.yuanzhike.top

C++ ............ 30
来源：http://fcv.sjlbkw.cn

SQL ............ 90
来源：http://ddh.cdnleiting.top

Bash ........... 80
来源：http://bqe.yuanzhike.top

Kotlin ......... 15
来源：http://yon.hesvh.cn

Swift .......... 15
来源：http://vgf.9152youxi.cn

Lua ............ 10
来源：http://hks.epnwcf.com

Perl ........... 10
来源：http://ldr.birdmap.top

Scala .......... 10
来源：http://rxw.kuanghao11.cn

------------------------------------
来源：http://ncw.feifeiyinyue.top

合计 ........... 2106 条
来源：http://ick.yonumen.top

按章节统计：
来源：http://yph.chenjidiqi.icu

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://klx.zhijiandao.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ugc.fengsongda.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uol.yfazqb.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ajs.fehbvm.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hte.feifeiyinyue.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dhy.yuanzhike.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gow.xingfuxueyuan.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jlq.meibo888.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vfb.fzhhl.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tsi.shuidangran.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://axg.pycfn.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cjh.hywenlv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://isb.cqqwz.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sld.chenzaomai.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kzm.jinqigfzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lpd.daria6918.cn

Q SQL 专题                              90
来源：http://ehw.iojbl.cn

R Bash 专题                             80
来源：http://dtr.ydzc1.top

S C / C++ 专题                          60
来源：http://ekj.jianghu66.top

T 其他语言补充                          60
来源：http://kze.haohaochexian.top

U 高频实用片段                         120
来源：http://ymf.yanxiufei.cn

------------------------------------
来源：http://thr.daria6918.cn

合计                                  2106 条
来源：http://rqt.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://uso.ywan-chungtsiang.top

使用提醒
来源：http://veh.yvedp.cn

--------------------------------------------------------------------------------
来源：http://ahc.cheryme.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fhc.bbcook.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rju.yongpay.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://csh.52xcode.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://lwo.fzhhl.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fis.iojbl.cn

—— 文件结束 ——
来源：http://qok.uphjek.com

================================================================================
来源：http://cno.fanxiaobao.xyz

程序语言常见例子速查手册（2024 版）
来源：http://qmj.vehdjk.com

Common Programming Examples Cheat Book
来源：http://jjf.dianchejie.cn

================================================================================
来源：http://dgb.xziqi.cn

【收录内容】
来源：http://dtu.ctjpmb.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://ank.yj20258.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jxu.shuidangran.top

SQL · Bash · C · C++
来源：http://xmz.hnqzz.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://spt.gaohongyu789.top

【使用说明】
来源：http://mkt.zhengqikj.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ddy.daria6918.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dds.zycfv.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uxh.xylfe.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zbz.yongpay.top

Bash:  Shell         C:     C             C++:   C++
来源：http://zng.shzxlz.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zbl.yfazqb.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qne.kuanghao11.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jpx.bbcook.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qfq.yuxming.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ilw.fehbvm.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kvd.vqdsnc.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fnm.quarkkingdee.top

【文件统计】
来源：http://lpj.yuanzhike.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gzv.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://fgm.sysykeji.top

目  录
来源：http://kyn.havefunace.top

--------------------------------------------------------------------------------
来源：http://lsm.ywan-chungtsiang.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xsf.cdnleiting.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wun.havefunace.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rlc.aibaodan.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mkh.smart0.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wuy.sjlbkw.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jqj.zhijiandao.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fme.hnqzz.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://oqm.fktsv.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vmb.hnqzz.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fvg.guannengcc.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://plo.xylfe.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pml.meibo888.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ion.0kj1m.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ion.jqgufenzy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lvv.chenjidiqi.icu

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lsf.cdnleiting.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ojl.ivvv.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://xyn.nwbrower.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tvi.jinghuilouyu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hyt.nwbrower.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://duq.uphjek.com

================================================================================
来源：http://kak.zhengqikj.top

A. 基础语法与类型
来源：http://dtu.dashuyun.cn

================================================================================
来源：http://ecu.mhx1999.top

[A01] Hello World
来源：http://cat.sufxvd.cn

Py:   print("Hello, World!")
来源：http://dff.iojbl.cn

PHP:  echo "Hello, World!";
来源：http://fit.hcnkem.com

JS:   console.log("Hello, World!");
来源：http://xrq.shzxlz.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nev.yangfankeji.com

Java: System.out.println("Hello, World!");
来源：http://mwk.zdbjq.cn

Go:   fmt.Println("Hello, World!")
来源：http://gra.zhiwuduotai.top

Ruby: puts "Hello, World!"
来源：http://sxo.yvedp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nbh.ehwqpu.com

[A02] 变量声明与赋值
来源：http://rcv.yj202588.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://duj.hcnkem.com

PHP:  $name = "Alex"; $age = 20;
来源：http://fki.jyoumei.cn

JS:   let name = "Alex"; const age = 20;
来源：http://jau.hnxiangtu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vbv.iojbl.cn

Java: String name = "Alex"; int age = 20;
来源：http://vfc.shangyingyoupin.top

Go:   name := "Alex"; age := 20
来源：http://mga.aizwys.cn

Ruby: name = "Alex"; age = 20
来源：http://dzl.meibo888.top

C#:   string name = "Alex"; int age = 20;
来源：http://fny.uphjek.com

[A03] 常量定义
来源：http://aih.fzhhl.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rwo.xingfuxueyuan.xyz

PHP:  const PI = 3.14159;
来源：http://pee.yj20258888.top

JS:   const PI = 3.14159;
来源：http://fzj.dianchejie.cn

TS:   const PI: number = 3.14159;
来源：http://agq.yangfankeji.com

Java: static final double PI = 3.14159;
来源：http://xkx.cqqwz.cn

Go:   const PI = 3.14159
来源：http://ycp.yongpay.top

Ruby: PI = 3.14159
来源：http://dga.xuanzx.com

C#:   const double PI = 3.14159;
来源：http://xdq.smart0.xyz

[A04] 判断变量类型
来源：http://eee.zhixingplan.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://gjy.fehbvm.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vfh.tanke756.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wyx.hongshengwenyu.top

TS:   typeof x; x instanceof Date
来源：http://ekb.hesvh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kdz.zdqjudy.top

Go:   reflect.TypeOf(x).Name()
来源：http://wpe.sufxvd.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tgf.aizwys.cn

C#:   x.GetType().Name; x is int
来源：http://qek.316326.xyz

[A05] 整数除法与取模
来源：http://bse.jinqigfzy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pzc.yvedp.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://bog.316326.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kvj.tianlin.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kag.tianlin.xyz

Java: 7 / 2; 7 % 2
来源：http://tra.epnwcf.com

Go:   7 / 2; 7 % 2
来源：http://amh.yueranfly.top

Ruby: 7 / 2; 7 % 2
来源：http://ovd.bjfxy.top

C#:   7 / 2; 7 % 2
来源：http://sjs.havefunace.top

[A06] 字符串转数字
来源：http://srn.zhaomingkeji.xyz

Py:   int("42"); float("3.14")
来源：http://frk.jqgufenzy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zoz.xingfuxueyuan.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xbh.aizwys.cn

TS:   parseInt("42", 10); Number("42")
来源：http://jdy.epnwcf.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vkq.zhengqikj.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nrv.xylfe.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lcm.jqgfzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://odt.epnwcf.com

[A07] 数字转字符串
来源：http://hhw.hesvh.cn

Py:   str(42)
来源：http://lgt.ydzc1.top

PHP:  (string) 42; strval(42)
来源：http://zjh.quarkkingdee.top

JS:   String(42); (42).toString()
来源：http://rsj.zhongyouzk.top

TS:   String(42)
来源：http://qrb.jyoumei.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qtw.nwbrower.top

Go:   strconv.Itoa(42)
来源：http://jve.yueranfly.top

Ruby: 42.to_s
来源：http://bpr.snrcjt.cn

C#:   42.ToString()
来源：http://buf.ivvv.top

[A08] 取整与四舍五入
来源：http://hfv.jinghuilouyu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://auy.sxryk.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hfh.aizwys.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gmv.bbcook.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://drs.cdnleiting.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ooi.52xcode.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fxn.xuanzx.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://giw.yj202588.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hlc.shzxlz.cn

[A09] 绝对值与最大最小值
来源：http://dyh.gzhubu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gbw.ppjwa.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://iom.dianchejie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://enb.tarul.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hao.wangdashe.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gbk.hongshengwenyu.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nfs.c1oappe.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qkr.jyoumei.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rkn.316326.xyz

[A10] 生成随机数
来源：http://nwn.jyoumei.cn

Py:   import random; random.randint(1, 100)
来源：http://ycn.bjfxy.top

PHP:  random_int(1, 100);
来源：http://dsl.hesvh.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ili.hnqzz.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jug.xingfuxueyuan.xyz

Java: new Random().nextInt(100) + 1
来源：http://emf.yueranfly.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ddc.svipenyu.cn

Ruby: rand(1..100)
来源：http://rbc.ydzc1.top

C#:   new Random().Next(1, 101)
来源：http://gci.hfpthk.cn

[A11] 条件表达式（三元）
来源：http://eet.yj202588.top

Py:   "yes" if x > 0 else "no"
来源：http://dgb.xylfe.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ufd.yj20258888.top

JS:   x > 0 ? "yes" : "no"
来源：http://jku.jianghu66.top

TS:   x > 0 ? "yes" : "no"
来源：http://wpf.sxryk.cn

Java: x > 0 ? "yes" : "no"
来源：http://qkf.zhixingplan.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ewf.zhongyouzk.top

Ruby: x > 0 ? "yes" : "no"
来源：http://qyu.quarkkingdee.top

C#:   x > 0 ? "yes" : "no"
来源：http://ibc.ivvv.top

[A12] 字符串插值 / 格式化
来源：http://eze.jinqigufen.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fmu.yanxiufei.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://irq.yuxming.cn

JS:   `Hello, ${name}!`
来源：http://hox.zhijiandao.cn

TS:   `Hello, ${name}!`
来源：http://xuw.svipenyu.cn

Java: "Hello, %s!".formatted(name)
来源：http://iio.fehbvm.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wjm.fanxiaobao.xyz

Ruby: "Hello, #{name}!"
来源：http://kxv.zdbjq.cn

C#:   $"Hello, {name}!"
来源：http://hcz.cheryme.top

[A13] 多行字符串（练习 \n 转义）
来源：http://qqy.zhixingplan.top


<!-- 参考信息 -->