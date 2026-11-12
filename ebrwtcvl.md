代发 wailian999

[U63] PHP：文件读写
来源：http://zoc.zdbjq.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nrm.tian-w.cn

[U64] PHP：目录遍历
来源：http://jss.aizwys.cn

glob("dir/*.php");  scandir("dir");
来源：http://egf.yongpay.top

[U65] PHP：会话
来源：http://nsb.redwolf501.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vcj.zdqjudy.top

[U66] PHP：设置 Cookie
来源：http://cil.havefunace.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kcj.jinyuanbaomall.cn

[U67] PHP：处理文件上传
来源：http://clg.epnwcf.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ezc.xingfuxueyuan.xyz

[U68] PHP：PDO 连接
来源：http://rxb.52xcode.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gzm.yj20258888.top

[U69] PHP：PDO 预处理
来源：http://fdq.fehbvm.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zhm.fzhhl.top

[U70] PHP：PDO 事务
来源：http://gvr.hfpthk.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kee.redwolf501.top

[U71] PHP：抛出异常
来源：http://ubk.daria6918.cn

throw new RuntimeException("失败", 500);
来源：http://wtx.yuanzhike.top

[U72] PHP：写错误日志
来源：http://yca.jinqigufen.top

error_log("失败: " . $e->getMessage());
来源：http://qyq.yuanzhike.top

[U73] PHP：读取 ini 配置
来源：http://ywr.shuidangran.top

parse_ini_file("config.ini", true)
来源：http://lcy.52xcode.cn

[U74] PHP：读取环境变量
来源：http://ptu.andypj.xyz

getenv("APP_ENV") ?: "production"
来源：http://pqg.jinqigfzy.top

[U75] PHP：依赖注入
来源：http://xgh.tarul.cn

composer require psr/container
来源：http://sfo.316326.xyz

[U76] PHP：简单路由
来源：http://plx.redwolf501.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dgr.shangyingyoupin.top

[U77] PHP：模板渲染
来源：http://blr.fzhhl.top

composer require twig/twig
来源：http://uxw.ivvv.top

[U78] PHP：单元测试
来源：http://rfo.zhengqikj.top

composer require --dev phpunit/phpunit
来源：http://gbo.chenzaomai.com

[U79] PHP：静态分析
来源：http://xci.gogol.net.cn

composer require --dev phpstan/phpstan
来源：http://ajs.yueranfly.top

[U80] PHP：代码规范修复
来源：http://ysi.xingfuxueyuan.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://ozs.shuidangran.top

[U81] JS：初始化项目
来源：http://vxq.316326.xyz

npm init -y;  npm i express
来源：http://wny.ywan-chungtsiang.top

[U82] JS：package.json 脚本
来源：http://sgs.ivvv.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xqu.yvedp.cn

[U83] JS：ES Module 导入导出
来源：http://fmh.yongpay.top

export const a = 1;  import { a } from "./m.js";
来源：http://bqg.316326.xyz

[U84] JS：CommonJS 写法
来源：http://owf.feifeiyinyue.top

module.exports = { a };  const { a } = require("./m");
来源：http://lbp.sweek.top

[U85] JS：可选链
来源：http://wux.yj20258.top

a?.b?.c
来源：http://deb.shuidangran.top

[U86] JS：空值合并
来源：http://erc.ydzc1.top

a ?? b
来源：http://avu.c1oappe.top

[U87] JS：解构默认值
来源：http://mwh.chenzaomai.com

const { a = 1, b = 2 } = obj;
来源：http://fyh.cucudq.cn

[U88] JS：对象展开合并
来源：http://gvu.c1oappe.top

{ ...a, ...b }
来源：http://ekg.fktsv.cn

[U89] JS：数组去重
来源：http://hgh.fktsv.cn

[...new Set(arr)]
来源：http://pjs.yanxiufei.cn

[U90] JS：数字数组排序
来源：http://rnv.pycfn.com

[...arr].sort((a, b) => a - b)
来源：http://tpj.jinqigfzy.top

[U91] JS：对象键值遍历
来源：http://izj.gotoacloud.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vrk.jianghu66.top

[U92] JS：深拷贝
来源：http://ent.zhiwuduotai.top

structuredClone(obj)
来源：http://dbj.ywan-chungtsiang.top

[U93] JS：模板字符串
来源：http://mnx.jinyuanbaomall.cn

`共 ${n} 条`
来源：http://sew.andypj.xyz

[U94] JS：箭头函数
来源：http://oxm.daria6918.cn

const double = x => x * 2;
来源：http://wyr.jqgfzy.top

[U95] JS：Promise 包装
来源：http://yxg.sufxvd.cn

new Promise((resolve, reject) => {})
来源：http://wru.jqgufenzy.top

[U96] JS：async/await 与异常
来源：http://kef.hnqzz.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hdu.zdqjudy.top

[U97] JS：并发请求
来源：http://ntb.daria6918.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pkn.xuetiantiany.cn

[U98] JS：fetch 带 JSON
来源：http://uao.jianghu66.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xwd.fktsv.cn

[U99] JS：事件监听
来源：http://zux.aibaodan.cn

el.addEventListener("click", e => {})
来源：http://pux.wangshuangyany.cn

[U100] JS：DOM 查询
来源：http://lyy.gogol.net.cn

document.querySelector(".item")
来源：http://zvg.yuxming.cn

[U101] JS：classList 操作
来源：http://ifb.cheryme.top

el.classList.toggle("active")
来源：http://ygi.hysaishi.cn

[U102] JS：本地存储
来源：http://dbl.fzhhl.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://kyj.yuanzhike.top

[U103] JS：定时器
来源：http://deq.birdmap.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ars.hnxiangtu.top

[U104] JS：防抖
来源：http://tad.quarkkingdee.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zlr.jinqigfzy.top

[U105] JS：节流
来源：http://vvx.hammf.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kty.ivvv.top

[U106] JS：日期格式化
来源：http://qac.cdnleiting.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dsg.gzhubu.top

[U107] JS：数字千分位
来源：http://roh.gaohongyu789.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://asd.sysykeji.top

[U108] JS：随机整数
来源：http://gmn.0kj1m.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mkr.wangdashe.top

[U109] JS：数组分组
来源：http://pge.yj202588.top

Object.groupBy(arr, x => x.type)
来源：http://zpg.ivvv.top

[U110] JS：数组分块
来源：http://ibt.cucudq.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bfr.gotoacloud.top

[U111] JS：对象转 Map
来源：http://kjr.yuanzhike.top

new Map(Object.entries(obj))
来源：http://ugb.hfpthk.cn

[U112] JS：字符串补位
来源：http://zsy.yanxiufei.cn

"7".padStart(3, "0")
来源：http://zzz.guannengcc.top

[U113] JS：正则替换全部
来源：http://ajs.gogol.net.cn

s.replaceAll("a", "b")
来源：http://jwx.shanyushiyangkeji.top

[U114] JS：JSON 深比较
来源：http://qaa.daxiang520.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://qud.yuxming.cn

[U115] JS：生成 UUID
来源：http://mcw.hnxiangtu.top

crypto.randomUUID()
来源：http://biy.yonumen.top

[U116] JS：类型检查（JSDoc）
来源：http://ymr.zdqjudy.top

/** @param {string} name */ function f(name) {}
来源：http://zay.yvedp.cn

[U117] JS：单元测试
来源：http://vrz.gaohongyu789.top

npm i -D vitest;  npx vitest
来源：http://wcm.haohaochexian.top

[U118] JS：开发服务器
来源：http://axf.ppjwa.cn

npm i -D vite;  npx vite
来源：http://quk.pycfn.com

[U119] JS：生产构建
来源：http://mxe.xinyue.icu

npx vite build
来源：http://qck.yongpay.top

[U120] JS：读取环境变量（Vite）
来源：http://tmb.tarul.cn

import.meta.env.VITE_API_URL
来源：http://ppg.yueranfly.top

================================================================================
来源：http://kdg.snrcjt.cn

统计汇总
来源：http://zjc.meibo888.top

================================================================================
来源：http://fwl.hywenlv.cn

按语言统计（条）：
来源：http://zyu.jinqigufen.top

Python ......... 252
来源：http://uad.shuidangran.top

PHP ............ 252
来源：http://pin.bbcook.cn

JavaScript ..... 252
来源：http://zoh.316326.xyz

TypeScript ..... 212
来源：http://uni.zdbjq.cn

Java ........... 212
来源：http://wmt.nanxuanxn.top

Go ............. 212
来源：http://srj.gogol.net.cn

Ruby ........... 212
来源：http://vtn.wangdashe.top

C# ............. 212
来源：http://plk.jinqigufen.top

C .............. 30
来源：http://wye.yongpay.top

C++ ............ 30
来源：http://wlu.hysaishi.cn

SQL ............ 90
来源：http://ohp.jqgufenzy.top

Bash ........... 80
来源：http://aqa.jyoumei.cn

Kotlin ......... 15
来源：http://sty.sjlbkw.cn

Swift .......... 15
来源：http://tyr.xylfe.cn

Lua ............ 10
来源：http://lrg.nwbrower.top

Perl ........... 10
来源：http://ntv.haohaochexian.top

Scala .......... 10
来源：http://quh.xylfe.cn

------------------------------------
来源：http://hpl.zhixingplan.top

合计 ........... 2106 条
来源：http://vxy.ivvv.top

按章节统计：
来源：http://nly.wangdashe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://adl.tianlin.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mwx.cdnleiting.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lir.vehdjk.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://luw.cdnleiting.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yux.daxiang520.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cos.jinghuilouyu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://swr.cucudq.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zsk.uphjek.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tqz.zhiwuduotai.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bdd.wangdashe.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wos.yueranfly.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hhr.aibaodan.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gox.svipenyu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kqm.nwbrower.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://izv.haohaochexian.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nlm.jqgufenzy.top

Q SQL 专题                              90
来源：http://psn.jianghu66.top

R Bash 专题                             80
来源：http://nvb.shzxlz.cn

S C / C++ 专题                          60
来源：http://kzm.ehwqpu.com

T 其他语言补充                          60
来源：http://yac.zdbjq.cn

U 高频实用片段                         120
来源：http://lgl.shuidangran.top

------------------------------------
来源：http://lve.yuanzhike.top

合计                                  2106 条
来源：http://mgz.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://lfr.ydjk.org.cn

使用提醒
来源：http://hze.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://rfh.jlsjyb.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dyc.redwolf501.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hlw.ehwqpu.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lna.nanxinkj.top

在旧版本上使用前请先确认语法支持情况。
来源：http://oox.wangdashe.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vyy.yj202588.top

—— 文件结束 ——
来源：http://dae.zdqjudy.top

================================================================================
来源：http://gow.bbcook.cn

程序语言常见例子速查手册（2024 版）
来源：http://nrr.feifeiyinyue.top

Common Programming Examples Cheat Book
来源：http://xea.hysaishi.cn

================================================================================
来源：http://cej.fengsongda.top

【收录内容】
来源：http://ivl.zdbjq.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://oao.quarkkingdee.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://umy.xuanzx.com

SQL · Bash · C · C++
来源：http://xot.daxiang520.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hpa.tanke756.top

【使用说明】
来源：http://aee.epnwcf.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pvf.yanxiufei.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://llo.ydjk.org.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kkz.guannengcc.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://axl.52xcode.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jij.hesvh.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cxz.shzxlz.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://omn.sxryk.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wbk.shangyingyoupin.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ewn.bbcook.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ywc.jyoumei.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://det.zhongyouzk.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kje.iojbl.cn

【文件统计】
来源：http://kuv.fengsongda.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://srb.bbcook.cn

--------------------------------------------------------------------------------
来源：http://zua.xuetiantiany.cn

目  录
来源：http://uvq.wangdashe.top

--------------------------------------------------------------------------------
来源：http://hjq.yuxming.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xmw.gzhubu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://svp.chenjidiqi.icu

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://amj.gzhubu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ppd.xuanzx.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://koh.fehbvm.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gmp.yuanzhike.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fey.nanxuanxn.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hcx.jianghu66.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yvn.wangshuangyany.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kpg.jianghu66.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wfv.hammf.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kah.hysaishi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://amc.yfazqb.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jit.yangfankeji.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pbt.chenlongwang.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cyt.jqgufenzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fup.jinghuilouyu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://pnr.ppjwa.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zsx.andypj.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cku.fengsongda.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mev.aizwys.cn

================================================================================
来源：http://dtm.zhixingplan.top

A. 基础语法与类型
来源：http://adf.xuanzx.com

================================================================================
来源：http://hve.jinyuanbaomall.cn

[A01] Hello World
来源：http://dow.bjfxy.top

Py:   print("Hello, World!")
来源：http://xiw.9152youxi.cn

PHP:  echo "Hello, World!";
来源：http://kbw.yj20258888.top

JS:   console.log("Hello, World!");
来源：http://xda.yueranfly.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ske.yj20258.top

Java: System.out.println("Hello, World!");
来源：http://dit.chenlongwang.top

Go:   fmt.Println("Hello, World!")
来源：http://uyy.9152youxi.cn

Ruby: puts "Hello, World!"
来源：http://caw.hongshengwenyu.top

C#:   Console.WriteLine("Hello, World!");
来源：http://jng.uphjek.com

[A02] 变量声明与赋值
来源：http://cpk.zhiwuduotai.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zja.wangshuangyany.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kun.zhengqikj.top

JS:   let name = "Alex"; const age = 20;
来源：http://itj.dashuyun.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mtq.shanyushiyangkeji.top

Java: String name = "Alex"; int age = 20;
来源：http://cka.fehbvm.com

Go:   name := "Alex"; age := 20
来源：http://xjy.guowangkeji.top

Ruby: name = "Alex"; age = 20
来源：http://bdm.gaohongyu789.top

C#:   string name = "Alex"; int age = 20;
来源：http://bjz.bjfxy.top

[A03] 常量定义
来源：http://jvw.gzhubu.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hfg.xuanzx.com

PHP:  const PI = 3.14159;
来源：http://uti.fktsv.cn

JS:   const PI = 3.14159;
来源：http://hiu.jqgufenzy.top

TS:   const PI: number = 3.14159;
来源：http://mow.jianghu66.top

Java: static final double PI = 3.14159;
来源：http://dwt.hesvh.cn

Go:   const PI = 3.14159
来源：http://dpz.gotoacloud.top

Ruby: PI = 3.14159
来源：http://vjx.sufxvd.cn

C#:   const double PI = 3.14159;
来源：http://lzx.hcnkem.com

[A04] 判断变量类型
来源：http://mum.zycfv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jtk.guowangkeji.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fhr.meibo888.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://iqw.hesvh.cn

TS:   typeof x; x instanceof Date
来源：http://uwf.yfazqb.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gqn.yj202588.top

Go:   reflect.TypeOf(x).Name()
来源：http://wpn.fengsongda.top

Ruby: x.class; x.is_a?(Integer)
来源：http://uis.shanyushiyangkeji.top

C#:   x.GetType().Name; x is int
来源：http://jls.yuanzhike.top

[A05] 整数除法与取模
来源：http://yub.gotoacloud.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wmz.hywenlv.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ipe.yangfankeji.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rgn.wangdashe.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vvy.kuanghao11.cn

Java: 7 / 2; 7 % 2
来源：http://jdv.ctjpmb.com

Go:   7 / 2; 7 % 2
来源：http://ipl.jinqigufen.top

Ruby: 7 / 2; 7 % 2
来源：http://peo.hysaishi.cn

C#:   7 / 2; 7 % 2
来源：http://psz.yvedp.cn

[A06] 字符串转数字
来源：http://cxz.iojbl.cn

Py:   int("42"); float("3.14")
来源：http://cvk.316326.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ntp.yueranfly.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pww.tian-w.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pbv.fehbvm.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zgk.ydjk.org.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sfb.iojbl.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hoi.gaohongyu789.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lfb.smart0.xyz

[A07] 数字转字符串
来源：http://nxx.tanke756.top

Py:   str(42)
来源：http://mgw.shzxlz.cn

PHP:  (string) 42; strval(42)
来源：http://mzj.fanxiaobao.xyz

JS:   String(42); (42).toString()
来源：http://pmk.tian-w.cn

TS:   String(42)
来源：http://gbo.sysykeji.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://nrk.guannengcc.top

Go:   strconv.Itoa(42)
来源：http://ojk.tanke756.top

Ruby: 42.to_s
来源：http://hfx.zhiwuduotai.top

C#:   42.ToString()
来源：http://okn.hnxiangtu.top

[A08] 取整与四舍五入
来源：http://ncc.hesvh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://srw.cqqwz.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tnt.haohaochexian.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://egh.jqgufenzy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://uwh.havefunace.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rmn.shzxlz.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ecu.tian-w.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ezp.meibo888.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ewt.sjlbkw.cn

[A09] 绝对值与最大最小值
来源：http://ykg.zhixingplan.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bev.zhiwuduotai.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://agn.ydzc1.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gtu.yangfankeji.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ttl.chenjidiqi.icu


<!-- 参考信息 -->