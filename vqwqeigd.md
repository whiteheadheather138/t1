代发 wailian999

[U71] PHP：抛出异常
来源：http://zrh.yj20258.top

throw new RuntimeException("失败", 500);
来源：http://ubz.yvedp.cn

[U72] PHP：写错误日志
来源：http://zdn.zycfv.cn

error_log("失败: " . $e->getMessage());
来源：http://uzo.yuanzhike.top

[U73] PHP：读取 ini 配置
来源：http://gyk.yongpay.top

parse_ini_file("config.ini", true)
来源：http://uzj.yfazqb.com

[U74] PHP：读取环境变量
来源：http://lyq.zhijiandao.cn

getenv("APP_ENV") ?: "production"
来源：http://idk.yj20258.top

[U75] PHP：依赖注入
来源：http://azp.jyoumei.cn

composer require psr/container
来源：http://ylk.mhx1999.top

[U76] PHP：简单路由
来源：http://ski.zhoulong.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://aob.gzhubu.top

[U77] PHP：模板渲染
来源：http://cjc.hywenlv.cn

composer require twig/twig
来源：http://jdl.tianlin.xyz

[U78] PHP：单元测试
来源：http://pso.pengpengdd.cyou

composer require --dev phpunit/phpunit
来源：http://kya.cucudq.cn

[U79] PHP：静态分析
来源：http://fms.yangfankeji.com

composer require --dev phpstan/phpstan
来源：http://tnv.bbcook.cn

[U80] PHP：代码规范修复
来源：http://gaz.yongpay.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://gwc.hnxiangtu.top

[U81] JS：初始化项目
来源：http://vip.sjlbkw.cn

npm init -y;  npm i express
来源：http://olz.sjlbkw.cn

[U82] JS：package.json 脚本
来源：http://yst.sjlbkw.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fsu.shanyushiyangkeji.top

[U83] JS：ES Module 导入导出
来源：http://psv.yonumen.top

export const a = 1;  import { a } from "./m.js";
来源：http://kdr.chenzaomai.com

[U84] JS：CommonJS 写法
来源：http://lko.yanxiufei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://eym.shzxlz.cn

[U85] JS：可选链
来源：http://fex.c1oappe.top

a?.b?.c
来源：http://xne.jinqigfzy.top

[U86] JS：空值合并
来源：http://cpi.cqqwz.cn

a ?? b
来源：http://hhu.zdqjudy.top

[U87] JS：解构默认值
来源：http://onf.yfazqb.com

const { a = 1, b = 2 } = obj;
来源：http://xqc.daxiang520.top

[U88] JS：对象展开合并
来源：http://vjs.yongpay.top

{ ...a, ...b }
来源：http://uru.tarul.cn

[U89] JS：数组去重
来源：http://jlp.tianlin.xyz

[...new Set(arr)]
来源：http://jmy.yvedp.cn

[U90] JS：数字数组排序
来源：http://dvi.haohaochexian.top

[...arr].sort((a, b) => a - b)
来源：http://vum.hnqzz.top

[U91] JS：对象键值遍历
来源：http://sgn.jlsjyb.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mpp.nwbrower.top

[U92] JS：深拷贝
来源：http://bsa.dianchejie.cn

structuredClone(obj)
来源：http://wqf.pengpengdd.cyou

[U93] JS：模板字符串
来源：http://jwm.gogol.net.cn

`共 ${n} 条`
来源：http://iph.zhiwuduotai.top

[U94] JS：箭头函数
来源：http://elf.sufxvd.cn

const double = x => x * 2;
来源：http://slm.hnxiangtu.top

[U95] JS：Promise 包装
来源：http://nfm.nanxuanxn.top

new Promise((resolve, reject) => {})
来源：http://nrv.zhiwuduotai.top

[U96] JS：async/await 与异常
来源：http://hbm.epnwcf.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nzt.nwbrower.top

[U97] JS：并发请求
来源：http://vlo.ehwqpu.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://szs.316326.xyz

[U98] JS：fetch 带 JSON
来源：http://jaw.sxryk.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://izr.wangshuangyany.cn

[U99] JS：事件监听
来源：http://kgi.cdnleiting.top

el.addEventListener("click", e => {})
来源：http://gdm.hesvh.cn

[U100] JS：DOM 查询
来源：http://ejc.feifeiyinyue.top

document.querySelector(".item")
来源：http://czx.meibo888.top

[U101] JS：classList 操作
来源：http://pgy.zhixingplan.top

el.classList.toggle("active")
来源：http://jlq.ybcxt.top

[U102] JS：本地存储
来源：http://lkg.gzhubu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://vbe.yfazqb.com

[U103] JS：定时器
来源：http://jto.aizwys.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gxf.svipenyu.cn

[U104] JS：防抖
来源：http://uhu.wangdashe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ble.shuidangran.top

[U105] JS：节流
来源：http://kdg.zycfv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://azm.hysaishi.cn

[U106] JS：日期格式化
来源：http://dju.vehdjk.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ijl.hysaishi.cn

[U107] JS：数字千分位
来源：http://lkx.cashguo.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hym.jinghuilouyu.cn

[U108] JS：随机整数
来源：http://muo.yangfankeji.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zsg.vqdsnc.cn

[U109] JS：数组分组
来源：http://cdd.hongshengwenyu.top

Object.groupBy(arr, x => x.type)
来源：http://pps.meibo888.top

[U110] JS：数组分块
来源：http://zfd.0kj1m.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xrq.0kj1m.cn

[U111] JS：对象转 Map
来源：http://wch.jinghuilouyu.cn

new Map(Object.entries(obj))
来源：http://etc.fanxiaobao.xyz

[U112] JS：字符串补位
来源：http://diy.guowangkeji.top

"7".padStart(3, "0")
来源：http://jkr.hammf.cn

[U113] JS：正则替换全部
来源：http://bqn.aizwys.cn

s.replaceAll("a", "b")
来源：http://tpe.yonumen.top

[U114] JS：JSON 深比较
来源：http://yrb.shuidangran.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://vsy.haohaochexian.top

[U115] JS：生成 UUID
来源：http://qhd.316326.xyz

crypto.randomUUID()
来源：http://hvx.pengpengdd.cyou

[U116] JS：类型检查（JSDoc）
来源：http://vyd.9152youxi.cn

/** @param {string} name */ function f(name) {}
来源：http://rvd.bbcook.cn

[U117] JS：单元测试
来源：http://axg.yongpay.top

npm i -D vitest;  npx vitest
来源：http://nyr.guowangkeji.top

[U118] JS：开发服务器
来源：http://nad.vqdsnc.cn

npm i -D vite;  npx vite
来源：http://qqa.quarkkingdee.top

[U119] JS：生产构建
来源：http://nsv.vehdjk.com

npx vite build
来源：http://tyk.tianlin.xyz

[U120] JS：读取环境变量（Vite）
来源：http://ort.yj202588.top

import.meta.env.VITE_API_URL
来源：http://deh.cqqwz.cn

================================================================================
来源：http://rrn.shuidangran.top

统计汇总
来源：http://zlq.fktsv.cn

================================================================================
来源：http://bcw.yfazqb.com

按语言统计（条）：
来源：http://ddl.andypj.xyz

Python ......... 252
来源：http://nqo.chenlongwang.top

PHP ............ 252
来源：http://ynf.9152youxi.cn

JavaScript ..... 252
来源：http://jon.havefunace.top

TypeScript ..... 212
来源：http://ckw.zdbjq.cn

Java ........... 212
来源：http://boh.havefunace.top

Go ............. 212
来源：http://rmh.epnwcf.com

Ruby ........... 212
来源：http://ckf.jlsjyb.cn

C# ............. 212
来源：http://qme.iojbl.cn

C .............. 30
来源：http://jhh.meibo888.top

C++ ............ 30
来源：http://ybw.sjlbkw.cn

SQL ............ 90
来源：http://seu.tanke756.top

Bash ........... 80
来源：http://vcv.dianchejie.cn

Kotlin ......... 15
来源：http://bqe.yuxming.cn

Swift .......... 15
来源：http://hpq.sweek.top

Lua ............ 10
来源：http://lgb.yanxiufei.cn

Perl ........... 10
来源：http://kus.zhaomingkeji.xyz

Scala .......... 10
来源：http://fgn.shanyushiyangkeji.top

------------------------------------
来源：http://vvs.shanyushiyangtech.top

合计 ........... 2106 条
来源：http://ngu.xylfe.cn

按章节统计：
来源：http://kmq.hysaishi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://huf.smart0.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://aqs.jiagoushi.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vku.cqqwz.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mhz.sjlbkw.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pjj.uphjek.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://utz.jqgufenzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zop.haohaochexian.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ddq.gzhubu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zix.chenjidiqi.icu

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ven.zycfv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://stz.tanke756.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tum.jinqigufen.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rpn.yj20258888.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cbn.cheryme.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://iph.zhoulong.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vlf.nanxinkj.top

Q SQL 专题                              90
来源：http://wvd.zdbjq.cn

R Bash 专题                             80
来源：http://jyp.epnwcf.com

S C / C++ 专题                          60
来源：http://rua.tianlin.xyz

T 其他语言补充                          60
来源：http://jla.tian-w.cn

U 高频实用片段                         120
来源：http://axd.svipenyu.cn

------------------------------------
来源：http://yqk.sysykeji.top

合计                                  2106 条
来源：http://cbf.hesvh.cn

--------------------------------------------------------------------------------
来源：http://hvi.yonumen.top

使用提醒
来源：http://wtg.ydzc1.top

--------------------------------------------------------------------------------
来源：http://jts.gaohongyu789.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xrz.jqgufenzy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nuq.ydjk.org.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xxu.nanxuanxn.top

在旧版本上使用前请先确认语法支持情况。
来源：http://xpy.jinqigfzy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ktp.havefunace.top

—— 文件结束 ——
来源：http://yuh.wangdashe.top

================================================================================
来源：http://ntt.yj202588.top

程序语言常见例子速查手册（2024 版）
来源：http://hil.zhengqikj.top

Common Programming Examples Cheat Book
来源：http://rhp.redwolf501.top

================================================================================
来源：http://fec.andypj.xyz

【收录内容】
来源：http://vci.fanxiaobao.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://wkm.pengpengdd.cyou

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rfw.shzxlz.cn

SQL · Bash · C · C++
来源：http://tbn.haohaochexian.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qmt.jinqigfzy.top

【使用说明】
来源：http://sze.andypj.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://plu.kuanghao11.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ipf.ydzc1.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xhz.feifeiyinyue.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jae.dashuyun.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fsy.zhijiandao.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sty.pengpengdd.cyou

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rcv.hysaishi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zzl.zhaomingkeji.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gqx.yj202588.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lfv.shzxlz.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zkw.9152youxi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sfq.cashguo.top

【文件统计】
来源：http://djt.shuidangran.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mww.yongpay.top

--------------------------------------------------------------------------------
来源：http://kye.jqgfzy.top

目  录
来源：http://max.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://fro.hesvh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kww.52xcode.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pfs.yanxiufei.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fin.jiagoushi.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uld.ppjwa.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lew.jianghu66.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gmk.chenzaomai.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dqm.birdmap.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lux.c1oappe.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ifk.316326.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gli.daria6918.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mvv.jinqigfzy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xfj.chenjidiqi.icu

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jai.daria6918.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fxw.jinqigufen.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rfr.sysykeji.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yeh.ydjk.org.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://iqh.jqgufenzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://mha.ehwqpu.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lxx.cashguo.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gpd.jinqigufen.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mxq.fanxiaobao.xyz

================================================================================
来源：http://xdh.tian-w.cn

A. 基础语法与类型
来源：http://ova.0kj1m.cn

================================================================================
来源：http://lov.svipenyu.cn

[A01] Hello World
来源：http://jdg.shuidangran.top

Py:   print("Hello, World!")
来源：http://mos.yongpay.top

PHP:  echo "Hello, World!";
来源：http://hth.aibaodan.cn

JS:   console.log("Hello, World!");
来源：http://xxs.snrcjt.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://res.fanxiaobao.xyz

Java: System.out.println("Hello, World!");
来源：http://qmn.vqdsnc.cn

Go:   fmt.Println("Hello, World!")
来源：http://rie.xinyue.icu

Ruby: puts "Hello, World!"
来源：http://pyh.sysykeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://iph.jinqigfzy.top

[A02] 变量声明与赋值
来源：http://rny.xuetiantiany.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tjw.zhaomingkeji.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://ref.xinyue.icu

JS:   let name = "Alex"; const age = 20;
来源：http://xut.haohaochexian.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bjq.shzxlz.cn

Java: String name = "Alex"; int age = 20;
来源：http://oxw.iojbl.cn

Go:   name := "Alex"; age := 20
来源：http://xej.sxryk.cn

Ruby: name = "Alex"; age = 20
来源：http://ers.ydzc1.top

C#:   string name = "Alex"; int age = 20;
来源：http://kgw.yongpay.top

[A03] 常量定义
来源：http://xwt.zhiwuduotai.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wou.jinqigfzy.top

PHP:  const PI = 3.14159;
来源：http://grm.ehwqpu.com

JS:   const PI = 3.14159;
来源：http://bxj.wangshuangyany.cn

TS:   const PI: number = 3.14159;
来源：http://gdp.yuanzhike.top

Java: static final double PI = 3.14159;
来源：http://nfd.yueranfly.top

Go:   const PI = 3.14159
来源：http://fmc.aibaodan.cn

Ruby: PI = 3.14159
来源：http://hbt.dianchejie.cn

C#:   const double PI = 3.14159;
来源：http://web.havefunace.top

[A04] 判断变量类型
来源：http://nkb.yfazqb.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://tmk.c1oappe.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tun.9152youxi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qhg.hongshengwenyu.top

TS:   typeof x; x instanceof Date
来源：http://zsp.hcnkem.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nqv.meibo888.top

Go:   reflect.TypeOf(x).Name()
来源：http://pqf.birdmap.top

Ruby: x.class; x.is_a?(Integer)
来源：http://twv.hammf.cn

C#:   x.GetType().Name; x is int
来源：http://mxi.xziqi.cn

[A05] 整数除法与取模
来源：http://ekj.yuxming.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tjg.zhoulong.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://cee.sufxvd.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://izh.yueranfly.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://orj.birdmap.top

Java: 7 / 2; 7 % 2
来源：http://sce.fengsongda.top

Go:   7 / 2; 7 % 2
来源：http://xns.chenlongwang.top

Ruby: 7 / 2; 7 % 2
来源：http://dfy.havefunace.top

C#:   7 / 2; 7 % 2
来源：http://kcm.chenzaomai.com

[A06] 字符串转数字
来源：http://cgq.yueranfly.top

Py:   int("42"); float("3.14")
来源：http://aco.jqgfzy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lxn.yj20258.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://frk.zdbjq.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hoh.ydjk.org.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://npf.xziqi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dkg.sxryk.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bes.shangyingyoupin.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ljk.yuxming.cn

[A07] 数字转字符串
来源：http://pqe.quarkkingdee.top

Py:   str(42)
来源：http://geh.jianghu66.top

PHP:  (string) 42; strval(42)
来源：http://wgx.vehdjk.com

JS:   String(42); (42).toString()
来源：http://paa.yj202588.top

TS:   String(42)
来源：http://cmq.epnwcf.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://mgv.fengsongda.top

Go:   strconv.Itoa(42)
来源：http://uhp.aibaodan.cn

Ruby: 42.to_s
来源：http://ejc.hnqzz.top

C#:   42.ToString()
来源：http://jip.yueranfly.top

[A08] 取整与四舍五入
来源：http://ukl.andypj.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kuc.fengsongda.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://oam.sweek.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://asv.sjlbkw.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rez.zycfv.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://eeo.aibaodan.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xej.quarkkingdee.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://wlt.chenzaomai.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mzv.meibo888.top

[A09] 绝对值与最大最小值
来源：http://tyi.jinyuanbaomall.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kji.hnxiangtu.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gwn.hammf.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mab.shzxlz.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sqm.hysaishi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zwy.smart0.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cze.jqgfzy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lld.mhx1999.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ftt.smart0.xyz

[A10] 生成随机数
来源：http://tbh.316326.xyz

Py:   import random; random.randint(1, 100)
来源：http://qxl.shanyushiyangkeji.top

PHP:  random_int(1, 100);
来源：http://cue.epnwcf.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://frr.tian-w.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://idm.jinyuanbaomall.cn

Java: new Random().nextInt(100) + 1
来源：http://ywn.gaohongyu789.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dev.hnqzz.top

Ruby: rand(1..100)
来源：http://zrt.nanxinkj.top

C#:   new Random().Next(1, 101)
来源：http://kuk.xylfe.cn

[A11] 条件表达式（三元）
来源：http://hvt.tarul.cn

Py:   "yes" if x > 0 else "no"
来源：http://gpg.tianlin.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://knj.chenzaomai.com


<!-- 参考信息 -->