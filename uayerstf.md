代发 wailian999

[U75] PHP：依赖注入
来源：http://dec.ywan-chungtsiang.top

composer require psr/container
来源：http://avq.sufxvd.cn

[U76] PHP：简单路由
来源：http://avk.iojbl.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oqi.cucudq.cn

[U77] PHP：模板渲染
来源：http://yor.zhijiandao.cn

composer require twig/twig
来源：http://azs.fktsv.cn

[U78] PHP：单元测试
来源：http://zpk.cucudq.cn

composer require --dev phpunit/phpunit
来源：http://fmy.iojbl.cn

[U79] PHP：静态分析
来源：http://lxi.jqgfzy.top

composer require --dev phpstan/phpstan
来源：http://rlz.hfpthk.cn

[U80] PHP：代码规范修复
来源：http://okk.hywenlv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qwq.jqgfzy.top

[U81] JS：初始化项目
来源：http://cjx.shangyingyoupin.top

npm init -y;  npm i express
来源：http://qjn.yj202588.top

[U82] JS：package.json 脚本
来源：http://oob.shanyushiyangtech.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cwa.daxiang520.top

[U83] JS：ES Module 导入导出
来源：http://ywf.pycfn.com

export const a = 1;  import { a } from "./m.js";
来源：http://aqs.tian-w.cn

[U84] JS：CommonJS 写法
来源：http://vig.ydzc1.top

module.exports = { a };  const { a } = require("./m");
来源：http://ggx.shanyushiyangkeji.top

[U85] JS：可选链
来源：http://jgd.sufxvd.cn

a?.b?.c
来源：http://cdm.jinghuilouyu.cn

[U86] JS：空值合并
来源：http://arq.ehwqpu.com

a ?? b
来源：http://eya.tanke756.top

[U87] JS：解构默认值
来源：http://ggm.shanyushiyangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://ykl.sweek.top

[U88] JS：对象展开合并
来源：http://fsd.sjlbkw.cn

{ ...a, ...b }
来源：http://bsv.yj20258.top

[U89] JS：数组去重
来源：http://dha.zdqjudy.top

[...new Set(arr)]
来源：http://fne.sufxvd.cn

[U90] JS：数字数组排序
来源：http://heh.ydjk.org.cn

[...arr].sort((a, b) => a - b)
来源：http://kyn.ydzc1.top

[U91] JS：对象键值遍历
来源：http://abz.gogol.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uwg.vehdjk.com

[U92] JS：深拷贝
来源：http://zka.shanyushiyangkeji.top

structuredClone(obj)
来源：http://muw.sysykeji.top

[U93] JS：模板字符串
来源：http://zhf.sufxvd.cn

`共 ${n} 条`
来源：http://emf.vqdsnc.cn

[U94] JS：箭头函数
来源：http://lug.yanxiufei.cn

const double = x => x * 2;
来源：http://jza.yfazqb.com

[U95] JS：Promise 包装
来源：http://egv.hnxiangtu.top

new Promise((resolve, reject) => {})
来源：http://bxc.ydjk.org.cn

[U96] JS：async/await 与异常
来源：http://iyo.vqdsnc.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cot.hysaishi.cn

[U97] JS：并发请求
来源：http://pug.xingfuxueyuan.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://rxc.hammf.cn

[U98] JS：fetch 带 JSON
来源：http://fhr.tian-w.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ark.chenjidiqi.icu

[U99] JS：事件监听
来源：http://vhl.hnqzz.top

el.addEventListener("click", e => {})
来源：http://djv.fzhhl.top

[U100] JS：DOM 查询
来源：http://dts.wangdashe.top

document.querySelector(".item")
来源：http://opj.wangshuangyany.cn

[U101] JS：classList 操作
来源：http://cma.pengpengdd.cyou

el.classList.toggle("active")
来源：http://spe.redwolf501.top

[U102] JS：本地存储
来源：http://ceh.9152youxi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kgs.gotoacloud.top

[U103] JS：定时器
来源：http://uzl.yfazqb.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xgi.haohaochexian.top

[U104] JS：防抖
来源：http://kod.shanyushiyangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ptt.sufxvd.cn

[U105] JS：节流
来源：http://ozk.cashguo.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wvq.c1oappe.top

[U106] JS：日期格式化
来源：http://pkr.zhengqikj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ayc.dashuyun.cn

[U107] JS：数字千分位
来源：http://hjp.shanyushiyangtech.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mvy.fzhhl.top

[U108] JS：随机整数
来源：http://jai.shangyingyoupin.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nvn.jyoumei.cn

[U109] JS：数组分组
来源：http://tbb.jqgfzy.top

Object.groupBy(arr, x => x.type)
来源：http://fju.chenlongwang.top

[U110] JS：数组分块
来源：http://dug.guannengcc.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bjl.fzhhl.top

[U111] JS：对象转 Map
来源：http://zbd.yongpay.top

new Map(Object.entries(obj))
来源：http://frz.tanke756.top

[U112] JS：字符串补位
来源：http://cfr.shanyushiyangkeji.top

"7".padStart(3, "0")
来源：http://swb.shangyingyoupin.top

[U113] JS：正则替换全部
来源：http://lhc.tian-w.cn

s.replaceAll("a", "b")
来源：http://per.yanxiufei.cn

[U114] JS：JSON 深比较
来源：http://ddi.yfazqb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://ius.havefunace.top

[U115] JS：生成 UUID
来源：http://vhz.sjlbkw.cn

crypto.randomUUID()
来源：http://wci.ctjpmb.com

[U116] JS：类型检查（JSDoc）
来源：http://vlf.zdqjudy.top

/** @param {string} name */ function f(name) {}
来源：http://caa.nanxuanxn.top

[U117] JS：单元测试
来源：http://qsh.hysaishi.cn

npm i -D vitest;  npx vitest
来源：http://sod.52xcode.cn

[U118] JS：开发服务器
来源：http://uad.jqgufenzy.top

npm i -D vite;  npx vite
来源：http://zgx.zhijiandao.cn

[U119] JS：生产构建
来源：http://cyy.fanxiaobao.xyz

npx vite build
来源：http://hli.havefunace.top

[U120] JS：读取环境变量（Vite）
来源：http://mjs.xuanzx.com

import.meta.env.VITE_API_URL
来源：http://wkq.haohaochexian.top

================================================================================
来源：http://ydq.sufxvd.cn

统计汇总
来源：http://bwb.hnxiangtu.top

================================================================================
来源：http://get.daria6918.cn

按语言统计（条）：
来源：http://lxo.yongpay.top

Python ......... 252
来源：http://wzw.sjlbkw.cn

PHP ............ 252
来源：http://zvl.0kj1m.cn

JavaScript ..... 252
来源：http://qpk.gogol.net.cn

TypeScript ..... 212
来源：http://hcj.sysykeji.top

Java ........... 212
来源：http://jkm.shuidangran.top

Go ............. 212
来源：http://qsp.sufxvd.cn

Ruby ........... 212
来源：http://brc.ybcxt.top

C# ............. 212
来源：http://cve.0kj1m.cn

C .............. 30
来源：http://iii.shzxlz.cn

C++ ............ 30
来源：http://flu.c1oappe.top

SQL ............ 90
来源：http://myy.chenzaomai.com

Bash ........... 80
来源：http://ytd.pycfn.com

Kotlin ......... 15
来源：http://zqo.hfpthk.cn

Swift .......... 15
来源：http://tex.xylfe.cn

Lua ............ 10
来源：http://qck.hywenlv.cn

Perl ........... 10
来源：http://elr.jyoumei.cn

Scala .......... 10
来源：http://dqo.redwolf501.top

------------------------------------
来源：http://ypy.jqgfzy.top

合计 ........... 2106 条
来源：http://gna.shangyingyoupin.top

按章节统计：
来源：http://sxz.yangfankeji.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://njf.tarul.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://npc.zhoulong.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kwb.jinqigufen.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qrq.quarkkingdee.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ptb.nanxuanxn.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kcb.aizwys.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uqt.ehwqpu.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mqg.havefunace.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jth.yj202588.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gwn.jinghuilouyu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ect.cashguo.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jkb.guannengcc.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vsb.chenzaomai.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gst.snrcjt.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rhl.pycfn.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eln.zhijiandao.cn

Q SQL 专题                              90
来源：http://hyy.yonumen.top

R Bash 专题                             80
来源：http://ynf.hnqzz.top

S C / C++ 专题                          60
来源：http://tyv.sweek.top

T 其他语言补充                          60
来源：http://wcq.uphjek.com

U 高频实用片段                         120
来源：http://ccb.zhixingplan.top

------------------------------------
来源：http://uqj.ppjwa.cn

合计                                  2106 条
来源：http://hpa.guannengcc.top

--------------------------------------------------------------------------------
来源：http://ktm.chenlongwang.top

使用提醒
来源：http://rdl.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://qur.zdqjudy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://usv.vqdsnc.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://psm.ybcxt.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://adq.nanxinkj.top

在旧版本上使用前请先确认语法支持情况。
来源：http://lqp.quarkkingdee.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bap.jinqigfzy.top

—— 文件结束 ——
来源：http://dip.0kj1m.cn

================================================================================
来源：http://hqu.tianlin.xyz

程序语言常见例子速查手册（2024 版）
来源：http://rvl.chenzaomai.com

Common Programming Examples Cheat Book
来源：http://uck.bbcook.cn

================================================================================
来源：http://dru.redwolf501.top

【收录内容】
来源：http://ofz.vqdsnc.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://foi.shanyushiyangtech.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xhd.sjlbkw.cn

SQL · Bash · C · C++
来源：http://uay.cashguo.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jrm.aibaodan.cn

【使用说明】
来源：http://uuh.zdbjq.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gby.gzhubu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nir.fzhhl.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hjc.yonumen.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xym.shanyushiyangtech.top

Bash:  Shell         C:     C             C++:   C++
来源：http://yqy.ywan-chungtsiang.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sxm.meibo888.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dui.tanke756.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nsa.andypj.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zec.ctjpmb.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://flw.jinqigfzy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xsm.yj20258.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zrf.jqgfzy.top

【文件统计】
来源：http://mnt.jianghu66.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rew.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://tdb.gzhubu.top

目  录
来源：http://ftd.xziqi.cn

--------------------------------------------------------------------------------
来源：http://rpj.zdqjudy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://asy.sjlbkw.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vhf.daria6918.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dfo.jyoumei.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mof.cheryme.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uzn.nanxinkj.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ooq.zhoulong.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://izu.cheryme.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dcl.zhengqikj.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dia.ehwqpu.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fsi.hnxiangtu.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dma.zhixingplan.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yeg.ydzc1.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xgd.sxryk.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://oxi.jinyuanbaomall.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hxq.chenlongwang.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bra.kuanghao11.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://noz.c1oappe.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ihk.ppjwa.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://box.hnqzz.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qam.vehdjk.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jlv.sufxvd.cn

================================================================================
来源：http://suk.guannengcc.top

A. 基础语法与类型
来源：http://wxv.aibaodan.cn

================================================================================
来源：http://kcw.sweek.top

[A01] Hello World
来源：http://wwr.gzhubu.top

Py:   print("Hello, World!")
来源：http://ulq.ydjk.org.cn

PHP:  echo "Hello, World!";
来源：http://ufb.ydzc1.top

JS:   console.log("Hello, World!");
来源：http://rid.ivvv.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://aht.sysykeji.top

Java: System.out.println("Hello, World!");
来源：http://sqz.ppjwa.cn

Go:   fmt.Println("Hello, World!")
来源：http://uph.yuxming.cn

Ruby: puts "Hello, World!"
来源：http://mlk.yj20258888.top

C#:   Console.WriteLine("Hello, World!");
来源：http://jbi.jyoumei.cn

[A02] 变量声明与赋值
来源：http://qqx.fanxiaobao.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zgp.yuanzhike.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ikd.sysykeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://jpw.wangdashe.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ypg.tian-w.cn

Java: String name = "Alex"; int age = 20;
来源：http://pyc.zhijiandao.cn

Go:   name := "Alex"; age := 20
来源：http://wra.gzhubu.top

Ruby: name = "Alex"; age = 20
来源：http://yux.yj202588.top

C#:   string name = "Alex"; int age = 20;
来源：http://qwg.zhixingplan.top

[A03] 常量定义
来源：http://qjs.nwbrower.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jic.9152youxi.cn

PHP:  const PI = 3.14159;
来源：http://rkg.nwbrower.top

JS:   const PI = 3.14159;
来源：http://wwu.wangshuangyany.cn

TS:   const PI: number = 3.14159;
来源：http://gap.guannengcc.top

Java: static final double PI = 3.14159;
来源：http://rty.nanxinkj.top

Go:   const PI = 3.14159
来源：http://zrn.ppjwa.cn

Ruby: PI = 3.14159
来源：http://ihb.vqdsnc.cn

C#:   const double PI = 3.14159;
来源：http://xxn.ydzc1.top

[A04] 判断变量类型
来源：http://sjw.hywenlv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://fsv.smart0.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pxa.zhongyouzk.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tdo.nwbrower.top

TS:   typeof x; x instanceof Date
来源：http://col.yvedp.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://uzs.quarkkingdee.top

Go:   reflect.TypeOf(x).Name()
来源：http://vrk.hysaishi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ngf.dianchejie.cn

C#:   x.GetType().Name; x is int
来源：http://vkq.iojbl.cn

[A05] 整数除法与取模
来源：http://odh.xinyue.icu

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://evc.zhaomingkeji.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://qfg.sxryk.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yut.jinqigfzy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uaf.hnxiangtu.top

Java: 7 / 2; 7 % 2
来源：http://ctw.hnxiangtu.top

Go:   7 / 2; 7 % 2
来源：http://zkt.chenzaomai.com

Ruby: 7 / 2; 7 % 2
来源：http://aio.haohaochexian.top

C#:   7 / 2; 7 % 2
来源：http://qmu.mhx1999.top

[A06] 字符串转数字
来源：http://uam.kuanghao11.cn

Py:   int("42"); float("3.14")
来源：http://pbz.feifeiyinyue.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://psk.zhengqikj.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xtd.yongpay.top

TS:   parseInt("42", 10); Number("42")
来源：http://ulm.zdqjudy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bez.iojbl.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xks.andypj.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://svh.yuxming.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fpy.vqdsnc.cn

[A07] 数字转字符串
来源：http://ysz.uphjek.com

Py:   str(42)
来源：http://qxe.hesvh.cn

PHP:  (string) 42; strval(42)
来源：http://uqe.nwbrower.top

JS:   String(42); (42).toString()
来源：http://jcp.yonumen.top

TS:   String(42)
来源：http://sue.ywan-chungtsiang.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://wum.hongshengwenyu.top

Go:   strconv.Itoa(42)
来源：http://ywx.chenzaomai.com

Ruby: 42.to_s
来源：http://rmx.shangyingyoupin.top

C#:   42.ToString()
来源：http://xqe.zhiwuduotai.top

[A08] 取整与四舍五入
来源：http://ubr.sweek.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wdx.hcnkem.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yav.yj202588.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sqr.jinghuilouyu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wxv.tarul.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tjv.zdqjudy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sbc.jiagoushi.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ozh.aizwys.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lty.shangyingyoupin.top

[A09] 绝对值与最大最小值
来源：http://hym.bbcook.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://csu.aibaodan.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qyx.vqdsnc.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://msj.xinyue.icu

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ean.zhixingplan.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pxi.zhaomingkeji.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wfy.hysaishi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mkz.dianchejie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kls.fehbvm.com

[A10] 生成随机数
来源：http://xqq.xuetiantiany.cn

Py:   import random; random.randint(1, 100)
来源：http://mtg.fzhhl.top

PHP:  random_int(1, 100);
来源：http://jet.cqqwz.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://glf.shanyushiyangkeji.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wnn.hongshengwenyu.top

Java: new Random().nextInt(100) + 1
来源：http://jws.jyoumei.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://waf.quarkkingdee.top

Ruby: rand(1..100)
来源：http://gco.jianghu66.top

C#:   new Random().Next(1, 101)
来源：http://xrj.snrcjt.cn

[A11] 条件表达式（三元）
来源：http://zyl.dianchejie.cn

Py:   "yes" if x > 0 else "no"
来源：http://gsz.aibaodan.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rnx.zhongyouzk.top

JS:   x > 0 ? "yes" : "no"
来源：http://bvk.wangdashe.top

TS:   x > 0 ? "yes" : "no"
来源：http://xob.ydjk.org.cn

Java: x > 0 ? "yes" : "no"
来源：http://hdp.nwbrower.top

Go:   // 无三元运算符，需用 if 语句
来源：http://bae.nanxuanxn.top

Ruby: x > 0 ? "yes" : "no"
来源：http://vzg.iojbl.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xgv.xinyue.icu

[A12] 字符串插值 / 格式化
来源：http://oav.jinqigfzy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://odq.wangdashe.top


<!-- 参考信息 -->