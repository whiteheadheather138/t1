代发 wailian999

[U63] PHP：文件读写
来源：http://yab.snrcjt.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ivz.hongshengwenyu.top

[U64] PHP：目录遍历
来源：http://ynu.iojbl.cn

glob("dir/*.php");  scandir("dir");
来源：http://yec.bjfxy.top

[U65] PHP：会话
来源：http://pgh.hfpthk.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lsq.yuanzhike.top

[U66] PHP：设置 Cookie
来源：http://din.smart0.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uvz.meibo888.top

[U67] PHP：处理文件上传
来源：http://qcn.chenjidiqi.icu

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rzm.hcnkem.com

[U68] PHP：PDO 连接
来源：http://cpr.nanxuanxn.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vvc.zhijiandao.cn

[U69] PHP：PDO 预处理
来源：http://ewx.sysykeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://aod.jqgfzy.top

[U70] PHP：PDO 事务
来源：http://gsh.andypj.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xxb.yongpay.top

[U71] PHP：抛出异常
来源：http://pkz.jinghuilouyu.cn

throw new RuntimeException("失败", 500);
来源：http://oqt.iojbl.cn

[U72] PHP：写错误日志
来源：http://psp.havefunace.top

error_log("失败: " . $e->getMessage());
来源：http://ijn.mhx1999.top

[U73] PHP：读取 ini 配置
来源：http://laz.shuidangran.top

parse_ini_file("config.ini", true)
来源：http://aoo.aizwys.cn

[U74] PHP：读取环境变量
来源：http://bsy.gogol.net.cn

getenv("APP_ENV") ?: "production"
来源：http://dsy.yonumen.top

[U75] PHP：依赖注入
来源：http://giq.cashguo.top

composer require psr/container
来源：http://urr.guannengcc.top

[U76] PHP：简单路由
来源：http://yuu.chenzaomai.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pgp.hnqzz.top

[U77] PHP：模板渲染
来源：http://xux.316326.xyz

composer require twig/twig
来源：http://abi.fktsv.cn

[U78] PHP：单元测试
来源：http://tkm.hongshengwenyu.top

composer require --dev phpunit/phpunit
来源：http://nmh.jinqigfzy.top

[U79] PHP：静态分析
来源：http://zap.chenzaomai.com

composer require --dev phpstan/phpstan
来源：http://zfl.ehwqpu.com

[U80] PHP：代码规范修复
来源：http://lvd.xylfe.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kve.yj20258888.top

[U81] JS：初始化项目
来源：http://csc.hongshengwenyu.top

npm init -y;  npm i express
来源：http://gzx.chenzaomai.com

[U82] JS：package.json 脚本
来源：http://por.shuidangran.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://raw.xinyue.icu

[U83] JS：ES Module 导入导出
来源：http://blk.shanyushiyangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://zxo.chenjidiqi.icu

[U84] JS：CommonJS 写法
来源：http://sym.uphjek.com

module.exports = { a };  const { a } = require("./m");
来源：http://erl.havefunace.top

[U85] JS：可选链
来源：http://rda.smart0.xyz

a?.b?.c
来源：http://cvh.yuanzhike.top

[U86] JS：空值合并
来源：http://nvn.hywenlv.cn

a ?? b
来源：http://yaf.redwolf501.top

[U87] JS：解构默认值
来源：http://lkx.zhengqikj.top

const { a = 1, b = 2 } = obj;
来源：http://jqn.guowangkeji.top

[U88] JS：对象展开合并
来源：http://vas.cqqwz.cn

{ ...a, ...b }
来源：http://pup.hongshengwenyu.top

[U89] JS：数组去重
来源：http://axn.aibaodan.cn

[...new Set(arr)]
来源：http://xwi.jqgufenzy.top

[U90] JS：数字数组排序
来源：http://qjr.jqgfzy.top

[...arr].sort((a, b) => a - b)
来源：http://cuz.yonumen.top

[U91] JS：对象键值遍历
来源：http://drn.bjfxy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wpx.sjlbkw.cn

[U92] JS：深拷贝
来源：http://fqd.jinyuanbaomall.cn

structuredClone(obj)
来源：http://qya.feifeiyinyue.top

[U93] JS：模板字符串
来源：http://irf.hcnkem.com

`共 ${n} 条`
来源：http://iya.snrcjt.cn

[U94] JS：箭头函数
来源：http://hne.ybcxt.top

const double = x => x * 2;
来源：http://ist.redwolf501.top

[U95] JS：Promise 包装
来源：http://udh.shzxlz.cn

new Promise((resolve, reject) => {})
来源：http://aae.uphjek.com

[U96] JS：async/await 与异常
来源：http://uco.yueranfly.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://iyk.sjlbkw.cn

[U97] JS：并发请求
来源：http://rtf.0kj1m.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://nwc.c1oappe.top

[U98] JS：fetch 带 JSON
来源：http://jrb.cucudq.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kks.shuidangran.top

[U99] JS：事件监听
来源：http://obz.chenzaomai.com

el.addEventListener("click", e => {})
来源：http://ewg.ppjwa.cn

[U100] JS：DOM 查询
来源：http://zst.jlsjyb.cn

document.querySelector(".item")
来源：http://xnv.nanxuanxn.top

[U101] JS：classList 操作
来源：http://irb.cucudq.cn

el.classList.toggle("active")
来源：http://xat.zdqjudy.top

[U102] JS：本地存储
来源：http://xiz.sysykeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://iom.meibo888.top

[U103] JS：定时器
来源：http://nzu.cqqwz.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vwe.c1oappe.top

[U104] JS：防抖
来源：http://vnp.tanke756.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://azh.0kj1m.cn

[U105] JS：节流
来源：http://rre.zhongyouzk.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ibb.yfazqb.com

[U106] JS：日期格式化
来源：http://xqt.yfazqb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dqp.shzxlz.cn

[U107] JS：数字千分位
来源：http://zfg.wangshuangyany.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mnw.shuidangran.top

[U108] JS：随机整数
来源：http://xqh.jinqigufen.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://eek.feifeiyinyue.top

[U109] JS：数组分组
来源：http://ocx.aibaodan.cn

Object.groupBy(arr, x => x.type)
来源：http://jlz.birdmap.top

[U110] JS：数组分块
来源：http://ief.yangfankeji.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yyd.daria6918.cn

[U111] JS：对象转 Map
来源：http://xvf.52xcode.cn

new Map(Object.entries(obj))
来源：http://lgw.gzhubu.top

[U112] JS：字符串补位
来源：http://nvh.gogol.net.cn

"7".padStart(3, "0")
来源：http://rhn.zhijiandao.cn

[U113] JS：正则替换全部
来源：http://gqv.zhaomingkeji.xyz

s.replaceAll("a", "b")
来源：http://gam.hfpthk.cn

[U114] JS：JSON 深比较
来源：http://vud.daxiang520.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hxd.hfpthk.cn

[U115] JS：生成 UUID
来源：http://lci.shuidangran.top

crypto.randomUUID()
来源：http://joh.cdnleiting.top

[U116] JS：类型检查（JSDoc）
来源：http://hkp.uphjek.com

/** @param {string} name */ function f(name) {}
来源：http://wke.xingfuxueyuan.xyz

[U117] JS：单元测试
来源：http://iwa.hesvh.cn

npm i -D vitest;  npx vitest
来源：http://qmx.feifeiyinyue.top

[U118] JS：开发服务器
来源：http://yji.cheryme.top

npm i -D vite;  npx vite
来源：http://obr.hnxiangtu.top

[U119] JS：生产构建
来源：http://agz.cheryme.top

npx vite build
来源：http://iqp.jinyuanbaomall.cn

[U120] JS：读取环境变量（Vite）
来源：http://hgn.cqqwz.cn

import.meta.env.VITE_API_URL
来源：http://yqn.pycfn.com

================================================================================
来源：http://fif.fengsongda.top

统计汇总
来源：http://jnk.hnqzz.top

================================================================================
来源：http://ezi.ydzc1.top

按语言统计（条）：
来源：http://nze.hesvh.cn

Python ......... 252
来源：http://bba.yanxiufei.cn

PHP ............ 252
来源：http://htg.iojbl.cn

JavaScript ..... 252
来源：http://kgr.pengpengdd.cyou

TypeScript ..... 212
来源：http://bpo.cdnleiting.top

Java ........... 212
来源：http://sla.52xcode.cn

Go ............. 212
来源：http://ryz.jiagoushi.top

Ruby ........... 212
来源：http://ixg.tian-w.cn

C# ............. 212
来源：http://wxi.wangshuangyany.cn

C .............. 30
来源：http://quh.yangfankeji.com

C++ ............ 30
来源：http://zoo.uphjek.com

SQL ............ 90
来源：http://mwj.mhx1999.top

Bash ........... 80
来源：http://dax.xuetiantiany.cn

Kotlin ......... 15
来源：http://hww.gaohongyu789.top

Swift .......... 15
来源：http://osz.jqgfzy.top

Lua ............ 10
来源：http://kcs.sysykeji.top

Perl ........... 10
来源：http://dsb.yangfankeji.com

Scala .......... 10
来源：http://isc.yj20258888.top

------------------------------------
来源：http://wxt.xuanzx.com

合计 ........... 2106 条
来源：http://mja.cucudq.cn

按章节统计：
来源：http://til.shanyushiyangkeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ftl.smart0.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://imk.gogol.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sgk.pengpengdd.cyou

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://swq.yj20258.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rvu.zhiwuduotai.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ehs.gzhubu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qlj.zhengqikj.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hyu.haohaochexian.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hsp.snrcjt.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ctt.cdnleiting.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qjy.hammf.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dtu.quarkkingdee.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cur.hnqzz.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tqi.xingfuxueyuan.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://duy.yanxiufei.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://roe.yj202588.top

Q SQL 专题                              90
来源：http://zxs.yangfankeji.com

R Bash 专题                             80
来源：http://eik.shuidangran.top

S C / C++ 专题                          60
来源：http://yuh.shuidangran.top

T 其他语言补充                          60
来源：http://ygd.chenzaomai.com

U 高频实用片段                         120
来源：http://vgt.ydzc1.top

------------------------------------
来源：http://mdb.chenzaomai.com

合计                                  2106 条
来源：http://oss.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://epl.ydzc1.top

使用提醒
来源：http://uck.hesvh.cn

--------------------------------------------------------------------------------
来源：http://mvp.cashguo.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hzl.fanxiaobao.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bbf.aibaodan.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bfd.shanyushiyangtech.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ybd.uphjek.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://znq.fengsongda.top

—— 文件结束 ——
来源：http://btr.shangyingyoupin.top

================================================================================
来源：http://fsf.haohaochexian.top

程序语言常见例子速查手册（2024 版）
来源：http://all.shzxlz.cn

Common Programming Examples Cheat Book
来源：http://iwl.jinqigfzy.top

================================================================================
来源：http://tmx.nanxuanxn.top

【收录内容】
来源：http://ywh.pycfn.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://rnq.316326.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dts.kuanghao11.cn

SQL · Bash · C · C++
来源：http://bqj.nanxinkj.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rak.sweek.top

【使用说明】
来源：http://sbn.tian-w.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pei.gotoacloud.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uzw.hnqzz.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kuc.hysaishi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kum.mhx1999.top

Bash:  Shell         C:     C             C++:   C++
来源：http://idv.redwolf501.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://flf.fzhhl.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mkg.aizwys.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hbq.sweek.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://igb.quarkkingdee.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pjf.zhixingplan.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tgq.fktsv.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://olr.sxryk.cn

【文件统计】
来源：http://zqd.jiagoushi.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xck.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://bma.wangshuangyany.cn

目  录
来源：http://gnu.yj202588.top

--------------------------------------------------------------------------------
来源：http://xia.smart0.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wya.sweek.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mzv.aizwys.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bsj.sjlbkw.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jaz.zhixingplan.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nib.cheryme.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://apw.svipenyu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://eip.tanke756.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pan.sysykeji.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jvc.316326.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tmq.feifeiyinyue.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tuf.sweek.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://umw.pengpengdd.cyou

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fkn.jinyuanbaomall.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bsv.yuanzhike.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zfh.hesvh.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xht.snrcjt.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vbd.smart0.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://sll.jqgfzy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rax.jinqigfzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://djg.xinyue.icu

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tjw.yongpay.top

================================================================================
来源：http://alh.gogol.net.cn

A. 基础语法与类型
来源：http://kpm.snrcjt.cn

================================================================================
来源：http://jdn.ehwqpu.com

[A01] Hello World
来源：http://xsu.feifeiyinyue.top

Py:   print("Hello, World!")
来源：http://efo.hywenlv.cn

PHP:  echo "Hello, World!";
来源：http://yjy.jianghu66.top

JS:   console.log("Hello, World!");
来源：http://pgi.vehdjk.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://iec.cdnleiting.top

Java: System.out.println("Hello, World!");
来源：http://knk.chenzaomai.com

Go:   fmt.Println("Hello, World!")
来源：http://ref.ydjk.org.cn

Ruby: puts "Hello, World!"
来源：http://fsl.yanxiufei.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://odf.nanxuanxn.top

[A02] 变量声明与赋值
来源：http://ntj.feifeiyinyue.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yor.sweek.top

PHP:  $name = "Alex"; $age = 20;
来源：http://aba.yangfankeji.com

JS:   let name = "Alex"; const age = 20;
来源：http://rpo.shanyushiyangtech.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://itl.chenzaomai.com

Java: String name = "Alex"; int age = 20;
来源：http://uzk.xinyue.icu

Go:   name := "Alex"; age := 20
来源：http://bvy.daria6918.cn

Ruby: name = "Alex"; age = 20
来源：http://pfx.xylfe.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xpt.hesvh.cn

[A03] 常量定义
来源：http://kxa.yj202588.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fch.jinqigufen.top

PHP:  const PI = 3.14159;
来源：http://mnz.hongshengwenyu.top

JS:   const PI = 3.14159;
来源：http://mwu.jqgfzy.top

TS:   const PI: number = 3.14159;
来源：http://cfi.jiagoushi.top

Java: static final double PI = 3.14159;
来源：http://bae.zhoulong.xyz

Go:   const PI = 3.14159
来源：http://ayl.xuanzx.com

Ruby: PI = 3.14159
来源：http://aqm.yj20258888.top

C#:   const double PI = 3.14159;
来源：http://sel.zhongyouzk.top

[A04] 判断变量类型
来源：http://ryq.fanxiaobao.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://krz.yueranfly.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jwy.iojbl.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://why.jianghu66.top

TS:   typeof x; x instanceof Date
来源：http://ijp.guowangkeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pwl.aibaodan.cn

Go:   reflect.TypeOf(x).Name()
来源：http://zke.dashuyun.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lrh.bjfxy.top

C#:   x.GetType().Name; x is int
来源：http://lhk.uphjek.com

[A05] 整数除法与取模
来源：http://ahk.52xcode.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://chc.fzhhl.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://clk.hongshengwenyu.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://btm.kuanghao11.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zmt.ydjk.org.cn

Java: 7 / 2; 7 % 2
来源：http://oic.zhongyouzk.top

Go:   7 / 2; 7 % 2
来源：http://ufl.uphjek.com

Ruby: 7 / 2; 7 % 2
来源：http://ktq.gzhubu.top

C#:   7 / 2; 7 % 2
来源：http://nnq.yuxming.cn

[A06] 字符串转数字
来源：http://kkh.zhongyouzk.top

Py:   int("42"); float("3.14")
来源：http://nkt.cqqwz.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yqh.havefunace.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zon.chenjidiqi.icu

TS:   parseInt("42", 10); Number("42")
来源：http://npa.fktsv.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rwa.jqgufenzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kvi.shanyushiyangkeji.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ypo.feifeiyinyue.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uxs.ivvv.top

[A07] 数字转字符串
来源：http://tyr.ppjwa.cn

Py:   str(42)
来源：http://jfj.guowangkeji.top

PHP:  (string) 42; strval(42)
来源：http://hza.sufxvd.cn

JS:   String(42); (42).toString()
来源：http://zka.tanke756.top

TS:   String(42)
来源：http://rcq.ydjk.org.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://wxq.gzhubu.top

Go:   strconv.Itoa(42)
来源：http://wgr.shangyingyoupin.top

Ruby: 42.to_s
来源：http://hki.ydjk.org.cn

C#:   42.ToString()
来源：http://dzy.ppjwa.cn

[A08] 取整与四舍五入
来源：http://hdg.smart0.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wwp.havefunace.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tcm.pycfn.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://uwj.xinyue.icu

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://uge.sufxvd.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sut.52xcode.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wff.jinyuanbaomall.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://etv.hfpthk.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jhs.zhijiandao.cn

[A09] 绝对值与最大最小值
来源：http://plk.shanyushiyangtech.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qrv.yj20258.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qhg.hnxiangtu.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fwr.hysaishi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jis.feifeiyinyue.top


<!-- 参考信息 -->