代发 wailian999

[U71] PHP：抛出异常
来源：http://oqx.gaohongyu789.top

throw new RuntimeException("失败", 500);
来源：http://kqg.zdqjudy.top

[U72] PHP：写错误日志
来源：http://bcc.yj20258888.top

error_log("失败: " . $e->getMessage());
来源：http://tbh.yuanzhike.top

[U73] PHP：读取 ini 配置
来源：http://pmf.yongpay.top

parse_ini_file("config.ini", true)
来源：http://smd.jinqigfzy.top

[U74] PHP：读取环境变量
来源：http://pfa.cheryme.top

getenv("APP_ENV") ?: "production"
来源：http://nuv.wangshuangyany.cn

[U75] PHP：依赖注入
来源：http://skb.cucudq.cn

composer require psr/container
来源：http://lwo.zdqjudy.top

[U76] PHP：简单路由
来源：http://ybj.snrcjt.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bxl.jyoumei.cn

[U77] PHP：模板渲染
来源：http://vcp.zdbjq.cn

composer require twig/twig
来源：http://xci.fengsongda.top

[U78] PHP：单元测试
来源：http://kha.shangyingyoupin.top

composer require --dev phpunit/phpunit
来源：http://kot.gaohongyu789.top

[U79] PHP：静态分析
来源：http://jsm.zhijiandao.cn

composer require --dev phpstan/phpstan
来源：http://ccr.shangyingyoupin.top

[U80] PHP：代码规范修复
来源：http://zco.ydjk.org.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yuh.zhoulong.xyz

[U81] JS：初始化项目
来源：http://wix.jinyuanbaomall.cn

npm init -y;  npm i express
来源：http://gwa.xuetiantiany.cn

[U82] JS：package.json 脚本
来源：http://nab.ydjk.org.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://coy.meibo888.top

[U83] JS：ES Module 导入导出
来源：http://tgl.hongshengwenyu.top

export const a = 1;  import { a } from "./m.js";
来源：http://djg.jinqigufen.top

[U84] JS：CommonJS 写法
来源：http://cec.jinghuilouyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://sqq.jinqigfzy.top

[U85] JS：可选链
来源：http://svo.andypj.xyz

a?.b?.c
来源：http://ebh.fehbvm.com

[U86] JS：空值合并
来源：http://siy.redwolf501.top

a ?? b
来源：http://uuy.shanyushiyangtech.top

[U87] JS：解构默认值
来源：http://moa.hongshengwenyu.top

const { a = 1, b = 2 } = obj;
来源：http://ydz.chenzaomai.com

[U88] JS：对象展开合并
来源：http://nkn.52xcode.cn

{ ...a, ...b }
来源：http://xhl.zhoulong.xyz

[U89] JS：数组去重
来源：http://pwm.jyoumei.cn

[...new Set(arr)]
来源：http://hjo.yuxming.cn

[U90] JS：数字数组排序
来源：http://wpt.nanxinkj.top

[...arr].sort((a, b) => a - b)
来源：http://qja.wangdashe.top

[U91] JS：对象键值遍历
来源：http://ahm.bbcook.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rdu.fehbvm.com

[U92] JS：深拷贝
来源：http://gpw.hnxiangtu.top

structuredClone(obj)
来源：http://mir.snrcjt.cn

[U93] JS：模板字符串
来源：http://mjv.ywan-chungtsiang.top

`共 ${n} 条`
来源：http://tpp.yj202588.top

[U94] JS：箭头函数
来源：http://tfl.bbcook.cn

const double = x => x * 2;
来源：http://ryq.havefunace.top

[U95] JS：Promise 包装
来源：http://hzr.yvedp.cn

new Promise((resolve, reject) => {})
来源：http://uwv.iojbl.cn

[U96] JS：async/await 与异常
来源：http://lsr.guannengcc.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://emo.ehwqpu.com

[U97] JS：并发请求
来源：http://hhz.hnxiangtu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://jra.fanxiaobao.xyz

[U98] JS：fetch 带 JSON
来源：http://jkq.shzxlz.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hyn.xuetiantiany.cn

[U99] JS：事件监听
来源：http://tio.haohaochexian.top

el.addEventListener("click", e => {})
来源：http://ljf.nwbrower.top

[U100] JS：DOM 查询
来源：http://bke.epnwcf.com

document.querySelector(".item")
来源：http://enc.jyoumei.cn

[U101] JS：classList 操作
来源：http://tuv.hysaishi.cn

el.classList.toggle("active")
来源：http://jzh.zycfv.cn

[U102] JS：本地存储
来源：http://izt.wangdashe.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://dqs.zhijiandao.cn

[U103] JS：定时器
来源：http://uxo.yfazqb.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gnq.hfpthk.cn

[U104] JS：防抖
来源：http://lzj.shuidangran.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nah.cashguo.top

[U105] JS：节流
来源：http://bak.yanxiufei.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mbu.gotoacloud.top

[U106] JS：日期格式化
来源：http://xwd.chenzaomai.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hyo.sysykeji.top

[U107] JS：数字千分位
来源：http://cze.zhoulong.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xyn.shzxlz.cn

[U108] JS：随机整数
来源：http://iqf.yonumen.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zaw.sxryk.cn

[U109] JS：数组分组
来源：http://gql.quarkkingdee.top

Object.groupBy(arr, x => x.type)
来源：http://nvv.iojbl.cn

[U110] JS：数组分块
来源：http://sjv.vehdjk.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kjh.chenlongwang.top

[U111] JS：对象转 Map
来源：http://zuz.c1oappe.top

new Map(Object.entries(obj))
来源：http://jdt.yuxming.cn

[U112] JS：字符串补位
来源：http://sij.yangfankeji.com

"7".padStart(3, "0")
来源：http://yse.ydjk.org.cn

[U113] JS：正则替换全部
来源：http://sjo.xingfuxueyuan.xyz

s.replaceAll("a", "b")
来源：http://csh.yfazqb.com

[U114] JS：JSON 深比较
来源：http://sxe.jianghu66.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://axb.shzxlz.cn

[U115] JS：生成 UUID
来源：http://xrc.zhijiandao.cn

crypto.randomUUID()
来源：http://irw.yuxming.cn

[U116] JS：类型检查（JSDoc）
来源：http://hne.zhixingplan.top

/** @param {string} name */ function f(name) {}
来源：http://ztw.hesvh.cn

[U117] JS：单元测试
来源：http://lfr.pycfn.com

npm i -D vitest;  npx vitest
来源：http://rla.gotoacloud.top

[U118] JS：开发服务器
来源：http://xjh.chenjidiqi.icu

npm i -D vite;  npx vite
来源：http://jwv.jinghuilouyu.cn

[U119] JS：生产构建
来源：http://ufh.fengsongda.top

npx vite build
来源：http://ztt.iojbl.cn

[U120] JS：读取环境变量（Vite）
来源：http://egx.epnwcf.com

import.meta.env.VITE_API_URL
来源：http://eef.yonumen.top

================================================================================
来源：http://tul.jyoumei.cn

统计汇总
来源：http://hru.zdqjudy.top

================================================================================
来源：http://gbc.smart0.xyz

按语言统计（条）：
来源：http://ptn.uphjek.com

Python ......... 252
来源：http://tvc.feifeiyinyue.top

PHP ............ 252
来源：http://ohc.yangfankeji.com

JavaScript ..... 252
来源：http://cmr.zhijiandao.cn

TypeScript ..... 212
来源：http://czy.svipenyu.cn

Java ........... 212
来源：http://tah.ywan-chungtsiang.top

Go ............. 212
来源：http://lnv.yanxiufei.cn

Ruby ........... 212
来源：http://qwk.sweek.top

C# ............. 212
来源：http://lcy.yuxming.cn

C .............. 30
来源：http://ztz.uphjek.com

C++ ............ 30
来源：http://ujw.daria6918.cn

SQL ............ 90
来源：http://eip.yueranfly.top

Bash ........... 80
来源：http://eah.yanxiufei.cn

Kotlin ......... 15
来源：http://smr.nwbrower.top

Swift .......... 15
来源：http://dvt.hongshengwenyu.top

Lua ............ 10
来源：http://cll.zhoulong.xyz

Perl ........... 10
来源：http://zks.hfpthk.cn

Scala .......... 10
来源：http://hpk.jinqigufen.top

------------------------------------
来源：http://cvf.chenlongwang.top

合计 ........... 2106 条
来源：http://mbo.jiagoushi.top

按章节统计：
来源：http://fza.yueranfly.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dwb.cashguo.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nfg.gaohongyu789.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xgw.feifeiyinyue.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ssl.sufxvd.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ekh.zhengqikj.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gdu.gaohongyu789.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cmb.vqdsnc.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vob.xingfuxueyuan.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xmk.fehbvm.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vwk.vehdjk.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dbl.andypj.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sif.52xcode.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vvr.vqdsnc.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tep.svipenyu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://whr.ybcxt.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://krl.tanke756.top

Q SQL 专题                              90
来源：http://ahd.chenlongwang.top

R Bash 专题                             80
来源：http://bay.yonumen.top

S C / C++ 专题                          60
来源：http://kpt.svipenyu.cn

T 其他语言补充                          60
来源：http://myl.yj20258.top

U 高频实用片段                         120
来源：http://bsb.zdqjudy.top

------------------------------------
来源：http://fpa.hnxiangtu.top

合计                                  2106 条
来源：http://twc.yj20258888.top

--------------------------------------------------------------------------------
来源：http://bnh.epnwcf.com

使用提醒
来源：http://igz.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://ejg.52xcode.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qmw.tianlin.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yqy.haohaochexian.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zzv.hongshengwenyu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://gwn.birdmap.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mrn.zhiwuduotai.top

—— 文件结束 ——
来源：http://crx.zhengqikj.top

================================================================================
来源：http://qsx.yj202588.top

程序语言常见例子速查手册（2024 版）
来源：http://tda.yongpay.top

Common Programming Examples Cheat Book
来源：http://har.ywan-chungtsiang.top

================================================================================
来源：http://hpj.nanxinkj.top

【收录内容】
来源：http://gfb.snrcjt.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xqt.jinqigufen.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://otf.cqqwz.cn

SQL · Bash · C · C++
来源：http://fje.snrcjt.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ltk.zdqjudy.top

【使用说明】
来源：http://azz.zhengqikj.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kqd.sufxvd.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xfm.gogol.net.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lxz.gaohongyu789.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sjb.sysykeji.top

Bash:  Shell         C:     C             C++:   C++
来源：http://aig.cheryme.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ktt.mhx1999.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bmb.ydzc1.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cai.andypj.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mzm.0kj1m.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://oza.smart0.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bhf.andypj.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gci.zdqjudy.top

【文件统计】
来源：http://dco.yonumen.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zal.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://jye.meibo888.top

目  录
来源：http://vpv.yangfankeji.com

--------------------------------------------------------------------------------
来源：http://qjz.hysaishi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lro.wangshuangyany.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pqr.daria6918.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://twx.cqqwz.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rlk.uphjek.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://auz.jinqigfzy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://spd.aizwys.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kzr.jinqigfzy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nod.jinyuanbaomall.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cop.sysykeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cpa.jyoumei.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zof.havefunace.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kpg.sweek.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nyw.nwbrower.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wxl.gaohongyu789.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bad.epnwcf.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vkq.zhengqikj.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://uuo.kuanghao11.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gxd.hongshengwenyu.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mfo.fengsongda.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kgf.xziqi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lkk.nanxinkj.top

================================================================================
来源：http://jbk.yuxming.cn

A. 基础语法与类型
来源：http://wqi.yuxming.cn

================================================================================
来源：http://jaj.shzxlz.cn

[A01] Hello World
来源：http://xbj.zdbjq.cn

Py:   print("Hello, World!")
来源：http://hzf.smart0.xyz

PHP:  echo "Hello, World!";
来源：http://yxg.zhijiandao.cn

JS:   console.log("Hello, World!");
来源：http://nhm.ydjk.org.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pxp.hnqzz.top

Java: System.out.println("Hello, World!");
来源：http://zyi.fehbvm.com

Go:   fmt.Println("Hello, World!")
来源：http://nwl.daria6918.cn

Ruby: puts "Hello, World!"
来源：http://gvx.shanyushiyangtech.top

C#:   Console.WriteLine("Hello, World!");
来源：http://qgh.zhoulong.xyz

[A02] 变量声明与赋值
来源：http://ylf.yfazqb.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xpu.xziqi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://nas.jinqigfzy.top

JS:   let name = "Alex"; const age = 20;
来源：http://nzz.cheryme.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dbv.fanxiaobao.xyz

Java: String name = "Alex"; int age = 20;
来源：http://dzc.yangfankeji.com

Go:   name := "Alex"; age := 20
来源：http://uae.daria6918.cn

Ruby: name = "Alex"; age = 20
来源：http://wqs.fengsongda.top

C#:   string name = "Alex"; int age = 20;
来源：http://hdz.yuxming.cn

[A03] 常量定义
来源：http://yht.chenjidiqi.icu

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wvs.hammf.cn

PHP:  const PI = 3.14159;
来源：http://wzj.shanyushiyangkeji.top

JS:   const PI = 3.14159;
来源：http://rqq.meibo888.top

TS:   const PI: number = 3.14159;
来源：http://vnp.jiagoushi.top

Java: static final double PI = 3.14159;
来源：http://klo.haohaochexian.top

Go:   const PI = 3.14159
来源：http://fwz.jinqigufen.top

Ruby: PI = 3.14159
来源：http://bit.kuanghao11.cn

C#:   const double PI = 3.14159;
来源：http://nji.bjfxy.top

[A04] 判断变量类型
来源：http://eme.shangyingyoupin.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ifk.xingfuxueyuan.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ayq.hnxiangtu.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://edz.zycfv.cn

TS:   typeof x; x instanceof Date
来源：http://hxk.xziqi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://aol.haohaochexian.top

Go:   reflect.TypeOf(x).Name()
来源：http://rmw.fehbvm.com

Ruby: x.class; x.is_a?(Integer)
来源：http://bde.yongpay.top

C#:   x.GetType().Name; x is int
来源：http://dlg.jinqigufen.top

[A05] 整数除法与取模
来源：http://wqv.vehdjk.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://usj.jianghu66.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://upd.cheryme.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zyz.epnwcf.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://htu.cheryme.top

Java: 7 / 2; 7 % 2
来源：http://uzx.zdbjq.cn

Go:   7 / 2; 7 % 2
来源：http://fzf.tarul.cn

Ruby: 7 / 2; 7 % 2
来源：http://tsz.cashguo.top

C#:   7 / 2; 7 % 2
来源：http://jzi.yangfankeji.com

[A06] 字符串转数字
来源：http://krv.ctjpmb.com

Py:   int("42"); float("3.14")
来源：http://fzh.shanyushiyangtech.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sup.pengpengdd.cyou

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jlw.vqdsnc.cn

TS:   parseInt("42", 10); Number("42")
来源：http://upp.hammf.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mdk.chenjidiqi.icu

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wuk.vehdjk.com

Ruby: "42".to_i; "3.14".to_f
来源：http://mce.sufxvd.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://azs.fktsv.cn

[A07] 数字转字符串
来源：http://kqr.wangshuangyany.cn

Py:   str(42)
来源：http://ngl.zhoulong.xyz

PHP:  (string) 42; strval(42)
来源：http://ght.yj202588.top

JS:   String(42); (42).toString()
来源：http://vvh.hnxiangtu.top

TS:   String(42)
来源：http://pvb.ctjpmb.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://ktw.cqqwz.cn

Go:   strconv.Itoa(42)
来源：http://ucx.gaohongyu789.top

Ruby: 42.to_s
来源：http://thn.andypj.xyz

C#:   42.ToString()
来源：http://bjl.gotoacloud.top

[A08] 取整与四舍五入
来源：http://eew.vqdsnc.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uha.hcnkem.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ixb.chenzaomai.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://djj.bbcook.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yek.cqqwz.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://snl.aibaodan.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cov.hesvh.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hxn.ppjwa.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wcn.316326.xyz

[A09] 绝对值与最大最小值
来源：http://vxx.sufxvd.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dse.cashguo.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://muj.gaohongyu789.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tok.andypj.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://oej.nwbrower.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rwd.vqdsnc.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cfw.jqgufenzy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nmk.shanyushiyangtech.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://usz.zhoulong.xyz

[A10] 生成随机数
来源：http://gsq.tianlin.xyz

Py:   import random; random.randint(1, 100)
来源：http://dfz.meibo888.top

PHP:  random_int(1, 100);
来源：http://dab.cdnleiting.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ajs.sjlbkw.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ltg.shanyushiyangkeji.top

Java: new Random().nextInt(100) + 1
来源：http://doh.yfazqb.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fej.cashguo.top

Ruby: rand(1..100)
来源：http://max.feifeiyinyue.top

C#:   new Random().Next(1, 101)
来源：http://unw.bbcook.cn

[A11] 条件表达式（三元）
来源：http://ntz.jinqigfzy.top

Py:   "yes" if x > 0 else "no"
来源：http://okx.yonumen.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://hsj.andypj.xyz


<!-- 参考信息 -->