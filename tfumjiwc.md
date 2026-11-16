代发 wailian999

[U67] PHP：处理文件上传
来源：http://ktv.shanyushiyangkeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hfq.sjlbkw.cn

[U68] PHP：PDO 连接
来源：http://vbw.gaohongyu789.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://aey.bbcook.cn

[U69] PHP：PDO 预处理
来源：http://nnp.ydzc1.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lrp.fehbvm.com

[U70] PHP：PDO 事务
来源：http://kyq.0kj1m.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hte.cashguo.top

[U71] PHP：抛出异常
来源：http://fur.ppjwa.cn

throw new RuntimeException("失败", 500);
来源：http://wrf.aibaodan.cn

[U72] PHP：写错误日志
来源：http://mhz.guowangkeji.top

error_log("失败: " . $e->getMessage());
来源：http://cwy.sxryk.cn

[U73] PHP：读取 ini 配置
来源：http://khw.hnxiangtu.top

parse_ini_file("config.ini", true)
来源：http://fxe.9152youxi.cn

[U74] PHP：读取环境变量
来源：http://vqp.hammf.cn

getenv("APP_ENV") ?: "production"
来源：http://uok.shuidangran.top

[U75] PHP：依赖注入
来源：http://nog.hysaishi.cn

composer require psr/container
来源：http://hnh.jyoumei.cn

[U76] PHP：简单路由
来源：http://pmp.redwolf501.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cei.chenjidiqi.icu

[U77] PHP：模板渲染
来源：http://ksa.c1oappe.top

composer require twig/twig
来源：http://oyu.jlsjyb.cn

[U78] PHP：单元测试
来源：http://win.nanxinkj.top

composer require --dev phpunit/phpunit
来源：http://cjj.vqdsnc.cn

[U79] PHP：静态分析
来源：http://huk.yueranfly.top

composer require --dev phpstan/phpstan
来源：http://kxm.mhx1999.top

[U80] PHP：代码规范修复
来源：http://wee.shanyushiyangtech.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ees.redwolf501.top

[U81] JS：初始化项目
来源：http://ziq.wangdashe.top

npm init -y;  npm i express
来源：http://nvi.c1oappe.top

[U82] JS：package.json 脚本
来源：http://icr.zhiwuduotai.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fcy.sufxvd.cn

[U83] JS：ES Module 导入导出
来源：http://ddc.cucudq.cn

export const a = 1;  import { a } from "./m.js";
来源：http://oyf.zhaomingkeji.xyz

[U84] JS：CommonJS 写法
来源：http://cva.zhiwuduotai.top

module.exports = { a };  const { a } = require("./m");
来源：http://awk.tanke756.top

[U85] JS：可选链
来源：http://rkl.mhx1999.top

a?.b?.c
来源：http://xqx.0kj1m.cn

[U86] JS：空值合并
来源：http://cwc.epnwcf.com

a ?? b
来源：http://rrg.cashguo.top

[U87] JS：解构默认值
来源：http://xep.ywan-chungtsiang.top

const { a = 1, b = 2 } = obj;
来源：http://lpr.jlsjyb.cn

[U88] JS：对象展开合并
来源：http://jkr.jinyuanbaomall.cn

{ ...a, ...b }
来源：http://uwe.c1oappe.top

[U89] JS：数组去重
来源：http://shb.sxryk.cn

[...new Set(arr)]
来源：http://ykl.smart0.xyz

[U90] JS：数字数组排序
来源：http://kny.ydzc1.top

[...arr].sort((a, b) => a - b)
来源：http://bae.jinqigufen.top

[U91] JS：对象键值遍历
来源：http://xgw.cucudq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dpp.zhoulong.xyz

[U92] JS：深拷贝
来源：http://yrw.yj20258888.top

structuredClone(obj)
来源：http://rrs.dashuyun.cn

[U93] JS：模板字符串
来源：http://qtb.hysaishi.cn

`共 ${n} 条`
来源：http://umr.yuxming.cn

[U94] JS：箭头函数
来源：http://puo.zhijiandao.cn

const double = x => x * 2;
来源：http://erc.yj20258888.top

[U95] JS：Promise 包装
来源：http://xvi.chenzaomai.com

new Promise((resolve, reject) => {})
来源：http://nas.ywan-chungtsiang.top

[U96] JS：async/await 与异常
来源：http://zrm.316326.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jng.xinyue.icu

[U97] JS：并发请求
来源：http://bfc.hnqzz.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ahe.smart0.xyz

[U98] JS：fetch 带 JSON
来源：http://wbo.sysykeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eyp.yvedp.cn

[U99] JS：事件监听
来源：http://wbw.fzhhl.top

el.addEventListener("click", e => {})
来源：http://eqp.hnqzz.top

[U100] JS：DOM 查询
来源：http://njs.sweek.top

document.querySelector(".item")
来源：http://ktx.xinyue.icu

[U101] JS：classList 操作
来源：http://imz.xylfe.cn

el.classList.toggle("active")
来源：http://kev.zhixingplan.top

[U102] JS：本地存储
来源：http://fze.yangfankeji.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://ixu.yfazqb.com

[U103] JS：定时器
来源：http://nlq.ydjk.org.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jnv.sxryk.cn

[U104] JS：防抖
来源：http://ivz.cqqwz.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aec.zhoulong.xyz

[U105] JS：节流
来源：http://lca.52xcode.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://non.tanke756.top

[U106] JS：日期格式化
来源：http://dvz.zhengqikj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nyg.nanxinkj.top

[U107] JS：数字千分位
来源：http://lvf.jinqigufen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://chx.shuidangran.top

[U108] JS：随机整数
来源：http://krf.nanxuanxn.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dmw.jinghuilouyu.cn

[U109] JS：数组分组
来源：http://ohk.shzxlz.cn

Object.groupBy(arr, x => x.type)
来源：http://zbv.zycfv.cn

[U110] JS：数组分块
来源：http://mku.dashuyun.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://awu.xuetiantiany.cn

[U111] JS：对象转 Map
来源：http://bsb.xziqi.cn

new Map(Object.entries(obj))
来源：http://rit.xuanzx.com

[U112] JS：字符串补位
来源：http://rdc.quarkkingdee.top

"7".padStart(3, "0")
来源：http://prj.tianlin.xyz

[U113] JS：正则替换全部
来源：http://lzk.yonumen.top

s.replaceAll("a", "b")
来源：http://pyl.ydzc1.top

[U114] JS：JSON 深比较
来源：http://xqq.jinghuilouyu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://olv.zhixingplan.top

[U115] JS：生成 UUID
来源：http://lcq.yvedp.cn

crypto.randomUUID()
来源：http://xmh.shangyingyoupin.top

[U116] JS：类型检查（JSDoc）
来源：http://eqj.redwolf501.top

/** @param {string} name */ function f(name) {}
来源：http://cor.jiagoushi.top

[U117] JS：单元测试
来源：http://lnw.tarul.cn

npm i -D vitest;  npx vitest
来源：http://sks.wangdashe.top

[U118] JS：开发服务器
来源：http://ppd.ctjpmb.com

npm i -D vite;  npx vite
来源：http://hqh.wangshuangyany.cn

[U119] JS：生产构建
来源：http://cfe.wangshuangyany.cn

npx vite build
来源：http://ebp.tanke756.top

[U120] JS：读取环境变量（Vite）
来源：http://suw.shanyushiyangkeji.top

import.meta.env.VITE_API_URL
来源：http://djd.hesvh.cn

================================================================================
来源：http://xnd.jinyuanbaomall.cn

统计汇总
来源：http://sua.daxiang520.top

================================================================================
来源：http://lvl.yuxming.cn

按语言统计（条）：
来源：http://qqd.yuanzhike.top

Python ......... 252
来源：http://cll.sxryk.cn

PHP ............ 252
来源：http://gwi.cucudq.cn

JavaScript ..... 252
来源：http://kad.gotoacloud.top

TypeScript ..... 212
来源：http://zfs.zdbjq.cn

Java ........... 212
来源：http://tok.shzxlz.cn

Go ............. 212
来源：http://krz.yvedp.cn

Ruby ........... 212
来源：http://tfg.kuanghao11.cn

C# ............. 212
来源：http://zhf.shanyushiyangtech.top

C .............. 30
来源：http://tip.fengsongda.top

C++ ............ 30
来源：http://vbw.redwolf501.top

SQL ............ 90
来源：http://ccw.cucudq.cn

Bash ........... 80
来源：http://clt.tianlin.xyz

Kotlin ......... 15
来源：http://hlg.dashuyun.cn

Swift .......... 15
来源：http://shv.316326.xyz

Lua ............ 10
来源：http://osx.nanxinkj.top

Perl ........... 10
来源：http://owf.birdmap.top

Scala .......... 10
来源：http://qcm.snrcjt.cn

------------------------------------
来源：http://mai.uphjek.com

合计 ........... 2106 条
来源：http://fia.cdnleiting.top

按章节统计：
来源：http://wkp.ywan-chungtsiang.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rce.nanxuanxn.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gqq.yanxiufei.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://roj.shangyingyoupin.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vhy.hcnkem.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mvn.yj202588.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://prw.cashguo.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mvx.jinqigufen.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://eno.jiagoushi.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nep.ivvv.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dtc.jqgufenzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ijb.jianghu66.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lqf.hammf.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ybm.zhaomingkeji.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://eca.daxiang520.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nsh.xingfuxueyuan.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xql.xuetiantiany.cn

Q SQL 专题                              90
来源：http://fzn.tanke756.top

R Bash 专题                             80
来源：http://opk.yj20258888.top

S C / C++ 专题                          60
来源：http://dwb.andypj.xyz

T 其他语言补充                          60
来源：http://pnr.chenzaomai.com

U 高频实用片段                         120
来源：http://hiv.shangyingyoupin.top

------------------------------------
来源：http://fxi.cheryme.top

合计                                  2106 条
来源：http://gpj.birdmap.top

--------------------------------------------------------------------------------
来源：http://kmy.dashuyun.cn

使用提醒
来源：http://gqt.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://jev.ivvv.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://shs.zdqjudy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://myc.52xcode.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ftw.tarul.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ylk.fktsv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sid.sjlbkw.cn

—— 文件结束 ——
来源：http://uun.hywenlv.cn

================================================================================
来源：http://ulq.shangyingyoupin.top

程序语言常见例子速查手册（2024 版）
来源：http://cyi.yongpay.top

Common Programming Examples Cheat Book
来源：http://pmw.quarkkingdee.top

================================================================================
来源：http://fcd.zdqjudy.top

【收录内容】
来源：http://lzz.zdqjudy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://pfg.316326.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xgt.hongshengwenyu.top

SQL · Bash · C · C++
来源：http://ctp.cheryme.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ytg.sxryk.cn

【使用说明】
来源：http://hpj.aibaodan.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fjj.tian-w.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://poi.redwolf501.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xcc.cucudq.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://uuk.zhoulong.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://dlu.zdbjq.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wxo.jlsjyb.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yua.yonumen.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xtl.hesvh.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vsw.pycfn.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rqm.ivvv.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pbb.zhoulong.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fzq.jqgufenzy.top

【文件统计】
来源：http://wfy.yj20258.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rci.sweek.top

--------------------------------------------------------------------------------
来源：http://fcd.bjfxy.top

目  录
来源：http://ewo.ivvv.top

--------------------------------------------------------------------------------
来源：http://vrt.gotoacloud.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://eat.gogol.net.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pgs.fktsv.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cyo.zdqjudy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zqj.shangyingyoupin.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://byl.haohaochexian.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tvc.nanxinkj.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://owe.zhixingplan.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://etn.haohaochexian.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kvf.vqdsnc.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dcx.aizwys.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tou.yanxiufei.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qnk.dianchejie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tem.gzhubu.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wiv.yuanzhike.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://djf.jianghu66.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hpo.hysaishi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vst.fehbvm.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://cqg.ywan-chungtsiang.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ghg.fzhhl.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ief.xinyue.icu

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tjq.hcnkem.com

================================================================================
来源：http://rkj.xylfe.cn

A. 基础语法与类型
来源：http://wok.zhongyouzk.top

================================================================================
来源：http://weo.smart0.xyz

[A01] Hello World
来源：http://dya.shangyingyoupin.top

Py:   print("Hello, World!")
来源：http://nyw.jiagoushi.top

PHP:  echo "Hello, World!";
来源：http://rlc.shzxlz.cn

JS:   console.log("Hello, World!");
来源：http://qli.zhaomingkeji.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://irr.jiagoushi.top

Java: System.out.println("Hello, World!");
来源：http://jdc.yuxming.cn

Go:   fmt.Println("Hello, World!")
来源：http://ubl.gzhubu.top

Ruby: puts "Hello, World!"
来源：http://hac.fzhhl.top

C#:   Console.WriteLine("Hello, World!");
来源：http://jmc.redwolf501.top

[A02] 变量声明与赋值
来源：http://rsw.jinyuanbaomall.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fwv.gogol.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ncc.zhixingplan.top

JS:   let name = "Alex"; const age = 20;
来源：http://ffi.cqqwz.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qsj.nanxuanxn.top

Java: String name = "Alex"; int age = 20;
来源：http://zgn.daxiang520.top

Go:   name := "Alex"; age := 20
来源：http://sdg.birdmap.top

Ruby: name = "Alex"; age = 20
来源：http://gup.aizwys.cn

C#:   string name = "Alex"; int age = 20;
来源：http://grc.jlsjyb.cn

[A03] 常量定义
来源：http://kls.chenzaomai.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jst.wangshuangyany.cn

PHP:  const PI = 3.14159;
来源：http://dtk.hysaishi.cn

JS:   const PI = 3.14159;
来源：http://qtu.sysykeji.top

TS:   const PI: number = 3.14159;
来源：http://abo.dianchejie.cn

Java: static final double PI = 3.14159;
来源：http://hkn.nanxinkj.top

Go:   const PI = 3.14159
来源：http://ntm.jinqigufen.top

Ruby: PI = 3.14159
来源：http://nxf.ehwqpu.com

C#:   const double PI = 3.14159;
来源：http://oxq.ywan-chungtsiang.top

[A04] 判断变量类型
来源：http://mqr.c1oappe.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ctk.tanke756.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pmx.hysaishi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://uqs.smart0.xyz

TS:   typeof x; x instanceof Date
来源：http://cpy.yonumen.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xvp.yuxming.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dke.dashuyun.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ray.yj20258.top

C#:   x.GetType().Name; x is int
来源：http://vaw.iojbl.cn

[A05] 整数除法与取模
来源：http://bgm.tanke756.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pqf.hcnkem.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://rao.cqqwz.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://isj.dashuyun.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ncn.jlsjyb.cn

Java: 7 / 2; 7 % 2
来源：http://rlg.jinqigfzy.top

Go:   7 / 2; 7 % 2
来源：http://xbe.yangfankeji.com

Ruby: 7 / 2; 7 % 2
来源：http://cmu.zdqjudy.top

C#:   7 / 2; 7 % 2
来源：http://uza.ydzc1.top

[A06] 字符串转数字
来源：http://ojh.aizwys.cn

Py:   int("42"); float("3.14")
来源：http://slr.kuanghao11.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lkw.jqgufenzy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mti.cheryme.top

TS:   parseInt("42", 10); Number("42")
来源：http://bxh.jinqigufen.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xbt.meibo888.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hff.xziqi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://kjv.hnxiangtu.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ver.cdnleiting.top

[A07] 数字转字符串
来源：http://ujl.pycfn.com

Py:   str(42)
来源：http://rle.cashguo.top

PHP:  (string) 42; strval(42)
来源：http://vfg.cqqwz.cn

JS:   String(42); (42).toString()
来源：http://yan.jqgfzy.top

TS:   String(42)
来源：http://lcs.xuanzx.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://yah.birdmap.top

Go:   strconv.Itoa(42)
来源：http://fxw.yongpay.top

Ruby: 42.to_s
来源：http://ipd.sysykeji.top

C#:   42.ToString()
来源：http://msb.yanxiufei.cn

[A08] 取整与四舍五入
来源：http://jct.kuanghao11.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yrp.chenzaomai.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ugl.redwolf501.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jvk.quarkkingdee.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wou.jinghuilouyu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uwh.shuidangran.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://eao.dianchejie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://tey.52xcode.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ygv.yangfankeji.com

[A09] 绝对值与最大最小值
来源：http://dkb.xziqi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cxg.hnqzz.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://caq.jiagoushi.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jgp.bjfxy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://oeq.jqgfzy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kzm.ybcxt.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gwf.tian-w.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://exv.tianlin.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qos.gaohongyu789.top

[A10] 生成随机数
来源：http://dfr.zhijiandao.cn

Py:   import random; random.randint(1, 100)
来源：http://zcs.jyoumei.cn

PHP:  random_int(1, 100);
来源：http://ijw.fktsv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ach.jqgfzy.top


<!-- 参考信息 -->