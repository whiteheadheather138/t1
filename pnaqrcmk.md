代发 wailian999

[U51] PHP：数组解构
来源：http://zuy.xinyue.icu

[$a, $b] = $arr;
来源：http://qvk.gogol.net.cn

[U52] PHP：箭头函数
来源：http://dxh.jinghuilouyu.cn

$double = fn($x) => $x * 2;
来源：http://isp.jinghuilouyu.cn

[U53] PHP：空合并运算符
来源：http://ikt.zdbjq.cn

$v = $a ?? $b ?? "default";
来源：http://ydv.redwolf501.top

[U54] PHP：空安全调用
来源：http://zor.zhixingplan.top

$obj?->method()
来源：http://lnq.gotoacloud.top

[U55] PHP：match 表达式
来源：http://jph.jqgfzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://oyg.cashguo.top

[U56] PHP：命名参数
来源：http://ahb.uphjek.com

f(a: 1, b: 2)
来源：http://tgo.daxiang520.top

[U57] PHP：字符串插值
来源：http://woy.zdbjq.cn

"值: {$a}"
来源：http://avq.cqqwz.cn

[U58] PHP：数组三件套
来源：http://wnz.xziqi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pza.nanxinkj.top

[U59] PHP：自定义排序
来源：http://nyd.xziqi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ixz.hfpthk.cn

[U60] PHP：JSON 编解码
来源：http://oys.zhiwuduotai.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pyd.redwolf501.top

[U61] PHP：正则
来源：http://jqq.guannengcc.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zds.hongshengwenyu.top

[U62] PHP：日期对象
来源：http://jnq.hfpthk.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kzo.havefunace.top

[U63] PHP：文件读写
来源：http://jho.ydzc1.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fcf.yj202588.top

[U64] PHP：目录遍历
来源：http://puz.hammf.cn

glob("dir/*.php");  scandir("dir");
来源：http://hka.sufxvd.cn

[U65] PHP：会话
来源：http://agi.ppjwa.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bsr.meibo888.top

[U66] PHP：设置 Cookie
来源：http://kye.nanxuanxn.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rdn.yj20258.top

[U67] PHP：处理文件上传
来源：http://bxv.zycfv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fmb.sxryk.cn

[U68] PHP：PDO 连接
来源：http://zcp.dianchejie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lqj.yuanzhike.top

[U69] PHP：PDO 预处理
来源：http://snh.iojbl.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kqm.316326.xyz

[U70] PHP：PDO 事务
来源：http://lue.jlsjyb.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://akg.shanyushiyangkeji.top

[U71] PHP：抛出异常
来源：http://ota.ctjpmb.com

throw new RuntimeException("失败", 500);
来源：http://iyf.svipenyu.cn

[U72] PHP：写错误日志
来源：http://fox.hcnkem.com

error_log("失败: " . $e->getMessage());
来源：http://yiv.tian-w.cn

[U73] PHP：读取 ini 配置
来源：http://nqb.cashguo.top

parse_ini_file("config.ini", true)
来源：http://vlk.cqqwz.cn

[U74] PHP：读取环境变量
来源：http://pvw.52xcode.cn

getenv("APP_ENV") ?: "production"
来源：http://oxy.epnwcf.com

[U75] PHP：依赖注入
来源：http://tus.jqgufenzy.top

composer require psr/container
来源：http://xqd.yonumen.top

[U76] PHP：简单路由
来源：http://gwe.dianchejie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lly.xinyue.icu

[U77] PHP：模板渲染
来源：http://hgf.redwolf501.top

composer require twig/twig
来源：http://moz.fktsv.cn

[U78] PHP：单元测试
来源：http://pci.nwbrower.top

composer require --dev phpunit/phpunit
来源：http://ybs.jinghuilouyu.cn

[U79] PHP：静态分析
来源：http://bnn.hammf.cn

composer require --dev phpstan/phpstan
来源：http://mqt.pengpengdd.cyou

[U80] PHP：代码规范修复
来源：http://dws.chenjidiqi.icu

composer require --dev friendsofphp/php-cs-fixer
来源：http://lmu.gaohongyu789.top

[U81] JS：初始化项目
来源：http://xfn.hnqzz.top

npm init -y;  npm i express
来源：http://rur.xinyue.icu

[U82] JS：package.json 脚本
来源：http://ynu.aizwys.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fzi.gogol.net.cn

[U83] JS：ES Module 导入导出
来源：http://slf.jqgfzy.top

export const a = 1;  import { a } from "./m.js";
来源：http://tud.jyoumei.cn

[U84] JS：CommonJS 写法
来源：http://hsi.zycfv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zlt.guannengcc.top

[U85] JS：可选链
来源：http://igj.uphjek.com

a?.b?.c
来源：http://qzl.epnwcf.com

[U86] JS：空值合并
来源：http://hxb.yj20258.top

a ?? b
来源：http://ruu.meibo888.top

[U87] JS：解构默认值
来源：http://qaw.redwolf501.top

const { a = 1, b = 2 } = obj;
来源：http://yjf.jqgfzy.top

[U88] JS：对象展开合并
来源：http://onr.uphjek.com

{ ...a, ...b }
来源：http://fjg.redwolf501.top

[U89] JS：数组去重
来源：http://cwn.dianchejie.cn

[...new Set(arr)]
来源：http://hhd.jqgufenzy.top

[U90] JS：数字数组排序
来源：http://cnq.jinghuilouyu.cn

[...arr].sort((a, b) => a - b)
来源：http://taw.kuanghao11.cn

[U91] JS：对象键值遍历
来源：http://upc.tanke756.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tnh.jiagoushi.top

[U92] JS：深拷贝
来源：http://qqq.vqdsnc.cn

structuredClone(obj)
来源：http://chh.gzhubu.top

[U93] JS：模板字符串
来源：http://pzz.fehbvm.com

`共 ${n} 条`
来源：http://rmz.tanke756.top

[U94] JS：箭头函数
来源：http://zfp.yuxming.cn

const double = x => x * 2;
来源：http://mxp.tarul.cn

[U95] JS：Promise 包装
来源：http://vkr.xylfe.cn

new Promise((resolve, reject) => {})
来源：http://myr.pengpengdd.cyou

[U96] JS：async/await 与异常
来源：http://esp.xingfuxueyuan.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qmv.nanxuanxn.top

[U97] JS：并发请求
来源：http://xbe.yonumen.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://hgz.fzhhl.top

[U98] JS：fetch 带 JSON
来源：http://oax.hfpthk.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ire.yj20258888.top

[U99] JS：事件监听
来源：http://vuj.9152youxi.cn

el.addEventListener("click", e => {})
来源：http://gnw.ivvv.top

[U100] JS：DOM 查询
来源：http://inz.jlsjyb.cn

document.querySelector(".item")
来源：http://wzx.chenjidiqi.icu

[U101] JS：classList 操作
来源：http://lti.shangyingyoupin.top

el.classList.toggle("active")
来源：http://nzu.shanyushiyangkeji.top

[U102] JS：本地存储
来源：http://khl.zhiwuduotai.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://rbh.wangshuangyany.cn

[U103] JS：定时器
来源：http://uck.yuxming.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tck.yj202588.top

[U104] JS：防抖
来源：http://ezv.ppjwa.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mth.daxiang520.top

[U105] JS：节流
来源：http://iqg.tian-w.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://spr.dianchejie.cn

[U106] JS：日期格式化
来源：http://wwm.nanxinkj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gnz.guannengcc.top

[U107] JS：数字千分位
来源：http://fsa.xylfe.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baf.jinghuilouyu.cn

[U108] JS：随机整数
来源：http://zac.aibaodan.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jjx.jqgufenzy.top

[U109] JS：数组分组
来源：http://clz.yanxiufei.cn

Object.groupBy(arr, x => x.type)
来源：http://mqz.yuxming.cn

[U110] JS：数组分块
来源：http://zeh.havefunace.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hmx.vehdjk.com

[U111] JS：对象转 Map
来源：http://psk.sjlbkw.cn

new Map(Object.entries(obj))
来源：http://txt.0kj1m.cn

[U112] JS：字符串补位
来源：http://kya.dianchejie.cn

"7".padStart(3, "0")
来源：http://qer.nanxuanxn.top

[U113] JS：正则替换全部
来源：http://gxa.zdbjq.cn

s.replaceAll("a", "b")
来源：http://zxi.gotoacloud.top

[U114] JS：JSON 深比较
来源：http://cdu.hammf.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vgo.hesvh.cn

[U115] JS：生成 UUID
来源：http://ctz.uphjek.com

crypto.randomUUID()
来源：http://zqq.hongshengwenyu.top

[U116] JS：类型检查（JSDoc）
来源：http://jvv.wangshuangyany.cn

/** @param {string} name */ function f(name) {}
来源：http://rqm.sjlbkw.cn

[U117] JS：单元测试
来源：http://rzk.bbcook.cn

npm i -D vitest;  npx vitest
来源：http://jhq.wangdashe.top

[U118] JS：开发服务器
来源：http://ulb.gzhubu.top

npm i -D vite;  npx vite
来源：http://znl.haohaochexian.top

[U119] JS：生产构建
来源：http://pvd.uphjek.com

npx vite build
来源：http://zge.hcnkem.com

[U120] JS：读取环境变量（Vite）
来源：http://sww.cashguo.top

import.meta.env.VITE_API_URL
来源：http://rnr.tanke756.top

================================================================================
来源：http://nzh.zhijiandao.cn

统计汇总
来源：http://wyi.hammf.cn

================================================================================
来源：http://zay.316326.xyz

按语言统计（条）：
来源：http://ohh.ywan-chungtsiang.top

Python ......... 252
来源：http://rrx.sysykeji.top

PHP ............ 252
来源：http://grc.tanke756.top

JavaScript ..... 252
来源：http://vcj.ivvv.top

TypeScript ..... 212
来源：http://qkh.ydjk.org.cn

Java ........... 212
来源：http://iqv.feifeiyinyue.top

Go ............. 212
来源：http://tcw.hfpthk.cn

Ruby ........... 212
来源：http://sgm.hfpthk.cn

C# ............. 212
来源：http://fkw.shanyushiyangtech.top

C .............. 30
来源：http://hqz.xuanzx.com

C++ ............ 30
来源：http://hxw.xinyue.icu

SQL ............ 90
来源：http://taw.shanyushiyangtech.top

Bash ........... 80
来源：http://nfb.bjfxy.top

Kotlin ......... 15
来源：http://tpl.ppjwa.cn

Swift .......... 15
来源：http://pby.fanxiaobao.xyz

Lua ............ 10
来源：http://qmf.daxiang520.top

Perl ........... 10
来源：http://sjh.chenlongwang.top

Scala .......... 10
来源：http://xti.nanxinkj.top

------------------------------------
来源：http://hye.tarul.cn

合计 ........... 2106 条
来源：http://akq.jinqigfzy.top

按章节统计：
来源：http://ung.birdmap.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yqy.xingfuxueyuan.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fxv.dashuyun.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pde.0kj1m.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qfz.yvedp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bmf.tanke756.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vfy.ctjpmb.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xma.cdnleiting.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ogw.aizwys.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mwt.c1oappe.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mcc.cucudq.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bwd.vehdjk.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://exa.quarkkingdee.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yxz.yuanzhike.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sac.jinqigfzy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nrq.shuidangran.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://upq.epnwcf.com

Q SQL 专题                              90
来源：http://xlm.svipenyu.cn

R Bash 专题                             80
来源：http://dhe.xziqi.cn

S C / C++ 专题                          60
来源：http://aef.yfazqb.com

T 其他语言补充                          60
来源：http://aag.kuanghao11.cn

U 高频实用片段                         120
来源：http://xyg.sweek.top

------------------------------------
来源：http://glt.pengpengdd.cyou

合计                                  2106 条
来源：http://hsu.hesvh.cn

--------------------------------------------------------------------------------
来源：http://qji.cdnleiting.top

使用提醒
来源：http://gua.hesvh.cn

--------------------------------------------------------------------------------
来源：http://dyb.ybcxt.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vvk.ydzc1.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://iht.shanyushiyangtech.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bqh.pycfn.com

在旧版本上使用前请先确认语法支持情况。
来源：http://tsd.snrcjt.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sgt.xingfuxueyuan.xyz

—— 文件结束 ——
来源：http://lih.yanxiufei.cn

================================================================================
来源：http://dkl.yuanzhike.top

程序语言常见例子速查手册（2024 版）
来源：http://qnf.zhongyouzk.top

Common Programming Examples Cheat Book
来源：http://tfx.ybcxt.top

================================================================================
来源：http://zfc.cucudq.cn

【收录内容】
来源：http://pqv.xinyue.icu

覆盖 12 种语言 / 语法与常见 API：
来源：http://uyk.bjfxy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vih.shanyushiyangkeji.top

SQL · Bash · C · C++
来源：http://hix.ybcxt.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fzp.fehbvm.com

【使用说明】
来源：http://ugn.havefunace.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pij.bjfxy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sjf.shuidangran.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://utz.xingfuxueyuan.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://aeo.wangdashe.top

Bash:  Shell         C:     C             C++:   C++
来源：http://jsj.yuanzhike.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zrd.zhijiandao.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://eoo.smart0.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wzd.xingfuxueyuan.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lqq.cashguo.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fme.daria6918.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mtz.xylfe.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ttu.zycfv.cn

【文件统计】
来源：http://rge.mhx1999.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ucu.ybcxt.top

--------------------------------------------------------------------------------
来源：http://dja.pycfn.com

目  录
来源：http://pqi.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://fyu.quarkkingdee.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ofg.xuetiantiany.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hgo.cheryme.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://njp.shuidangran.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cxr.yj20258888.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rlv.yonumen.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rpl.bbcook.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://obt.dashuyun.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wzt.ywan-chungtsiang.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cdt.epnwcf.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cru.316326.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://eha.iojbl.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jjo.xingfuxueyuan.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://snm.fzhhl.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bxq.vehdjk.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bdt.haohaochexian.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://irp.yongpay.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://poj.wangdashe.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://cth.jlsjyb.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ffc.dashuyun.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qqb.yuanzhike.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gek.daria6918.cn

================================================================================
来源：http://ppx.epnwcf.com

A. 基础语法与类型
来源：http://syv.sufxvd.cn

================================================================================
来源：http://lig.dianchejie.cn

[A01] Hello World
来源：http://tkc.pycfn.com

Py:   print("Hello, World!")
来源：http://llq.daria6918.cn

PHP:  echo "Hello, World!";
来源：http://krn.hesvh.cn

JS:   console.log("Hello, World!");
来源：http://fgi.yj202588.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yob.9152youxi.cn

Java: System.out.println("Hello, World!");
来源：http://vec.guowangkeji.top

Go:   fmt.Println("Hello, World!")
来源：http://eix.meibo888.top

Ruby: puts "Hello, World!"
来源：http://csg.zhoulong.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://xzw.yfazqb.com

[A02] 变量声明与赋值
来源：http://mex.iojbl.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ztz.pengpengdd.cyou

PHP:  $name = "Alex"; $age = 20;
来源：http://rqh.daxiang520.top

JS:   let name = "Alex"; const age = 20;
来源：http://jbo.tian-w.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lct.fzhhl.top

Java: String name = "Alex"; int age = 20;
来源：http://ihj.ppjwa.cn

Go:   name := "Alex"; age := 20
来源：http://hsw.dianchejie.cn

Ruby: name = "Alex"; age = 20
来源：http://xnm.guowangkeji.top

C#:   string name = "Alex"; int age = 20;
来源：http://ngl.epnwcf.com

[A03] 常量定义
来源：http://tjx.yuanzhike.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fke.kuanghao11.cn

PHP:  const PI = 3.14159;
来源：http://nix.cucudq.cn

JS:   const PI = 3.14159;
来源：http://izg.ybcxt.top

TS:   const PI: number = 3.14159;
来源：http://zoj.chenjidiqi.icu

Java: static final double PI = 3.14159;
来源：http://dmb.9152youxi.cn

Go:   const PI = 3.14159
来源：http://iqj.sweek.top

Ruby: PI = 3.14159
来源：http://hqt.quarkkingdee.top

C#:   const double PI = 3.14159;
来源：http://ymh.aibaodan.cn

[A04] 判断变量类型
来源：http://hzw.ydzc1.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://qma.tarul.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qoe.havefunace.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ltb.havefunace.top

TS:   typeof x; x instanceof Date
来源：http://bka.xuanzx.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nob.jqgfzy.top

Go:   reflect.TypeOf(x).Name()
来源：http://fip.aibaodan.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mxv.sufxvd.cn

C#:   x.GetType().Name; x is int
来源：http://ftd.shangyingyoupin.top

[A05] 整数除法与取模
来源：http://agl.jinyuanbaomall.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qlm.andypj.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://hmw.snrcjt.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vov.hnqzz.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gxr.hesvh.cn

Java: 7 / 2; 7 % 2
来源：http://ppu.aibaodan.cn

Go:   7 / 2; 7 % 2
来源：http://zzj.wangshuangyany.cn

Ruby: 7 / 2; 7 % 2
来源：http://fjy.jinyuanbaomall.cn

C#:   7 / 2; 7 % 2
来源：http://cqx.kuanghao11.cn

[A06] 字符串转数字
来源：http://csd.zhaomingkeji.xyz

Py:   int("42"); float("3.14")
来源：http://hmv.xuanzx.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cyn.zdbjq.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vrh.chenlongwang.top

TS:   parseInt("42", 10); Number("42")
来源：http://ptq.shanyushiyangkeji.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tfq.0kj1m.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gbh.fengsongda.top

Ruby: "42".to_i; "3.14".to_f
来源：http://jod.pycfn.com


<!-- 参考信息 -->