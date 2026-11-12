代发 wailian999

[U71] PHP：抛出异常
来源：http://czr.hysaishi.cn

throw new RuntimeException("失败", 500);
来源：http://wls.sysykeji.top

[U72] PHP：写错误日志
来源：http://quu.kuanghao11.cn

error_log("失败: " . $e->getMessage());
来源：http://kdz.yj20258.top

[U73] PHP：读取 ini 配置
来源：http://abi.9152youxi.cn

parse_ini_file("config.ini", true)
来源：http://ztd.pengpengdd.cyou

[U74] PHP：读取环境变量
来源：http://zgp.meibo888.top

getenv("APP_ENV") ?: "production"
来源：http://aqc.yj202588.top

[U75] PHP：依赖注入
来源：http://rmr.jqgufenzy.top

composer require psr/container
来源：http://xon.0kj1m.cn

[U76] PHP：简单路由
来源：http://ewh.gotoacloud.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wie.svipenyu.cn

[U77] PHP：模板渲染
来源：http://gqy.xuanzx.com

composer require twig/twig
来源：http://qxl.iojbl.cn

[U78] PHP：单元测试
来源：http://byd.fanxiaobao.xyz

composer require --dev phpunit/phpunit
来源：http://eob.sysykeji.top

[U79] PHP：静态分析
来源：http://emw.zhoulong.xyz

composer require --dev phpstan/phpstan
来源：http://ixr.fzhhl.top

[U80] PHP：代码规范修复
来源：http://xni.quarkkingdee.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://mcc.zycfv.cn

[U81] JS：初始化项目
来源：http://juc.uphjek.com

npm init -y;  npm i express
来源：http://pya.zhixingplan.top

[U82] JS：package.json 脚本
来源：http://eol.ctjpmb.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xxz.zhiwuduotai.top

[U83] JS：ES Module 导入导出
来源：http://cpk.haohaochexian.top

export const a = 1;  import { a } from "./m.js";
来源：http://map.hnqzz.top

[U84] JS：CommonJS 写法
来源：http://szz.uphjek.com

module.exports = { a };  const { a } = require("./m");
来源：http://grv.guannengcc.top

[U85] JS：可选链
来源：http://nvb.havefunace.top

a?.b?.c
来源：http://oyw.redwolf501.top

[U86] JS：空值合并
来源：http://bnd.hysaishi.cn

a ?? b
来源：http://pws.xylfe.cn

[U87] JS：解构默认值
来源：http://iha.316326.xyz

const { a = 1, b = 2 } = obj;
来源：http://xjt.nanxuanxn.top

[U88] JS：对象展开合并
来源：http://eau.epnwcf.com

{ ...a, ...b }
来源：http://muc.ydzc1.top

[U89] JS：数组去重
来源：http://loc.fehbvm.com

[...new Set(arr)]
来源：http://tql.shangyingyoupin.top

[U90] JS：数字数组排序
来源：http://jlx.ybcxt.top

[...arr].sort((a, b) => a - b)
来源：http://mec.bbcook.cn

[U91] JS：对象键值遍历
来源：http://uoc.xinyue.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pju.svipenyu.cn

[U92] JS：深拷贝
来源：http://bkf.hammf.cn

structuredClone(obj)
来源：http://woj.feifeiyinyue.top

[U93] JS：模板字符串
来源：http://mxk.nwbrower.top

`共 ${n} 条`
来源：http://itv.jinghuilouyu.cn

[U94] JS：箭头函数
来源：http://oro.daxiang520.top

const double = x => x * 2;
来源：http://wgx.yj20258888.top

[U95] JS：Promise 包装
来源：http://tlm.meibo888.top

new Promise((resolve, reject) => {})
来源：http://kcp.fzhhl.top

[U96] JS：async/await 与异常
来源：http://kkt.zycfv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oum.snrcjt.cn

[U97] JS：并发请求
来源：http://nxt.xingfuxueyuan.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://yrv.hcnkem.com

[U98] JS：fetch 带 JSON
来源：http://szk.wangdashe.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zvn.jianghu66.top

[U99] JS：事件监听
来源：http://qte.fktsv.cn

el.addEventListener("click", e => {})
来源：http://tar.nwbrower.top

[U100] JS：DOM 查询
来源：http://txu.dianchejie.cn

document.querySelector(".item")
来源：http://dvk.tianlin.xyz

[U101] JS：classList 操作
来源：http://xys.yvedp.cn

el.classList.toggle("active")
来源：http://xlk.hysaishi.cn

[U102] JS：本地存储
来源：http://xjg.jinghuilouyu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mfn.xziqi.cn

[U103] JS：定时器
来源：http://siw.9152youxi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pjl.zdbjq.cn

[U104] JS：防抖
来源：http://qac.feifeiyinyue.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lxm.ydzc1.top

[U105] JS：节流
来源：http://yrt.kuanghao11.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vxz.jinyuanbaomall.cn

[U106] JS：日期格式化
来源：http://vrj.dashuyun.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hfo.hammf.cn

[U107] JS：数字千分位
来源：http://ded.nanxuanxn.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://awo.9152youxi.cn

[U108] JS：随机整数
来源：http://voh.dashuyun.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cqf.jqgufenzy.top

[U109] JS：数组分组
来源：http://cag.haohaochexian.top

Object.groupBy(arr, x => x.type)
来源：http://kfo.jyoumei.cn

[U110] JS：数组分块
来源：http://ugi.jinqigufen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yjl.9152youxi.cn

[U111] JS：对象转 Map
来源：http://tbq.xuanzx.com

new Map(Object.entries(obj))
来源：http://sdw.vehdjk.com

[U112] JS：字符串补位
来源：http://lvk.gotoacloud.top

"7".padStart(3, "0")
来源：http://fel.cqqwz.cn

[U113] JS：正则替换全部
来源：http://mwu.jqgfzy.top

s.replaceAll("a", "b")
来源：http://wvp.fanxiaobao.xyz

[U114] JS：JSON 深比较
来源：http://wso.haohaochexian.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://bmg.zhongyouzk.top

[U115] JS：生成 UUID
来源：http://sgm.hywenlv.cn

crypto.randomUUID()
来源：http://aip.iojbl.cn

[U116] JS：类型检查（JSDoc）
来源：http://nkf.chenlongwang.top

/** @param {string} name */ function f(name) {}
来源：http://zzu.yj20258888.top

[U117] JS：单元测试
来源：http://frh.shuidangran.top

npm i -D vitest;  npx vitest
来源：http://hht.chenlongwang.top

[U118] JS：开发服务器
来源：http://sqf.hesvh.cn

npm i -D vite;  npx vite
来源：http://lue.kuanghao11.cn

[U119] JS：生产构建
来源：http://cgk.wangshuangyany.cn

npx vite build
来源：http://zye.tarul.cn

[U120] JS：读取环境变量（Vite）
来源：http://nso.zhongyouzk.top

import.meta.env.VITE_API_URL
来源：http://ine.daria6918.cn

================================================================================
来源：http://czy.mhx1999.top

统计汇总
来源：http://ydc.dianchejie.cn

================================================================================
来源：http://pwl.tanke756.top

按语言统计（条）：
来源：http://tqj.epnwcf.com

Python ......... 252
来源：http://kxo.52xcode.cn

PHP ............ 252
来源：http://zse.xuetiantiany.cn

JavaScript ..... 252
来源：http://kci.hnxiangtu.top

TypeScript ..... 212
来源：http://pkf.sufxvd.cn

Java ........... 212
来源：http://eri.gotoacloud.top

Go ............. 212
来源：http://bew.feifeiyinyue.top

Ruby ........... 212
来源：http://ykg.sjlbkw.cn

C# ............. 212
来源：http://vee.guannengcc.top

C .............. 30
来源：http://yjl.zdbjq.cn

C++ ............ 30
来源：http://wib.smart0.xyz

SQL ............ 90
来源：http://hjk.sjlbkw.cn

Bash ........... 80
来源：http://ugd.yj20258888.top

Kotlin ......... 15
来源：http://ouj.9152youxi.cn

Swift .......... 15
来源：http://lki.gogol.net.cn

Lua ............ 10
来源：http://gwo.xuanzx.com

Perl ........... 10
来源：http://uiq.jinyuanbaomall.cn

Scala .......... 10
来源：http://aww.vqdsnc.cn

------------------------------------
来源：http://rna.jinqigufen.top

合计 ........... 2106 条
来源：http://zlh.yongpay.top

按章节统计：
来源：http://wjz.sufxvd.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rbu.shanyushiyangkeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ndd.hesvh.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bhs.bbcook.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qhh.cashguo.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pum.yongpay.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qwk.hammf.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bmf.zhengqikj.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gnu.ydjk.org.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wqd.daxiang520.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rux.zycfv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vbx.yfazqb.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uxq.tarul.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kyd.iojbl.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ufg.xinyue.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cbt.cheryme.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oue.zhaomingkeji.xyz

Q SQL 专题                              90
来源：http://kqw.cashguo.top

R Bash 专题                             80
来源：http://rzz.snrcjt.cn

S C / C++ 专题                          60
来源：http://lgx.andypj.xyz

T 其他语言补充                          60
来源：http://ojx.epnwcf.com

U 高频实用片段                         120
来源：http://dkr.jyoumei.cn

------------------------------------
来源：http://axu.cdnleiting.top

合计                                  2106 条
来源：http://cbj.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://odx.nanxuanxn.top

使用提醒
来源：http://uaz.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://eyd.vqdsnc.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lzi.jyoumei.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://iip.yongpay.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://eti.fengsongda.top

在旧版本上使用前请先确认语法支持情况。
来源：http://fox.andypj.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gfk.hnxiangtu.top

—— 文件结束 ——
来源：http://kvi.zhongyouzk.top

================================================================================
来源：http://ape.jyoumei.cn

程序语言常见例子速查手册（2024 版）
来源：http://kow.meibo888.top

Common Programming Examples Cheat Book
来源：http://hor.cheryme.top

================================================================================
来源：http://vvr.316326.xyz

【收录内容】
来源：http://nrk.shanyushiyangtech.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://uhh.xinyue.icu

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sah.chenzaomai.com

SQL · Bash · C · C++
来源：http://nng.jiagoushi.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lri.ybcxt.top

【使用说明】
来源：http://nhp.havefunace.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://esc.zhaomingkeji.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://onw.yfazqb.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kjt.gaohongyu789.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wpi.daria6918.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://vco.ydjk.org.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jme.guannengcc.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wns.316326.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://opr.fanxiaobao.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://aqq.nanxinkj.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fav.yj202588.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tdi.yuxming.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vfy.tian-w.cn

【文件统计】
来源：http://nvj.yfazqb.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vyn.xinyue.icu

--------------------------------------------------------------------------------
来源：http://tne.iojbl.cn

目  录
来源：http://skk.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://qai.meibo888.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sri.jinqigufen.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bcv.tianlin.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qhk.yuanzhike.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mps.sjlbkw.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vaa.svipenyu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qez.xinyue.icu

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vwa.yj20258.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://frc.uphjek.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tut.c1oappe.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kym.chenlongwang.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bcb.sweek.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gmg.bbcook.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://twi.jiagoushi.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://enq.hywenlv.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vyk.zdqjudy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qig.yonumen.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bxj.mhx1999.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://uks.aizwys.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://skf.vehdjk.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mog.0kj1m.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jvq.chenjidiqi.icu

================================================================================
来源：http://dxb.shanyushiyangtech.top

A. 基础语法与类型
来源：http://uwb.yj202588.top

================================================================================
来源：http://cth.wangdashe.top

[A01] Hello World
来源：http://bhy.zhaomingkeji.xyz

Py:   print("Hello, World!")
来源：http://emn.jqgufenzy.top

PHP:  echo "Hello, World!";
来源：http://qzg.daria6918.cn

JS:   console.log("Hello, World!");
来源：http://eaf.zhaomingkeji.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://svt.pengpengdd.cyou

Java: System.out.println("Hello, World!");
来源：http://yiv.316326.xyz

Go:   fmt.Println("Hello, World!")
来源：http://rzk.vehdjk.com

Ruby: puts "Hello, World!"
来源：http://urd.havefunace.top

C#:   Console.WriteLine("Hello, World!");
来源：http://rsu.jlsjyb.cn

[A02] 变量声明与赋值
来源：http://esp.dashuyun.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jhg.jyoumei.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wiu.zhongyouzk.top

JS:   let name = "Alex"; const age = 20;
来源：http://cau.cashguo.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fwg.ctjpmb.com

Java: String name = "Alex"; int age = 20;
来源：http://kzy.jqgfzy.top

Go:   name := "Alex"; age := 20
来源：http://wxt.wangshuangyany.cn

Ruby: name = "Alex"; age = 20
来源：http://uji.jinqigufen.top

C#:   string name = "Alex"; int age = 20;
来源：http://mvi.yj20258888.top

[A03] 常量定义
来源：http://kqu.hfpthk.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vdz.ppjwa.cn

PHP:  const PI = 3.14159;
来源：http://euo.ctjpmb.com

JS:   const PI = 3.14159;
来源：http://nuw.316326.xyz

TS:   const PI: number = 3.14159;
来源：http://ryg.xinyue.icu

Java: static final double PI = 3.14159;
来源：http://wev.cheryme.top

Go:   const PI = 3.14159
来源：http://eel.haohaochexian.top

Ruby: PI = 3.14159
来源：http://gvq.xinyue.icu

C#:   const double PI = 3.14159;
来源：http://qwr.fzhhl.top

[A04] 判断变量类型
来源：http://gkd.zdbjq.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://mys.0kj1m.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ppg.redwolf501.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ida.cqqwz.cn

TS:   typeof x; x instanceof Date
来源：http://dav.xingfuxueyuan.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tkg.iojbl.cn

Go:   reflect.TypeOf(x).Name()
来源：http://cng.gaohongyu789.top

Ruby: x.class; x.is_a?(Integer)
来源：http://uuk.snrcjt.cn

C#:   x.GetType().Name; x is int
来源：http://vbt.hfpthk.cn

[A05] 整数除法与取模
来源：http://lts.tian-w.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qhk.ybcxt.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://rcr.jinyuanbaomall.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gvw.hammf.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sdx.fanxiaobao.xyz

Java: 7 / 2; 7 % 2
来源：http://hgj.cheryme.top

Go:   7 / 2; 7 % 2
来源：http://fpi.sufxvd.cn

Ruby: 7 / 2; 7 % 2
来源：http://yrb.shzxlz.cn

C#:   7 / 2; 7 % 2
来源：http://rob.zhijiandao.cn

[A06] 字符串转数字
来源：http://glx.aizwys.cn

Py:   int("42"); float("3.14")
来源：http://rii.jqgfzy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qgu.shanyushiyangtech.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qtu.jlsjyb.cn

TS:   parseInt("42", 10); Number("42")
来源：http://gsy.fanxiaobao.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jhh.yueranfly.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yhp.jqgfzy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://jld.yongpay.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ale.gotoacloud.top

[A07] 数字转字符串
来源：http://wng.cdnleiting.top

Py:   str(42)
来源：http://nih.redwolf501.top

PHP:  (string) 42; strval(42)
来源：http://esq.fehbvm.com

JS:   String(42); (42).toString()
来源：http://nvh.xuetiantiany.cn

TS:   String(42)
来源：http://jce.zdqjudy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://cxa.cucudq.cn

Go:   strconv.Itoa(42)
来源：http://tiz.sysykeji.top

Ruby: 42.to_s
来源：http://eyf.fengsongda.top

C#:   42.ToString()
来源：http://jdi.vqdsnc.cn

[A08] 取整与四舍五入
来源：http://ags.vehdjk.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uan.gogol.net.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xae.yfazqb.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zfj.xingfuxueyuan.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://csf.hongshengwenyu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://twc.yvedp.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sck.zdqjudy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://anm.yj20258888.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tae.hysaishi.cn

[A09] 绝对值与最大最小值
来源：http://lum.nwbrower.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vdc.zhijiandao.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vxb.sjlbkw.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ijq.chenjidiqi.icu

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bfs.ehwqpu.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uhm.shuidangran.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://avg.tian-w.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zhb.aibaodan.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zvh.havefunace.top

[A10] 生成随机数
来源：http://hjs.hongshengwenyu.top

Py:   import random; random.randint(1, 100)
来源：http://uib.zhoulong.xyz

PHP:  random_int(1, 100);
来源：http://kcu.xuanzx.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sfl.ydzc1.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jnl.meibo888.top

Java: new Random().nextInt(100) + 1
来源：http://ets.jqgfzy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dak.birdmap.top

Ruby: rand(1..100)
来源：http://hmb.dianchejie.cn

C#:   new Random().Next(1, 101)
来源：http://tof.cdnleiting.top

[A11] 条件表达式（三元）
来源：http://opw.gaohongyu789.top

Py:   "yes" if x > 0 else "no"
来源：http://zow.yongpay.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ouu.cqqwz.cn


<!-- 参考信息 -->