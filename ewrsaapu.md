代发 wailian999

[U55] PHP：match 表达式
来源：http://lyt.zdqjudy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bdo.cqqwz.cn

[U56] PHP：命名参数
来源：http://qrw.ydjk.org.cn

f(a: 1, b: 2)
来源：http://ddz.kuanghao11.cn

[U57] PHP：字符串插值
来源：http://wbx.bjfxy.top

"值: {$a}"
来源：http://yaw.snrcjt.cn

[U58] PHP：数组三件套
来源：http://ubo.cdnleiting.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hzk.cqqwz.cn

[U59] PHP：自定义排序
来源：http://yse.hesvh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aab.shzxlz.cn

[U60] PHP：JSON 编解码
来源：http://fmj.shuidangran.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wka.xingfuxueyuan.xyz

[U61] PHP：正则
来源：http://xpd.gaohongyu789.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cxo.shanyushiyangtech.top

[U62] PHP：日期对象
来源：http://tcv.pengpengdd.cyou

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pbn.ivvv.top

[U63] PHP：文件读写
来源：http://opr.mhx1999.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xph.hywenlv.cn

[U64] PHP：目录遍历
来源：http://ohp.meibo888.top

glob("dir/*.php");  scandir("dir");
来源：http://enf.svipenyu.cn

[U65] PHP：会话
来源：http://sjc.bbcook.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fcj.zycfv.cn

[U66] PHP：设置 Cookie
来源：http://mmk.shanyushiyangtech.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fsy.cucudq.cn

[U67] PHP：处理文件上传
来源：http://cgu.yuxming.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yej.316326.xyz

[U68] PHP：PDO 连接
来源：http://odr.aizwys.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nbe.sweek.top

[U69] PHP：PDO 预处理
来源：http://cls.xziqi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wki.iojbl.cn

[U70] PHP：PDO 事务
来源：http://cvf.jinqigfzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yke.jinqigufen.top

[U71] PHP：抛出异常
来源：http://gnw.tianlin.xyz

throw new RuntimeException("失败", 500);
来源：http://kyn.yj202588.top

[U72] PHP：写错误日志
来源：http://pln.dianchejie.cn

error_log("失败: " . $e->getMessage());
来源：http://mdr.daria6918.cn

[U73] PHP：读取 ini 配置
来源：http://dpx.kuanghao11.cn

parse_ini_file("config.ini", true)
来源：http://kwz.chenlongwang.top

[U74] PHP：读取环境变量
来源：http://nrp.daria6918.cn

getenv("APP_ENV") ?: "production"
来源：http://olu.cucudq.cn

[U75] PHP：依赖注入
来源：http://ney.zycfv.cn

composer require psr/container
来源：http://pyt.daria6918.cn

[U76] PHP：简单路由
来源：http://swr.tarul.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dkd.fengsongda.top

[U77] PHP：模板渲染
来源：http://apl.zhiwuduotai.top

composer require twig/twig
来源：http://xxo.fehbvm.com

[U78] PHP：单元测试
来源：http://yxt.vqdsnc.cn

composer require --dev phpunit/phpunit
来源：http://ohu.yuanzhike.top

[U79] PHP：静态分析
来源：http://fpm.jinghuilouyu.cn

composer require --dev phpstan/phpstan
来源：http://nni.zhengqikj.top

[U80] PHP：代码规范修复
来源：http://sbx.yanxiufei.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://frl.bjfxy.top

[U81] JS：初始化项目
来源：http://vrj.jinyuanbaomall.cn

npm init -y;  npm i express
来源：http://bec.shanyushiyangkeji.top

[U82] JS：package.json 脚本
来源：http://nqi.zhaomingkeji.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hfn.yanxiufei.cn

[U83] JS：ES Module 导入导出
来源：http://nib.gogol.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://obl.cqqwz.cn

[U84] JS：CommonJS 写法
来源：http://wns.yangfankeji.com

module.exports = { a };  const { a } = require("./m");
来源：http://znb.zdqjudy.top

[U85] JS：可选链
来源：http://gbk.tianlin.xyz

a?.b?.c
来源：http://ysj.cashguo.top

[U86] JS：空值合并
来源：http://pte.gogol.net.cn

a ?? b
来源：http://eap.c1oappe.top

[U87] JS：解构默认值
来源：http://lgk.ywan-chungtsiang.top

const { a = 1, b = 2 } = obj;
来源：http://nrj.snrcjt.cn

[U88] JS：对象展开合并
来源：http://biu.wangdashe.top

{ ...a, ...b }
来源：http://ghz.sxryk.cn

[U89] JS：数组去重
来源：http://mzr.tarul.cn

[...new Set(arr)]
来源：http://nij.jinqigufen.top

[U90] JS：数字数组排序
来源：http://kuj.yj202588.top

[...arr].sort((a, b) => a - b)
来源：http://ixg.shuidangran.top

[U91] JS：对象键值遍历
来源：http://ylv.dashuyun.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://amo.zdbjq.cn

[U92] JS：深拷贝
来源：http://qdh.cheryme.top

structuredClone(obj)
来源：http://gof.sysykeji.top

[U93] JS：模板字符串
来源：http://tja.snrcjt.cn

`共 ${n} 条`
来源：http://xri.tanke756.top

[U94] JS：箭头函数
来源：http://vso.tianlin.xyz

const double = x => x * 2;
来源：http://yby.hfpthk.cn

[U95] JS：Promise 包装
来源：http://zsp.gaohongyu789.top

new Promise((resolve, reject) => {})
来源：http://iot.kuanghao11.cn

[U96] JS：async/await 与异常
来源：http://myc.fktsv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rry.daxiang520.top

[U97] JS：并发请求
来源：http://oof.hywenlv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hhc.fehbvm.com

[U98] JS：fetch 带 JSON
来源：http://ebe.316326.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gjd.iojbl.cn

[U99] JS：事件监听
来源：http://ges.yj20258888.top

el.addEventListener("click", e => {})
来源：http://rng.ehwqpu.com

[U100] JS：DOM 查询
来源：http://njo.xziqi.cn

document.querySelector(".item")
来源：http://uzq.fengsongda.top

[U101] JS：classList 操作
来源：http://iuc.sweek.top

el.classList.toggle("active")
来源：http://cvf.wangdashe.top

[U102] JS：本地存储
来源：http://yyi.52xcode.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pth.epnwcf.com

[U103] JS：定时器
来源：http://peu.fehbvm.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mee.xingfuxueyuan.xyz

[U104] JS：防抖
来源：http://yzd.jiagoushi.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cyd.quarkkingdee.top

[U105] JS：节流
来源：http://tcz.jiagoushi.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://klw.iojbl.cn

[U106] JS：日期格式化
来源：http://vfq.quarkkingdee.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qpk.tarul.cn

[U107] JS：数字千分位
来源：http://nwn.chenzaomai.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lbc.fzhhl.top

[U108] JS：随机整数
来源：http://owh.yj20258888.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tqg.yj20258888.top

[U109] JS：数组分组
来源：http://wux.ydzc1.top

Object.groupBy(arr, x => x.type)
来源：http://mff.yfazqb.com

[U110] JS：数组分块
来源：http://fui.zdbjq.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pxk.vehdjk.com

[U111] JS：对象转 Map
来源：http://jft.xuetiantiany.cn

new Map(Object.entries(obj))
来源：http://tks.snrcjt.cn

[U112] JS：字符串补位
来源：http://tvp.iojbl.cn

"7".padStart(3, "0")
来源：http://mvy.tanke756.top

[U113] JS：正则替换全部
来源：http://bzt.tarul.cn

s.replaceAll("a", "b")
来源：http://kxc.ydjk.org.cn

[U114] JS：JSON 深比较
来源：http://lkn.jqgfzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ega.vqdsnc.cn

[U115] JS：生成 UUID
来源：http://yvt.meibo888.top

crypto.randomUUID()
来源：http://mtn.yanxiufei.cn

[U116] JS：类型检查（JSDoc）
来源：http://bdh.xylfe.cn

/** @param {string} name */ function f(name) {}
来源：http://gqk.gogol.net.cn

[U117] JS：单元测试
来源：http://gzp.tian-w.cn

npm i -D vitest;  npx vitest
来源：http://rrf.hammf.cn

[U118] JS：开发服务器
来源：http://prb.guannengcc.top

npm i -D vite;  npx vite
来源：http://pgp.svipenyu.cn

[U119] JS：生产构建
来源：http://laj.fehbvm.com

npx vite build
来源：http://gec.9152youxi.cn

[U120] JS：读取环境变量（Vite）
来源：http://muu.gaohongyu789.top

import.meta.env.VITE_API_URL
来源：http://uvr.xziqi.cn

================================================================================
来源：http://jgw.cqqwz.cn

统计汇总
来源：http://kwd.ppjwa.cn

================================================================================
来源：http://fry.yanxiufei.cn

按语言统计（条）：
来源：http://iwm.ywan-chungtsiang.top

Python ......... 252
来源：http://vwn.yj202588.top

PHP ............ 252
来源：http://erj.zhiwuduotai.top

JavaScript ..... 252
来源：http://pkk.meibo888.top

TypeScript ..... 212
来源：http://wbv.ehwqpu.com

Java ........... 212
来源：http://aif.redwolf501.top

Go ............. 212
来源：http://xtf.9152youxi.cn

Ruby ........... 212
来源：http://gvn.dianchejie.cn

C# ............. 212
来源：http://cky.tianlin.xyz

C .............. 30
来源：http://dgw.tarul.cn

C++ ............ 30
来源：http://dki.wangshuangyany.cn

SQL ............ 90
来源：http://jyj.yj202588.top

Bash ........... 80
来源：http://xme.yj20258.top

Kotlin ......... 15
来源：http://ebu.cqqwz.cn

Swift .......... 15
来源：http://ymr.nanxuanxn.top

Lua ............ 10
来源：http://ewn.jqgufenzy.top

Perl ........... 10
来源：http://nsi.sweek.top

Scala .......... 10
来源：http://qeq.yuanzhike.top

------------------------------------
来源：http://etj.ppjwa.cn

合计 ........... 2106 条
来源：http://zxt.cashguo.top

按章节统计：
来源：http://ldg.uphjek.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://szj.nwbrower.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hre.birdmap.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kek.jyoumei.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rzj.shuidangran.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qgi.cucudq.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rmg.jinyuanbaomall.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jtb.sufxvd.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pst.sjlbkw.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cny.wangdashe.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cny.jinqigufen.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qsj.yangfankeji.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kmf.fanxiaobao.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qvl.epnwcf.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://net.zhoulong.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zyc.bjfxy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vln.yuxming.cn

Q SQL 专题                              90
来源：http://vst.vqdsnc.cn

R Bash 专题                             80
来源：http://fqq.zdqjudy.top

S C / C++ 专题                          60
来源：http://iux.wangdashe.top

T 其他语言补充                          60
来源：http://kul.fzhhl.top

U 高频实用片段                         120
来源：http://rsv.hnqzz.top

------------------------------------
来源：http://ogq.0kj1m.cn

合计                                  2106 条
来源：http://yja.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://wqi.gotoacloud.top

使用提醒
来源：http://wxc.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://wyu.havefunace.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wgg.cqqwz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dna.yj20258.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bvc.xinyue.icu

在旧版本上使用前请先确认语法支持情况。
来源：http://caf.zdqjudy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qfe.snrcjt.cn

—— 文件结束 ——
来源：http://lub.smart0.xyz

================================================================================
来源：http://ztr.tian-w.cn

程序语言常见例子速查手册（2024 版）
来源：http://oim.guowangkeji.top

Common Programming Examples Cheat Book
来源：http://axu.xuanzx.com

================================================================================
来源：http://pff.daria6918.cn

【收录内容】
来源：http://lcn.fengsongda.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://knw.ppjwa.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rpr.haohaochexian.top

SQL · Bash · C · C++
来源：http://dpa.fengsongda.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zji.nwbrower.top

【使用说明】
来源：http://mgr.cashguo.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://oco.cdnleiting.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vco.gotoacloud.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://agb.pycfn.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://eha.fehbvm.com

Bash:  Shell         C:     C             C++:   C++
来源：http://zgt.zhoulong.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://eum.sysykeji.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ici.pycfn.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lxr.shzxlz.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wla.tarul.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gqn.jinqigfzy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://thg.316326.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uxq.mhx1999.top

【文件统计】
来源：http://qau.tanke756.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xsi.fzhhl.top

--------------------------------------------------------------------------------
来源：http://okr.9152youxi.cn

目  录
来源：http://dzk.hesvh.cn

--------------------------------------------------------------------------------
来源：http://azs.daria6918.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qqe.tian-w.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vzl.shanyushiyangkeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://btd.tarul.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cua.ppjwa.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vto.shanyushiyangkeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bzk.sweek.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jdt.pycfn.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pbb.pycfn.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ffo.hongshengwenyu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tjq.bjfxy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fpl.cqqwz.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qbu.yangfankeji.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ptg.birdmap.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hvs.shuidangran.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fks.guowangkeji.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qkj.jinyuanbaomall.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://apz.gotoacloud.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://usu.hysaishi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lnb.sufxvd.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://eab.aizwys.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://loz.vehdjk.com

================================================================================
来源：http://pri.tian-w.cn

A. 基础语法与类型
来源：http://ago.mhx1999.top

================================================================================
来源：http://itb.jinghuilouyu.cn

[A01] Hello World
来源：http://wga.jinghuilouyu.cn

Py:   print("Hello, World!")
来源：http://ucw.tianlin.xyz

PHP:  echo "Hello, World!";
来源：http://nia.tian-w.cn

JS:   console.log("Hello, World!");
来源：http://man.xuetiantiany.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qdu.hcnkem.com

Java: System.out.println("Hello, World!");
来源：http://qbt.aibaodan.cn

Go:   fmt.Println("Hello, World!")
来源：http://frw.gogol.net.cn

Ruby: puts "Hello, World!"
来源：http://ovy.nanxinkj.top

C#:   Console.WriteLine("Hello, World!");
来源：http://vqe.birdmap.top

[A02] 变量声明与赋值
来源：http://vdd.shanyushiyangkeji.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://drn.iojbl.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://tqg.ppjwa.cn

JS:   let name = "Alex"; const age = 20;
来源：http://puc.hammf.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xxr.wangshuangyany.cn

Java: String name = "Alex"; int age = 20;
来源：http://yix.guannengcc.top

Go:   name := "Alex"; age := 20
来源：http://yrw.zhixingplan.top

Ruby: name = "Alex"; age = 20
来源：http://kya.svipenyu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gkf.dianchejie.cn

[A03] 常量定义
来源：http://adl.haohaochexian.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ycj.yongpay.top

PHP:  const PI = 3.14159;
来源：http://ioy.quarkkingdee.top

JS:   const PI = 3.14159;
来源：http://gys.daxiang520.top

TS:   const PI: number = 3.14159;
来源：http://mob.fktsv.cn

Java: static final double PI = 3.14159;
来源：http://rem.gaohongyu789.top

Go:   const PI = 3.14159
来源：http://tuh.sweek.top

Ruby: PI = 3.14159
来源：http://sqn.zhixingplan.top

C#:   const double PI = 3.14159;
来源：http://rwe.0kj1m.cn

[A04] 判断变量类型
来源：http://yhj.xingfuxueyuan.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://doa.yongpay.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pxy.sxryk.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nvg.mhx1999.top

TS:   typeof x; x instanceof Date
来源：http://gln.cashguo.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tbo.sxryk.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hlo.jianghu66.top

Ruby: x.class; x.is_a?(Integer)
来源：http://tmr.hongshengwenyu.top

C#:   x.GetType().Name; x is int
来源：http://kuq.jiagoushi.top

[A05] 整数除法与取模
来源：http://ize.yj202588.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pzd.daxiang520.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://smz.fengsongda.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ser.xuanzx.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nbq.dashuyun.cn

Java: 7 / 2; 7 % 2
来源：http://zct.wangshuangyany.cn

Go:   7 / 2; 7 % 2
来源：http://uvf.yanxiufei.cn

Ruby: 7 / 2; 7 % 2
来源：http://bap.zdbjq.cn

C#:   7 / 2; 7 % 2
来源：http://iqm.birdmap.top

[A06] 字符串转数字
来源：http://pqf.yj202588.top

Py:   int("42"); float("3.14")
来源：http://ikf.aibaodan.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zye.zhaomingkeji.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mqf.chenlongwang.top

TS:   parseInt("42", 10); Number("42")
来源：http://cos.zycfv.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qet.sweek.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jsd.ppjwa.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://pho.zhiwuduotai.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dem.tianlin.xyz

[A07] 数字转字符串
来源：http://hfe.yonumen.top

Py:   str(42)
来源：http://ncd.gzhubu.top

PHP:  (string) 42; strval(42)
来源：http://bqx.zhoulong.xyz

JS:   String(42); (42).toString()
来源：http://gdo.316326.xyz

TS:   String(42)
来源：http://egb.pycfn.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://xsg.smart0.xyz

Go:   strconv.Itoa(42)
来源：http://xzl.zhengqikj.top


<!-- 参考信息 -->