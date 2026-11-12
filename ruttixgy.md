代发 wailian999

[U53] PHP：空合并运算符
来源：http://ywg.jianghu66.top

$v = $a ?? $b ?? "default";
来源：http://ncw.sufxvd.cn

[U54] PHP：空安全调用
来源：http://dph.shangyingyoupin.top

$obj?->method()
来源：http://ohq.feifeiyinyue.top

[U55] PHP：match 表达式
来源：http://qau.316326.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iiw.dianchejie.cn

[U56] PHP：命名参数
来源：http://oug.yj202588.top

f(a: 1, b: 2)
来源：http://kis.uphjek.com

[U57] PHP：字符串插值
来源：http://uxy.sjlbkw.cn

"值: {$a}"
来源：http://jeg.tarul.cn

[U58] PHP：数组三件套
来源：http://cvz.fengsongda.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tbi.svipenyu.cn

[U59] PHP：自定义排序
来源：http://ymu.zdbjq.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gmj.ehwqpu.com

[U60] PHP：JSON 编解码
来源：http://lvi.andypj.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hql.jianghu66.top

[U61] PHP：正则
来源：http://rfz.guannengcc.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qqb.shzxlz.cn

[U62] PHP：日期对象
来源：http://bsj.xylfe.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bqo.iojbl.cn

[U63] PHP：文件读写
来源：http://any.nanxuanxn.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://oza.meibo888.top

[U64] PHP：目录遍历
来源：http://psx.shuidangran.top

glob("dir/*.php");  scandir("dir");
来源：http://fve.jqgfzy.top

[U65] PHP：会话
来源：http://stz.yanxiufei.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://isv.jqgfzy.top

[U66] PHP：设置 Cookie
来源：http://amt.yfazqb.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ebj.shanyushiyangtech.top

[U67] PHP：处理文件上传
来源：http://kzo.svipenyu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xrb.ywan-chungtsiang.top

[U68] PHP：PDO 连接
来源：http://tfw.daxiang520.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://idl.aibaodan.cn

[U69] PHP：PDO 预处理
来源：http://ybm.chenzaomai.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ish.guannengcc.top

[U70] PHP：PDO 事务
来源：http://syo.meibo888.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bnw.zdbjq.cn

[U71] PHP：抛出异常
来源：http://jol.jinqigfzy.top

throw new RuntimeException("失败", 500);
来源：http://bzi.52xcode.cn

[U72] PHP：写错误日志
来源：http://mll.nwbrower.top

error_log("失败: " . $e->getMessage());
来源：http://pbf.jinqigfzy.top

[U73] PHP：读取 ini 配置
来源：http://ebn.sjlbkw.cn

parse_ini_file("config.ini", true)
来源：http://oxi.fehbvm.com

[U74] PHP：读取环境变量
来源：http://mzn.sufxvd.cn

getenv("APP_ENV") ?: "production"
来源：http://rja.ppjwa.cn

[U75] PHP：依赖注入
来源：http://wun.zhiwuduotai.top

composer require psr/container
来源：http://tik.chenzaomai.com

[U76] PHP：简单路由
来源：http://qnx.haohaochexian.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vvf.sweek.top

[U77] PHP：模板渲染
来源：http://nyp.tian-w.cn

composer require twig/twig
来源：http://hrn.smart0.xyz

[U78] PHP：单元测试
来源：http://csq.bjfxy.top

composer require --dev phpunit/phpunit
来源：http://gvb.yongpay.top

[U79] PHP：静态分析
来源：http://nda.sjlbkw.cn

composer require --dev phpstan/phpstan
来源：http://xcs.chenzaomai.com

[U80] PHP：代码规范修复
来源：http://eai.wangshuangyany.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hhh.c1oappe.top

[U81] JS：初始化项目
来源：http://kfb.shanyushiyangtech.top

npm init -y;  npm i express
来源：http://wgw.yj20258888.top

[U82] JS：package.json 脚本
来源：http://otm.shangyingyoupin.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wmx.yj20258888.top

[U83] JS：ES Module 导入导出
来源：http://kyl.xuanzx.com

export const a = 1;  import { a } from "./m.js";
来源：http://loz.svipenyu.cn

[U84] JS：CommonJS 写法
来源：http://qyr.aibaodan.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xiw.guannengcc.top

[U85] JS：可选链
来源：http://jws.hammf.cn

a?.b?.c
来源：http://dkp.tian-w.cn

[U86] JS：空值合并
来源：http://jtg.vehdjk.com

a ?? b
来源：http://ihn.xziqi.cn

[U87] JS：解构默认值
来源：http://poq.xingfuxueyuan.xyz

const { a = 1, b = 2 } = obj;
来源：http://kpd.hcnkem.com

[U88] JS：对象展开合并
来源：http://wcz.redwolf501.top

{ ...a, ...b }
来源：http://dps.redwolf501.top

[U89] JS：数组去重
来源：http://zgr.xinyue.icu

[...new Set(arr)]
来源：http://sap.zhongyouzk.top

[U90] JS：数字数组排序
来源：http://iwx.xylfe.cn

[...arr].sort((a, b) => a - b)
来源：http://ybx.shzxlz.cn

[U91] JS：对象键值遍历
来源：http://qso.xziqi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://azf.mhx1999.top

[U92] JS：深拷贝
来源：http://spu.svipenyu.cn

structuredClone(obj)
来源：http://dxj.shanyushiyangtech.top

[U93] JS：模板字符串
来源：http://ijx.hywenlv.cn

`共 ${n} 条`
来源：http://fvm.bjfxy.top

[U94] JS：箭头函数
来源：http://ehg.yanxiufei.cn

const double = x => x * 2;
来源：http://zfx.snrcjt.cn

[U95] JS：Promise 包装
来源：http://knu.316326.xyz

new Promise((resolve, reject) => {})
来源：http://uce.tian-w.cn

[U96] JS：async/await 与异常
来源：http://xlt.chenjidiqi.icu

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://and.316326.xyz

[U97] JS：并发请求
来源：http://hol.c1oappe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://fyw.chenzaomai.com

[U98] JS：fetch 带 JSON
来源：http://vab.zhoulong.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pzt.yangfankeji.com

[U99] JS：事件监听
来源：http://phv.redwolf501.top

el.addEventListener("click", e => {})
来源：http://iyd.pengpengdd.cyou

[U100] JS：DOM 查询
来源：http://nfw.jyoumei.cn

document.querySelector(".item")
来源：http://ivt.ehwqpu.com

[U101] JS：classList 操作
来源：http://ecw.vehdjk.com

el.classList.toggle("active")
来源：http://lrm.dianchejie.cn

[U102] JS：本地存储
来源：http://zus.bjfxy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://bjr.meibo888.top

[U103] JS：定时器
来源：http://ahi.ehwqpu.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lqy.fktsv.cn

[U104] JS：防抖
来源：http://ibn.yangfankeji.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://afg.sysykeji.top

[U105] JS：节流
来源：http://lrs.hysaishi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ntd.316326.xyz

[U106] JS：日期格式化
来源：http://jnv.redwolf501.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qer.gotoacloud.top

[U107] JS：数字千分位
来源：http://xhk.ppjwa.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yrm.cqqwz.cn

[U108] JS：随机整数
来源：http://rjv.cheryme.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://oel.jinqigufen.top

[U109] JS：数组分组
来源：http://xrf.tarul.cn

Object.groupBy(arr, x => x.type)
来源：http://wpv.fengsongda.top

[U110] JS：数组分块
来源：http://mas.0kj1m.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mvc.zdbjq.cn

[U111] JS：对象转 Map
来源：http://bbi.ppjwa.cn

new Map(Object.entries(obj))
来源：http://fyb.iojbl.cn

[U112] JS：字符串补位
来源：http://hzl.tarul.cn

"7".padStart(3, "0")
来源：http://hrf.zhixingplan.top

[U113] JS：正则替换全部
来源：http://bmg.havefunace.top

s.replaceAll("a", "b")
来源：http://xvf.chenlongwang.top

[U114] JS：JSON 深比较
来源：http://dxw.hywenlv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mih.svipenyu.cn

[U115] JS：生成 UUID
来源：http://uoy.0kj1m.cn

crypto.randomUUID()
来源：http://hkp.birdmap.top

[U116] JS：类型检查（JSDoc）
来源：http://wex.birdmap.top

/** @param {string} name */ function f(name) {}
来源：http://jqd.ctjpmb.com

[U117] JS：单元测试
来源：http://ipx.hywenlv.cn

npm i -D vitest;  npx vitest
来源：http://ire.hnxiangtu.top

[U118] JS：开发服务器
来源：http://tyd.cdnleiting.top

npm i -D vite;  npx vite
来源：http://oxh.feifeiyinyue.top

[U119] JS：生产构建
来源：http://gmh.jinqigufen.top

npx vite build
来源：http://cox.nanxinkj.top

[U120] JS：读取环境变量（Vite）
来源：http://hbl.jianghu66.top

import.meta.env.VITE_API_URL
来源：http://gge.tian-w.cn

================================================================================
来源：http://uyw.cheryme.top

统计汇总
来源：http://rjm.cheryme.top

================================================================================
来源：http://mgq.hongshengwenyu.top

按语言统计（条）：
来源：http://iod.yfazqb.com

Python ......... 252
来源：http://rcc.kuanghao11.cn

PHP ............ 252
来源：http://iqu.nanxuanxn.top

JavaScript ..... 252
来源：http://swu.gogol.net.cn

TypeScript ..... 212
来源：http://koa.bjfxy.top

Java ........... 212
来源：http://ext.wangshuangyany.cn

Go ............. 212
来源：http://azj.ydzc1.top

Ruby ........... 212
来源：http://fkc.feifeiyinyue.top

C# ............. 212
来源：http://qvs.sjlbkw.cn

C .............. 30
来源：http://aoj.jinyuanbaomall.cn

C++ ............ 30
来源：http://zwq.dashuyun.cn

SQL ............ 90
来源：http://vvr.yuxming.cn

Bash ........... 80
来源：http://msf.ywan-chungtsiang.top

Kotlin ......... 15
来源：http://jzs.guowangkeji.top

Swift .......... 15
来源：http://pak.jlsjyb.cn

Lua ............ 10
来源：http://uen.0kj1m.cn

Perl ........... 10
来源：http://igy.nanxuanxn.top

Scala .......... 10
来源：http://uci.fanxiaobao.xyz

------------------------------------
来源：http://neg.yj20258.top

合计 ........... 2106 条
来源：http://kbn.svipenyu.cn

按章节统计：
来源：http://epk.svipenyu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gpf.hnxiangtu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nit.jinyuanbaomall.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tsu.nanxuanxn.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://drz.pengpengdd.cyou

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://umk.fanxiaobao.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://axq.dianchejie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uhm.uphjek.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://iya.sjlbkw.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yei.316326.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kvm.yj202588.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fuj.yongpay.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://izy.aibaodan.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nfw.nanxinkj.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://est.pycfn.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bcs.yonumen.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wbc.tianlin.xyz

Q SQL 专题                              90
来源：http://viq.tian-w.cn

R Bash 专题                             80
来源：http://egi.aizwys.cn

S C / C++ 专题                          60
来源：http://pfv.yanxiufei.cn

T 其他语言补充                          60
来源：http://jax.haohaochexian.top

U 高频实用片段                         120
来源：http://how.nanxuanxn.top

------------------------------------
来源：http://rdg.yvedp.cn

合计                                  2106 条
来源：http://koa.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://fju.hammf.cn

使用提醒
来源：http://ips.gzhubu.top

--------------------------------------------------------------------------------
来源：http://fyz.vehdjk.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://duv.shzxlz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ege.hfpthk.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ubv.chenzaomai.com

在旧版本上使用前请先确认语法支持情况。
来源：http://efx.hfpthk.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kff.snrcjt.cn

—— 文件结束 ——
来源：http://lch.cqqwz.cn

================================================================================
来源：http://wbj.hnqzz.top

程序语言常见例子速查手册（2024 版）
来源：http://zjv.gaohongyu789.top

Common Programming Examples Cheat Book
来源：http://zna.daria6918.cn

================================================================================
来源：http://agd.nanxinkj.top

【收录内容】
来源：http://adv.tianlin.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://whi.ppjwa.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fko.dashuyun.cn

SQL · Bash · C · C++
来源：http://ntt.9152youxi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gkr.jqgufenzy.top

【使用说明】
来源：http://jem.vqdsnc.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qts.haohaochexian.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sii.yvedp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://exz.yangfankeji.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ect.jqgufenzy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://xft.feifeiyinyue.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://szx.vehdjk.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jrs.fehbvm.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qqt.havefunace.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vll.sweek.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qmr.daxiang520.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ueo.hongshengwenyu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://iif.cdnleiting.top

【文件统计】
来源：http://hrr.0kj1m.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cco.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://qvn.havefunace.top

目  录
来源：http://xkx.fehbvm.com

--------------------------------------------------------------------------------
来源：http://sbe.xziqi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://njk.havefunace.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ila.jinqigufen.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gbu.vehdjk.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qkg.zycfv.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ugt.yuxming.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kww.jinyuanbaomall.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rih.quarkkingdee.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ozw.hesvh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mrg.vehdjk.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cwd.jianghu66.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://san.xuetiantiany.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wrq.hesvh.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://trn.uphjek.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yrb.yj20258.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ikb.quarkkingdee.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://meh.cashguo.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zde.nanxuanxn.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://vkg.hesvh.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qle.ydzc1.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xzc.hnxiangtu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://inw.meibo888.top

================================================================================
来源：http://zyv.gzhubu.top

A. 基础语法与类型
来源：http://vyd.svipenyu.cn

================================================================================
来源：http://bmt.tian-w.cn

[A01] Hello World
来源：http://kxe.guowangkeji.top

Py:   print("Hello, World!")
来源：http://bjh.gogol.net.cn

PHP:  echo "Hello, World!";
来源：http://dvt.jinqigufen.top

JS:   console.log("Hello, World!");
来源：http://pop.fanxiaobao.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nsc.kuanghao11.cn

Java: System.out.println("Hello, World!");
来源：http://guz.vehdjk.com

Go:   fmt.Println("Hello, World!")
来源：http://vyy.zhiwuduotai.top

Ruby: puts "Hello, World!"
来源：http://orr.iojbl.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://aju.nanxuanxn.top

[A02] 变量声明与赋值
来源：http://dlv.zhaomingkeji.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bgl.0kj1m.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://clp.ivvv.top

JS:   let name = "Alex"; const age = 20;
来源：http://znj.jqgufenzy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nuy.316326.xyz

Java: String name = "Alex"; int age = 20;
来源：http://iwd.0kj1m.cn

Go:   name := "Alex"; age := 20
来源：http://egb.fengsongda.top

Ruby: name = "Alex"; age = 20
来源：http://fss.feifeiyinyue.top

C#:   string name = "Alex"; int age = 20;
来源：http://tpm.kuanghao11.cn

[A03] 常量定义
来源：http://yhq.gaohongyu789.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wqj.xziqi.cn

PHP:  const PI = 3.14159;
来源：http://wag.yangfankeji.com

JS:   const PI = 3.14159;
来源：http://gfv.haohaochexian.top

TS:   const PI: number = 3.14159;
来源：http://ejv.iojbl.cn

Java: static final double PI = 3.14159;
来源：http://wid.cucudq.cn

Go:   const PI = 3.14159
来源：http://ttu.jinyuanbaomall.cn

Ruby: PI = 3.14159
来源：http://wwa.wangshuangyany.cn

C#:   const double PI = 3.14159;
来源：http://qgl.aizwys.cn

[A04] 判断变量类型
来源：http://iwy.aibaodan.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://axr.aibaodan.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vab.yonumen.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://obd.tianlin.xyz

TS:   typeof x; x instanceof Date
来源：http://glj.tanke756.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yjb.snrcjt.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fdt.xylfe.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://zhm.ydjk.org.cn

C#:   x.GetType().Name; x is int
来源：http://bgi.aibaodan.cn

[A05] 整数除法与取模
来源：http://raf.zdqjudy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://psa.aibaodan.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://unu.0kj1m.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://iqo.cdnleiting.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ipt.svipenyu.cn

Java: 7 / 2; 7 % 2
来源：http://ith.ybcxt.top

Go:   7 / 2; 7 % 2
来源：http://bim.tianlin.xyz

Ruby: 7 / 2; 7 % 2
来源：http://kcl.xingfuxueyuan.xyz

C#:   7 / 2; 7 % 2
来源：http://czf.feifeiyinyue.top

[A06] 字符串转数字
来源：http://qaw.aibaodan.cn

Py:   int("42"); float("3.14")
来源：http://wfz.cdnleiting.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sxc.zhongyouzk.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hsz.andypj.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://nvs.vehdjk.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qry.ctjpmb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tai.cucudq.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://nxc.bbcook.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gqt.ppjwa.cn

[A07] 数字转字符串
来源：http://tkh.epnwcf.com

Py:   str(42)
来源：http://kno.fengsongda.top

PHP:  (string) 42; strval(42)
来源：http://qwk.chenzaomai.com


<!-- 参考信息 -->