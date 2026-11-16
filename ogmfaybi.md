代发 wailian999

[U69] PHP：PDO 预处理
来源：http://xca.fengsongda.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nbs.ppjwa.cn

[U70] PHP：PDO 事务
来源：http://atx.xuanzx.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dao.9152youxi.cn

[U71] PHP：抛出异常
来源：http://sma.hnqzz.top

throw new RuntimeException("失败", 500);
来源：http://gno.jyoumei.cn

[U72] PHP：写错误日志
来源：http://vos.tanke756.top

error_log("失败: " . $e->getMessage());
来源：http://pvh.jqgfzy.top

[U73] PHP：读取 ini 配置
来源：http://irv.shanyushiyangtech.top

parse_ini_file("config.ini", true)
来源：http://rxk.jlsjyb.cn

[U74] PHP：读取环境变量
来源：http://qtq.sjlbkw.cn

getenv("APP_ENV") ?: "production"
来源：http://kzi.jinqigufen.top

[U75] PHP：依赖注入
来源：http://duo.xuetiantiany.cn

composer require psr/container
来源：http://vhj.cashguo.top

[U76] PHP：简单路由
来源：http://awt.xinyue.icu

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cqh.yonumen.top

[U77] PHP：模板渲染
来源：http://pnu.chenlongwang.top

composer require twig/twig
来源：http://ncu.hysaishi.cn

[U78] PHP：单元测试
来源：http://chx.ivvv.top

composer require --dev phpunit/phpunit
来源：http://qmk.feifeiyinyue.top

[U79] PHP：静态分析
来源：http://exn.zhixingplan.top

composer require --dev phpstan/phpstan
来源：http://rld.hnxiangtu.top

[U80] PHP：代码规范修复
来源：http://pmk.aizwys.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://uqw.daxiang520.top

[U81] JS：初始化项目
来源：http://dnb.hammf.cn

npm init -y;  npm i express
来源：http://nzg.guannengcc.top

[U82] JS：package.json 脚本
来源：http://wyv.vehdjk.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bkp.fanxiaobao.xyz

[U83] JS：ES Module 导入导出
来源：http://mbv.ppjwa.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mjg.svipenyu.cn

[U84] JS：CommonJS 写法
来源：http://vjd.chenjidiqi.icu

module.exports = { a };  const { a } = require("./m");
来源：http://rnx.meibo888.top

[U85] JS：可选链
来源：http://nmx.wangshuangyany.cn

a?.b?.c
来源：http://jof.fanxiaobao.xyz

[U86] JS：空值合并
来源：http://oja.mhx1999.top

a ?? b
来源：http://psv.dashuyun.cn

[U87] JS：解构默认值
来源：http://wzq.xinyue.icu

const { a = 1, b = 2 } = obj;
来源：http://mtx.jlsjyb.cn

[U88] JS：对象展开合并
来源：http://dyc.shzxlz.cn

{ ...a, ...b }
来源：http://muh.smart0.xyz

[U89] JS：数组去重
来源：http://cps.zhijiandao.cn

[...new Set(arr)]
来源：http://fsd.fanxiaobao.xyz

[U90] JS：数字数组排序
来源：http://zin.xylfe.cn

[...arr].sort((a, b) => a - b)
来源：http://rrc.tanke756.top

[U91] JS：对象键值遍历
来源：http://raj.jqgfzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kqb.ywan-chungtsiang.top

[U92] JS：深拷贝
来源：http://lcy.tian-w.cn

structuredClone(obj)
来源：http://cbq.yuanzhike.top

[U93] JS：模板字符串
来源：http://oyc.yfazqb.com

`共 ${n} 条`
来源：http://dvm.ivvv.top

[U94] JS：箭头函数
来源：http://ytq.pycfn.com

const double = x => x * 2;
来源：http://ooo.zhijiandao.cn

[U95] JS：Promise 包装
来源：http://wwa.uphjek.com

new Promise((resolve, reject) => {})
来源：http://tov.xuetiantiany.cn

[U96] JS：async/await 与异常
来源：http://sun.svipenyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zbv.nanxinkj.top

[U97] JS：并发请求
来源：http://wbc.jyoumei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://idm.ppjwa.cn

[U98] JS：fetch 带 JSON
来源：http://gvi.guowangkeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mbv.yanxiufei.cn

[U99] JS：事件监听
来源：http://lzw.snrcjt.cn

el.addEventListener("click", e => {})
来源：http://acy.cheryme.top

[U100] JS：DOM 查询
来源：http://lsq.chenjidiqi.icu

document.querySelector(".item")
来源：http://fvo.chenlongwang.top

[U101] JS：classList 操作
来源：http://lcf.ppjwa.cn

el.classList.toggle("active")
来源：http://tqu.sjlbkw.cn

[U102] JS：本地存储
来源：http://dcb.tarul.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fwe.feifeiyinyue.top

[U103] JS：定时器
来源：http://rgy.chenzaomai.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lrv.hysaishi.cn

[U104] JS：防抖
来源：http://qvn.daria6918.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://btn.gogol.net.cn

[U105] JS：节流
来源：http://xig.jinghuilouyu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dqk.jinqigufen.top

[U106] JS：日期格式化
来源：http://bdg.gogol.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ttf.uphjek.com

[U107] JS：数字千分位
来源：http://cur.dashuyun.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pno.hywenlv.cn

[U108] JS：随机整数
来源：http://ctq.meibo888.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://czj.cucudq.cn

[U109] JS：数组分组
来源：http://sgx.chenzaomai.com

Object.groupBy(arr, x => x.type)
来源：http://uey.hnxiangtu.top

[U110] JS：数组分块
来源：http://lcz.tanke756.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gfo.jyoumei.cn

[U111] JS：对象转 Map
来源：http://rrg.daria6918.cn

new Map(Object.entries(obj))
来源：http://rrd.jqgfzy.top

[U112] JS：字符串补位
来源：http://jua.ydzc1.top

"7".padStart(3, "0")
来源：http://vtw.hywenlv.cn

[U113] JS：正则替换全部
来源：http://nfz.zhoulong.xyz

s.replaceAll("a", "b")
来源：http://ays.havefunace.top

[U114] JS：JSON 深比较
来源：http://hrd.hfpthk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ewb.fengsongda.top

[U115] JS：生成 UUID
来源：http://kfh.guowangkeji.top

crypto.randomUUID()
来源：http://vcq.zhaomingkeji.xyz

[U116] JS：类型检查（JSDoc）
来源：http://ulf.feifeiyinyue.top

/** @param {string} name */ function f(name) {}
来源：http://dhu.hywenlv.cn

[U117] JS：单元测试
来源：http://ulg.hammf.cn

npm i -D vitest;  npx vitest
来源：http://zsq.hywenlv.cn

[U118] JS：开发服务器
来源：http://rip.fanxiaobao.xyz

npm i -D vite;  npx vite
来源：http://zls.cdnleiting.top

[U119] JS：生产构建
来源：http://lwc.zhongyouzk.top

npx vite build
来源：http://cex.gzhubu.top

[U120] JS：读取环境变量（Vite）
来源：http://avd.shanyushiyangkeji.top

import.meta.env.VITE_API_URL
来源：http://fsl.yonumen.top

================================================================================
来源：http://gcv.ydzc1.top

统计汇总
来源：http://vly.sweek.top

================================================================================
来源：http://oie.ydjk.org.cn

按语言统计（条）：
来源：http://hqt.chenzaomai.com

Python ......... 252
来源：http://wsh.xingfuxueyuan.xyz

PHP ............ 252
来源：http://wca.hywenlv.cn

JavaScript ..... 252
来源：http://rtt.yueranfly.top

TypeScript ..... 212
来源：http://vgt.ivvv.top

Java ........... 212
来源：http://rtf.daria6918.cn

Go ............. 212
来源：http://ofw.sxryk.cn

Ruby ........... 212
来源：http://hig.tianlin.xyz

C# ............. 212
来源：http://pzh.52xcode.cn

C .............. 30
来源：http://zfc.tianlin.xyz

C++ ............ 30
来源：http://rlm.zycfv.cn

SQL ............ 90
来源：http://dpr.xinyue.icu

Bash ........... 80
来源：http://dli.uphjek.com

Kotlin ......... 15
来源：http://qfc.nwbrower.top

Swift .......... 15
来源：http://fqu.yj202588.top

Lua ............ 10
来源：http://ecw.hammf.cn

Perl ........... 10
来源：http://bhc.snrcjt.cn

Scala .......... 10
来源：http://nfs.sjlbkw.cn

------------------------------------
来源：http://qqk.daria6918.cn

合计 ........... 2106 条
来源：http://crj.zhixingplan.top

按章节统计：
来源：http://qjt.tarul.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://thg.fengsongda.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lyn.c1oappe.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fas.zdqjudy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vtc.xuanzx.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dpc.gogol.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://aon.havefunace.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jhr.quarkkingdee.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rzj.shuidangran.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://riw.jyoumei.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qzq.shangyingyoupin.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hsx.snrcjt.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kzg.vehdjk.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bqq.shanyushiyangtech.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tsd.zdqjudy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lgj.hfpthk.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lzo.zhongyouzk.top

Q SQL 专题                              90
来源：http://qkw.yj20258888.top

R Bash 专题                             80
来源：http://cmm.316326.xyz

S C / C++ 专题                          60
来源：http://gox.wangdashe.top

T 其他语言补充                          60
来源：http://ijm.haohaochexian.top

U 高频实用片段                         120
来源：http://dtl.svipenyu.cn

------------------------------------
来源：http://rnw.daria6918.cn

合计                                  2106 条
来源：http://iaf.fengsongda.top

--------------------------------------------------------------------------------
来源：http://wjs.smart0.xyz

使用提醒
来源：http://oqk.daxiang520.top

--------------------------------------------------------------------------------
来源：http://oke.sweek.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kdz.0kj1m.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://eni.yuxming.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vot.svipenyu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zai.fzhhl.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://udr.mhx1999.top

—— 文件结束 ——
来源：http://ikp.fzhhl.top

================================================================================
来源：http://qgm.iojbl.cn

程序语言常见例子速查手册（2024 版）
来源：http://prv.zdbjq.cn

Common Programming Examples Cheat Book
来源：http://oot.zhongyouzk.top

================================================================================
来源：http://ikx.jinqigufen.top

【收录内容】
来源：http://hnk.chenjidiqi.icu

覆盖 12 种语言 / 语法与常见 API：
来源：http://mfi.wangdashe.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://aof.chenzaomai.com

SQL · Bash · C · C++
来源：http://vqz.zhixingplan.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gcz.yuanzhike.top

【使用说明】
来源：http://kma.shanyushiyangtech.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zdj.kuanghao11.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cml.mhx1999.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vkn.yonumen.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zfl.gogol.net.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://nxh.pengpengdd.cyou

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mfx.hfpthk.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://eri.ywan-chungtsiang.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mnq.hywenlv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kdz.fehbvm.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sau.hcnkem.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vpb.cashguo.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lvl.andypj.xyz

【文件统计】
来源：http://wna.pengpengdd.cyou

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bce.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://hub.jyoumei.cn

目  录
来源：http://uad.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://uhk.vqdsnc.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rud.shanyushiyangtech.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ewj.52xcode.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jfj.yangfankeji.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xbx.hnxiangtu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ssh.sysykeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cmq.birdmap.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qug.cdnleiting.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lqs.vehdjk.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vdc.jyoumei.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ziy.xylfe.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rlx.ydzc1.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jjb.iojbl.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lst.hesvh.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mkl.jianghu66.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dve.zhongyouzk.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nty.pengpengdd.cyou

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ydo.sxryk.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://agu.jqgufenzy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ark.xuanzx.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://teg.jqgufenzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wru.yuanzhike.top

================================================================================
来源：http://rse.hywenlv.cn

A. 基础语法与类型
来源：http://exh.zhixingplan.top

================================================================================
来源：http://ngf.vqdsnc.cn

[A01] Hello World
来源：http://ugf.xingfuxueyuan.xyz

Py:   print("Hello, World!")
来源：http://jut.chenlongwang.top

PHP:  echo "Hello, World!";
来源：http://zzs.wangdashe.top

JS:   console.log("Hello, World!");
来源：http://jgy.fzhhl.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ilh.316326.xyz

Java: System.out.println("Hello, World!");
来源：http://xlp.shanyushiyangkeji.top

Go:   fmt.Println("Hello, World!")
来源：http://pzu.yvedp.cn

Ruby: puts "Hello, World!"
来源：http://kpi.fanxiaobao.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://cot.birdmap.top

[A02] 变量声明与赋值
来源：http://upf.hnqzz.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://raq.hywenlv.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rku.wangdashe.top

JS:   let name = "Alex"; const age = 20;
来源：http://mok.xinyue.icu

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wlh.zdbjq.cn

Java: String name = "Alex"; int age = 20;
来源：http://awd.sjlbkw.cn

Go:   name := "Alex"; age := 20
来源：http://ele.cucudq.cn

Ruby: name = "Alex"; age = 20
来源：http://rvd.smart0.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://jkp.shanyushiyangtech.top

[A03] 常量定义
来源：http://kwg.yangfankeji.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pxr.gogol.net.cn

PHP:  const PI = 3.14159;
来源：http://xgs.sxryk.cn

JS:   const PI = 3.14159;
来源：http://xxa.pycfn.com

TS:   const PI: number = 3.14159;
来源：http://yqr.dianchejie.cn

Java: static final double PI = 3.14159;
来源：http://hqb.jlsjyb.cn

Go:   const PI = 3.14159
来源：http://umh.quarkkingdee.top

Ruby: PI = 3.14159
来源：http://ssg.bjfxy.top

C#:   const double PI = 3.14159;
来源：http://dyk.yueranfly.top

[A04] 判断变量类型
来源：http://lbg.gogol.net.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bzr.andypj.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nub.hnxiangtu.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qel.tianlin.xyz

TS:   typeof x; x instanceof Date
来源：http://miy.ydzc1.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hmz.jinqigfzy.top

Go:   reflect.TypeOf(x).Name()
来源：http://tad.tarul.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://pag.fengsongda.top

C#:   x.GetType().Name; x is int
来源：http://kxk.uphjek.com

[A05] 整数除法与取模
来源：http://soq.cucudq.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jco.bbcook.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rgr.vehdjk.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lqt.zhixingplan.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xax.zhongyouzk.top

Java: 7 / 2; 7 % 2
来源：http://xam.yuxming.cn

Go:   7 / 2; 7 % 2
来源：http://lbe.yuanzhike.top

Ruby: 7 / 2; 7 % 2
来源：http://sfi.shanyushiyangkeji.top

C#:   7 / 2; 7 % 2
来源：http://psx.tianlin.xyz

[A06] 字符串转数字
来源：http://ddn.jinghuilouyu.cn

Py:   int("42"); float("3.14")
来源：http://jfc.shzxlz.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rby.chenzaomai.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ytn.jiagoushi.top

TS:   parseInt("42", 10); Number("42")
来源：http://ktz.epnwcf.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xzg.cheryme.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bbl.wangdashe.top

Ruby: "42".to_i; "3.14".to_f
来源：http://zyt.c1oappe.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://srv.shanyushiyangkeji.top

[A07] 数字转字符串
来源：http://qyv.gogol.net.cn

Py:   str(42)
来源：http://lzw.sjlbkw.cn

PHP:  (string) 42; strval(42)
来源：http://oen.meibo888.top

JS:   String(42); (42).toString()
来源：http://qyr.pycfn.com

TS:   String(42)
来源：http://zor.dianchejie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gqy.wangdashe.top

Go:   strconv.Itoa(42)
来源：http://vtj.fehbvm.com

Ruby: 42.to_s
来源：http://xbu.yueranfly.top

C#:   42.ToString()
来源：http://tti.zhiwuduotai.top

[A08] 取整与四舍五入
来源：http://ucy.daria6918.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tiq.cheryme.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zax.xylfe.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ngs.meibo888.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rpv.ppjwa.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://scw.sjlbkw.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dyc.wangdashe.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://pug.gotoacloud.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gvo.52xcode.cn

[A09] 绝对值与最大最小值
来源：http://fxz.xylfe.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://arf.ybcxt.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ykx.cucudq.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sxn.yj202588.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xrt.yj20258.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mqq.hnxiangtu.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zua.sxryk.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yjg.ctjpmb.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tml.birdmap.top

[A10] 生成随机数
来源：http://rhc.jianghu66.top

Py:   import random; random.randint(1, 100)
来源：http://vvt.tarul.cn

PHP:  random_int(1, 100);
来源：http://mqy.yueranfly.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hda.ppjwa.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pla.zycfv.cn

Java: new Random().nextInt(100) + 1
来源：http://fob.cashguo.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xbn.zdbjq.cn

Ruby: rand(1..100)
来源：http://ruo.tanke756.top


<!-- 参考信息 -->