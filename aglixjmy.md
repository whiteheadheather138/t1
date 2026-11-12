代发 wailian999

[U63] PHP：文件读写
来源：http://lgr.nanxuanxn.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jma.gogol.net.cn

[U64] PHP：目录遍历
来源：http://pca.jinghuilouyu.cn

glob("dir/*.php");  scandir("dir");
来源：http://hdk.zhongyouzk.top

[U65] PHP：会话
来源：http://yvt.cqqwz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bzr.tarul.cn

[U66] PHP：设置 Cookie
来源：http://hlz.jiagoushi.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ksh.gaohongyu789.top

[U67] PHP：处理文件上传
来源：http://fng.ctjpmb.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ozh.316326.xyz

[U68] PHP：PDO 连接
来源：http://vxc.chenjidiqi.icu

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tsn.hcnkem.com

[U69] PHP：PDO 预处理
来源：http://lug.sufxvd.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bdw.chenlongwang.top

[U70] PHP：PDO 事务
来源：http://llr.sjlbkw.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sve.zhongyouzk.top

[U71] PHP：抛出异常
来源：http://rkr.jqgufenzy.top

throw new RuntimeException("失败", 500);
来源：http://wwk.jinghuilouyu.cn

[U72] PHP：写错误日志
来源：http://ljj.gzhubu.top

error_log("失败: " . $e->getMessage());
来源：http://tok.fanxiaobao.xyz

[U73] PHP：读取 ini 配置
来源：http://zbw.tian-w.cn

parse_ini_file("config.ini", true)
来源：http://ltm.shzxlz.cn

[U74] PHP：读取环境变量
来源：http://gsm.zhixingplan.top

getenv("APP_ENV") ?: "production"
来源：http://xac.ydjk.org.cn

[U75] PHP：依赖注入
来源：http://pmm.yanxiufei.cn

composer require psr/container
来源：http://bfr.xziqi.cn

[U76] PHP：简单路由
来源：http://rxz.tianlin.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pie.zhijiandao.cn

[U77] PHP：模板渲染
来源：http://ndu.xuetiantiany.cn

composer require twig/twig
来源：http://oxj.guannengcc.top

[U78] PHP：单元测试
来源：http://dic.cheryme.top

composer require --dev phpunit/phpunit
来源：http://yuf.hammf.cn

[U79] PHP：静态分析
来源：http://qsh.snrcjt.cn

composer require --dev phpstan/phpstan
来源：http://fqk.zdbjq.cn

[U80] PHP：代码规范修复
来源：http://ltv.meibo888.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://boc.chenzaomai.com

[U81] JS：初始化项目
来源：http://rws.zhaomingkeji.xyz

npm init -y;  npm i express
来源：http://wgs.316326.xyz

[U82] JS：package.json 脚本
来源：http://wlw.yj202588.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qul.jinqigufen.top

[U83] JS：ES Module 导入导出
来源：http://gfy.shanyushiyangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://hls.tianlin.xyz

[U84] JS：CommonJS 写法
来源：http://vbv.gaohongyu789.top

module.exports = { a };  const { a } = require("./m");
来源：http://zpu.kuanghao11.cn

[U85] JS：可选链
来源：http://ack.dashuyun.cn

a?.b?.c
来源：http://bpa.ydjk.org.cn

[U86] JS：空值合并
来源：http://hnn.jiagoushi.top

a ?? b
来源：http://jes.shangyingyoupin.top

[U87] JS：解构默认值
来源：http://kte.svipenyu.cn

const { a = 1, b = 2 } = obj;
来源：http://vvx.nanxuanxn.top

[U88] JS：对象展开合并
来源：http://oud.gotoacloud.top

{ ...a, ...b }
来源：http://rxa.cashguo.top

[U89] JS：数组去重
来源：http://btl.xziqi.cn

[...new Set(arr)]
来源：http://ywv.kuanghao11.cn

[U90] JS：数字数组排序
来源：http://ion.smart0.xyz

[...arr].sort((a, b) => a - b)
来源：http://kor.hongshengwenyu.top

[U91] JS：对象键值遍历
来源：http://hzy.chenjidiqi.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qzc.yueranfly.top

[U92] JS：深拷贝
来源：http://nev.guowangkeji.top

structuredClone(obj)
来源：http://bcw.quarkkingdee.top

[U93] JS：模板字符串
来源：http://hgj.iojbl.cn

`共 ${n} 条`
来源：http://khd.yuxming.cn

[U94] JS：箭头函数
来源：http://vwi.shanyushiyangtech.top

const double = x => x * 2;
来源：http://puo.0kj1m.cn

[U95] JS：Promise 包装
来源：http://glb.sjlbkw.cn

new Promise((resolve, reject) => {})
来源：http://ycd.sjlbkw.cn

[U96] JS：async/await 与异常
来源：http://ogn.shanyushiyangtech.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uds.xingfuxueyuan.xyz

[U97] JS：并发请求
来源：http://zxv.hammf.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fbl.hfpthk.cn

[U98] JS：fetch 带 JSON
来源：http://hia.yuanzhike.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://edx.9152youxi.cn

[U99] JS：事件监听
来源：http://ori.hywenlv.cn

el.addEventListener("click", e => {})
来源：http://qyi.yj20258.top

[U100] JS：DOM 查询
来源：http://ejw.vqdsnc.cn

document.querySelector(".item")
来源：http://emh.fzhhl.top

[U101] JS：classList 操作
来源：http://tyd.aizwys.cn

el.classList.toggle("active")
来源：http://qyj.cucudq.cn

[U102] JS：本地存储
来源：http://rlu.xingfuxueyuan.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://cfo.hnqzz.top

[U103] JS：定时器
来源：http://sss.yj20258.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kut.316326.xyz

[U104] JS：防抖
来源：http://tha.chenzaomai.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oer.zhiwuduotai.top

[U105] JS：节流
来源：http://unw.chenjidiqi.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://iii.chenjidiqi.icu

[U106] JS：日期格式化
来源：http://oxr.guowangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://svo.ehwqpu.com

[U107] JS：数字千分位
来源：http://xoc.sjlbkw.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cku.ydjk.org.cn

[U108] JS：随机整数
来源：http://sbm.jinqigfzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qhp.xylfe.cn

[U109] JS：数组分组
来源：http://iuo.jinghuilouyu.cn

Object.groupBy(arr, x => x.type)
来源：http://rri.aizwys.cn

[U110] JS：数组分块
来源：http://hol.fengsongda.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cpf.tianlin.xyz

[U111] JS：对象转 Map
来源：http://xxa.tanke756.top

new Map(Object.entries(obj))
来源：http://uxv.gotoacloud.top

[U112] JS：字符串补位
来源：http://uvu.yanxiufei.cn

"7".padStart(3, "0")
来源：http://kwr.shzxlz.cn

[U113] JS：正则替换全部
来源：http://gss.zhiwuduotai.top

s.replaceAll("a", "b")
来源：http://ezu.fehbvm.com

[U114] JS：JSON 深比较
来源：http://eif.jianghu66.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hns.gogol.net.cn

[U115] JS：生成 UUID
来源：http://vgd.feifeiyinyue.top

crypto.randomUUID()
来源：http://tyu.9152youxi.cn

[U116] JS：类型检查（JSDoc）
来源：http://eua.hongshengwenyu.top

/** @param {string} name */ function f(name) {}
来源：http://uzk.zdqjudy.top

[U117] JS：单元测试
来源：http://jno.zhiwuduotai.top

npm i -D vitest;  npx vitest
来源：http://vsy.wangdashe.top

[U118] JS：开发服务器
来源：http://ibr.zhengqikj.top

npm i -D vite;  npx vite
来源：http://dqc.yonumen.top

[U119] JS：生产构建
来源：http://xaf.yj20258888.top

npx vite build
来源：http://ufw.shanyushiyangkeji.top

[U120] JS：读取环境变量（Vite）
来源：http://dqe.fanxiaobao.xyz

import.meta.env.VITE_API_URL
来源：http://vnw.jlsjyb.cn

================================================================================
来源：http://jab.hongshengwenyu.top

统计汇总
来源：http://uex.shangyingyoupin.top

================================================================================
来源：http://zeb.nanxuanxn.top

按语言统计（条）：
来源：http://uma.cucudq.cn

Python ......... 252
来源：http://oel.shzxlz.cn

PHP ............ 252
来源：http://xve.snrcjt.cn

JavaScript ..... 252
来源：http://fdw.yuxming.cn

TypeScript ..... 212
来源：http://emq.cdnleiting.top

Java ........... 212
来源：http://obr.xinyue.icu

Go ............. 212
来源：http://poy.tanke756.top

Ruby ........... 212
来源：http://sjd.yueranfly.top

C# ............. 212
来源：http://rqw.nwbrower.top

C .............. 30
来源：http://isb.zhengqikj.top

C++ ............ 30
来源：http://crm.xylfe.cn

SQL ............ 90
来源：http://fkf.fzhhl.top

Bash ........... 80
来源：http://wrc.yj20258.top

Kotlin ......... 15
来源：http://zlh.tanke756.top

Swift .......... 15
来源：http://nac.jinghuilouyu.cn

Lua ............ 10
来源：http://ehf.aibaodan.cn

Perl ........... 10
来源：http://vje.ivvv.top

Scala .......... 10
来源：http://wrg.9152youxi.cn

------------------------------------
来源：http://crz.wangshuangyany.cn

合计 ........... 2106 条
来源：http://ahj.ivvv.top

按章节统计：
来源：http://zth.bbcook.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hrt.tianlin.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lhu.snrcjt.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oes.zhaomingkeji.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://njx.fengsongda.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ydx.ivvv.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://aec.yuxming.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bfl.chenjidiqi.icu

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gxq.havefunace.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://khw.shuidangran.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qeb.svipenyu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mut.feifeiyinyue.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qdb.ctjpmb.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gmd.svipenyu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://udi.yvedp.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qkj.mhx1999.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://epb.kuanghao11.cn

Q SQL 专题                              90
来源：http://wpg.hesvh.cn

R Bash 专题                             80
来源：http://xab.yfazqb.com

S C / C++ 专题                          60
来源：http://oty.aizwys.cn

T 其他语言补充                          60
来源：http://gwi.jinyuanbaomall.cn

U 高频实用片段                         120
来源：http://acb.jinyuanbaomall.cn

------------------------------------
来源：http://tvp.cdnleiting.top

合计                                  2106 条
来源：http://ojd.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://twu.nanxinkj.top

使用提醒
来源：http://nay.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://tsr.shanyushiyangtech.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hap.yj20258888.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wkq.zhixingplan.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nhf.guannengcc.top

在旧版本上使用前请先确认语法支持情况。
来源：http://uhx.andypj.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pcp.nwbrower.top

—— 文件结束 ——
来源：http://eau.fanxiaobao.xyz

================================================================================
来源：http://jow.jianghu66.top

程序语言常见例子速查手册（2024 版）
来源：http://qyb.hcnkem.com

Common Programming Examples Cheat Book
来源：http://pxh.havefunace.top

================================================================================
来源：http://ndd.birdmap.top

【收录内容】
来源：http://cvj.nanxinkj.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://vnb.hfpthk.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kkw.daria6918.cn

SQL · Bash · C · C++
来源：http://hnt.hesvh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ydb.epnwcf.com

【使用说明】
来源：http://dtu.yonumen.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://eiv.ivvv.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tvh.fengsongda.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gny.tanke756.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qpu.shuidangran.top

Bash:  Shell         C:     C             C++:   C++
来源：http://cii.wangdashe.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ddy.chenlongwang.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yot.hongshengwenyu.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nzb.haohaochexian.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wzp.nanxuanxn.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://khd.tarul.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wye.sjlbkw.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tqi.yj20258888.top

【文件统计】
来源：http://fsv.sweek.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rzt.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://osr.tianlin.xyz

目  录
来源：http://fhi.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://cwz.ctjpmb.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lfm.xylfe.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pbg.fehbvm.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xle.ybcxt.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wta.gaohongyu789.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wzz.nanxinkj.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://evs.hongshengwenyu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nwf.zhongyouzk.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bcz.snrcjt.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rfh.svipenyu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dow.sjlbkw.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uyz.xuanzx.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ohk.nanxinkj.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mtq.jlsjyb.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ndh.hammf.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ldw.daxiang520.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pfj.chenzaomai.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cgp.cdnleiting.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ysm.cheryme.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gni.birdmap.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://biw.redwolf501.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kyo.guannengcc.top

================================================================================
来源：http://gfo.smart0.xyz

A. 基础语法与类型
来源：http://qhr.bjfxy.top

================================================================================
来源：http://blk.tarul.cn

[A01] Hello World
来源：http://hlu.tanke756.top

Py:   print("Hello, World!")
来源：http://inj.quarkkingdee.top

PHP:  echo "Hello, World!";
来源：http://vbl.nanxuanxn.top

JS:   console.log("Hello, World!");
来源：http://cxk.ywan-chungtsiang.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://psc.ehwqpu.com

Java: System.out.println("Hello, World!");
来源：http://bfp.gzhubu.top

Go:   fmt.Println("Hello, World!")
来源：http://dhx.jinqigufen.top

Ruby: puts "Hello, World!"
来源：http://yun.hnqzz.top

C#:   Console.WriteLine("Hello, World!");
来源：http://brn.ppjwa.cn

[A02] 变量声明与赋值
来源：http://ffz.fzhhl.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://axa.zhixingplan.top

PHP:  $name = "Alex"; $age = 20;
来源：http://mdm.jianghu66.top

JS:   let name = "Alex"; const age = 20;
来源：http://ate.zhaomingkeji.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nzh.birdmap.top

Java: String name = "Alex"; int age = 20;
来源：http://avo.jinqigfzy.top

Go:   name := "Alex"; age := 20
来源：http://tuq.xylfe.cn

Ruby: name = "Alex"; age = 20
来源：http://atr.cdnleiting.top

C#:   string name = "Alex"; int age = 20;
来源：http://lmp.daxiang520.top

[A03] 常量定义
来源：http://tiw.xuanzx.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nbu.cqqwz.cn

PHP:  const PI = 3.14159;
来源：http://dqp.pycfn.com

JS:   const PI = 3.14159;
来源：http://iiw.tanke756.top

TS:   const PI: number = 3.14159;
来源：http://ein.mhx1999.top

Java: static final double PI = 3.14159;
来源：http://mnl.hfpthk.cn

Go:   const PI = 3.14159
来源：http://qlg.ybcxt.top

Ruby: PI = 3.14159
来源：http://rhj.vqdsnc.cn

C#:   const double PI = 3.14159;
来源：http://nzs.nwbrower.top

[A04] 判断变量类型
来源：http://okv.cqqwz.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ajy.gaohongyu789.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dbs.cashguo.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://won.gotoacloud.top

TS:   typeof x; x instanceof Date
来源：http://pci.ivvv.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bzd.tianlin.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://kol.cqqwz.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kns.guannengcc.top

C#:   x.GetType().Name; x is int
来源：http://lpy.nanxinkj.top

[A05] 整数除法与取模
来源：http://ahv.yonumen.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gyj.yj202588.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://dux.guannengcc.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zjm.zhongyouzk.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ova.snrcjt.cn

Java: 7 / 2; 7 % 2
来源：http://zbd.hcnkem.com

Go:   7 / 2; 7 % 2
来源：http://dwt.cucudq.cn

Ruby: 7 / 2; 7 % 2
来源：http://zfo.ydzc1.top

C#:   7 / 2; 7 % 2
来源：http://wug.shuidangran.top

[A06] 字符串转数字
来源：http://wnh.bjfxy.top

Py:   int("42"); float("3.14")
来源：http://jje.ppjwa.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://crv.sjlbkw.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://djy.yj20258888.top

TS:   parseInt("42", 10); Number("42")
来源：http://lba.yuxming.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fpy.tanke756.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yut.tanke756.top

Ruby: "42".to_i; "3.14".to_f
来源：http://tvq.hfpthk.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cbf.jinghuilouyu.cn

[A07] 数字转字符串
来源：http://gij.guannengcc.top

Py:   str(42)
来源：http://lyp.hywenlv.cn

PHP:  (string) 42; strval(42)
来源：http://kst.shangyingyoupin.top

JS:   String(42); (42).toString()
来源：http://bls.gaohongyu789.top

TS:   String(42)
来源：http://mod.chenzaomai.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://pbo.nanxuanxn.top

Go:   strconv.Itoa(42)
来源：http://rlb.smart0.xyz

Ruby: 42.to_s
来源：http://wbs.gogol.net.cn

C#:   42.ToString()
来源：http://dzo.hywenlv.cn

[A08] 取整与四舍五入
来源：http://tnr.sjlbkw.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mhv.ppjwa.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rej.ydjk.org.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vms.aizwys.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rqe.52xcode.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wlx.aizwys.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://occ.hywenlv.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qvi.yuanzhike.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cbi.snrcjt.cn

[A09] 绝对值与最大最小值
来源：http://ofx.aizwys.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://isd.bjfxy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pti.hesvh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://soh.zdqjudy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zmd.yuanzhike.top


<!-- 参考信息 -->