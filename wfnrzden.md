代发 wailian999

[U55] PHP：match 表达式
来源：http://abe.hesvh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://trs.52xcode.cn

[U56] PHP：命名参数
来源：http://ekl.fktsv.cn

f(a: 1, b: 2)
来源：http://pyp.ydzc1.top

[U57] PHP：字符串插值
来源：http://uzn.yj20258888.top

"值: {$a}"
来源：http://qrs.sjlbkw.cn

[U58] PHP：数组三件套
来源：http://lss.gotoacloud.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ozd.xingfuxueyuan.xyz

[U59] PHP：自定义排序
来源：http://ufc.dianchejie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jlg.shangyingyoupin.top

[U60] PHP：JSON 编解码
来源：http://zge.yongpay.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zdp.gaohongyu789.top

[U61] PHP：正则
来源：http://nxi.daxiang520.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://oci.ywan-chungtsiang.top

[U62] PHP：日期对象
来源：http://ock.shzxlz.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://poc.tarul.cn

[U63] PHP：文件读写
来源：http://rcd.gaohongyu789.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://akt.zdqjudy.top

[U64] PHP：目录遍历
来源：http://jxk.9152youxi.cn

glob("dir/*.php");  scandir("dir");
来源：http://ark.nanxinkj.top

[U65] PHP：会话
来源：http://huv.316326.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://gpc.sufxvd.cn

[U66] PHP：设置 Cookie
来源：http://zzk.gaohongyu789.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jxa.chenlongwang.top

[U67] PHP：处理文件上传
来源：http://btx.zhaomingkeji.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rvl.hnqzz.top

[U68] PHP：PDO 连接
来源：http://wzq.xinyue.icu

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://osh.jinqigufen.top

[U69] PHP：PDO 预处理
来源：http://dca.daria6918.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vbp.fktsv.cn

[U70] PHP：PDO 事务
来源：http://xxp.dashuyun.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kup.shanyushiyangtech.top

[U71] PHP：抛出异常
来源：http://zug.chenzaomai.com

throw new RuntimeException("失败", 500);
来源：http://soh.haohaochexian.top

[U72] PHP：写错误日志
来源：http://vkm.jinqigufen.top

error_log("失败: " . $e->getMessage());
来源：http://rdw.hywenlv.cn

[U73] PHP：读取 ini 配置
来源：http://tel.zdqjudy.top

parse_ini_file("config.ini", true)
来源：http://gzz.shuidangran.top

[U74] PHP：读取环境变量
来源：http://zvn.jinyuanbaomall.cn

getenv("APP_ENV") ?: "production"
来源：http://skg.yj20258888.top

[U75] PHP：依赖注入
来源：http://dbl.jinqigfzy.top

composer require psr/container
来源：http://pma.ybcxt.top

[U76] PHP：简单路由
来源：http://ukr.cqqwz.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yep.bjfxy.top

[U77] PHP：模板渲染
来源：http://ukt.zhoulong.xyz

composer require twig/twig
来源：http://qfl.xuanzx.com

[U78] PHP：单元测试
来源：http://whf.yvedp.cn

composer require --dev phpunit/phpunit
来源：http://naw.sjlbkw.cn

[U79] PHP：静态分析
来源：http://rfc.pengpengdd.cyou

composer require --dev phpstan/phpstan
来源：http://qfa.yj20258888.top

[U80] PHP：代码规范修复
来源：http://npn.gzhubu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://yjw.yj20258888.top

[U81] JS：初始化项目
来源：http://odu.52xcode.cn

npm init -y;  npm i express
来源：http://kqf.wangdashe.top

[U82] JS：package.json 脚本
来源：http://hxt.shzxlz.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pdn.sweek.top

[U83] JS：ES Module 导入导出
来源：http://fia.epnwcf.com

export const a = 1;  import { a } from "./m.js";
来源：http://kpl.bjfxy.top

[U84] JS：CommonJS 写法
来源：http://nbp.nwbrower.top

module.exports = { a };  const { a } = require("./m");
来源：http://lma.jinqigufen.top

[U85] JS：可选链
来源：http://anl.xuanzx.com

a?.b?.c
来源：http://vol.smart0.xyz

[U86] JS：空值合并
来源：http://sho.ehwqpu.com

a ?? b
来源：http://dqr.fktsv.cn

[U87] JS：解构默认值
来源：http://ane.ywan-chungtsiang.top

const { a = 1, b = 2 } = obj;
来源：http://ofu.meibo888.top

[U88] JS：对象展开合并
来源：http://nvj.mhx1999.top

{ ...a, ...b }
来源：http://pxp.hnxiangtu.top

[U89] JS：数组去重
来源：http://jtf.yvedp.cn

[...new Set(arr)]
来源：http://fxx.nwbrower.top

[U90] JS：数字数组排序
来源：http://jsw.guannengcc.top

[...arr].sort((a, b) => a - b)
来源：http://oaq.sxryk.cn

[U91] JS：对象键值遍历
来源：http://hhr.hysaishi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mil.fktsv.cn

[U92] JS：深拷贝
来源：http://qpr.fehbvm.com

structuredClone(obj)
来源：http://zaw.havefunace.top

[U93] JS：模板字符串
来源：http://jxf.c1oappe.top

`共 ${n} 条`
来源：http://vpo.nanxinkj.top

[U94] JS：箭头函数
来源：http://jda.xuanzx.com

const double = x => x * 2;
来源：http://pco.aizwys.cn

[U95] JS：Promise 包装
来源：http://qyd.ivvv.top

new Promise((resolve, reject) => {})
来源：http://xjg.zdbjq.cn

[U96] JS：async/await 与异常
来源：http://giq.yangfankeji.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mkb.xingfuxueyuan.xyz

[U97] JS：并发请求
来源：http://axt.xinyue.icu

await Promise.all(urls.map(u => fetch(u)))
来源：http://byk.haohaochexian.top

[U98] JS：fetch 带 JSON
来源：http://xoy.yuxming.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://etm.fktsv.cn

[U99] JS：事件监听
来源：http://nsm.smart0.xyz

el.addEventListener("click", e => {})
来源：http://eij.vehdjk.com

[U100] JS：DOM 查询
来源：http://ndv.svipenyu.cn

document.querySelector(".item")
来源：http://rfu.yj202588.top

[U101] JS：classList 操作
来源：http://vpq.sxryk.cn

el.classList.toggle("active")
来源：http://grz.hnxiangtu.top

[U102] JS：本地存储
来源：http://wrd.dianchejie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://yma.xuetiantiany.cn

[U103] JS：定时器
来源：http://nmv.haohaochexian.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wzp.9152youxi.cn

[U104] JS：防抖
来源：http://fyz.hammf.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cpe.redwolf501.top

[U105] JS：节流
来源：http://iqe.ehwqpu.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uwo.shzxlz.cn

[U106] JS：日期格式化
来源：http://btj.yuanzhike.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wjf.yonumen.top

[U107] JS：数字千分位
来源：http://pfe.jinqigfzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wll.ppjwa.cn

[U108] JS：随机整数
来源：http://xil.hongshengwenyu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://csg.hnxiangtu.top

[U109] JS：数组分组
来源：http://auh.zdqjudy.top

Object.groupBy(arr, x => x.type)
来源：http://ouw.snrcjt.cn

[U110] JS：数组分块
来源：http://qeo.316326.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fcz.vqdsnc.cn

[U111] JS：对象转 Map
来源：http://mhm.yonumen.top

new Map(Object.entries(obj))
来源：http://pbw.zdqjudy.top

[U112] JS：字符串补位
来源：http://oec.tian-w.cn

"7".padStart(3, "0")
来源：http://hkk.zycfv.cn

[U113] JS：正则替换全部
来源：http://tkf.haohaochexian.top

s.replaceAll("a", "b")
来源：http://wkn.cashguo.top

[U114] JS：JSON 深比较
来源：http://bvl.hfpthk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nax.jqgufenzy.top

[U115] JS：生成 UUID
来源：http://dtn.shanyushiyangtech.top

crypto.randomUUID()
来源：http://psb.jqgfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://wkj.wangshuangyany.cn

/** @param {string} name */ function f(name) {}
来源：http://eqi.xinyue.icu

[U117] JS：单元测试
来源：http://fwr.zhongyouzk.top

npm i -D vitest;  npx vitest
来源：http://jrh.haohaochexian.top

[U118] JS：开发服务器
来源：http://vhu.fzhhl.top

npm i -D vite;  npx vite
来源：http://mqt.zhongyouzk.top

[U119] JS：生产构建
来源：http://xmb.sxryk.cn

npx vite build
来源：http://cqj.yj20258.top

[U120] JS：读取环境变量（Vite）
来源：http://vld.yj202588.top

import.meta.env.VITE_API_URL
来源：http://dlf.yangfankeji.com

================================================================================
来源：http://ebf.andypj.xyz

统计汇总
来源：http://ugb.smart0.xyz

================================================================================
来源：http://zee.iojbl.cn

按语言统计（条）：
来源：http://kmo.jinghuilouyu.cn

Python ......... 252
来源：http://uis.andypj.xyz

PHP ............ 252
来源：http://pkn.wangshuangyany.cn

JavaScript ..... 252
来源：http://vbh.9152youxi.cn

TypeScript ..... 212
来源：http://chi.9152youxi.cn

Java ........... 212
来源：http://vou.zhijiandao.cn

Go ............. 212
来源：http://bbm.bjfxy.top

Ruby ........... 212
来源：http://cud.shangyingyoupin.top

C# ............. 212
来源：http://ljw.wangdashe.top

C .............. 30
来源：http://qhd.zhoulong.xyz

C++ ............ 30
来源：http://mmt.chenzaomai.com

SQL ............ 90
来源：http://tqf.jiagoushi.top

Bash ........... 80
来源：http://gbr.fanxiaobao.xyz

Kotlin ......... 15
来源：http://suf.epnwcf.com

Swift .......... 15
来源：http://tjo.hesvh.cn

Lua ............ 10
来源：http://vpv.birdmap.top

Perl ........... 10
来源：http://dua.tanke756.top

Scala .......... 10
来源：http://sky.ydzc1.top

------------------------------------
来源：http://iqs.9152youxi.cn

合计 ........... 2106 条
来源：http://wet.nwbrower.top

按章节统计：
来源：http://yje.xziqi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zck.mhx1999.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://eoa.mhx1999.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hia.guowangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://eqi.redwolf501.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zuh.ydzc1.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hgc.hfpthk.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hwe.uphjek.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://abt.yangfankeji.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://iwg.zhongyouzk.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mus.gzhubu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rwf.c1oappe.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qox.jqgufenzy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://noq.nanxinkj.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bmm.birdmap.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wkj.jqgfzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nuc.shanyushiyangkeji.top

Q SQL 专题                              90
来源：http://jkx.wangshuangyany.cn

R Bash 专题                             80
来源：http://osp.fzhhl.top

S C / C++ 专题                          60
来源：http://rnh.tian-w.cn

T 其他语言补充                          60
来源：http://wtn.52xcode.cn

U 高频实用片段                         120
来源：http://heb.hysaishi.cn

------------------------------------
来源：http://kbo.zdbjq.cn

合计                                  2106 条
来源：http://xeu.smart0.xyz

--------------------------------------------------------------------------------
来源：http://ypl.iojbl.cn

使用提醒
来源：http://lrn.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://qsl.hcnkem.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rro.vqdsnc.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tkc.mhx1999.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tro.cqqwz.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gtr.ydjk.org.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ehq.bbcook.cn

—— 文件结束 ——
来源：http://wyw.uphjek.com

================================================================================
来源：http://ckt.jinqigfzy.top

程序语言常见例子速查手册（2024 版）
来源：http://bro.feifeiyinyue.top

Common Programming Examples Cheat Book
来源：http://aax.ivvv.top

================================================================================
来源：http://eyc.guannengcc.top

【收录内容】
来源：http://duo.uphjek.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://clm.aibaodan.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://geh.xinyue.icu

SQL · Bash · C · C++
来源：http://gtn.nwbrower.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bte.zhiwuduotai.top

【使用说明】
来源：http://hyv.hongshengwenyu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pjb.cdnleiting.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://eei.vqdsnc.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ewl.jyoumei.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kxs.cashguo.top

Bash:  Shell         C:     C             C++:   C++
来源：http://rak.meibo888.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jpc.ehwqpu.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yas.hywenlv.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pvl.vqdsnc.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yaa.hysaishi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sug.epnwcf.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qck.ctjpmb.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xph.fktsv.cn

【文件统计】
来源：http://uga.nanxuanxn.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://are.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://tjy.redwolf501.top

目  录
来源：http://foy.jianghu66.top

--------------------------------------------------------------------------------
来源：http://lgz.hcnkem.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://oix.ydzc1.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hww.xuanzx.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qku.hammf.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ofu.yj20258888.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zjo.jiagoushi.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dff.fzhhl.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rfu.dianchejie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bbd.feifeiyinyue.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yra.dashuyun.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lbg.yonumen.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fge.chenjidiqi.icu

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ger.cucudq.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://oah.yfazqb.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://eqm.bjfxy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hld.ydjk.org.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://oxb.jlsjyb.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://eos.cqqwz.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tvc.jinqigfzy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nuc.jianghu66.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ywb.guowangkeji.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rzs.zdbjq.cn

================================================================================
来源：http://mex.birdmap.top

A. 基础语法与类型
来源：http://vju.andypj.xyz

================================================================================
来源：http://awi.52xcode.cn

[A01] Hello World
来源：http://wri.hesvh.cn

Py:   print("Hello, World!")
来源：http://vkh.pengpengdd.cyou

PHP:  echo "Hello, World!";
来源：http://jog.ydzc1.top

JS:   console.log("Hello, World!");
来源：http://sdy.havefunace.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rje.cheryme.top

Java: System.out.println("Hello, World!");
来源：http://vnj.zhoulong.xyz

Go:   fmt.Println("Hello, World!")
来源：http://qwx.hnqzz.top

Ruby: puts "Hello, World!"
来源：http://dnq.zdqjudy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://scq.zhiwuduotai.top

[A02] 变量声明与赋值
来源：http://ugo.yonumen.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://sgj.cheryme.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ykg.gaohongyu789.top

JS:   let name = "Alex"; const age = 20;
来源：http://srz.fzhhl.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://iec.yueranfly.top

Java: String name = "Alex"; int age = 20;
来源：http://rjn.xylfe.cn

Go:   name := "Alex"; age := 20
来源：http://rux.vehdjk.com

Ruby: name = "Alex"; age = 20
来源：http://uzy.yj202588.top

C#:   string name = "Alex"; int age = 20;
来源：http://ydo.nanxinkj.top

[A03] 常量定义
来源：http://dea.daria6918.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zjr.jqgufenzy.top

PHP:  const PI = 3.14159;
来源：http://ehc.ivvv.top

JS:   const PI = 3.14159;
来源：http://lww.jinqigufen.top

TS:   const PI: number = 3.14159;
来源：http://myf.hywenlv.cn

Java: static final double PI = 3.14159;
来源：http://rty.yongpay.top

Go:   const PI = 3.14159
来源：http://hau.aibaodan.cn

Ruby: PI = 3.14159
来源：http://trk.hfpthk.cn

C#:   const double PI = 3.14159;
来源：http://zzu.0kj1m.cn

[A04] 判断变量类型
来源：http://zrz.guowangkeji.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://mxf.jinqigufen.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ipo.hysaishi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vlu.yongpay.top

TS:   typeof x; x instanceof Date
来源：http://yri.ehwqpu.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zeg.hongshengwenyu.top

Go:   reflect.TypeOf(x).Name()
来源：http://iea.snrcjt.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wbd.snrcjt.cn

C#:   x.GetType().Name; x is int
来源：http://qeq.kuanghao11.cn

[A05] 整数除法与取模
来源：http://ylz.shanyushiyangkeji.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xgz.svipenyu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://uct.dianchejie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bjn.yj20258.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dsu.ctjpmb.com

Java: 7 / 2; 7 % 2
来源：http://gcm.yj20258.top

Go:   7 / 2; 7 % 2
来源：http://jli.jinyuanbaomall.cn

Ruby: 7 / 2; 7 % 2
来源：http://sbn.zdqjudy.top

C#:   7 / 2; 7 % 2
来源：http://ieo.zhengqikj.top

[A06] 字符串转数字
来源：http://gjc.svipenyu.cn

Py:   int("42"); float("3.14")
来源：http://eui.zycfv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fvn.chenjidiqi.icu

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gmq.nwbrower.top

TS:   parseInt("42", 10); Number("42")
来源：http://jgx.ehwqpu.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lij.zhoulong.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://oil.yfazqb.com

Ruby: "42".to_i; "3.14".to_f
来源：http://kyz.ivvv.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jdz.dianchejie.cn

[A07] 数字转字符串
来源：http://kpw.ppjwa.cn

Py:   str(42)
来源：http://xmr.zycfv.cn

PHP:  (string) 42; strval(42)
来源：http://erc.nanxinkj.top

JS:   String(42); (42).toString()
来源：http://zeq.smart0.xyz

TS:   String(42)
来源：http://acb.havefunace.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://cyn.hcnkem.com

Go:   strconv.Itoa(42)
来源：http://umb.chenlongwang.top


<!-- 参考信息 -->