代发 wailian999

[U65] PHP：会话
来源：http://rmz.daria6918.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xfo.guowangkeji.top

[U66] PHP：设置 Cookie
来源：http://nkd.feifeiyinyue.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zrh.52xcode.cn

[U67] PHP：处理文件上传
来源：http://bbw.zdqjudy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yas.iojbl.cn

[U68] PHP：PDO 连接
来源：http://buk.svipenyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://eiy.yj20258888.top

[U69] PHP：PDO 预处理
来源：http://lxe.svipenyu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cdm.yfazqb.com

[U70] PHP：PDO 事务
来源：http://hnh.cashguo.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tlt.yuanzhike.top

[U71] PHP：抛出异常
来源：http://ugb.hywenlv.cn

throw new RuntimeException("失败", 500);
来源：http://izy.ctjpmb.com

[U72] PHP：写错误日志
来源：http://ekt.guannengcc.top

error_log("失败: " . $e->getMessage());
来源：http://mzw.epnwcf.com

[U73] PHP：读取 ini 配置
来源：http://zmg.hywenlv.cn

parse_ini_file("config.ini", true)
来源：http://xfb.yangfankeji.com

[U74] PHP：读取环境变量
来源：http://qdh.guannengcc.top

getenv("APP_ENV") ?: "production"
来源：http://nev.iojbl.cn

[U75] PHP：依赖注入
来源：http://fbx.xylfe.cn

composer require psr/container
来源：http://wdq.tian-w.cn

[U76] PHP：简单路由
来源：http://mpv.zycfv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://adq.gotoacloud.top

[U77] PHP：模板渲染
来源：http://lwf.bbcook.cn

composer require twig/twig
来源：http://ezw.svipenyu.cn

[U78] PHP：单元测试
来源：http://jlq.zdbjq.cn

composer require --dev phpunit/phpunit
来源：http://iid.feifeiyinyue.top

[U79] PHP：静态分析
来源：http://btp.nanxinkj.top

composer require --dev phpstan/phpstan
来源：http://wfl.snrcjt.cn

[U80] PHP：代码规范修复
来源：http://vwe.xuanzx.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://fav.fanxiaobao.xyz

[U81] JS：初始化项目
来源：http://gho.chenlongwang.top

npm init -y;  npm i express
来源：http://nkt.ctjpmb.com

[U82] JS：package.json 脚本
来源：http://jyv.tianlin.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eha.dianchejie.cn

[U83] JS：ES Module 导入导出
来源：http://dtj.uphjek.com

export const a = 1;  import { a } from "./m.js";
来源：http://bhy.yvedp.cn

[U84] JS：CommonJS 写法
来源：http://pwl.zdqjudy.top

module.exports = { a };  const { a } = require("./m");
来源：http://tnl.redwolf501.top

[U85] JS：可选链
来源：http://cfk.dianchejie.cn

a?.b?.c
来源：http://del.epnwcf.com

[U86] JS：空值合并
来源：http://tke.xylfe.cn

a ?? b
来源：http://nqm.yangfankeji.com

[U87] JS：解构默认值
来源：http://taf.pengpengdd.cyou

const { a = 1, b = 2 } = obj;
来源：http://qjb.birdmap.top

[U88] JS：对象展开合并
来源：http://xfi.gotoacloud.top

{ ...a, ...b }
来源：http://xww.gogol.net.cn

[U89] JS：数组去重
来源：http://slv.cheryme.top

[...new Set(arr)]
来源：http://vqx.9152youxi.cn

[U90] JS：数字数组排序
来源：http://uvs.hysaishi.cn

[...arr].sort((a, b) => a - b)
来源：http://vjo.wangshuangyany.cn

[U91] JS：对象键值遍历
来源：http://rpc.jianghu66.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dxk.yj20258.top

[U92] JS：深拷贝
来源：http://gwl.gaohongyu789.top

structuredClone(obj)
来源：http://hou.uphjek.com

[U93] JS：模板字符串
来源：http://flk.zdqjudy.top

`共 ${n} 条`
来源：http://nnn.zhengqikj.top

[U94] JS：箭头函数
来源：http://gfr.jinyuanbaomall.cn

const double = x => x * 2;
来源：http://arc.zycfv.cn

[U95] JS：Promise 包装
来源：http://awa.hesvh.cn

new Promise((resolve, reject) => {})
来源：http://vzj.yanxiufei.cn

[U96] JS：async/await 与异常
来源：http://yvq.guannengcc.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hns.tanke756.top

[U97] JS：并发请求
来源：http://fpk.xingfuxueyuan.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://tcz.daria6918.cn

[U98] JS：fetch 带 JSON
来源：http://eus.shuidangran.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://iah.dashuyun.cn

[U99] JS：事件监听
来源：http://wzk.sweek.top

el.addEventListener("click", e => {})
来源：http://bkj.ydzc1.top

[U100] JS：DOM 查询
来源：http://oaw.yuanzhike.top

document.querySelector(".item")
来源：http://kiy.meibo888.top

[U101] JS：classList 操作
来源：http://kzh.xingfuxueyuan.xyz

el.classList.toggle("active")
来源：http://yhw.xingfuxueyuan.xyz

[U102] JS：本地存储
来源：http://fvk.aibaodan.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ult.quarkkingdee.top

[U103] JS：定时器
来源：http://ubt.bjfxy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fyc.yuanzhike.top

[U104] JS：防抖
来源：http://vxi.yvedp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ypi.xuanzx.com

[U105] JS：节流
来源：http://izh.jlsjyb.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ipx.vehdjk.com

[U106] JS：日期格式化
来源：http://ibf.yuxming.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://den.smart0.xyz

[U107] JS：数字千分位
来源：http://sgn.jlsjyb.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zff.gaohongyu789.top

[U108] JS：随机整数
来源：http://kef.316326.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://czu.hammf.cn

[U109] JS：数组分组
来源：http://qxt.jinqigufen.top

Object.groupBy(arr, x => x.type)
来源：http://znh.zhixingplan.top

[U110] JS：数组分块
来源：http://uuh.tarul.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nie.yuanzhike.top

[U111] JS：对象转 Map
来源：http://mnk.xziqi.cn

new Map(Object.entries(obj))
来源：http://zgl.cashguo.top

[U112] JS：字符串补位
来源：http://lzd.gogol.net.cn

"7".padStart(3, "0")
来源：http://mry.gogol.net.cn

[U113] JS：正则替换全部
来源：http://zco.havefunace.top

s.replaceAll("a", "b")
来源：http://zzh.meibo888.top

[U114] JS：JSON 深比较
来源：http://yem.ydzc1.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jgt.jlsjyb.cn

[U115] JS：生成 UUID
来源：http://qet.zhongyouzk.top

crypto.randomUUID()
来源：http://pdd.zycfv.cn

[U116] JS：类型检查（JSDoc）
来源：http://ise.jyoumei.cn

/** @param {string} name */ function f(name) {}
来源：http://ota.sjlbkw.cn

[U117] JS：单元测试
来源：http://urt.feifeiyinyue.top

npm i -D vitest;  npx vitest
来源：http://fyc.wangshuangyany.cn

[U118] JS：开发服务器
来源：http://hnm.cdnleiting.top

npm i -D vite;  npx vite
来源：http://ysu.shanyushiyangkeji.top

[U119] JS：生产构建
来源：http://kux.hywenlv.cn

npx vite build
来源：http://iog.xuetiantiany.cn

[U120] JS：读取环境变量（Vite）
来源：http://opz.haohaochexian.top

import.meta.env.VITE_API_URL
来源：http://nac.yvedp.cn

================================================================================
来源：http://oji.yangfankeji.com

统计汇总
来源：http://zly.hongshengwenyu.top

================================================================================
来源：http://vas.yj202588.top

按语言统计（条）：
来源：http://jmv.yj20258.top

Python ......... 252
来源：http://qpz.tian-w.cn

PHP ............ 252
来源：http://whg.xylfe.cn

JavaScript ..... 252
来源：http://iqx.sweek.top

TypeScript ..... 212
来源：http://vlq.yangfankeji.com

Java ........... 212
来源：http://eqi.mhx1999.top

Go ............. 212
来源：http://dfb.kuanghao11.cn

Ruby ........... 212
来源：http://obm.xylfe.cn

C# ............. 212
来源：http://wom.xinyue.icu

C .............. 30
来源：http://xpg.guowangkeji.top

C++ ............ 30
来源：http://csf.ehwqpu.com

SQL ............ 90
来源：http://njc.guowangkeji.top

Bash ........... 80
来源：http://yun.jqgfzy.top

Kotlin ......... 15
来源：http://kss.ydjk.org.cn

Swift .......... 15
来源：http://knt.pycfn.com

Lua ............ 10
来源：http://kge.zhixingplan.top

Perl ........... 10
来源：http://gmi.zhongyouzk.top

Scala .......... 10
来源：http://tpj.yfazqb.com

------------------------------------
来源：http://wom.c1oappe.top

合计 ........... 2106 条
来源：http://lge.yfazqb.com

按章节统计：
来源：http://wir.daxiang520.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mcf.snrcjt.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wrn.gaohongyu789.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://que.tarul.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://crz.birdmap.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wgz.hfpthk.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rym.zhengqikj.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fdy.quarkkingdee.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ntv.xinyue.icu

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qzh.52xcode.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nve.xingfuxueyuan.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oes.ywan-chungtsiang.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sen.zhixingplan.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uhz.jqgfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uum.yj20258.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hef.pengpengdd.cyou

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qxd.zhixingplan.top

Q SQL 专题                              90
来源：http://lbo.xinyue.icu

R Bash 专题                             80
来源：http://yfb.yonumen.top

S C / C++ 专题                          60
来源：http://sry.aibaodan.cn

T 其他语言补充                          60
来源：http://wml.xuanzx.com

U 高频实用片段                         120
来源：http://fuj.iojbl.cn

------------------------------------
来源：http://oed.xinyue.icu

合计                                  2106 条
来源：http://pqm.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://ets.hysaishi.cn

使用提醒
来源：http://igm.cashguo.top

--------------------------------------------------------------------------------
来源：http://yzv.uphjek.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://azh.zhoulong.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ych.pengpengdd.cyou

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sil.jyoumei.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://hen.jinghuilouyu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mvl.cqqwz.cn

—— 文件结束 ——
来源：http://ois.yanxiufei.cn

================================================================================
来源：http://ulg.meibo888.top

程序语言常见例子速查手册（2024 版）
来源：http://lkb.tanke756.top

Common Programming Examples Cheat Book
来源：http://poc.xinyue.icu

================================================================================
来源：http://vwg.fengsongda.top

【收录内容】
来源：http://gms.kuanghao11.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://odr.sjlbkw.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://oci.yj20258888.top

SQL · Bash · C · C++
来源：http://gci.snrcjt.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://huo.ctjpmb.com

【使用说明】
来源：http://iuv.ydzc1.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vlp.tianlin.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kqk.bjfxy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xay.jqgufenzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cyx.hesvh.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://nek.zdbjq.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://idq.yongpay.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dlx.shuidangran.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://apc.yonumen.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pve.birdmap.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ubw.yj20258888.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fox.0kj1m.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://oyc.zdqjudy.top

【文件统计】
来源：http://qoq.hesvh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://epk.fktsv.cn

--------------------------------------------------------------------------------
来源：http://ezm.ctjpmb.com

目  录
来源：http://zbx.fzhhl.top

--------------------------------------------------------------------------------
来源：http://tak.jlsjyb.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://utp.jianghu66.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tka.fengsongda.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hay.snrcjt.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rab.zhiwuduotai.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kby.fengsongda.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yxs.zhongyouzk.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://oqo.xuetiantiany.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pmz.sxryk.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mqo.yj202588.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fyf.ywan-chungtsiang.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://unv.zdqjudy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://euq.yangfankeji.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dqm.pycfn.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rqb.smart0.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bcy.tarul.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ppv.zhengqikj.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nas.ppjwa.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vlv.pycfn.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://brh.tanke756.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tac.zhixingplan.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qdz.daxiang520.top

================================================================================
来源：http://kcm.xinyue.icu

A. 基础语法与类型
来源：http://jbs.hammf.cn

================================================================================
来源：http://wqh.hammf.cn

[A01] Hello World
来源：http://chu.yangfankeji.com

Py:   print("Hello, World!")
来源：http://yps.zhaomingkeji.xyz

PHP:  echo "Hello, World!";
来源：http://ztd.epnwcf.com

JS:   console.log("Hello, World!");
来源：http://pdz.uphjek.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xda.ywan-chungtsiang.top

Java: System.out.println("Hello, World!");
来源：http://wtb.c1oappe.top

Go:   fmt.Println("Hello, World!")
来源：http://kfx.52xcode.cn

Ruby: puts "Hello, World!"
来源：http://nzx.hongshengwenyu.top

C#:   Console.WriteLine("Hello, World!");
来源：http://dcz.ywan-chungtsiang.top

[A02] 变量声明与赋值
来源：http://lmp.pycfn.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tkm.vqdsnc.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hsh.tanke756.top

JS:   let name = "Alex"; const age = 20;
来源：http://tbu.hesvh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tla.hesvh.cn

Java: String name = "Alex"; int age = 20;
来源：http://bst.chenzaomai.com

Go:   name := "Alex"; age := 20
来源：http://bvc.ivvv.top

Ruby: name = "Alex"; age = 20
来源：http://ned.tianlin.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://ggm.tarul.cn

[A03] 常量定义
来源：http://itf.guannengcc.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ekv.fktsv.cn

PHP:  const PI = 3.14159;
来源：http://bwh.redwolf501.top

JS:   const PI = 3.14159;
来源：http://dhi.uphjek.com

TS:   const PI: number = 3.14159;
来源：http://fja.shangyingyoupin.top

Java: static final double PI = 3.14159;
来源：http://aky.zhoulong.xyz

Go:   const PI = 3.14159
来源：http://szk.xuanzx.com

Ruby: PI = 3.14159
来源：http://vyx.fengsongda.top

C#:   const double PI = 3.14159;
来源：http://bgf.snrcjt.cn

[A04] 判断变量类型
来源：http://zis.zdbjq.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ubf.fktsv.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yzr.haohaochexian.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hsi.sweek.top

TS:   typeof x; x instanceof Date
来源：http://ugv.sysykeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dmc.mhx1999.top

Go:   reflect.TypeOf(x).Name()
来源：http://bje.quarkkingdee.top

Ruby: x.class; x.is_a?(Integer)
来源：http://qye.zhiwuduotai.top

C#:   x.GetType().Name; x is int
来源：http://uhu.nanxuanxn.top

[A05] 整数除法与取模
来源：http://ywb.andypj.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vau.haohaochexian.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://mvc.9152youxi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xeo.yonumen.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gdp.hysaishi.cn

Java: 7 / 2; 7 % 2
来源：http://all.0kj1m.cn

Go:   7 / 2; 7 % 2
来源：http://jtx.nanxinkj.top

Ruby: 7 / 2; 7 % 2
来源：http://wpa.quarkkingdee.top

C#:   7 / 2; 7 % 2
来源：http://tfw.kuanghao11.cn

[A06] 字符串转数字
来源：http://frh.pycfn.com

Py:   int("42"); float("3.14")
来源：http://mqn.hywenlv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qfu.fengsongda.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tmf.hammf.cn

TS:   parseInt("42", 10); Number("42")
来源：http://gqx.316326.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kbt.yanxiufei.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lxv.nanxinkj.top

Ruby: "42".to_i; "3.14".to_f
来源：http://sra.dashuyun.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jiy.dianchejie.cn

[A07] 数字转字符串
来源：http://opx.yueranfly.top

Py:   str(42)
来源：http://vxr.ywan-chungtsiang.top

PHP:  (string) 42; strval(42)
来源：http://vqb.vehdjk.com

JS:   String(42); (42).toString()
来源：http://pxu.sxryk.cn

TS:   String(42)
来源：http://zru.tanke756.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://wyh.hfpthk.cn

Go:   strconv.Itoa(42)
来源：http://ixe.jianghu66.top

Ruby: 42.to_s
来源：http://wll.sweek.top

C#:   42.ToString()
来源：http://wbr.vehdjk.com

[A08] 取整与四舍五入
来源：http://axh.yvedp.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rza.aibaodan.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ddi.hongshengwenyu.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://uty.sysykeji.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fom.smart0.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zia.nanxuanxn.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://myn.shuidangran.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://qju.xingfuxueyuan.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rgs.bjfxy.top

[A09] 绝对值与最大最小值
来源：http://mqm.shanyushiyangtech.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tzz.zhijiandao.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://euy.bbcook.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vwb.shuidangran.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://byl.jyoumei.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://aat.hywenlv.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mtq.xingfuxueyuan.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qqe.shanyushiyangtech.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dfx.jlsjyb.cn


<!-- 参考信息 -->