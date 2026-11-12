代发 wailian999

[U61] PHP：正则
来源：http://sbm.gzhubu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bfx.ywan-chungtsiang.top

[U62] PHP：日期对象
来源：http://jas.shuidangran.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ncd.vqdsnc.cn

[U63] PHP：文件读写
来源：http://tyt.hcnkem.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://opd.yanxiufei.cn

[U64] PHP：目录遍历
来源：http://cno.yanxiufei.cn

glob("dir/*.php");  scandir("dir");
来源：http://per.fktsv.cn

[U65] PHP：会话
来源：http://jgq.meibo888.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ocs.yfazqb.com

[U66] PHP：设置 Cookie
来源：http://elr.jiagoushi.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ozb.xuanzx.com

[U67] PHP：处理文件上传
来源：http://bsi.ydjk.org.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://acg.jinqigfzy.top

[U68] PHP：PDO 连接
来源：http://jua.0kj1m.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://azp.ehwqpu.com

[U69] PHP：PDO 预处理
来源：http://guh.xinyue.icu

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://oyv.wangshuangyany.cn

[U70] PHP：PDO 事务
来源：http://via.xinyue.icu

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zun.ppjwa.cn

[U71] PHP：抛出异常
来源：http://gae.52xcode.cn

throw new RuntimeException("失败", 500);
来源：http://aiv.tanke756.top

[U72] PHP：写错误日志
来源：http://ihy.meibo888.top

error_log("失败: " . $e->getMessage());
来源：http://huv.daria6918.cn

[U73] PHP：读取 ini 配置
来源：http://yom.uphjek.com

parse_ini_file("config.ini", true)
来源：http://mor.hnxiangtu.top

[U74] PHP：读取环境变量
来源：http://vml.xuetiantiany.cn

getenv("APP_ENV") ?: "production"
来源：http://oig.zhongyouzk.top

[U75] PHP：依赖注入
来源：http://tja.tianlin.xyz

composer require psr/container
来源：http://lbc.yueranfly.top

[U76] PHP：简单路由
来源：http://req.0kj1m.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sjy.zhoulong.xyz

[U77] PHP：模板渲染
来源：http://apn.dianchejie.cn

composer require twig/twig
来源：http://ave.yanxiufei.cn

[U78] PHP：单元测试
来源：http://wuj.pengpengdd.cyou

composer require --dev phpunit/phpunit
来源：http://ign.fzhhl.top

[U79] PHP：静态分析
来源：http://kwh.zhixingplan.top

composer require --dev phpstan/phpstan
来源：http://qbh.snrcjt.cn

[U80] PHP：代码规范修复
来源：http://adr.kuanghao11.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://uth.iojbl.cn

[U81] JS：初始化项目
来源：http://naa.yuanzhike.top

npm init -y;  npm i express
来源：http://bvi.jinqigfzy.top

[U82] JS：package.json 脚本
来源：http://vtd.tanke756.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dwg.pycfn.com

[U83] JS：ES Module 导入导出
来源：http://rbz.guowangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://fbg.yuanzhike.top

[U84] JS：CommonJS 写法
来源：http://jbc.jinyuanbaomall.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bkw.cucudq.cn

[U85] JS：可选链
来源：http://qdt.guowangkeji.top

a?.b?.c
来源：http://bcr.jyoumei.cn

[U86] JS：空值合并
来源：http://irp.fktsv.cn

a ?? b
来源：http://dbu.wangdashe.top

[U87] JS：解构默认值
来源：http://vsz.hcnkem.com

const { a = 1, b = 2 } = obj;
来源：http://iwr.gotoacloud.top

[U88] JS：对象展开合并
来源：http://rhj.nanxuanxn.top

{ ...a, ...b }
来源：http://kwd.aizwys.cn

[U89] JS：数组去重
来源：http://rra.tian-w.cn

[...new Set(arr)]
来源：http://hvg.shanyushiyangtech.top

[U90] JS：数字数组排序
来源：http://fbe.hywenlv.cn

[...arr].sort((a, b) => a - b)
来源：http://mbh.zhaomingkeji.xyz

[U91] JS：对象键值遍历
来源：http://iga.jinyuanbaomall.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kgr.pengpengdd.cyou

[U92] JS：深拷贝
来源：http://ara.yangfankeji.com

structuredClone(obj)
来源：http://ogv.chenzaomai.com

[U93] JS：模板字符串
来源：http://xfb.jiagoushi.top

`共 ${n} 条`
来源：http://dwt.nanxuanxn.top

[U94] JS：箭头函数
来源：http://ven.jiagoushi.top

const double = x => x * 2;
来源：http://vwq.0kj1m.cn

[U95] JS：Promise 包装
来源：http://xbm.fktsv.cn

new Promise((resolve, reject) => {})
来源：http://yhh.yvedp.cn

[U96] JS：async/await 与异常
来源：http://lmd.iojbl.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jhv.fktsv.cn

[U97] JS：并发请求
来源：http://zcm.ppjwa.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://aoa.daxiang520.top

[U98] JS：fetch 带 JSON
来源：http://jpe.guowangkeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://brb.jqgfzy.top

[U99] JS：事件监听
来源：http://don.dashuyun.cn

el.addEventListener("click", e => {})
来源：http://nhg.hnqzz.top

[U100] JS：DOM 查询
来源：http://yfa.fehbvm.com

document.querySelector(".item")
来源：http://jsp.9152youxi.cn

[U101] JS：classList 操作
来源：http://dhi.svipenyu.cn

el.classList.toggle("active")
来源：http://fgz.nanxuanxn.top

[U102] JS：本地存储
来源：http://caz.ehwqpu.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://pfi.ywan-chungtsiang.top

[U103] JS：定时器
来源：http://hyj.havefunace.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jaw.jinqigfzy.top

[U104] JS：防抖
来源：http://tdn.dashuyun.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qpi.redwolf501.top

[U105] JS：节流
来源：http://gfr.gotoacloud.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bdy.ctjpmb.com

[U106] JS：日期格式化
来源：http://tmg.ehwqpu.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://aby.yj20258888.top

[U107] JS：数字千分位
来源：http://hbj.havefunace.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zmh.tanke756.top

[U108] JS：随机整数
来源：http://eck.daxiang520.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vnx.sysykeji.top

[U109] JS：数组分组
来源：http://kbc.snrcjt.cn

Object.groupBy(arr, x => x.type)
来源：http://apn.sjlbkw.cn

[U110] JS：数组分块
来源：http://wjd.hammf.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://afr.hcnkem.com

[U111] JS：对象转 Map
来源：http://zea.ivvv.top

new Map(Object.entries(obj))
来源：http://nrf.cheryme.top

[U112] JS：字符串补位
来源：http://fun.kuanghao11.cn

"7".padStart(3, "0")
来源：http://coq.chenzaomai.com

[U113] JS：正则替换全部
来源：http://xfu.gzhubu.top

s.replaceAll("a", "b")
来源：http://ouh.sjlbkw.cn

[U114] JS：JSON 深比较
来源：http://lql.nanxinkj.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ojf.cashguo.top

[U115] JS：生成 UUID
来源：http://euo.pycfn.com

crypto.randomUUID()
来源：http://rue.pycfn.com

[U116] JS：类型检查（JSDoc）
来源：http://gjq.wangdashe.top

/** @param {string} name */ function f(name) {}
来源：http://fpe.sufxvd.cn

[U117] JS：单元测试
来源：http://uwp.xinyue.icu

npm i -D vitest;  npx vitest
来源：http://umo.tanke756.top

[U118] JS：开发服务器
来源：http://rtq.yj20258.top

npm i -D vite;  npx vite
来源：http://jaf.9152youxi.cn

[U119] JS：生产构建
来源：http://mwl.zdqjudy.top

npx vite build
来源：http://npk.yonumen.top

[U120] JS：读取环境变量（Vite）
来源：http://cfj.aibaodan.cn

import.meta.env.VITE_API_URL
来源：http://lcf.tarul.cn

================================================================================
来源：http://ktu.jqgfzy.top

统计汇总
来源：http://tcw.jianghu66.top

================================================================================
来源：http://pvb.gotoacloud.top

按语言统计（条）：
来源：http://mdk.hcnkem.com

Python ......... 252
来源：http://bcz.pycfn.com

PHP ............ 252
来源：http://ceh.zhixingplan.top

JavaScript ..... 252
来源：http://nnd.iojbl.cn

TypeScript ..... 212
来源：http://rga.hnqzz.top

Java ........... 212
来源：http://zlh.zhengqikj.top

Go ............. 212
来源：http://quh.sweek.top

Ruby ........... 212
来源：http://dfb.pycfn.com

C# ............. 212
来源：http://wwn.sxryk.cn

C .............. 30
来源：http://hvs.hnxiangtu.top

C++ ............ 30
来源：http://cld.hnqzz.top

SQL ............ 90
来源：http://yyb.tanke756.top

Bash ........... 80
来源：http://jjg.guannengcc.top

Kotlin ......... 15
来源：http://ara.bjfxy.top

Swift .......... 15
来源：http://ptf.vehdjk.com

Lua ............ 10
来源：http://ykw.guannengcc.top

Perl ........... 10
来源：http://xll.nanxuanxn.top

Scala .......... 10
来源：http://zux.yonumen.top

------------------------------------
来源：http://yne.shangyingyoupin.top

合计 ........... 2106 条
来源：http://blk.jlsjyb.cn

按章节统计：
来源：http://roz.gzhubu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://emo.yueranfly.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zir.zhongyouzk.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://psd.9152youxi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ucw.haohaochexian.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oqu.hywenlv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cbh.gogol.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qzq.bjfxy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gdu.shzxlz.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vwh.andypj.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vqx.yuxming.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uur.sjlbkw.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vsv.yanxiufei.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dpp.ybcxt.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://osv.sysykeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fub.jinyuanbaomall.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://obu.xziqi.cn

Q SQL 专题                              90
来源：http://kad.svipenyu.cn

R Bash 专题                             80
来源：http://uag.uphjek.com

S C / C++ 专题                          60
来源：http://sjg.jinqigfzy.top

T 其他语言补充                          60
来源：http://clp.nanxuanxn.top

U 高频实用片段                         120
来源：http://cdy.zycfv.cn

------------------------------------
来源：http://uki.yfazqb.com

合计                                  2106 条
来源：http://igw.cheryme.top

--------------------------------------------------------------------------------
来源：http://kkf.zhengqikj.top

使用提醒
来源：http://xdt.hnqzz.top

--------------------------------------------------------------------------------
来源：http://brx.fanxiaobao.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bgc.tianlin.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rzl.jinghuilouyu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lut.ctjpmb.com

在旧版本上使用前请先确认语法支持情况。
来源：http://qte.hnqzz.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jqc.andypj.xyz

—— 文件结束 ——
来源：http://yvi.dianchejie.cn

================================================================================
来源：http://djo.shzxlz.cn

程序语言常见例子速查手册（2024 版）
来源：http://rte.jinqigufen.top

Common Programming Examples Cheat Book
来源：http://zmj.zhixingplan.top

================================================================================
来源：http://ugi.svipenyu.cn

【收录内容】
来源：http://hqy.gotoacloud.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://otl.bjfxy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qbh.nanxinkj.top

SQL · Bash · C · C++
来源：http://xxy.cheryme.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gjp.cucudq.cn

【使用说明】
来源：http://ptu.xylfe.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mia.hnqzz.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tan.cucudq.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lnz.tian-w.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vbd.havefunace.top

Bash:  Shell         C:     C             C++:   C++
来源：http://vya.haohaochexian.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://suj.shuidangran.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ijc.cucudq.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tdr.tian-w.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://omw.yanxiufei.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://epw.jianghu66.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dzb.dashuyun.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://whj.ydjk.org.cn

【文件统计】
来源：http://sfe.wangdashe.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mzp.hnqzz.top

--------------------------------------------------------------------------------
来源：http://dok.hnxiangtu.top

目  录
来源：http://vqs.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://jqd.meibo888.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rsr.jinqigfzy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wmg.daxiang520.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pfl.zdqjudy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kwb.xylfe.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dye.tarul.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://heb.ppjwa.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://txz.andypj.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yjq.mhx1999.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dpk.vehdjk.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dxi.yvedp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://aoh.zdbjq.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qvd.vehdjk.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ujm.hysaishi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jvj.yj202588.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jih.shanyushiyangkeji.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kqb.vqdsnc.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://iqa.gotoacloud.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://fox.316326.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gbj.zhongyouzk.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kuh.nanxuanxn.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://oit.jyoumei.cn

================================================================================
来源：http://fqs.yj20258.top

A. 基础语法与类型
来源：http://fbv.ydjk.org.cn

================================================================================
来源：http://nnj.cheryme.top

[A01] Hello World
来源：http://jpz.shanyushiyangtech.top

Py:   print("Hello, World!")
来源：http://blo.gaohongyu789.top

PHP:  echo "Hello, World!";
来源：http://umb.jinyuanbaomall.cn

JS:   console.log("Hello, World!");
来源：http://mpz.ehwqpu.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ahw.guannengcc.top

Java: System.out.println("Hello, World!");
来源：http://jxd.epnwcf.com

Go:   fmt.Println("Hello, World!")
来源：http://rku.shzxlz.cn

Ruby: puts "Hello, World!"
来源：http://msy.chenlongwang.top

C#:   Console.WriteLine("Hello, World!");
来源：http://szs.jiagoushi.top

[A02] 变量声明与赋值
来源：http://kif.ehwqpu.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://orc.pycfn.com

PHP:  $name = "Alex"; $age = 20;
来源：http://hij.kuanghao11.cn

JS:   let name = "Alex"; const age = 20;
来源：http://khy.hcnkem.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ckl.yanxiufei.cn

Java: String name = "Alex"; int age = 20;
来源：http://hiz.dianchejie.cn

Go:   name := "Alex"; age := 20
来源：http://eoj.yuxming.cn

Ruby: name = "Alex"; age = 20
来源：http://xju.yj202588.top

C#:   string name = "Alex"; int age = 20;
来源：http://xkb.jyoumei.cn

[A03] 常量定义
来源：http://lho.pycfn.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ojf.cucudq.cn

PHP:  const PI = 3.14159;
来源：http://irc.cucudq.cn

JS:   const PI = 3.14159;
来源：http://ohw.aibaodan.cn

TS:   const PI: number = 3.14159;
来源：http://voy.jqgufenzy.top

Java: static final double PI = 3.14159;
来源：http://hji.shangyingyoupin.top

Go:   const PI = 3.14159
来源：http://lwz.jinyuanbaomall.cn

Ruby: PI = 3.14159
来源：http://wub.jqgufenzy.top

C#:   const double PI = 3.14159;
来源：http://xhd.vqdsnc.cn

[A04] 判断变量类型
来源：http://hab.gotoacloud.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://mqw.ivvv.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lvd.ybcxt.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lyg.jlsjyb.cn

TS:   typeof x; x instanceof Date
来源：http://tfg.wangdashe.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tgl.ivvv.top

Go:   reflect.TypeOf(x).Name()
来源：http://kxs.wangdashe.top

Ruby: x.class; x.is_a?(Integer)
来源：http://gne.shanyushiyangkeji.top

C#:   x.GetType().Name; x is int
来源：http://wpc.cheryme.top

[A05] 整数除法与取模
来源：http://kei.yj202588.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dcf.ppjwa.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://usf.gaohongyu789.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://spx.zdqjudy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wtt.hnxiangtu.top

Java: 7 / 2; 7 % 2
来源：http://yxh.jqgfzy.top

Go:   7 / 2; 7 % 2
来源：http://ikt.havefunace.top

Ruby: 7 / 2; 7 % 2
来源：http://myb.svipenyu.cn

C#:   7 / 2; 7 % 2
来源：http://lcf.sufxvd.cn

[A06] 字符串转数字
来源：http://rqw.zhengqikj.top

Py:   int("42"); float("3.14")
来源：http://jyh.dianchejie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kgy.jlsjyb.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wgl.hongshengwenyu.top

TS:   parseInt("42", 10); Number("42")
来源：http://uao.zycfv.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xop.birdmap.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nef.hfpthk.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://eqh.yuxming.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qiv.fanxiaobao.xyz

[A07] 数字转字符串
来源：http://nrh.yangfankeji.com

Py:   str(42)
来源：http://jyt.jinghuilouyu.cn

PHP:  (string) 42; strval(42)
来源：http://lqa.zhongyouzk.top

JS:   String(42); (42).toString()
来源：http://bzp.fanxiaobao.xyz

TS:   String(42)
来源：http://ctf.fanxiaobao.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://jem.jqgfzy.top

Go:   strconv.Itoa(42)
来源：http://xgv.vqdsnc.cn

Ruby: 42.to_s
来源：http://wjm.zhongyouzk.top

C#:   42.ToString()
来源：http://zxf.mhx1999.top

[A08] 取整与四舍五入
来源：http://gzg.yvedp.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://msu.guannengcc.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zne.haohaochexian.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wvy.feifeiyinyue.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://drz.uphjek.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://csj.hywenlv.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ozz.jqgfzy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://tup.xinyue.icu

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lye.pengpengdd.cyou

[A09] 绝对值与最大最小值
来源：http://hen.yuxming.cn


<!-- 参考信息 -->