代发 wailian999

[U71] PHP：抛出异常
来源：http://uko.nwbrower.top

throw new RuntimeException("失败", 500);
来源：http://lrv.aibaodan.cn

[U72] PHP：写错误日志
来源：http://tpr.vqdsnc.cn

error_log("失败: " . $e->getMessage());
来源：http://tey.zhoulong.xyz

[U73] PHP：读取 ini 配置
来源：http://zzr.yfazqb.com

parse_ini_file("config.ini", true)
来源：http://ykb.yuxming.cn

[U74] PHP：读取环境变量
来源：http://rji.dianchejie.cn

getenv("APP_ENV") ?: "production"
来源：http://ixj.yuanzhike.top

[U75] PHP：依赖注入
来源：http://cot.guowangkeji.top

composer require psr/container
来源：http://gaa.cucudq.cn

[U76] PHP：简单路由
来源：http://kuq.dashuyun.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cqr.cdnleiting.top

[U77] PHP：模板渲染
来源：http://wtp.fktsv.cn

composer require twig/twig
来源：http://kiz.meibo888.top

[U78] PHP：单元测试
来源：http://eqw.wangdashe.top

composer require --dev phpunit/phpunit
来源：http://rqn.yfazqb.com

[U79] PHP：静态分析
来源：http://uyh.andypj.xyz

composer require --dev phpstan/phpstan
来源：http://mcf.shanyushiyangtech.top

[U80] PHP：代码规范修复
来源：http://pch.haohaochexian.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://pnb.ctjpmb.com

[U81] JS：初始化项目
来源：http://srj.zdqjudy.top

npm init -y;  npm i express
来源：http://nfz.xuetiantiany.cn

[U82] JS：package.json 脚本
来源：http://agt.pengpengdd.cyou

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zni.zhongyouzk.top

[U83] JS：ES Module 导入导出
来源：http://egy.gotoacloud.top

export const a = 1;  import { a } from "./m.js";
来源：http://ofs.gogol.net.cn

[U84] JS：CommonJS 写法
来源：http://joq.c1oappe.top

module.exports = { a };  const { a } = require("./m");
来源：http://ttx.hywenlv.cn

[U85] JS：可选链
来源：http://qam.guowangkeji.top

a?.b?.c
来源：http://tho.ppjwa.cn

[U86] JS：空值合并
来源：http://aui.fengsongda.top

a ?? b
来源：http://xhz.smart0.xyz

[U87] JS：解构默认值
来源：http://fsv.zhoulong.xyz

const { a = 1, b = 2 } = obj;
来源：http://nqb.pycfn.com

[U88] JS：对象展开合并
来源：http://vur.cashguo.top

{ ...a, ...b }
来源：http://sak.zycfv.cn

[U89] JS：数组去重
来源：http://ttd.gotoacloud.top

[...new Set(arr)]
来源：http://mcq.mhx1999.top

[U90] JS：数字数组排序
来源：http://kfp.chenjidiqi.icu

[...arr].sort((a, b) => a - b)
来源：http://gxw.bjfxy.top

[U91] JS：对象键值遍历
来源：http://uph.sweek.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://auy.kuanghao11.cn

[U92] JS：深拷贝
来源：http://dta.xylfe.cn

structuredClone(obj)
来源：http://tty.hywenlv.cn

[U93] JS：模板字符串
来源：http://ozq.ywan-chungtsiang.top

`共 ${n} 条`
来源：http://iah.zhixingplan.top

[U94] JS：箭头函数
来源：http://bcw.yj20258888.top

const double = x => x * 2;
来源：http://cat.shzxlz.cn

[U95] JS：Promise 包装
来源：http://pxj.kuanghao11.cn

new Promise((resolve, reject) => {})
来源：http://crp.dianchejie.cn

[U96] JS：async/await 与异常
来源：http://sjw.shuidangran.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fnq.yj20258.top

[U97] JS：并发请求
来源：http://vfw.yvedp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rci.chenjidiqi.icu

[U98] JS：fetch 带 JSON
来源：http://tbu.ybcxt.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yon.sxryk.cn

[U99] JS：事件监听
来源：http://vno.dianchejie.cn

el.addEventListener("click", e => {})
来源：http://wrn.snrcjt.cn

[U100] JS：DOM 查询
来源：http://jtu.yuxming.cn

document.querySelector(".item")
来源：http://ysp.c1oappe.top

[U101] JS：classList 操作
来源：http://kby.sxryk.cn

el.classList.toggle("active")
来源：http://kny.havefunace.top

[U102] JS：本地存储
来源：http://iuc.guowangkeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://rdf.jinghuilouyu.cn

[U103] JS：定时器
来源：http://rxc.redwolf501.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hcl.zhijiandao.cn

[U104] JS：防抖
来源：http://wav.zhiwuduotai.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qxq.c1oappe.top

[U105] JS：节流
来源：http://lqz.hfpthk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ebr.ybcxt.top

[U106] JS：日期格式化
来源：http://nsn.zycfv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gpc.sysykeji.top

[U107] JS：数字千分位
来源：http://wkx.hnqzz.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kqf.jianghu66.top

[U108] JS：随机整数
来源：http://tsm.9152youxi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pet.gogol.net.cn

[U109] JS：数组分组
来源：http://nbz.hongshengwenyu.top

Object.groupBy(arr, x => x.type)
来源：http://anb.nanxinkj.top

[U110] JS：数组分块
来源：http://shg.fengsongda.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ync.nwbrower.top

[U111] JS：对象转 Map
来源：http://ths.meibo888.top

new Map(Object.entries(obj))
来源：http://jda.zhiwuduotai.top

[U112] JS：字符串补位
来源：http://tge.chenzaomai.com

"7".padStart(3, "0")
来源：http://ojl.ywan-chungtsiang.top

[U113] JS：正则替换全部
来源：http://ycm.gzhubu.top

s.replaceAll("a", "b")
来源：http://zvs.svipenyu.cn

[U114] JS：JSON 深比较
来源：http://eoq.smart0.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://kol.nwbrower.top

[U115] JS：生成 UUID
来源：http://ztl.yj20258.top

crypto.randomUUID()
来源：http://qny.kuanghao11.cn

[U116] JS：类型检查（JSDoc）
来源：http://smx.nanxuanxn.top

/** @param {string} name */ function f(name) {}
来源：http://llg.hfpthk.cn

[U117] JS：单元测试
来源：http://hsf.pycfn.com

npm i -D vitest;  npx vitest
来源：http://pck.52xcode.cn

[U118] JS：开发服务器
来源：http://dxj.havefunace.top

npm i -D vite;  npx vite
来源：http://ufi.shzxlz.cn

[U119] JS：生产构建
来源：http://aay.gzhubu.top

npx vite build
来源：http://qmg.chenlongwang.top

[U120] JS：读取环境变量（Vite）
来源：http://hfv.xinyue.icu

import.meta.env.VITE_API_URL
来源：http://zfp.daria6918.cn

================================================================================
来源：http://yzw.52xcode.cn

统计汇总
来源：http://feg.cashguo.top

================================================================================
来源：http://bex.cqqwz.cn

按语言统计（条）：
来源：http://mwh.hcnkem.com

Python ......... 252
来源：http://tow.iojbl.cn

PHP ............ 252
来源：http://okh.jiagoushi.top

JavaScript ..... 252
来源：http://tpv.ydjk.org.cn

TypeScript ..... 212
来源：http://emf.dashuyun.cn

Java ........... 212
来源：http://lha.dashuyun.cn

Go ............. 212
来源：http://azn.tian-w.cn

Ruby ........... 212
来源：http://ekw.sufxvd.cn

C# ............. 212
来源：http://yih.xuetiantiany.cn

C .............. 30
来源：http://fbl.jqgufenzy.top

C++ ............ 30
来源：http://nar.meibo888.top

SQL ............ 90
来源：http://pxn.nwbrower.top

Bash ........... 80
来源：http://lzb.hnxiangtu.top

Kotlin ......... 15
来源：http://mhq.hnxiangtu.top

Swift .......... 15
来源：http://pit.cheryme.top

Lua ............ 10
来源：http://nai.ydjk.org.cn

Perl ........... 10
来源：http://cxd.bbcook.cn

Scala .......... 10
来源：http://pal.gzhubu.top

------------------------------------
来源：http://nhi.jqgfzy.top

合计 ........... 2106 条
来源：http://phw.yangfankeji.com

按章节统计：
来源：http://rll.gzhubu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://iaf.zhijiandao.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ukm.xingfuxueyuan.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uft.kuanghao11.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ulk.birdmap.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oop.jqgfzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mph.xylfe.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wif.redwolf501.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bzu.zdbjq.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fwu.0kj1m.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nyi.zhijiandao.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://diu.jiagoushi.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pyf.gzhubu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ntf.hcnkem.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tue.tianlin.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zlv.guannengcc.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ymw.nanxinkj.top

Q SQL 专题                              90
来源：http://sbm.yonumen.top

R Bash 专题                             80
来源：http://vic.dianchejie.cn

S C / C++ 专题                          60
来源：http://fjg.birdmap.top

T 其他语言补充                          60
来源：http://fsl.haohaochexian.top

U 高频实用片段                         120
来源：http://qfo.meibo888.top

------------------------------------
来源：http://ohh.dashuyun.cn

合计                                  2106 条
来源：http://nma.yvedp.cn

--------------------------------------------------------------------------------
来源：http://jfg.jinqigufen.top

使用提醒
来源：http://gzq.yfazqb.com

--------------------------------------------------------------------------------
来源：http://adq.shuidangran.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://emn.dianchejie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vga.hesvh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jdi.meibo888.top

在旧版本上使用前请先确认语法支持情况。
来源：http://umo.shangyingyoupin.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mky.iojbl.cn

—— 文件结束 ——
来源：http://ydf.birdmap.top

================================================================================
来源：http://yzs.ydjk.org.cn

程序语言常见例子速查手册（2024 版）
来源：http://wmy.xuetiantiany.cn

Common Programming Examples Cheat Book
来源：http://org.haohaochexian.top

================================================================================
来源：http://uza.hammf.cn

【收录内容】
来源：http://pyp.hnxiangtu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://mub.jianghu66.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yps.tarul.cn

SQL · Bash · C · C++
来源：http://iye.shangyingyoupin.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vmy.mhx1999.top

【使用说明】
来源：http://wfm.zycfv.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bai.hcnkem.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pbn.c1oappe.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://esk.0kj1m.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://edc.ydzc1.top

Bash:  Shell         C:     C             C++:   C++
来源：http://nip.gotoacloud.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vac.sufxvd.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vkp.316326.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pzf.gaohongyu789.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yis.hesvh.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://npp.jlsjyb.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dhv.chenzaomai.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://skx.zhengqikj.top

【文件统计】
来源：http://huc.hesvh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gjp.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://isq.tanke756.top

目  录
来源：http://kna.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://glx.jlsjyb.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qsq.c1oappe.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xml.yongpay.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://awu.ydjk.org.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pwb.daria6918.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kjq.wangdashe.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qfd.fehbvm.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ngg.jqgufenzy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wnz.hfpthk.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://oje.daxiang520.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ulb.shanyushiyangkeji.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hmw.wangshuangyany.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kli.zdbjq.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nht.wangdashe.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ftm.guannengcc.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://oer.jiagoushi.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fec.jiagoushi.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ypo.birdmap.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://xpq.sxryk.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xsk.cdnleiting.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://psh.0kj1m.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fdj.ivvv.top

================================================================================
来源：http://bcc.nwbrower.top

A. 基础语法与类型
来源：http://gpk.nanxuanxn.top

================================================================================
来源：http://bra.mhx1999.top

[A01] Hello World
来源：http://hit.zhengqikj.top

Py:   print("Hello, World!")
来源：http://fad.shanyushiyangkeji.top

PHP:  echo "Hello, World!";
来源：http://ajk.aizwys.cn

JS:   console.log("Hello, World!");
来源：http://waa.kuanghao11.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xuz.chenlongwang.top

Java: System.out.println("Hello, World!");
来源：http://fql.aizwys.cn

Go:   fmt.Println("Hello, World!")
来源：http://opr.hammf.cn

Ruby: puts "Hello, World!"
来源：http://tud.gaohongyu789.top

C#:   Console.WriteLine("Hello, World!");
来源：http://wqx.daria6918.cn

[A02] 变量声明与赋值
来源：http://ntu.tianlin.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wvn.cucudq.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://slb.tianlin.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://hhx.zhengqikj.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dfd.0kj1m.cn

Java: String name = "Alex"; int age = 20;
来源：http://gqn.shanyushiyangkeji.top

Go:   name := "Alex"; age := 20
来源：http://nqs.xziqi.cn

Ruby: name = "Alex"; age = 20
来源：http://esj.xinyue.icu

C#:   string name = "Alex"; int age = 20;
来源：http://ymx.shuidangran.top

[A03] 常量定义
来源：http://aup.hammf.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vou.fktsv.cn

PHP:  const PI = 3.14159;
来源：http://nar.vqdsnc.cn

JS:   const PI = 3.14159;
来源：http://pat.daxiang520.top

TS:   const PI: number = 3.14159;
来源：http://ljj.yanxiufei.cn

Java: static final double PI = 3.14159;
来源：http://xay.zycfv.cn

Go:   const PI = 3.14159
来源：http://fok.aibaodan.cn

Ruby: PI = 3.14159
来源：http://fhd.tanke756.top

C#:   const double PI = 3.14159;
来源：http://yly.nanxuanxn.top

[A04] 判断变量类型
来源：http://gll.guannengcc.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ctw.jinqigufen.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xiu.yj20258.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xey.sxryk.cn

TS:   typeof x; x instanceof Date
来源：http://iml.snrcjt.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wwn.hongshengwenyu.top

Go:   reflect.TypeOf(x).Name()
来源：http://iuj.zdqjudy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://mas.tianlin.xyz

C#:   x.GetType().Name; x is int
来源：http://bcv.zhixingplan.top

[A05] 整数除法与取模
来源：http://ywr.epnwcf.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ykr.daxiang520.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://kga.zhijiandao.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://paf.xinyue.icu

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qdc.jinqigfzy.top

Java: 7 / 2; 7 % 2
来源：http://bfk.316326.xyz

Go:   7 / 2; 7 % 2
来源：http://puo.316326.xyz

Ruby: 7 / 2; 7 % 2
来源：http://iga.zhongyouzk.top

C#:   7 / 2; 7 % 2
来源：http://omb.vqdsnc.cn

[A06] 字符串转数字
来源：http://xry.epnwcf.com

Py:   int("42"); float("3.14")
来源：http://ziw.ywan-chungtsiang.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ryo.hywenlv.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jln.fanxiaobao.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://iww.xingfuxueyuan.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tfz.yfazqb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qej.jinqigufen.top

Ruby: "42".to_i; "3.14".to_f
来源：http://tmy.9152youxi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://len.cucudq.cn

[A07] 数字转字符串
来源：http://acc.jyoumei.cn

Py:   str(42)
来源：http://kwi.tianlin.xyz

PHP:  (string) 42; strval(42)
来源：http://rok.zhijiandao.cn

JS:   String(42); (42).toString()
来源：http://rqm.yuanzhike.top

TS:   String(42)
来源：http://wnx.nanxuanxn.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://hoh.jqgfzy.top

Go:   strconv.Itoa(42)
来源：http://zuc.nwbrower.top

Ruby: 42.to_s
来源：http://hyc.yonumen.top

C#:   42.ToString()
来源：http://bot.dianchejie.cn

[A08] 取整与四舍五入
来源：http://tuz.iojbl.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wvq.9152youxi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bsl.jinyuanbaomall.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kkm.svipenyu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gmb.jlsjyb.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hft.hcnkem.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nkz.yuanzhike.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://fvy.ppjwa.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pxe.cqqwz.cn

[A09] 绝对值与最大最小值
来源：http://sqz.zhijiandao.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ino.andypj.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://krq.gogol.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://aih.guowangkeji.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xhm.daria6918.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kfi.sysykeji.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fyj.zdqjudy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fcw.mhx1999.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xom.jinqigfzy.top

[A10] 生成随机数
来源：http://xqy.birdmap.top

Py:   import random; random.randint(1, 100)
来源：http://njw.xingfuxueyuan.xyz

PHP:  random_int(1, 100);
来源：http://xob.ehwqpu.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cwm.yfazqb.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://omv.jyoumei.cn

Java: new Random().nextInt(100) + 1
来源：http://klt.vqdsnc.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://elb.ppjwa.cn

Ruby: rand(1..100)
来源：http://dnd.zhoulong.xyz

C#:   new Random().Next(1, 101)
来源：http://kln.quarkkingdee.top

[A11] 条件表达式（三元）
来源：http://ljw.nanxinkj.top

Py:   "yes" if x > 0 else "no"
来源：http://xoh.zhongyouzk.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://jcr.fengsongda.top


<!-- 参考信息 -->