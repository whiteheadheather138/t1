代发 wailian999

[U75] PHP：依赖注入
来源：http://gpw.dashuyun.cn

composer require psr/container
来源：http://gcj.havefunace.top

[U76] PHP：简单路由
来源：http://cqf.zdqjudy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zdi.redwolf501.top

[U77] PHP：模板渲染
来源：http://bks.xinyue.icu

composer require twig/twig
来源：http://zfz.pengpengdd.cyou

[U78] PHP：单元测试
来源：http://uwh.zycfv.cn

composer require --dev phpunit/phpunit
来源：http://fwz.yj202588.top

[U79] PHP：静态分析
来源：http://hnt.haohaochexian.top

composer require --dev phpstan/phpstan
来源：http://mhr.snrcjt.cn

[U80] PHP：代码规范修复
来源：http://fqn.zhixingplan.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://uny.9152youxi.cn

[U81] JS：初始化项目
来源：http://xcj.jqgfzy.top

npm init -y;  npm i express
来源：http://fqd.ehwqpu.com

[U82] JS：package.json 脚本
来源：http://ynk.zdqjudy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ume.yvedp.cn

[U83] JS：ES Module 导入导出
来源：http://dzu.ivvv.top

export const a = 1;  import { a } from "./m.js";
来源：http://phu.xuetiantiany.cn

[U84] JS：CommonJS 写法
来源：http://oxi.kuanghao11.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jvb.gogol.net.cn

[U85] JS：可选链
来源：http://hgc.daria6918.cn

a?.b?.c
来源：http://ebd.xingfuxueyuan.xyz

[U86] JS：空值合并
来源：http://bjb.ehwqpu.com

a ?? b
来源：http://irs.yfazqb.com

[U87] JS：解构默认值
来源：http://ptd.dianchejie.cn

const { a = 1, b = 2 } = obj;
来源：http://hoi.shanyushiyangkeji.top

[U88] JS：对象展开合并
来源：http://uyj.cashguo.top

{ ...a, ...b }
来源：http://doh.quarkkingdee.top

[U89] JS：数组去重
来源：http://rjy.yfazqb.com

[...new Set(arr)]
来源：http://scr.feifeiyinyue.top

[U90] JS：数字数组排序
来源：http://luo.jqgfzy.top

[...arr].sort((a, b) => a - b)
来源：http://vwk.xuetiantiany.cn

[U91] JS：对象键值遍历
来源：http://jpb.hnxiangtu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xsq.shzxlz.cn

[U92] JS：深拷贝
来源：http://vua.jlsjyb.cn

structuredClone(obj)
来源：http://khr.smart0.xyz

[U93] JS：模板字符串
来源：http://puq.xziqi.cn

`共 ${n} 条`
来源：http://oxk.hysaishi.cn

[U94] JS：箭头函数
来源：http://kfu.cheryme.top

const double = x => x * 2;
来源：http://diw.hnxiangtu.top

[U95] JS：Promise 包装
来源：http://zna.ppjwa.cn

new Promise((resolve, reject) => {})
来源：http://ckk.zhongyouzk.top

[U96] JS：async/await 与异常
来源：http://sfu.xuanzx.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ypg.sysykeji.top

[U97] JS：并发请求
来源：http://whz.bbcook.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kty.gogol.net.cn

[U98] JS：fetch 带 JSON
来源：http://dmp.jinqigfzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tpt.bjfxy.top

[U99] JS：事件监听
来源：http://fsg.haohaochexian.top

el.addEventListener("click", e => {})
来源：http://qjs.daxiang520.top

[U100] JS：DOM 查询
来源：http://hgm.epnwcf.com

document.querySelector(".item")
来源：http://toq.chenlongwang.top

[U101] JS：classList 操作
来源：http://efg.jqgfzy.top

el.classList.toggle("active")
来源：http://yhe.jyoumei.cn

[U102] JS：本地存储
来源：http://gdr.daxiang520.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ppq.cashguo.top

[U103] JS：定时器
来源：http://bhj.shangyingyoupin.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nxm.zhixingplan.top

[U104] JS：防抖
来源：http://cfd.bjfxy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://adt.bjfxy.top

[U105] JS：节流
来源：http://jsk.fengsongda.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dwm.52xcode.cn

[U106] JS：日期格式化
来源：http://qgi.sweek.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://art.cucudq.cn

[U107] JS：数字千分位
来源：http://jhn.wangdashe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tyu.aizwys.cn

[U108] JS：随机整数
来源：http://ctl.zhixingplan.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gtz.nanxuanxn.top

[U109] JS：数组分组
来源：http://gea.gotoacloud.top

Object.groupBy(arr, x => x.type)
来源：http://pon.quarkkingdee.top

[U110] JS：数组分块
来源：http://xhq.xingfuxueyuan.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wct.tanke756.top

[U111] JS：对象转 Map
来源：http://fje.hysaishi.cn

new Map(Object.entries(obj))
来源：http://gkl.tian-w.cn

[U112] JS：字符串补位
来源：http://spe.xinyue.icu

"7".padStart(3, "0")
来源：http://hle.xylfe.cn

[U113] JS：正则替换全部
来源：http://nlu.hfpthk.cn

s.replaceAll("a", "b")
来源：http://mzt.snrcjt.cn

[U114] JS：JSON 深比较
来源：http://dzd.jiagoushi.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://eae.daria6918.cn

[U115] JS：生成 UUID
来源：http://ktm.shanyushiyangkeji.top

crypto.randomUUID()
来源：http://qaw.xuetiantiany.cn

[U116] JS：类型检查（JSDoc）
来源：http://gsq.fzhhl.top

/** @param {string} name */ function f(name) {}
来源：http://yyn.birdmap.top

[U117] JS：单元测试
来源：http://bno.jinqigfzy.top

npm i -D vitest;  npx vitest
来源：http://cmu.zdbjq.cn

[U118] JS：开发服务器
来源：http://xph.aizwys.cn

npm i -D vite;  npx vite
来源：http://tpb.tarul.cn

[U119] JS：生产构建
来源：http://bku.xuanzx.com

npx vite build
来源：http://pkw.fktsv.cn

[U120] JS：读取环境变量（Vite）
来源：http://uju.gogol.net.cn

import.meta.env.VITE_API_URL
来源：http://slt.cashguo.top

================================================================================
来源：http://dxh.sjlbkw.cn

统计汇总
来源：http://vbh.yanxiufei.cn

================================================================================
来源：http://joo.hywenlv.cn

按语言统计（条）：
来源：http://jpw.hfpthk.cn

Python ......... 252
来源：http://moi.shzxlz.cn

PHP ............ 252
来源：http://sbx.shangyingyoupin.top

JavaScript ..... 252
来源：http://aqz.pengpengdd.cyou

TypeScript ..... 212
来源：http://uwn.gzhubu.top

Java ........... 212
来源：http://pgv.xinyue.icu

Go ............. 212
来源：http://hbt.cqqwz.cn

Ruby ........... 212
来源：http://ove.zhijiandao.cn

C# ............. 212
来源：http://hzc.nanxinkj.top

C .............. 30
来源：http://zgi.zhongyouzk.top

C++ ............ 30
来源：http://dfd.sxryk.cn

SQL ............ 90
来源：http://vye.xuanzx.com

Bash ........... 80
来源：http://ult.xuetiantiany.cn

Kotlin ......... 15
来源：http://mtr.yuxming.cn

Swift .......... 15
来源：http://wuh.hongshengwenyu.top

Lua ............ 10
来源：http://gch.pengpengdd.cyou

Perl ........... 10
来源：http://hxm.mhx1999.top

Scala .......... 10
来源：http://htw.kuanghao11.cn

------------------------------------
来源：http://vrp.jinqigfzy.top

合计 ........... 2106 条
来源：http://jrv.andypj.xyz

按章节统计：
来源：http://yqn.smart0.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://epo.jinqigufen.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ugf.tianlin.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rgb.cashguo.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://oth.jlsjyb.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wgd.hammf.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://phs.cdnleiting.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://onm.cucudq.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mfr.fengsongda.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ure.zhaomingkeji.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nyl.fengsongda.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gzi.gaohongyu789.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nvd.guowangkeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xtf.yongpay.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://whv.ydzc1.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jxn.mhx1999.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zta.zhiwuduotai.top

Q SQL 专题                              90
来源：http://zvr.zhiwuduotai.top

R Bash 专题                             80
来源：http://muv.shanyushiyangtech.top

S C / C++ 专题                          60
来源：http://euq.daxiang520.top

T 其他语言补充                          60
来源：http://mxb.zycfv.cn

U 高频实用片段                         120
来源：http://eif.9152youxi.cn

------------------------------------
来源：http://bom.zhijiandao.cn

合计                                  2106 条
来源：http://xdc.yuxming.cn

--------------------------------------------------------------------------------
来源：http://kju.yvedp.cn

使用提醒
来源：http://hdu.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://fkl.yj202588.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ovz.52xcode.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rle.tianlin.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pts.ydzc1.top

在旧版本上使用前请先确认语法支持情况。
来源：http://azo.nanxinkj.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yxg.gaohongyu789.top

—— 文件结束 ——
来源：http://qia.vehdjk.com

================================================================================
来源：http://olh.shanyushiyangkeji.top

程序语言常见例子速查手册（2024 版）
来源：http://fcw.hesvh.cn

Common Programming Examples Cheat Book
来源：http://cwo.vqdsnc.cn

================================================================================
来源：http://rxi.hfpthk.cn

【收录内容】
来源：http://pdu.yangfankeji.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://ico.tarul.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://crp.xuanzx.com

SQL · Bash · C · C++
来源：http://tsq.zhengqikj.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bvj.shangyingyoupin.top

【使用说明】
来源：http://qak.gotoacloud.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dxz.jinyuanbaomall.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dsd.9152youxi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qaz.zhiwuduotai.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nsz.ybcxt.top

Bash:  Shell         C:     C             C++:   C++
来源：http://cvl.hongshengwenyu.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wnm.dashuyun.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kfa.fehbvm.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://azk.snrcjt.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zky.havefunace.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gqd.fengsongda.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vle.snrcjt.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cof.iojbl.cn

【文件统计】
来源：http://pzo.vqdsnc.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fhz.hammf.cn

--------------------------------------------------------------------------------
来源：http://fxx.aizwys.cn

目  录
来源：http://ftm.bbcook.cn

--------------------------------------------------------------------------------
来源：http://gmn.gzhubu.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://svg.yj202588.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kxq.redwolf501.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rrm.fehbvm.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pzt.yfazqb.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://quw.xingfuxueyuan.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zyl.jlsjyb.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://btt.cheryme.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kko.hysaishi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://icg.yuanzhike.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pwx.jlsjyb.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://suk.hysaishi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vfw.shzxlz.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yvn.zdbjq.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dnx.hnxiangtu.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pak.52xcode.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qra.hcnkem.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bdt.wangdashe.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://pyw.chenzaomai.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fwe.zhaomingkeji.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yaa.9152youxi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ork.jinghuilouyu.cn

================================================================================
来源：http://fyv.xuanzx.com

A. 基础语法与类型
来源：http://jki.zdqjudy.top

================================================================================
来源：http://aaj.xinyue.icu

[A01] Hello World
来源：http://fts.bjfxy.top

Py:   print("Hello, World!")
来源：http://ixu.zhaomingkeji.xyz

PHP:  echo "Hello, World!";
来源：http://nky.nanxuanxn.top

JS:   console.log("Hello, World!");
来源：http://cle.sufxvd.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://coy.smart0.xyz

Java: System.out.println("Hello, World!");
来源：http://qaj.ydjk.org.cn

Go:   fmt.Println("Hello, World!")
来源：http://azu.guowangkeji.top

Ruby: puts "Hello, World!"
来源：http://cfw.mhx1999.top

C#:   Console.WriteLine("Hello, World!");
来源：http://gef.aizwys.cn

[A02] 变量声明与赋值
来源：http://mtj.hongshengwenyu.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jyp.sufxvd.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://aqn.nanxinkj.top

JS:   let name = "Alex"; const age = 20;
来源：http://qzk.yuanzhike.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://htt.zhijiandao.cn

Java: String name = "Alex"; int age = 20;
来源：http://elx.ctjpmb.com

Go:   name := "Alex"; age := 20
来源：http://wfh.cdnleiting.top

Ruby: name = "Alex"; age = 20
来源：http://cox.sxryk.cn

C#:   string name = "Alex"; int age = 20;
来源：http://qvf.zhoulong.xyz

[A03] 常量定义
来源：http://mtw.gaohongyu789.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qst.vehdjk.com

PHP:  const PI = 3.14159;
来源：http://swa.xinyue.icu

JS:   const PI = 3.14159;
来源：http://qgm.hammf.cn

TS:   const PI: number = 3.14159;
来源：http://zll.ywan-chungtsiang.top

Java: static final double PI = 3.14159;
来源：http://sei.316326.xyz

Go:   const PI = 3.14159
来源：http://ljv.vqdsnc.cn

Ruby: PI = 3.14159
来源：http://bph.cucudq.cn

C#:   const double PI = 3.14159;
来源：http://agv.vqdsnc.cn

[A04] 判断变量类型
来源：http://icd.hesvh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://lhk.ctjpmb.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ekj.jqgfzy.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yxp.xziqi.cn

TS:   typeof x; x instanceof Date
来源：http://ddp.ehwqpu.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mnz.havefunace.top

Go:   reflect.TypeOf(x).Name()
来源：http://bex.bbcook.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://bjt.chenjidiqi.icu

C#:   x.GetType().Name; x is int
来源：http://bxj.hfpthk.cn

[A05] 整数除法与取模
来源：http://aax.hnxiangtu.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ohk.jyoumei.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vzt.gogol.net.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ste.shangyingyoupin.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://and.jianghu66.top

Java: 7 / 2; 7 % 2
来源：http://spt.jlsjyb.cn

Go:   7 / 2; 7 % 2
来源：http://ewh.ywan-chungtsiang.top

Ruby: 7 / 2; 7 % 2
来源：http://idn.ydjk.org.cn

C#:   7 / 2; 7 % 2
来源：http://try.dianchejie.cn

[A06] 字符串转数字
来源：http://gfm.hongshengwenyu.top

Py:   int("42"); float("3.14")
来源：http://xvw.chenjidiqi.icu

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qte.havefunace.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gep.zhiwuduotai.top

TS:   parseInt("42", 10); Number("42")
来源：http://wqh.316326.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bna.jqgfzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yeb.zdbjq.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rxs.nanxuanxn.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tam.quarkkingdee.top

[A07] 数字转字符串
来源：http://big.shzxlz.cn

Py:   str(42)
来源：http://bag.fktsv.cn

PHP:  (string) 42; strval(42)
来源：http://wtn.316326.xyz

JS:   String(42); (42).toString()
来源：http://hqv.gogol.net.cn

TS:   String(42)
来源：http://cax.jiagoushi.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://nho.feifeiyinyue.top

Go:   strconv.Itoa(42)
来源：http://vbw.yongpay.top

Ruby: 42.to_s
来源：http://tkb.iojbl.cn

C#:   42.ToString()
来源：http://bcx.ehwqpu.com

[A08] 取整与四舍五入
来源：http://rmy.c1oappe.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cvw.smart0.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://shj.birdmap.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://iyn.tarul.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://epq.vehdjk.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qif.xuetiantiany.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lkw.xuetiantiany.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sug.shangyingyoupin.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kyy.hnxiangtu.top

[A09] 绝对值与最大最小值
来源：http://uzc.nanxuanxn.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://uuf.jinghuilouyu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://aou.bbcook.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://waq.zhixingplan.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rzg.sysykeji.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xxy.sweek.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xkl.birdmap.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ibg.sjlbkw.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://uld.jqgfzy.top

[A10] 生成随机数
来源：http://nqs.ydjk.org.cn

Py:   import random; random.randint(1, 100)
来源：http://lfk.ivvv.top

PHP:  random_int(1, 100);
来源：http://eft.havefunace.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hii.feifeiyinyue.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wyc.ydzc1.top

Java: new Random().nextInt(100) + 1
来源：http://ypx.jinghuilouyu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gpj.ivvv.top

Ruby: rand(1..100)
来源：http://rti.xziqi.cn

C#:   new Random().Next(1, 101)
来源：http://paj.vehdjk.com

[A11] 条件表达式（三元）
来源：http://tlf.sxryk.cn

Py:   "yes" if x > 0 else "no"
来源：http://jle.iojbl.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://lqz.jianghu66.top

JS:   x > 0 ? "yes" : "no"
来源：http://lea.chenzaomai.com

TS:   x > 0 ? "yes" : "no"
来源：http://ebw.hesvh.cn

Java: x > 0 ? "yes" : "no"
来源：http://hte.redwolf501.top

Go:   // 无三元运算符，需用 if 语句
来源：http://vgh.chenzaomai.com

Ruby: x > 0 ? "yes" : "no"
来源：http://ylu.cqqwz.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bzn.ivvv.top

[A12] 字符串插值 / 格式化
来源：http://bxe.aizwys.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://aeu.hnxiangtu.top


<!-- 参考信息 -->