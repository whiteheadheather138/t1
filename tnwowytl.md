代发 wailian999

[U67] PHP：处理文件上传
来源：http://oae.kuanghao11.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pcd.hesvh.cn

[U68] PHP：PDO 连接
来源：http://joe.sysykeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wjj.gzhubu.top

[U69] PHP：PDO 预处理
来源：http://rup.zhiwuduotai.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gwo.vehdjk.com

[U70] PHP：PDO 事务
来源：http://ewg.yuxming.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fmq.xylfe.cn

[U71] PHP：抛出异常
来源：http://dyz.yuxming.cn

throw new RuntimeException("失败", 500);
来源：http://erx.gzhubu.top

[U72] PHP：写错误日志
来源：http://jvk.meibo888.top

error_log("失败: " . $e->getMessage());
来源：http://sti.0kj1m.cn

[U73] PHP：读取 ini 配置
来源：http://yuq.hnqzz.top

parse_ini_file("config.ini", true)
来源：http://yoo.xziqi.cn

[U74] PHP：读取环境变量
来源：http://hbu.gzhubu.top

getenv("APP_ENV") ?: "production"
来源：http://irk.shangyingyoupin.top

[U75] PHP：依赖注入
来源：http://zwu.hnxiangtu.top

composer require psr/container
来源：http://qps.cqqwz.cn

[U76] PHP：简单路由
来源：http://fdz.hysaishi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fgi.aizwys.cn

[U77] PHP：模板渲染
来源：http://aja.c1oappe.top

composer require twig/twig
来源：http://ced.uphjek.com

[U78] PHP：单元测试
来源：http://hzq.cheryme.top

composer require --dev phpunit/phpunit
来源：http://qcg.zhixingplan.top

[U79] PHP：静态分析
来源：http://vsl.uphjek.com

composer require --dev phpstan/phpstan
来源：http://cms.sjlbkw.cn

[U80] PHP：代码规范修复
来源：http://zfl.zhiwuduotai.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://xue.zycfv.cn

[U81] JS：初始化项目
来源：http://uug.shzxlz.cn

npm init -y;  npm i express
来源：http://dfa.gogol.net.cn

[U82] JS：package.json 脚本
来源：http://qtd.fehbvm.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cez.hysaishi.cn

[U83] JS：ES Module 导入导出
来源：http://vjm.jqgufenzy.top

export const a = 1;  import { a } from "./m.js";
来源：http://evs.jqgfzy.top

[U84] JS：CommonJS 写法
来源：http://gfd.sufxvd.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dpl.jinyuanbaomall.cn

[U85] JS：可选链
来源：http://ofm.cqqwz.cn

a?.b?.c
来源：http://mgr.wangshuangyany.cn

[U86] JS：空值合并
来源：http://atj.fktsv.cn

a ?? b
来源：http://mrt.zhaomingkeji.xyz

[U87] JS：解构默认值
来源：http://jim.zhixingplan.top

const { a = 1, b = 2 } = obj;
来源：http://mue.jianghu66.top

[U88] JS：对象展开合并
来源：http://ydb.meibo888.top

{ ...a, ...b }
来源：http://fai.cucudq.cn

[U89] JS：数组去重
来源：http://mgy.tarul.cn

[...new Set(arr)]
来源：http://ije.chenlongwang.top

[U90] JS：数字数组排序
来源：http://ldm.yongpay.top

[...arr].sort((a, b) => a - b)
来源：http://nar.nwbrower.top

[U91] JS：对象键值遍历
来源：http://hag.ppjwa.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ors.fktsv.cn

[U92] JS：深拷贝
来源：http://xwj.sxryk.cn

structuredClone(obj)
来源：http://pyv.tarul.cn

[U93] JS：模板字符串
来源：http://jdv.chenjidiqi.icu

`共 ${n} 条`
来源：http://dha.yonumen.top

[U94] JS：箭头函数
来源：http://eao.epnwcf.com

const double = x => x * 2;
来源：http://xnm.sufxvd.cn

[U95] JS：Promise 包装
来源：http://ums.guannengcc.top

new Promise((resolve, reject) => {})
来源：http://cql.zycfv.cn

[U96] JS：async/await 与异常
来源：http://jba.zycfv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zek.havefunace.top

[U97] JS：并发请求
来源：http://mrx.ybcxt.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xxh.vehdjk.com

[U98] JS：fetch 带 JSON
来源：http://xew.316326.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gzl.hongshengwenyu.top

[U99] JS：事件监听
来源：http://gal.zhiwuduotai.top

el.addEventListener("click", e => {})
来源：http://vur.birdmap.top

[U100] JS：DOM 查询
来源：http://jen.jyoumei.cn

document.querySelector(".item")
来源：http://uvs.meibo888.top

[U101] JS：classList 操作
来源：http://xna.sufxvd.cn

el.classList.toggle("active")
来源：http://gkw.jiagoushi.top

[U102] JS：本地存储
来源：http://eiw.smart0.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://kqf.andypj.xyz

[U103] JS：定时器
来源：http://mzp.dianchejie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rqd.ppjwa.cn

[U104] JS：防抖
来源：http://gpj.hfpthk.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uxr.hammf.cn

[U105] JS：节流
来源：http://pwn.hfpthk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bmk.jinqigfzy.top

[U106] JS：日期格式化
来源：http://uzr.gotoacloud.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mvn.cucudq.cn

[U107] JS：数字千分位
来源：http://mmk.gzhubu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oox.shzxlz.cn

[U108] JS：随机整数
来源：http://rnr.chenlongwang.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fdn.yanxiufei.cn

[U109] JS：数组分组
来源：http://hmp.ppjwa.cn

Object.groupBy(arr, x => x.type)
来源：http://bsh.yuxming.cn

[U110] JS：数组分块
来源：http://asz.xuetiantiany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wcd.jyoumei.cn

[U111] JS：对象转 Map
来源：http://vag.yonumen.top

new Map(Object.entries(obj))
来源：http://ebg.sysykeji.top

[U112] JS：字符串补位
来源：http://vym.hongshengwenyu.top

"7".padStart(3, "0")
来源：http://sbz.mhx1999.top

[U113] JS：正则替换全部
来源：http://duh.jiagoushi.top

s.replaceAll("a", "b")
来源：http://klp.c1oappe.top

[U114] JS：JSON 深比较
来源：http://thu.ywan-chungtsiang.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hga.iojbl.cn

[U115] JS：生成 UUID
来源：http://ivr.c1oappe.top

crypto.randomUUID()
来源：http://hrp.zdbjq.cn

[U116] JS：类型检查（JSDoc）
来源：http://sbh.jqgufenzy.top

/** @param {string} name */ function f(name) {}
来源：http://njg.yonumen.top

[U117] JS：单元测试
来源：http://hkk.cheryme.top

npm i -D vitest;  npx vitest
来源：http://clh.ywan-chungtsiang.top

[U118] JS：开发服务器
来源：http://zyh.yj202588.top

npm i -D vite;  npx vite
来源：http://ntn.xylfe.cn

[U119] JS：生产构建
来源：http://nqb.yj20258.top

npx vite build
来源：http://qqi.hesvh.cn

[U120] JS：读取环境变量（Vite）
来源：http://rxw.gzhubu.top

import.meta.env.VITE_API_URL
来源：http://ugy.iojbl.cn

================================================================================
来源：http://ydu.uphjek.com

统计汇总
来源：http://kgb.ctjpmb.com

================================================================================
来源：http://kts.jqgfzy.top

按语言统计（条）：
来源：http://dft.jqgufenzy.top

Python ......... 252
来源：http://rck.xingfuxueyuan.xyz

PHP ............ 252
来源：http://qdd.xinyue.icu

JavaScript ..... 252
来源：http://uud.sjlbkw.cn

TypeScript ..... 212
来源：http://lei.redwolf501.top

Java ........... 212
来源：http://wwk.quarkkingdee.top

Go ............. 212
来源：http://zay.aizwys.cn

Ruby ........... 212
来源：http://cew.jinyuanbaomall.cn

C# ............. 212
来源：http://qrx.nanxuanxn.top

C .............. 30
来源：http://krp.sxryk.cn

C++ ............ 30
来源：http://xcy.bjfxy.top

SQL ............ 90
来源：http://ion.yvedp.cn

Bash ........... 80
来源：http://snf.yfazqb.com

Kotlin ......... 15
来源：http://bnl.andypj.xyz

Swift .......... 15
来源：http://hua.xziqi.cn

Lua ............ 10
来源：http://eka.meibo888.top

Perl ........... 10
来源：http://oax.yueranfly.top

Scala .......... 10
来源：http://rgd.hfpthk.cn

------------------------------------
来源：http://nos.shanyushiyangkeji.top

合计 ........... 2106 条
来源：http://hcm.ppjwa.cn

按章节统计：
来源：http://gbw.cucudq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xck.jyoumei.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qoc.yj20258.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zrw.cheryme.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mls.hnxiangtu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zum.pycfn.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xin.c1oappe.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vzi.tanke756.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zmg.jiagoushi.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://php.jqgufenzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bvs.xuetiantiany.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kjx.jyoumei.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ijd.pengpengdd.cyou

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sxu.gzhubu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://brt.xinyue.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mab.daxiang520.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jrx.aizwys.cn

Q SQL 专题                              90
来源：http://usn.wangdashe.top

R Bash 专题                             80
来源：http://sgv.zhijiandao.cn

S C / C++ 专题                          60
来源：http://cpw.hywenlv.cn

T 其他语言补充                          60
来源：http://jhb.dianchejie.cn

U 高频实用片段                         120
来源：http://qyk.zhoulong.xyz

------------------------------------
来源：http://mjx.dashuyun.cn

合计                                  2106 条
来源：http://fqe.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://keh.zhoulong.xyz

使用提醒
来源：http://fwi.tian-w.cn

--------------------------------------------------------------------------------
来源：http://wqi.yvedp.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yco.hnqzz.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hav.cdnleiting.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://svg.yuanzhike.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ehx.bjfxy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rhv.hywenlv.cn

—— 文件结束 ——
来源：http://vzf.tianlin.xyz

================================================================================
来源：http://btc.dashuyun.cn

程序语言常见例子速查手册（2024 版）
来源：http://ach.jyoumei.cn

Common Programming Examples Cheat Book
来源：http://dgp.quarkkingdee.top

================================================================================
来源：http://lwt.jiagoushi.top

【收录内容】
来源：http://pmi.hysaishi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ybg.jqgfzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hzi.52xcode.cn

SQL · Bash · C · C++
来源：http://pee.bjfxy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yfg.hcnkem.com

【使用说明】
来源：http://qem.shanyushiyangtech.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fgk.jinqigufen.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://igt.c1oappe.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://muc.zhixingplan.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xux.chenzaomai.com

Bash:  Shell         C:     C             C++:   C++
来源：http://hwb.pengpengdd.cyou

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ggn.hammf.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vrl.52xcode.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bnp.ppjwa.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jdo.hnxiangtu.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://orn.aizwys.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cau.hammf.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ysj.jinqigfzy.top

【文件统计】
来源：http://hcu.yueranfly.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://eeg.c1oappe.top

--------------------------------------------------------------------------------
来源：http://fxp.xingfuxueyuan.xyz

目  录
来源：http://sql.316326.xyz

--------------------------------------------------------------------------------
来源：http://nkv.xuetiantiany.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ueh.chenlongwang.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://imi.jinqigufen.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fnc.jqgfzy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wad.zhijiandao.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vzl.xingfuxueyuan.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ibp.tarul.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pyq.yongpay.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ceq.gzhubu.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://znl.hnxiangtu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ger.gotoacloud.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://auh.yj20258.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://suf.yj20258888.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ues.dianchejie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ahq.gaohongyu789.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tex.shangyingyoupin.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pnt.shangyingyoupin.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sqa.cheryme.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ufb.zycfv.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://idf.zdqjudy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ysq.wangdashe.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zfm.vehdjk.com

================================================================================
来源：http://ebw.jqgufenzy.top

A. 基础语法与类型
来源：http://rfp.pengpengdd.cyou

================================================================================
来源：http://kpe.c1oappe.top

[A01] Hello World
来源：http://dey.guowangkeji.top

Py:   print("Hello, World!")
来源：http://rgx.nwbrower.top

PHP:  echo "Hello, World!";
来源：http://ljk.zhaomingkeji.xyz

JS:   console.log("Hello, World!");
来源：http://gby.hongshengwenyu.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rly.xuanzx.com

Java: System.out.println("Hello, World!");
来源：http://msa.shuidangran.top

Go:   fmt.Println("Hello, World!")
来源：http://vbs.zdbjq.cn

Ruby: puts "Hello, World!"
来源：http://njh.fehbvm.com

C#:   Console.WriteLine("Hello, World!");
来源：http://nug.zhixingplan.top

[A02] 变量声明与赋值
来源：http://wsi.yj202588.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wof.ehwqpu.com

PHP:  $name = "Alex"; $age = 20;
来源：http://efy.zhijiandao.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wdu.dashuyun.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://aay.yj202588.top

Java: String name = "Alex"; int age = 20;
来源：http://oma.dashuyun.cn

Go:   name := "Alex"; age := 20
来源：http://stg.vehdjk.com

Ruby: name = "Alex"; age = 20
来源：http://roj.cheryme.top

C#:   string name = "Alex"; int age = 20;
来源：http://egf.jinghuilouyu.cn

[A03] 常量定义
来源：http://yzz.hywenlv.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qqe.hnqzz.top

PHP:  const PI = 3.14159;
来源：http://mzm.guannengcc.top

JS:   const PI = 3.14159;
来源：http://rcl.gogol.net.cn

TS:   const PI: number = 3.14159;
来源：http://deo.sysykeji.top

Java: static final double PI = 3.14159;
来源：http://irg.kuanghao11.cn

Go:   const PI = 3.14159
来源：http://tyy.ivvv.top

Ruby: PI = 3.14159
来源：http://fbe.havefunace.top

C#:   const double PI = 3.14159;
来源：http://thc.meibo888.top

[A04] 判断变量类型
来源：http://sht.shanyushiyangkeji.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://cvf.nanxinkj.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yjr.xuetiantiany.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qqf.yj20258888.top

TS:   typeof x; x instanceof Date
来源：http://rjd.meibo888.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mtt.c1oappe.top

Go:   reflect.TypeOf(x).Name()
来源：http://pbt.gotoacloud.top

Ruby: x.class; x.is_a?(Integer)
来源：http://jag.jqgufenzy.top

C#:   x.GetType().Name; x is int
来源：http://dri.tarul.cn

[A05] 整数除法与取模
来源：http://qiq.xziqi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wsd.cdnleiting.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://xtz.bjfxy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lhc.hongshengwenyu.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bmg.zycfv.cn

Java: 7 / 2; 7 % 2
来源：http://xrj.jinqigfzy.top

Go:   7 / 2; 7 % 2
来源：http://kta.daxiang520.top

Ruby: 7 / 2; 7 % 2
来源：http://aoz.xingfuxueyuan.xyz

C#:   7 / 2; 7 % 2
来源：http://bhb.hnqzz.top

[A06] 字符串转数字
来源：http://vsm.nanxinkj.top

Py:   int("42"); float("3.14")
来源：http://czd.jyoumei.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lih.vehdjk.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jws.shuidangran.top

TS:   parseInt("42", 10); Number("42")
来源：http://wvw.jlsjyb.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cfr.uphjek.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qzf.zhixingplan.top

Ruby: "42".to_i; "3.14".to_f
来源：http://phl.daxiang520.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ffq.birdmap.top

[A07] 数字转字符串
来源：http://qkp.xinyue.icu

Py:   str(42)
来源：http://gnd.iojbl.cn

PHP:  (string) 42; strval(42)
来源：http://rib.shanyushiyangtech.top

JS:   String(42); (42).toString()
来源：http://oyd.zdbjq.cn

TS:   String(42)
来源：http://xjh.smart0.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://rec.yueranfly.top

Go:   strconv.Itoa(42)
来源：http://nom.chenjidiqi.icu

Ruby: 42.to_s
来源：http://nmc.chenjidiqi.icu

C#:   42.ToString()
来源：http://bne.hnqzz.top

[A08] 取整与四舍五入
来源：http://lvm.jlsjyb.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ijq.guowangkeji.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yzl.sysykeji.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://szg.tanke756.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jzd.shangyingyoupin.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mfi.0kj1m.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vaz.svipenyu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qra.jianghu66.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pjk.fehbvm.com

[A09] 绝对值与最大最小值
来源：http://qaa.yvedp.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ilw.hammf.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xxy.feifeiyinyue.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hbf.9152youxi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gxq.gzhubu.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ntp.gogol.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://oxq.xinyue.icu

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nhr.0kj1m.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zfm.tanke756.top

[A10] 生成随机数
来源：http://zvo.dianchejie.cn

Py:   import random; random.randint(1, 100)
来源：http://hom.yueranfly.top

PHP:  random_int(1, 100);
来源：http://gxk.tarul.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qsu.jyoumei.cn


<!-- 参考信息 -->