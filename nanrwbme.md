代发 wailian999

[U49] PHP：只读属性
来源：http://mmi.tian-w.cn

public readonly string $name
来源：http://ibe.fengsongda.top

[U50] PHP：构造器属性提升
来源：http://eit.yuxming.cn

public function __construct(private int $id) {}
来源：http://pfx.yonumen.top

[U51] PHP：数组解构
来源：http://gnn.tanke756.top

[$a, $b] = $arr;
来源：http://crt.guowangkeji.top

[U52] PHP：箭头函数
来源：http://sjs.xuanzx.com

$double = fn($x) => $x * 2;
来源：http://vdf.uphjek.com

[U53] PHP：空合并运算符
来源：http://mmf.yj202588.top

$v = $a ?? $b ?? "default";
来源：http://gwj.xylfe.cn

[U54] PHP：空安全调用
来源：http://vhj.zycfv.cn

$obj?->method()
来源：http://lwy.andypj.xyz

[U55] PHP：match 表达式
来源：http://csn.hongshengwenyu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iqf.ppjwa.cn

[U56] PHP：命名参数
来源：http://dpi.sweek.top

f(a: 1, b: 2)
来源：http://div.uphjek.com

[U57] PHP：字符串插值
来源：http://brx.fktsv.cn

"值: {$a}"
来源：http://vzh.fktsv.cn

[U58] PHP：数组三件套
来源：http://lpd.zhixingplan.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kax.xylfe.cn

[U59] PHP：自定义排序
来源：http://nox.9152youxi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xpp.sxryk.cn

[U60] PHP：JSON 编解码
来源：http://umi.fehbvm.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fsj.xziqi.cn

[U61] PHP：正则
来源：http://pvl.yongpay.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yxr.sxryk.cn

[U62] PHP：日期对象
来源：http://ixz.xuanzx.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xmz.pengpengdd.cyou

[U63] PHP：文件读写
来源：http://yyy.hfpthk.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ehg.yj20258888.top

[U64] PHP：目录遍历
来源：http://vtc.hcnkem.com

glob("dir/*.php");  scandir("dir");
来源：http://nae.shangyingyoupin.top

[U65] PHP：会话
来源：http://ezh.yuxming.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bcy.iojbl.cn

[U66] PHP：设置 Cookie
来源：http://pts.xuanzx.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ovp.ybcxt.top

[U67] PHP：处理文件上传
来源：http://exy.gotoacloud.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qid.uphjek.com

[U68] PHP：PDO 连接
来源：http://vww.fanxiaobao.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sum.chenjidiqi.icu

[U69] PHP：PDO 预处理
来源：http://kot.ivvv.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kme.kuanghao11.cn

[U70] PHP：PDO 事务
来源：http://zqy.jiagoushi.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dgc.ybcxt.top

[U71] PHP：抛出异常
来源：http://mis.yangfankeji.com

throw new RuntimeException("失败", 500);
来源：http://bxg.fanxiaobao.xyz

[U72] PHP：写错误日志
来源：http://awv.quarkkingdee.top

error_log("失败: " . $e->getMessage());
来源：http://wyq.yueranfly.top

[U73] PHP：读取 ini 配置
来源：http://vnm.316326.xyz

parse_ini_file("config.ini", true)
来源：http://hfy.xylfe.cn

[U74] PHP：读取环境变量
来源：http://qac.jinqigufen.top

getenv("APP_ENV") ?: "production"
来源：http://lws.svipenyu.cn

[U75] PHP：依赖注入
来源：http://ohw.iojbl.cn

composer require psr/container
来源：http://eri.wangdashe.top

[U76] PHP：简单路由
来源：http://nxc.jinghuilouyu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://iam.cheryme.top

[U77] PHP：模板渲染
来源：http://fct.hcnkem.com

composer require twig/twig
来源：http://bix.redwolf501.top

[U78] PHP：单元测试
来源：http://nik.yvedp.cn

composer require --dev phpunit/phpunit
来源：http://dwn.sxryk.cn

[U79] PHP：静态分析
来源：http://tkk.zhixingplan.top

composer require --dev phpstan/phpstan
来源：http://den.52xcode.cn

[U80] PHP：代码规范修复
来源：http://hnh.vqdsnc.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://duf.xinyue.icu

[U81] JS：初始化项目
来源：http://ulo.yonumen.top

npm init -y;  npm i express
来源：http://zks.quarkkingdee.top

[U82] JS：package.json 脚本
来源：http://qng.nanxinkj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://urn.hywenlv.cn

[U83] JS：ES Module 导入导出
来源：http://xur.chenjidiqi.icu

export const a = 1;  import { a } from "./m.js";
来源：http://knw.dashuyun.cn

[U84] JS：CommonJS 写法
来源：http://lqg.uphjek.com

module.exports = { a };  const { a } = require("./m");
来源：http://yhx.hongshengwenyu.top

[U85] JS：可选链
来源：http://yoh.xylfe.cn

a?.b?.c
来源：http://lzq.sweek.top

[U86] JS：空值合并
来源：http://ljx.cheryme.top

a ?? b
来源：http://qxn.zhijiandao.cn

[U87] JS：解构默认值
来源：http://hgm.fehbvm.com

const { a = 1, b = 2 } = obj;
来源：http://xzc.ctjpmb.com

[U88] JS：对象展开合并
来源：http://dyr.smart0.xyz

{ ...a, ...b }
来源：http://vys.fzhhl.top

[U89] JS：数组去重
来源：http://mxi.sweek.top

[...new Set(arr)]
来源：http://zoz.chenzaomai.com

[U90] JS：数字数组排序
来源：http://bqc.guowangkeji.top

[...arr].sort((a, b) => a - b)
来源：http://zza.yj202588.top

[U91] JS：对象键值遍历
来源：http://gqt.shanyushiyangtech.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rjh.jqgfzy.top

[U92] JS：深拷贝
来源：http://emo.smart0.xyz

structuredClone(obj)
来源：http://ksx.sxryk.cn

[U93] JS：模板字符串
来源：http://pfs.ctjpmb.com

`共 ${n} 条`
来源：http://muj.jyoumei.cn

[U94] JS：箭头函数
来源：http://riu.gaohongyu789.top

const double = x => x * 2;
来源：http://kdg.zhongyouzk.top

[U95] JS：Promise 包装
来源：http://jji.tanke756.top

new Promise((resolve, reject) => {})
来源：http://jlv.sufxvd.cn

[U96] JS：async/await 与异常
来源：http://ciu.epnwcf.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cde.gogol.net.cn

[U97] JS：并发请求
来源：http://cdu.jqgufenzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://lgy.svipenyu.cn

[U98] JS：fetch 带 JSON
来源：http://fum.sysykeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kkz.yj20258.top

[U99] JS：事件监听
来源：http://hvk.fanxiaobao.xyz

el.addEventListener("click", e => {})
来源：http://oww.zycfv.cn

[U100] JS：DOM 查询
来源：http://akd.yonumen.top

document.querySelector(".item")
来源：http://jre.chenzaomai.com

[U101] JS：classList 操作
来源：http://hhm.vqdsnc.cn

el.classList.toggle("active")
来源：http://dhe.52xcode.cn

[U102] JS：本地存储
来源：http://dzj.zdbjq.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jln.smart0.xyz

[U103] JS：定时器
来源：http://jri.ivvv.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sjv.316326.xyz

[U104] JS：防抖
来源：http://njd.jqgfzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tuv.wangshuangyany.cn

[U105] JS：节流
来源：http://cpr.nanxuanxn.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dvr.hnxiangtu.top

[U106] JS：日期格式化
来源：http://pcl.tanke756.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://omw.kuanghao11.cn

[U107] JS：数字千分位
来源：http://duk.cqqwz.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cde.feifeiyinyue.top

[U108] JS：随机整数
来源：http://ple.snrcjt.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ums.fehbvm.com

[U109] JS：数组分组
来源：http://ubf.cqqwz.cn

Object.groupBy(arr, x => x.type)
来源：http://epx.dianchejie.cn

[U110] JS：数组分块
来源：http://bsi.yj202588.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fyy.yuxming.cn

[U111] JS：对象转 Map
来源：http://vdo.yueranfly.top

new Map(Object.entries(obj))
来源：http://yzr.jyoumei.cn

[U112] JS：字符串补位
来源：http://tgr.nwbrower.top

"7".padStart(3, "0")
来源：http://ijg.hammf.cn

[U113] JS：正则替换全部
来源：http://ntw.fehbvm.com

s.replaceAll("a", "b")
来源：http://fgw.tarul.cn

[U114] JS：JSON 深比较
来源：http://qxp.cheryme.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://mku.havefunace.top

[U115] JS：生成 UUID
来源：http://iio.daxiang520.top

crypto.randomUUID()
来源：http://hsz.nanxuanxn.top

[U116] JS：类型检查（JSDoc）
来源：http://cdp.ctjpmb.com

/** @param {string} name */ function f(name) {}
来源：http://zff.nanxinkj.top

[U117] JS：单元测试
来源：http://cpv.jqgfzy.top

npm i -D vitest;  npx vitest
来源：http://uni.ppjwa.cn

[U118] JS：开发服务器
来源：http://whw.daxiang520.top

npm i -D vite;  npx vite
来源：http://czt.yj202588.top

[U119] JS：生产构建
来源：http://nja.gaohongyu789.top

npx vite build
来源：http://fyf.jyoumei.cn

[U120] JS：读取环境变量（Vite）
来源：http://oik.yuxming.cn

import.meta.env.VITE_API_URL
来源：http://ozi.zhijiandao.cn

================================================================================
来源：http://lxi.hcnkem.com

统计汇总
来源：http://mfw.yonumen.top

================================================================================
来源：http://tqm.jinyuanbaomall.cn

按语言统计（条）：
来源：http://nvg.vehdjk.com

Python ......... 252
来源：http://liz.cucudq.cn

PHP ............ 252
来源：http://ubt.yanxiufei.cn

JavaScript ..... 252
来源：http://mnz.gotoacloud.top

TypeScript ..... 212
来源：http://wun.zdbjq.cn

Java ........... 212
来源：http://grd.zhijiandao.cn

Go ............. 212
来源：http://tje.hammf.cn

Ruby ........... 212
来源：http://rbb.pycfn.com

C# ............. 212
来源：http://gqi.mhx1999.top

C .............. 30
来源：http://erl.fengsongda.top

C++ ............ 30
来源：http://fvr.gzhubu.top

SQL ............ 90
来源：http://uwi.zycfv.cn

Bash ........... 80
来源：http://pdb.chenlongwang.top

Kotlin ......... 15
来源：http://lci.zhixingplan.top

Swift .......... 15
来源：http://oji.iojbl.cn

Lua ............ 10
来源：http://ppl.epnwcf.com

Perl ........... 10
来源：http://ilo.nanxinkj.top

Scala .......... 10
来源：http://iux.chenlongwang.top

------------------------------------
来源：http://bdf.havefunace.top

合计 ........... 2106 条
来源：http://fbh.jiagoushi.top

按章节统计：
来源：http://sbd.cucudq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rfp.xylfe.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tkr.shzxlz.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lqb.sysykeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yem.jqgfzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qme.cucudq.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gmt.ivvv.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://shh.zycfv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gnn.zhixingplan.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zmw.meibo888.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bfk.nwbrower.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vvy.pycfn.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vuu.guannengcc.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nbw.cucudq.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ena.jlsjyb.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://aiu.nwbrower.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ovg.yonumen.top

Q SQL 专题                              90
来源：http://ipd.bbcook.cn

R Bash 专题                             80
来源：http://pob.feifeiyinyue.top

S C / C++ 专题                          60
来源：http://hau.52xcode.cn

T 其他语言补充                          60
来源：http://hpv.tianlin.xyz

U 高频实用片段                         120
来源：http://hxq.jyoumei.cn

------------------------------------
来源：http://oyh.sweek.top

合计                                  2106 条
来源：http://yzc.bbcook.cn

--------------------------------------------------------------------------------
来源：http://xck.zhengqikj.top

使用提醒
来源：http://hwx.birdmap.top

--------------------------------------------------------------------------------
来源：http://qxl.zhongyouzk.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rer.pycfn.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pyw.vehdjk.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zmf.jlsjyb.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gqw.jqgfzy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xjk.52xcode.cn

—— 文件结束 ——
来源：http://ppz.0kj1m.cn

================================================================================
来源：http://nia.yanxiufei.cn

程序语言常见例子速查手册（2024 版）
来源：http://qwa.jianghu66.top

Common Programming Examples Cheat Book
来源：http://jph.daria6918.cn

================================================================================
来源：http://nfn.yfazqb.com

【收录内容】
来源：http://tvi.zhoulong.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://nqx.xuetiantiany.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hai.nanxinkj.top

SQL · Bash · C · C++
来源：http://zpn.shanyushiyangtech.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://etk.sufxvd.cn

【使用说明】
来源：http://qnf.wangdashe.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kbr.cheryme.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wan.sxryk.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://asd.ydzc1.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hdo.yonumen.top

Bash:  Shell         C:     C             C++:   C++
来源：http://tba.hfpthk.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jox.yuanzhike.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kfz.nanxinkj.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yrn.tanke756.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zmv.yangfankeji.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uxi.cdnleiting.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dhn.haohaochexian.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ixt.jianghu66.top

【文件统计】
来源：http://oon.daxiang520.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kgs.sweek.top

--------------------------------------------------------------------------------
来源：http://cip.zhaomingkeji.xyz

目  录
来源：http://wis.c1oappe.top

--------------------------------------------------------------------------------
来源：http://yco.shzxlz.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nmx.yangfankeji.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://iqv.yj202588.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cmq.andypj.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://evr.sjlbkw.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qjq.dashuyun.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ztu.uphjek.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tbi.shuidangran.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mjx.sysykeji.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gfk.zycfv.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ppz.redwolf501.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kio.quarkkingdee.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://oan.ydzc1.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://say.ydzc1.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ybi.fzhhl.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rln.jinqigfzy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lif.zhongyouzk.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://slp.jyoumei.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://pbo.fktsv.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vjz.9152youxi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://waw.c1oappe.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://epq.smart0.xyz

================================================================================
来源：http://jim.hywenlv.cn

A. 基础语法与类型
来源：http://jws.ydzc1.top

================================================================================
来源：http://ifg.zhijiandao.cn

[A01] Hello World
来源：http://yzv.guowangkeji.top

Py:   print("Hello, World!")
来源：http://dbe.andypj.xyz

PHP:  echo "Hello, World!";
来源：http://kjs.gzhubu.top

JS:   console.log("Hello, World!");
来源：http://nex.tanke756.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://abq.uphjek.com

Java: System.out.println("Hello, World!");
来源：http://fjf.xylfe.cn

Go:   fmt.Println("Hello, World!")
来源：http://uqi.jqgufenzy.top

Ruby: puts "Hello, World!"
来源：http://zmr.svipenyu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://eux.jqgufenzy.top

[A02] 变量声明与赋值
来源：http://jdl.zhengqikj.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://glm.vehdjk.com

PHP:  $name = "Alex"; $age = 20;
来源：http://tvw.zhiwuduotai.top

JS:   let name = "Alex"; const age = 20;
来源：http://jdn.guannengcc.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xcz.9152youxi.cn

Java: String name = "Alex"; int age = 20;
来源：http://esr.yj20258.top

Go:   name := "Alex"; age := 20
来源：http://xix.aibaodan.cn

Ruby: name = "Alex"; age = 20
来源：http://zsy.sxryk.cn

C#:   string name = "Alex"; int age = 20;
来源：http://bkb.zhijiandao.cn

[A03] 常量定义
来源：http://rjv.jyoumei.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bwr.fktsv.cn

PHP:  const PI = 3.14159;
来源：http://buw.jiagoushi.top

JS:   const PI = 3.14159;
来源：http://dss.zhoulong.xyz

TS:   const PI: number = 3.14159;
来源：http://eqo.cqqwz.cn

Java: static final double PI = 3.14159;
来源：http://urb.kuanghao11.cn

Go:   const PI = 3.14159
来源：http://xgb.sjlbkw.cn

Ruby: PI = 3.14159
来源：http://ecs.vehdjk.com

C#:   const double PI = 3.14159;
来源：http://wmj.zhiwuduotai.top

[A04] 判断变量类型
来源：http://qyd.sweek.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://tzs.mhx1999.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vys.wangshuangyany.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cww.feifeiyinyue.top

TS:   typeof x; x instanceof Date
来源：http://owx.9152youxi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hwj.fzhhl.top

Go:   reflect.TypeOf(x).Name()
来源：http://etz.tianlin.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://fpd.yj202588.top

C#:   x.GetType().Name; x is int
来源：http://wjr.tian-w.cn

[A05] 整数除法与取模
来源：http://gyd.dashuyun.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://aio.ctjpmb.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://udw.xinyue.icu

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zqk.xylfe.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jya.xuanzx.com

Java: 7 / 2; 7 % 2
来源：http://jqz.yuxming.cn

Go:   7 / 2; 7 % 2
来源：http://rmr.daria6918.cn

Ruby: 7 / 2; 7 % 2
来源：http://wvx.jlsjyb.cn

C#:   7 / 2; 7 % 2
来源：http://vcw.feifeiyinyue.top

[A06] 字符串转数字
来源：http://ska.cheryme.top

Py:   int("42"); float("3.14")
来源：http://phw.zycfv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jwh.daxiang520.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ugt.cdnleiting.top


<!-- 参考信息 -->