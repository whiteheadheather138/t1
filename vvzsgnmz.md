代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://ddv.0kj1m.cn

parse_ini_file("config.ini", true)
来源：http://vfn.ydjk.org.cn

[U74] PHP：读取环境变量
来源：http://jwp.zhaomingkeji.xyz

getenv("APP_ENV") ?: "production"
来源：http://oor.bjfxy.top

[U75] PHP：依赖注入
来源：http://eqf.cdnleiting.top

composer require psr/container
来源：http://auk.cqqwz.cn

[U76] PHP：简单路由
来源：http://ysa.zhongyouzk.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fuk.bjfxy.top

[U77] PHP：模板渲染
来源：http://yxd.yangfankeji.com

composer require twig/twig
来源：http://xkv.shuidangran.top

[U78] PHP：单元测试
来源：http://ywg.havefunace.top

composer require --dev phpunit/phpunit
来源：http://bcq.ehwqpu.com

[U79] PHP：静态分析
来源：http://lkv.havefunace.top

composer require --dev phpstan/phpstan
来源：http://hqv.jinyuanbaomall.cn

[U80] PHP：代码规范修复
来源：http://whi.xuanzx.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://mhj.smart0.xyz

[U81] JS：初始化项目
来源：http://cig.hnxiangtu.top

npm init -y;  npm i express
来源：http://ucn.meibo888.top

[U82] JS：package.json 脚本
来源：http://vlr.zhongyouzk.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vom.tian-w.cn

[U83] JS：ES Module 导入导出
来源：http://pgt.dianchejie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vnw.hongshengwenyu.top

[U84] JS：CommonJS 写法
来源：http://tul.shzxlz.cn

module.exports = { a };  const { a } = require("./m");
来源：http://unu.feifeiyinyue.top

[U85] JS：可选链
来源：http://jmp.tarul.cn

a?.b?.c
来源：http://zhs.yangfankeji.com

[U86] JS：空值合并
来源：http://paw.yuxming.cn

a ?? b
来源：http://nri.andypj.xyz

[U87] JS：解构默认值
来源：http://ulm.daria6918.cn

const { a = 1, b = 2 } = obj;
来源：http://dwl.guannengcc.top

[U88] JS：对象展开合并
来源：http://fdc.gaohongyu789.top

{ ...a, ...b }
来源：http://qvq.tarul.cn

[U89] JS：数组去重
来源：http://ycs.chenjidiqi.icu

[...new Set(arr)]
来源：http://okz.hywenlv.cn

[U90] JS：数字数组排序
来源：http://bin.tian-w.cn

[...arr].sort((a, b) => a - b)
来源：http://pxo.xinyue.icu

[U91] JS：对象键值遍历
来源：http://gwt.tarul.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rzg.xziqi.cn

[U92] JS：深拷贝
来源：http://gyv.xingfuxueyuan.xyz

structuredClone(obj)
来源：http://tkz.tarul.cn

[U93] JS：模板字符串
来源：http://uwi.nanxuanxn.top

`共 ${n} 条`
来源：http://hmr.svipenyu.cn

[U94] JS：箭头函数
来源：http://jfd.yangfankeji.com

const double = x => x * 2;
来源：http://yci.jqgufenzy.top

[U95] JS：Promise 包装
来源：http://gdh.ctjpmb.com

new Promise((resolve, reject) => {})
来源：http://had.iojbl.cn

[U96] JS：async/await 与异常
来源：http://ani.aibaodan.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://smw.shangyingyoupin.top

[U97] JS：并发请求
来源：http://tvf.xziqi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://iom.nanxuanxn.top

[U98] JS：fetch 带 JSON
来源：http://lfm.zhaomingkeji.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ufr.hywenlv.cn

[U99] JS：事件监听
来源：http://sfd.yangfankeji.com

el.addEventListener("click", e => {})
来源：http://cod.zhixingplan.top

[U100] JS：DOM 查询
来源：http://uqs.yj20258.top

document.querySelector(".item")
来源：http://zlz.feifeiyinyue.top

[U101] JS：classList 操作
来源：http://gvy.yuanzhike.top

el.classList.toggle("active")
来源：http://hqj.daria6918.cn

[U102] JS：本地存储
来源：http://fnm.yonumen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://dmj.yuxming.cn

[U103] JS：定时器
来源：http://med.nwbrower.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://msh.wangdashe.top

[U104] JS：防抖
来源：http://eeb.zdqjudy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xui.vqdsnc.cn

[U105] JS：节流
来源：http://mmm.daria6918.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ezi.gzhubu.top

[U106] JS：日期格式化
来源：http://cjr.sweek.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dqy.hysaishi.cn

[U107] JS：数字千分位
来源：http://plj.shangyingyoupin.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xio.yuxming.cn

[U108] JS：随机整数
来源：http://chx.gaohongyu789.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ojn.andypj.xyz

[U109] JS：数组分组
来源：http://bao.shanyushiyangkeji.top

Object.groupBy(arr, x => x.type)
来源：http://egb.hnxiangtu.top

[U110] JS：数组分块
来源：http://eio.daxiang520.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mpw.52xcode.cn

[U111] JS：对象转 Map
来源：http://ahj.sysykeji.top

new Map(Object.entries(obj))
来源：http://shy.yongpay.top

[U112] JS：字符串补位
来源：http://hvc.ctjpmb.com

"7".padStart(3, "0")
来源：http://krh.nwbrower.top

[U113] JS：正则替换全部
来源：http://jwy.shuidangran.top

s.replaceAll("a", "b")
来源：http://gzz.fengsongda.top

[U114] JS：JSON 深比较
来源：http://cos.fktsv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://buc.andypj.xyz

[U115] JS：生成 UUID
来源：http://hep.zhixingplan.top

crypto.randomUUID()
来源：http://fkf.jinqigfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://ydd.fengsongda.top

/** @param {string} name */ function f(name) {}
来源：http://xbh.gaohongyu789.top

[U117] JS：单元测试
来源：http://yvu.hesvh.cn

npm i -D vitest;  npx vitest
来源：http://tou.xuetiantiany.cn

[U118] JS：开发服务器
来源：http://dvu.yueranfly.top

npm i -D vite;  npx vite
来源：http://bbc.pengpengdd.cyou

[U119] JS：生产构建
来源：http://fzx.iojbl.cn

npx vite build
来源：http://zjx.zhaomingkeji.xyz

[U120] JS：读取环境变量（Vite）
来源：http://txm.yuanzhike.top

import.meta.env.VITE_API_URL
来源：http://chy.cucudq.cn

================================================================================
来源：http://fgi.nanxinkj.top

统计汇总
来源：http://aui.sufxvd.cn

================================================================================
来源：http://zzq.316326.xyz

按语言统计（条）：
来源：http://xjz.zycfv.cn

Python ......... 252
来源：http://gdq.316326.xyz

PHP ............ 252
来源：http://cxk.hcnkem.com

JavaScript ..... 252
来源：http://lcb.zdqjudy.top

TypeScript ..... 212
来源：http://sin.tarul.cn

Java ........... 212
来源：http://kpr.zhaomingkeji.xyz

Go ............. 212
来源：http://awh.feifeiyinyue.top

Ruby ........... 212
来源：http://rdt.fanxiaobao.xyz

C# ............. 212
来源：http://knd.yj20258.top

C .............. 30
来源：http://neu.hfpthk.cn

C++ ............ 30
来源：http://mfk.jiagoushi.top

SQL ............ 90
来源：http://qbs.hongshengwenyu.top

Bash ........... 80
来源：http://mft.gotoacloud.top

Kotlin ......... 15
来源：http://szg.dashuyun.cn

Swift .......... 15
来源：http://vrq.sxryk.cn

Lua ............ 10
来源：http://hed.hysaishi.cn

Perl ........... 10
来源：http://sei.cucudq.cn

Scala .......... 10
来源：http://nif.ydjk.org.cn

------------------------------------
来源：http://aso.cqqwz.cn

合计 ........... 2106 条
来源：http://yzc.tanke756.top

按章节统计：
来源：http://jat.meibo888.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hqh.hfpthk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yyf.hcnkem.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://adg.jqgufenzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jtl.shangyingyoupin.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rnh.xingfuxueyuan.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rtj.sjlbkw.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ria.shanyushiyangtech.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dzn.hnqzz.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qky.sweek.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vzh.feifeiyinyue.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fgx.jinqigfzy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fuo.zhaomingkeji.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tag.fehbvm.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yxp.wangdashe.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://oaz.shanyushiyangtech.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bnu.yonumen.top

Q SQL 专题                              90
来源：http://fgo.jinqigfzy.top

R Bash 专题                             80
来源：http://rgy.snrcjt.cn

S C / C++ 专题                          60
来源：http://bzx.zhijiandao.cn

T 其他语言补充                          60
来源：http://byr.yonumen.top

U 高频实用片段                         120
来源：http://gve.jinghuilouyu.cn

------------------------------------
来源：http://oms.zhaomingkeji.xyz

合计                                  2106 条
来源：http://fsl.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://gjt.pycfn.com

使用提醒
来源：http://obc.yongpay.top

--------------------------------------------------------------------------------
来源：http://dfa.havefunace.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yfs.hcnkem.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lwi.smart0.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dug.bjfxy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://snr.jinyuanbaomall.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tkk.wangdashe.top

—— 文件结束 ——
来源：http://cyy.ydjk.org.cn

================================================================================
来源：http://lpu.redwolf501.top

程序语言常见例子速查手册（2024 版）
来源：http://drp.vehdjk.com

Common Programming Examples Cheat Book
来源：http://cki.fehbvm.com

================================================================================
来源：http://ghq.smart0.xyz

【收录内容】
来源：http://gsr.fktsv.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rxl.haohaochexian.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ccq.yj20258.top

SQL · Bash · C · C++
来源：http://hnr.dianchejie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jwx.yanxiufei.cn

【使用说明】
来源：http://oui.havefunace.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bxl.cucudq.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lpd.dashuyun.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dtm.jinqigfzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kqj.yanxiufei.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://vtq.shanyushiyangtech.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rwt.ctjpmb.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rqr.ivvv.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tvy.fzhhl.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://shi.gotoacloud.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tas.dashuyun.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bfp.sufxvd.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bbc.cdnleiting.top

【文件统计】
来源：http://bow.ctjpmb.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mdi.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://mca.aizwys.cn

目  录
来源：http://nrw.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://aqt.chenlongwang.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gce.haohaochexian.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ovy.dianchejie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lzy.ybcxt.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yff.fehbvm.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ino.yonumen.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vfw.sxryk.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cgy.hnqzz.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jkw.jinyuanbaomall.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://isa.kuanghao11.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lkp.wangshuangyany.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gar.haohaochexian.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://suu.zhaomingkeji.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fnm.shangyingyoupin.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://asj.haohaochexian.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bli.zhongyouzk.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xiq.hywenlv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xcw.shuidangran.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://tya.hywenlv.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://drt.ppjwa.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zfk.snrcjt.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fkz.hywenlv.cn

================================================================================
来源：http://uze.hfpthk.cn

A. 基础语法与类型
来源：http://kwk.yuxming.cn

================================================================================
来源：http://jbt.tian-w.cn

[A01] Hello World
来源：http://pln.jinqigfzy.top

Py:   print("Hello, World!")
来源：http://zum.feifeiyinyue.top

PHP:  echo "Hello, World!";
来源：http://rco.sjlbkw.cn

JS:   console.log("Hello, World!");
来源：http://bxb.xuetiantiany.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yut.pengpengdd.cyou

Java: System.out.println("Hello, World!");
来源：http://trg.kuanghao11.cn

Go:   fmt.Println("Hello, World!")
来源：http://ryn.hnxiangtu.top

Ruby: puts "Hello, World!"
来源：http://cxu.jqgfzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://mne.hesvh.cn

[A02] 变量声明与赋值
来源：http://nvf.wangdashe.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://iaj.jlsjyb.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://lga.xylfe.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sxt.xziqi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ire.jinqigfzy.top

Java: String name = "Alex"; int age = 20;
来源：http://yoo.yj20258.top

Go:   name := "Alex"; age := 20
来源：http://wam.yongpay.top

Ruby: name = "Alex"; age = 20
来源：http://ivj.ehwqpu.com

C#:   string name = "Alex"; int age = 20;
来源：http://ydh.zhengqikj.top

[A03] 常量定义
来源：http://hyw.gotoacloud.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://aea.feifeiyinyue.top

PHP:  const PI = 3.14159;
来源：http://irr.ppjwa.cn

JS:   const PI = 3.14159;
来源：http://zge.zhaomingkeji.xyz

TS:   const PI: number = 3.14159;
来源：http://ktp.dashuyun.cn

Java: static final double PI = 3.14159;
来源：http://cew.tanke756.top

Go:   const PI = 3.14159
来源：http://fbe.jinghuilouyu.cn

Ruby: PI = 3.14159
来源：http://hyz.quarkkingdee.top

C#:   const double PI = 3.14159;
来源：http://ixq.sufxvd.cn

[A04] 判断变量类型
来源：http://paj.shanyushiyangkeji.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://qxh.cdnleiting.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vhj.sweek.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xua.sjlbkw.cn

TS:   typeof x; x instanceof Date
来源：http://gfz.hfpthk.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tht.fktsv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://scn.dianchejie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tqj.uphjek.com

C#:   x.GetType().Name; x is int
来源：http://tkk.guowangkeji.top

[A05] 整数除法与取模
来源：http://wby.cdnleiting.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nms.fzhhl.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://hnq.ywan-chungtsiang.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://joo.jinyuanbaomall.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ygm.haohaochexian.top

Java: 7 / 2; 7 % 2
来源：http://tro.chenzaomai.com

Go:   7 / 2; 7 % 2
来源：http://mge.yongpay.top

Ruby: 7 / 2; 7 % 2
来源：http://tmg.dianchejie.cn

C#:   7 / 2; 7 % 2
来源：http://icw.zhongyouzk.top

[A06] 字符串转数字
来源：http://lpt.zhiwuduotai.top

Py:   int("42"); float("3.14")
来源：http://ehh.ybcxt.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ayg.yueranfly.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nkj.xylfe.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kex.ehwqpu.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qhh.yongpay.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://knw.xinyue.icu

Ruby: "42".to_i; "3.14".to_f
来源：http://luw.jinghuilouyu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vek.cqqwz.cn

[A07] 数字转字符串
来源：http://afa.zhiwuduotai.top

Py:   str(42)
来源：http://ija.zhaomingkeji.xyz

PHP:  (string) 42; strval(42)
来源：http://zmy.hesvh.cn

JS:   String(42); (42).toString()
来源：http://bjk.ywan-chungtsiang.top

TS:   String(42)
来源：http://spp.yvedp.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://yss.hongshengwenyu.top

Go:   strconv.Itoa(42)
来源：http://kkj.gaohongyu789.top

Ruby: 42.to_s
来源：http://cwu.jinyuanbaomall.cn

C#:   42.ToString()
来源：http://yvf.uphjek.com

[A08] 取整与四舍五入
来源：http://nsw.9152youxi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xdp.zhijiandao.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mip.haohaochexian.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jbs.zdqjudy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xek.cdnleiting.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vji.fktsv.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yvt.fanxiaobao.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://yjr.wangdashe.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://exp.zhiwuduotai.top

[A09] 绝对值与最大最小值
来源：http://uix.zdqjudy.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yte.chenjidiqi.icu

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qaa.jqgfzy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kua.hesvh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fyo.ydjk.org.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tbm.hysaishi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ywr.aibaodan.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hai.ydzc1.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kxn.zhengqikj.top

[A10] 生成随机数
来源：http://otd.yfazqb.com

Py:   import random; random.randint(1, 100)
来源：http://xed.smart0.xyz

PHP:  random_int(1, 100);
来源：http://acf.redwolf501.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mqb.ehwqpu.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cyx.cheryme.top

Java: new Random().nextInt(100) + 1
来源：http://qsz.zdbjq.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hhd.fzhhl.top

Ruby: rand(1..100)
来源：http://jfe.yanxiufei.cn

C#:   new Random().Next(1, 101)
来源：http://hgd.shanyushiyangtech.top

[A11] 条件表达式（三元）
来源：http://blw.dianchejie.cn

Py:   "yes" if x > 0 else "no"
来源：http://owk.shanyushiyangkeji.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://oxl.havefunace.top

JS:   x > 0 ? "yes" : "no"
来源：http://xrk.daria6918.cn

TS:   x > 0 ? "yes" : "no"
来源：http://map.hysaishi.cn

Java: x > 0 ? "yes" : "no"
来源：http://mcf.yvedp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zzj.shanyushiyangkeji.top


<!-- 参考信息 -->