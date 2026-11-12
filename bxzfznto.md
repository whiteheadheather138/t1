代发 wailian999

[U77] PHP：模板渲染
来源：http://iea.shzxlz.cn

composer require twig/twig
来源：http://uaz.daria6918.cn

[U78] PHP：单元测试
来源：http://jgi.feifeiyinyue.top

composer require --dev phpunit/phpunit
来源：http://tux.hongshengwenyu.top

[U79] PHP：静态分析
来源：http://yjn.hysaishi.cn

composer require --dev phpstan/phpstan
来源：http://iqf.iojbl.cn

[U80] PHP：代码规范修复
来源：http://wgq.sweek.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://pza.ppjwa.cn

[U81] JS：初始化项目
来源：http://qzr.ppjwa.cn

npm init -y;  npm i express
来源：http://gvw.tianlin.xyz

[U82] JS：package.json 脚本
来源：http://uoi.smart0.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fvd.ydzc1.top

[U83] JS：ES Module 导入导出
来源：http://hoh.tian-w.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ahr.ywan-chungtsiang.top

[U84] JS：CommonJS 写法
来源：http://cur.xuanzx.com

module.exports = { a };  const { a } = require("./m");
来源：http://pob.cqqwz.cn

[U85] JS：可选链
来源：http://jbq.chenzaomai.com

a?.b?.c
来源：http://jnf.bbcook.cn

[U86] JS：空值合并
来源：http://nma.hfpthk.cn

a ?? b
来源：http://osg.ppjwa.cn

[U87] JS：解构默认值
来源：http://fxv.svipenyu.cn

const { a = 1, b = 2 } = obj;
来源：http://rti.epnwcf.com

[U88] JS：对象展开合并
来源：http://cjr.yongpay.top

{ ...a, ...b }
来源：http://jby.vqdsnc.cn

[U89] JS：数组去重
来源：http://jnd.ctjpmb.com

[...new Set(arr)]
来源：http://fry.yuxming.cn

[U90] JS：数字数组排序
来源：http://cqt.yuxming.cn

[...arr].sort((a, b) => a - b)
来源：http://ucg.gogol.net.cn

[U91] JS：对象键值遍历
来源：http://cln.xziqi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dic.meibo888.top

[U92] JS：深拷贝
来源：http://udd.kuanghao11.cn

structuredClone(obj)
来源：http://iip.ybcxt.top

[U93] JS：模板字符串
来源：http://xvu.redwolf501.top

`共 ${n} 条`
来源：http://ouc.iojbl.cn

[U94] JS：箭头函数
来源：http://odh.52xcode.cn

const double = x => x * 2;
来源：http://muu.xziqi.cn

[U95] JS：Promise 包装
来源：http://eec.feifeiyinyue.top

new Promise((resolve, reject) => {})
来源：http://vsk.wangdashe.top

[U96] JS：async/await 与异常
来源：http://kkw.9152youxi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sqx.zhoulong.xyz

[U97] JS：并发请求
来源：http://ubd.0kj1m.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://avr.zhiwuduotai.top

[U98] JS：fetch 带 JSON
来源：http://moi.zycfv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://htf.fktsv.cn

[U99] JS：事件监听
来源：http://udg.snrcjt.cn

el.addEventListener("click", e => {})
来源：http://mgb.jqgfzy.top

[U100] JS：DOM 查询
来源：http://hru.epnwcf.com

document.querySelector(".item")
来源：http://aks.yonumen.top

[U101] JS：classList 操作
来源：http://pon.9152youxi.cn

el.classList.toggle("active")
来源：http://lyk.fktsv.cn

[U102] JS：本地存储
来源：http://onx.cheryme.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://pil.jqgufenzy.top

[U103] JS：定时器
来源：http://eec.hcnkem.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mlg.hammf.cn

[U104] JS：防抖
来源：http://jmk.hammf.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wfc.meibo888.top

[U105] JS：节流
来源：http://bqs.iojbl.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lmn.ydjk.org.cn

[U106] JS：日期格式化
来源：http://hxd.ywan-chungtsiang.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nmz.epnwcf.com

[U107] JS：数字千分位
来源：http://ywg.zycfv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mou.yj202588.top

[U108] JS：随机整数
来源：http://rgn.shangyingyoupin.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qyn.yanxiufei.cn

[U109] JS：数组分组
来源：http://ozm.hammf.cn

Object.groupBy(arr, x => x.type)
来源：http://sie.jlsjyb.cn

[U110] JS：数组分块
来源：http://mqi.fehbvm.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uaj.hysaishi.cn

[U111] JS：对象转 Map
来源：http://bby.aibaodan.cn

new Map(Object.entries(obj))
来源：http://hlx.cashguo.top

[U112] JS：字符串补位
来源：http://uaw.gzhubu.top

"7".padStart(3, "0")
来源：http://fuv.yfazqb.com

[U113] JS：正则替换全部
来源：http://tpi.tanke756.top

s.replaceAll("a", "b")
来源：http://dak.zhixingplan.top

[U114] JS：JSON 深比较
来源：http://cqn.jqgfzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://grj.meibo888.top

[U115] JS：生成 UUID
来源：http://yzm.zhaomingkeji.xyz

crypto.randomUUID()
来源：http://jnf.nwbrower.top

[U116] JS：类型检查（JSDoc）
来源：http://bgg.bjfxy.top

/** @param {string} name */ function f(name) {}
来源：http://kbl.aibaodan.cn

[U117] JS：单元测试
来源：http://khw.yj20258888.top

npm i -D vitest;  npx vitest
来源：http://vin.hesvh.cn

[U118] JS：开发服务器
来源：http://qep.quarkkingdee.top

npm i -D vite;  npx vite
来源：http://wmj.ctjpmb.com

[U119] JS：生产构建
来源：http://gko.vehdjk.com

npx vite build
来源：http://fxw.jlsjyb.cn

[U120] JS：读取环境变量（Vite）
来源：http://anm.vehdjk.com

import.meta.env.VITE_API_URL
来源：http://jyi.fzhhl.top

================================================================================
来源：http://cws.ppjwa.cn

统计汇总
来源：http://aro.jinghuilouyu.cn

================================================================================
来源：http://azp.yuxming.cn

按语言统计（条）：
来源：http://hwb.gaohongyu789.top

Python ......... 252
来源：http://gsd.dashuyun.cn

PHP ............ 252
来源：http://cpr.tian-w.cn

JavaScript ..... 252
来源：http://qxj.vehdjk.com

TypeScript ..... 212
来源：http://zvy.xingfuxueyuan.xyz

Java ........... 212
来源：http://yat.yangfankeji.com

Go ............. 212
来源：http://gyl.xuanzx.com

Ruby ........... 212
来源：http://bxl.zhoulong.xyz

C# ............. 212
来源：http://hsi.gogol.net.cn

C .............. 30
来源：http://lku.fanxiaobao.xyz

C++ ............ 30
来源：http://sxl.jqgfzy.top

SQL ............ 90
来源：http://pxx.sweek.top

Bash ........... 80
来源：http://ctt.cqqwz.cn

Kotlin ......... 15
来源：http://jjg.jinghuilouyu.cn

Swift .......... 15
来源：http://lhl.jiagoushi.top

Lua ............ 10
来源：http://jse.ywan-chungtsiang.top

Perl ........... 10
来源：http://ylt.ppjwa.cn

Scala .......... 10
来源：http://yja.jiagoushi.top

------------------------------------
来源：http://ypb.9152youxi.cn

合计 ........... 2106 条
来源：http://gzv.hfpthk.cn

按章节统计：
来源：http://xst.fengsongda.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://phn.cheryme.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lun.0kj1m.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ukx.fanxiaobao.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://onb.aizwys.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lxa.ivvv.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wfb.gotoacloud.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bds.pengpengdd.cyou

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wnr.dianchejie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gly.hnqzz.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://iuk.sjlbkw.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dji.wangdashe.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hqn.jianghu66.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ymv.chenjidiqi.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pny.zhijiandao.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ici.vqdsnc.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://krr.jianghu66.top

Q SQL 专题                              90
来源：http://fyw.sufxvd.cn

R Bash 专题                             80
来源：http://hut.gaohongyu789.top

S C / C++ 专题                          60
来源：http://azm.gotoacloud.top

T 其他语言补充                          60
来源：http://kqg.zhengqikj.top

U 高频实用片段                         120
来源：http://ryo.chenjidiqi.icu

------------------------------------
来源：http://uhr.epnwcf.com

合计                                  2106 条
来源：http://fwq.daria6918.cn

--------------------------------------------------------------------------------
来源：http://rac.aibaodan.cn

使用提醒
来源：http://uql.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://shw.hywenlv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jbt.fehbvm.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://azi.ybcxt.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cya.sweek.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jsm.yfazqb.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fmf.epnwcf.com

—— 文件结束 ——
来源：http://ltt.jiagoushi.top

================================================================================
来源：http://yid.52xcode.cn

程序语言常见例子速查手册（2024 版）
来源：http://zwr.jlsjyb.cn

Common Programming Examples Cheat Book
来源：http://wab.cqqwz.cn

================================================================================
来源：http://scc.havefunace.top

【收录内容】
来源：http://bxj.dashuyun.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://enk.xziqi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nxs.dashuyun.cn

SQL · Bash · C · C++
来源：http://rly.shuidangran.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cpr.fehbvm.com

【使用说明】
来源：http://roh.epnwcf.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tma.xylfe.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://owy.yj20258888.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fwp.bbcook.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fyu.feifeiyinyue.top

Bash:  Shell         C:     C             C++:   C++
来源：http://qvz.c1oappe.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bpf.hnxiangtu.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xib.ivvv.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ujl.jinghuilouyu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rxm.guannengcc.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lrv.daria6918.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ucd.xylfe.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zee.jianghu66.top

【文件统计】
来源：http://vsz.yuxming.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fjs.meibo888.top

--------------------------------------------------------------------------------
来源：http://afl.guannengcc.top

目  录
来源：http://qwy.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://tuk.zhengqikj.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pqn.jinghuilouyu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://smd.ybcxt.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ysn.andypj.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xpd.yanxiufei.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://djn.aibaodan.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cqd.birdmap.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hrj.chenlongwang.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hea.daxiang520.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hsc.quarkkingdee.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qwv.vqdsnc.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xhn.jinghuilouyu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pjp.chenzaomai.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lfn.sjlbkw.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cbn.zhiwuduotai.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cbl.hysaishi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nac.yj20258.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hzh.bjfxy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://yun.meibo888.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zjd.sysykeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://act.zdqjudy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gqo.316326.xyz

================================================================================
来源：http://hzw.nanxuanxn.top

A. 基础语法与类型
来源：http://orc.birdmap.top

================================================================================
来源：http://mjl.shuidangran.top

[A01] Hello World
来源：http://ocr.fzhhl.top

Py:   print("Hello, World!")
来源：http://rxy.zhiwuduotai.top

PHP:  echo "Hello, World!";
来源：http://ovt.hesvh.cn

JS:   console.log("Hello, World!");
来源：http://wos.0kj1m.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gjg.shuidangran.top

Java: System.out.println("Hello, World!");
来源：http://unm.iojbl.cn

Go:   fmt.Println("Hello, World!")
来源：http://wnw.52xcode.cn

Ruby: puts "Hello, World!"
来源：http://dmp.pengpengdd.cyou

C#:   Console.WriteLine("Hello, World!");
来源：http://rmr.cqqwz.cn

[A02] 变量声明与赋值
来源：http://tdt.yuanzhike.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fpu.0kj1m.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mjz.yuxming.cn

JS:   let name = "Alex"; const age = 20;
来源：http://rdr.epnwcf.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vcz.52xcode.cn

Java: String name = "Alex"; int age = 20;
来源：http://snl.cucudq.cn

Go:   name := "Alex"; age := 20
来源：http://ogq.tanke756.top

Ruby: name = "Alex"; age = 20
来源：http://efg.hnqzz.top

C#:   string name = "Alex"; int age = 20;
来源：http://fxx.hnqzz.top

[A03] 常量定义
来源：http://idw.andypj.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qhf.gotoacloud.top

PHP:  const PI = 3.14159;
来源：http://mkd.fanxiaobao.xyz

JS:   const PI = 3.14159;
来源：http://zrf.nanxuanxn.top

TS:   const PI: number = 3.14159;
来源：http://odq.xingfuxueyuan.xyz

Java: static final double PI = 3.14159;
来源：http://nhh.yvedp.cn

Go:   const PI = 3.14159
来源：http://vtt.cdnleiting.top

Ruby: PI = 3.14159
来源：http://tnw.ivvv.top

C#:   const double PI = 3.14159;
来源：http://utx.yuanzhike.top

[A04] 判断变量类型
来源：http://rjq.yuxming.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://iul.pycfn.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rnj.uphjek.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zmi.yfazqb.com

TS:   typeof x; x instanceof Date
来源：http://cfd.zycfv.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fux.epnwcf.com

Go:   reflect.TypeOf(x).Name()
来源：http://yjl.jinqigfzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ubg.shanyushiyangkeji.top

C#:   x.GetType().Name; x is int
来源：http://nyo.fehbvm.com

[A05] 整数除法与取模
来源：http://crw.daria6918.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vfl.yuanzhike.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://gvf.ppjwa.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zzk.jinghuilouyu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://btl.cheryme.top

Java: 7 / 2; 7 % 2
来源：http://vzb.pengpengdd.cyou

Go:   7 / 2; 7 % 2
来源：http://yht.zhiwuduotai.top

Ruby: 7 / 2; 7 % 2
来源：http://exw.tian-w.cn

C#:   7 / 2; 7 % 2
来源：http://bzm.xziqi.cn

[A06] 字符串转数字
来源：http://rex.guannengcc.top

Py:   int("42"); float("3.14")
来源：http://roo.jianghu66.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://elb.cheryme.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://muy.tarul.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ltq.xinyue.icu

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yuq.ydzc1.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kba.yj20258.top

Ruby: "42".to_i; "3.14".to_f
来源：http://fln.sufxvd.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://oru.smart0.xyz

[A07] 数字转字符串
来源：http://qsm.316326.xyz

Py:   str(42)
来源：http://ttm.hfpthk.cn

PHP:  (string) 42; strval(42)
来源：http://cna.iojbl.cn

JS:   String(42); (42).toString()
来源：http://zer.aibaodan.cn

TS:   String(42)
来源：http://lme.jqgufenzy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ogn.zycfv.cn

Go:   strconv.Itoa(42)
来源：http://doq.xinyue.icu

Ruby: 42.to_s
来源：http://fyr.hammf.cn

C#:   42.ToString()
来源：http://fdg.andypj.xyz

[A08] 取整与四舍五入
来源：http://ckg.gzhubu.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://syp.tian-w.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ffu.nwbrower.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://btv.cdnleiting.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ulb.gzhubu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yun.chenjidiqi.icu

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kmq.hcnkem.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://aif.meibo888.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://weu.yuxming.cn

[A09] 绝对值与最大最小值
来源：http://kww.yonumen.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wfr.zdqjudy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://swr.xuetiantiany.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cyp.yuxming.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yaa.guannengcc.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gvo.9152youxi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ofj.xuanzx.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://htx.jianghu66.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lsh.ppjwa.cn

[A10] 生成随机数
来源：http://pwv.cheryme.top

Py:   import random; random.randint(1, 100)
来源：http://bfc.shuidangran.top

PHP:  random_int(1, 100);
来源：http://mtd.redwolf501.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qyj.quarkkingdee.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rlo.shanyushiyangtech.top

Java: new Random().nextInt(100) + 1
来源：http://wkh.xuetiantiany.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lna.zhongyouzk.top

Ruby: rand(1..100)
来源：http://xni.hammf.cn

C#:   new Random().Next(1, 101)
来源：http://ymi.snrcjt.cn

[A11] 条件表达式（三元）
来源：http://hvc.zhiwuduotai.top

Py:   "yes" if x > 0 else "no"
来源：http://kpx.yfazqb.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://dkf.jinghuilouyu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://nui.sxryk.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bjr.nwbrower.top

Java: x > 0 ? "yes" : "no"
来源：http://yjr.aibaodan.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ufo.316326.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://uid.tianlin.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://hbc.dashuyun.cn

[A12] 字符串插值 / 格式化
来源：http://bqf.zhijiandao.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jok.yangfankeji.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sge.fehbvm.com

JS:   `Hello, ${name}!`
来源：http://weq.sweek.top

TS:   `Hello, ${name}!`
来源：http://tsn.yvedp.cn

Java: "Hello, %s!".formatted(name)
来源：http://noo.dashuyun.cn


<!-- 参考信息 -->