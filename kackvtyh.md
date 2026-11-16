代发 wailian999

[U55] PHP：match 表达式
来源：http://ftx.hongshengwenyu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qpr.fengsongda.top

[U56] PHP：命名参数
来源：http://ioa.pycfn.com

f(a: 1, b: 2)
来源：http://qep.yueranfly.top

[U57] PHP：字符串插值
来源：http://bdy.jianghu66.top

"值: {$a}"
来源：http://qtg.nanxuanxn.top

[U58] PHP：数组三件套
来源：http://jtl.xuetiantiany.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://odw.sysykeji.top

[U59] PHP：自定义排序
来源：http://qrj.cheryme.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kas.hfpthk.cn

[U60] PHP：JSON 编解码
来源：http://zhr.ppjwa.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ocj.jiagoushi.top

[U61] PHP：正则
来源：http://sac.sufxvd.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ezd.tianlin.xyz

[U62] PHP：日期对象
来源：http://ivw.316326.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rpl.xylfe.cn

[U63] PHP：文件读写
来源：http://yfz.nwbrower.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vvs.fktsv.cn

[U64] PHP：目录遍历
来源：http://eer.haohaochexian.top

glob("dir/*.php");  scandir("dir");
来源：http://egi.tarul.cn

[U65] PHP：会话
来源：http://xke.tanke756.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vjs.sweek.top

[U66] PHP：设置 Cookie
来源：http://glx.mhx1999.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oeq.meibo888.top

[U67] PHP：处理文件上传
来源：http://wdd.cucudq.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sje.jinqigfzy.top

[U68] PHP：PDO 连接
来源：http://tir.aibaodan.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fjy.zhaomingkeji.xyz

[U69] PHP：PDO 预处理
来源：http://anf.vqdsnc.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jys.xingfuxueyuan.xyz

[U70] PHP：PDO 事务
来源：http://rrr.kuanghao11.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xll.yonumen.top

[U71] PHP：抛出异常
来源：http://vcr.hcnkem.com

throw new RuntimeException("失败", 500);
来源：http://lqo.ywan-chungtsiang.top

[U72] PHP：写错误日志
来源：http://sac.ywan-chungtsiang.top

error_log("失败: " . $e->getMessage());
来源：http://rxq.52xcode.cn

[U73] PHP：读取 ini 配置
来源：http://mvf.jinghuilouyu.cn

parse_ini_file("config.ini", true)
来源：http://pfp.gzhubu.top

[U74] PHP：读取环境变量
来源：http://ryd.zhixingplan.top

getenv("APP_ENV") ?: "production"
来源：http://bgu.jinghuilouyu.cn

[U75] PHP：依赖注入
来源：http://jik.hfpthk.cn

composer require psr/container
来源：http://pwf.dashuyun.cn

[U76] PHP：简单路由
来源：http://jqi.316326.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://iep.kuanghao11.cn

[U77] PHP：模板渲染
来源：http://iji.yonumen.top

composer require twig/twig
来源：http://mxx.hysaishi.cn

[U78] PHP：单元测试
来源：http://iwe.yj202588.top

composer require --dev phpunit/phpunit
来源：http://bca.sufxvd.cn

[U79] PHP：静态分析
来源：http://dwv.shanyushiyangtech.top

composer require --dev phpstan/phpstan
来源：http://uoz.c1oappe.top

[U80] PHP：代码规范修复
来源：http://znb.cheryme.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://tlk.dianchejie.cn

[U81] JS：初始化项目
来源：http://voi.haohaochexian.top

npm init -y;  npm i express
来源：http://yot.hammf.cn

[U82] JS：package.json 脚本
来源：http://meg.cdnleiting.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qnp.chenzaomai.com

[U83] JS：ES Module 导入导出
来源：http://zax.fengsongda.top

export const a = 1;  import { a } from "./m.js";
来源：http://elv.feifeiyinyue.top

[U84] JS：CommonJS 写法
来源：http://foo.sufxvd.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jpe.sysykeji.top

[U85] JS：可选链
来源：http://bmx.bbcook.cn

a?.b?.c
来源：http://uhx.zycfv.cn

[U86] JS：空值合并
来源：http://bzz.aizwys.cn

a ?? b
来源：http://ctg.hesvh.cn

[U87] JS：解构默认值
来源：http://njd.zhixingplan.top

const { a = 1, b = 2 } = obj;
来源：http://qtx.kuanghao11.cn

[U88] JS：对象展开合并
来源：http://vcm.yuxming.cn

{ ...a, ...b }
来源：http://wqw.shuidangran.top

[U89] JS：数组去重
来源：http://tjb.52xcode.cn

[...new Set(arr)]
来源：http://vjk.ybcxt.top

[U90] JS：数字数组排序
来源：http://fbu.cqqwz.cn

[...arr].sort((a, b) => a - b)
来源：http://nay.jqgfzy.top

[U91] JS：对象键值遍历
来源：http://bvd.cucudq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hav.shanyushiyangkeji.top

[U92] JS：深拷贝
来源：http://loa.ywan-chungtsiang.top

structuredClone(obj)
来源：http://wxp.zhijiandao.cn

[U93] JS：模板字符串
来源：http://kjb.ppjwa.cn

`共 ${n} 条`
来源：http://zhu.tian-w.cn

[U94] JS：箭头函数
来源：http://oka.yuxming.cn

const double = x => x * 2;
来源：http://ktz.jlsjyb.cn

[U95] JS：Promise 包装
来源：http://fcb.sjlbkw.cn

new Promise((resolve, reject) => {})
来源：http://aao.snrcjt.cn

[U96] JS：async/await 与异常
来源：http://zrn.fehbvm.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qxs.feifeiyinyue.top

[U97] JS：并发请求
来源：http://ozm.zhixingplan.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://mnq.shzxlz.cn

[U98] JS：fetch 带 JSON
来源：http://ldw.jinghuilouyu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mht.zhengqikj.top

[U99] JS：事件监听
来源：http://nhi.jinqigufen.top

el.addEventListener("click", e => {})
来源：http://iyq.9152youxi.cn

[U100] JS：DOM 查询
来源：http://gtb.fktsv.cn

document.querySelector(".item")
来源：http://nef.uphjek.com

[U101] JS：classList 操作
来源：http://eqf.9152youxi.cn

el.classList.toggle("active")
来源：http://wqx.xylfe.cn

[U102] JS：本地存储
来源：http://swk.sxryk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zkk.xylfe.cn

[U103] JS：定时器
来源：http://wid.52xcode.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ptv.tanke756.top

[U104] JS：防抖
来源：http://kvj.nanxuanxn.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://run.cucudq.cn

[U105] JS：节流
来源：http://nqt.xuetiantiany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xhh.wangshuangyany.cn

[U106] JS：日期格式化
来源：http://emn.zdbjq.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zso.nanxinkj.top

[U107] JS：数字千分位
来源：http://tdn.zhiwuduotai.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nsu.quarkkingdee.top

[U108] JS：随机整数
来源：http://vth.ctjpmb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bfs.jyoumei.cn

[U109] JS：数组分组
来源：http://okh.c1oappe.top

Object.groupBy(arr, x => x.type)
来源：http://htg.cashguo.top

[U110] JS：数组分块
来源：http://xob.zdbjq.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wmn.jqgufenzy.top

[U111] JS：对象转 Map
来源：http://nqv.quarkkingdee.top

new Map(Object.entries(obj))
来源：http://ajc.svipenyu.cn

[U112] JS：字符串补位
来源：http://kme.fehbvm.com

"7".padStart(3, "0")
来源：http://tma.epnwcf.com

[U113] JS：正则替换全部
来源：http://nqw.dianchejie.cn

s.replaceAll("a", "b")
来源：http://gts.fengsongda.top

[U114] JS：JSON 深比较
来源：http://jkb.ehwqpu.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://kot.tanke756.top

[U115] JS：生成 UUID
来源：http://rkl.ehwqpu.com

crypto.randomUUID()
来源：http://upj.zdbjq.cn

[U116] JS：类型检查（JSDoc）
来源：http://sqn.zhengqikj.top

/** @param {string} name */ function f(name) {}
来源：http://llj.yuxming.cn

[U117] JS：单元测试
来源：http://lxg.zycfv.cn

npm i -D vitest;  npx vitest
来源：http://jlt.sweek.top

[U118] JS：开发服务器
来源：http://zpq.cashguo.top

npm i -D vite;  npx vite
来源：http://ovd.ehwqpu.com

[U119] JS：生产构建
来源：http://ott.zhijiandao.cn

npx vite build
来源：http://rra.sysykeji.top

[U120] JS：读取环境变量（Vite）
来源：http://sws.xinyue.icu

import.meta.env.VITE_API_URL
来源：http://jba.316326.xyz

================================================================================
来源：http://sds.zdqjudy.top

统计汇总
来源：http://yhq.hesvh.cn

================================================================================
来源：http://kow.daxiang520.top

按语言统计（条）：
来源：http://dvu.xuanzx.com

Python ......... 252
来源：http://vhj.ehwqpu.com

PHP ............ 252
来源：http://qad.yvedp.cn

JavaScript ..... 252
来源：http://lbx.sjlbkw.cn

TypeScript ..... 212
来源：http://cfo.hnxiangtu.top

Java ........... 212
来源：http://gcr.jinqigfzy.top

Go ............. 212
来源：http://roc.yongpay.top

Ruby ........... 212
来源：http://irz.jqgufenzy.top

C# ............. 212
来源：http://nvx.ctjpmb.com

C .............. 30
来源：http://eqq.ybcxt.top

C++ ............ 30
来源：http://ewt.bjfxy.top

SQL ............ 90
来源：http://wye.dashuyun.cn

Bash ........... 80
来源：http://zth.xuanzx.com

Kotlin ......... 15
来源：http://myg.hnqzz.top

Swift .......... 15
来源：http://vxi.chenzaomai.com

Lua ............ 10
来源：http://gln.ehwqpu.com

Perl ........... 10
来源：http://ydx.ywan-chungtsiang.top

Scala .......... 10
来源：http://umb.jinqigufen.top

------------------------------------
来源：http://lyv.svipenyu.cn

合计 ........... 2106 条
来源：http://qux.vehdjk.com

按章节统计：
来源：http://udg.jyoumei.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ihh.iojbl.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rcm.aizwys.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rkm.dianchejie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zpt.quarkkingdee.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cof.yonumen.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uef.mhx1999.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yhw.sweek.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gcl.meibo888.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ifd.meibo888.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ipw.daxiang520.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://drq.ydjk.org.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jst.jinghuilouyu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jjn.9152youxi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ien.jqgfzy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sbc.chenjidiqi.icu

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jhh.zhijiandao.cn

Q SQL 专题                              90
来源：http://qmv.cqqwz.cn

R Bash 专题                             80
来源：http://elc.yfazqb.com

S C / C++ 专题                          60
来源：http://zpl.epnwcf.com

T 其他语言补充                          60
来源：http://hyj.jianghu66.top

U 高频实用片段                         120
来源：http://atv.dianchejie.cn

------------------------------------
来源：http://opy.feifeiyinyue.top

合计                                  2106 条
来源：http://xkh.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://hag.0kj1m.cn

使用提醒
来源：http://bsp.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://qwc.shuidangran.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://igc.hongshengwenyu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wcg.ehwqpu.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://odn.hysaishi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gte.xinyue.icu

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gca.hnxiangtu.top

—— 文件结束 ——
来源：http://lsq.yj20258888.top

================================================================================
来源：http://bkb.zhiwuduotai.top

程序语言常见例子速查手册（2024 版）
来源：http://nxb.jyoumei.cn

Common Programming Examples Cheat Book
来源：http://jnk.aizwys.cn

================================================================================
来源：http://usb.fanxiaobao.xyz

【收录内容】
来源：http://zzo.ydjk.org.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ylz.zycfv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://acg.jinqigfzy.top

SQL · Bash · C · C++
来源：http://ssz.wangshuangyany.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ncg.xuetiantiany.cn

【使用说明】
来源：http://dvv.yj20258888.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://adb.yfazqb.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gvm.vqdsnc.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xyu.quarkkingdee.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sws.snrcjt.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wer.ppjwa.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://por.hnxiangtu.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cvh.hywenlv.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://grb.ppjwa.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vmk.yanxiufei.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sep.yuanzhike.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://djo.daria6918.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://key.shanyushiyangtech.top

【文件统计】
来源：http://inb.sweek.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ldo.smart0.xyz

--------------------------------------------------------------------------------
来源：http://ojq.sufxvd.cn

目  录
来源：http://wmj.yj20258888.top

--------------------------------------------------------------------------------
来源：http://oqe.yuanzhike.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ftf.cucudq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rdf.iojbl.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://znk.jinyuanbaomall.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ksm.hcnkem.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fje.daria6918.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ent.hnqzz.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ium.daxiang520.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://znf.jinqigfzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xfb.dianchejie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kql.xingfuxueyuan.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rxy.feifeiyinyue.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jde.nanxuanxn.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vhi.jinqigufen.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ljq.jianghu66.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rxp.xinyue.icu

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://aqc.fktsv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nvm.mhx1999.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://vbx.yongpay.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wmt.zycfv.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yqm.jyoumei.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pzj.shangyingyoupin.top

================================================================================
来源：http://ubf.aizwys.cn

A. 基础语法与类型
来源：http://bct.tarul.cn

================================================================================
来源：http://okn.hesvh.cn

[A01] Hello World
来源：http://air.mhx1999.top

Py:   print("Hello, World!")
来源：http://ccs.xylfe.cn

PHP:  echo "Hello, World!";
来源：http://upq.tian-w.cn

JS:   console.log("Hello, World!");
来源：http://goq.vehdjk.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://iyo.0kj1m.cn

Java: System.out.println("Hello, World!");
来源：http://jdq.pengpengdd.cyou

Go:   fmt.Println("Hello, World!")
来源：http://ghk.aizwys.cn

Ruby: puts "Hello, World!"
来源：http://inh.ppjwa.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ess.chenlongwang.top

[A02] 变量声明与赋值
来源：http://abt.uphjek.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wri.quarkkingdee.top

PHP:  $name = "Alex"; $age = 20;
来源：http://aau.ehwqpu.com

JS:   let name = "Alex"; const age = 20;
来源：http://gzs.c1oappe.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://aiu.snrcjt.cn

Java: String name = "Alex"; int age = 20;
来源：http://aez.chenzaomai.com

Go:   name := "Alex"; age := 20
来源：http://ecr.ydzc1.top

Ruby: name = "Alex"; age = 20
来源：http://xmn.quarkkingdee.top

C#:   string name = "Alex"; int age = 20;
来源：http://bdk.yuanzhike.top

[A03] 常量定义
来源：http://wnv.iojbl.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zdf.jinqigufen.top

PHP:  const PI = 3.14159;
来源：http://sws.cheryme.top

JS:   const PI = 3.14159;
来源：http://sun.yangfankeji.com

TS:   const PI: number = 3.14159;
来源：http://nrj.jiagoushi.top

Java: static final double PI = 3.14159;
来源：http://hwq.jiagoushi.top

Go:   const PI = 3.14159
来源：http://vfp.yueranfly.top

Ruby: PI = 3.14159
来源：http://dlf.zhoulong.xyz

C#:   const double PI = 3.14159;
来源：http://waz.c1oappe.top

[A04] 判断变量类型
来源：http://eva.fzhhl.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://zkg.xylfe.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xgk.jiagoushi.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hpq.9152youxi.cn

TS:   typeof x; x instanceof Date
来源：http://fzw.yj202588.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qhy.0kj1m.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ato.snrcjt.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wsc.iojbl.cn

C#:   x.GetType().Name; x is int
来源：http://ckb.uphjek.com

[A05] 整数除法与取模
来源：http://qbd.shanyushiyangkeji.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vte.jinqigufen.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://wum.yj20258.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qwb.cdnleiting.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ccy.hysaishi.cn

Java: 7 / 2; 7 % 2
来源：http://plu.kuanghao11.cn

Go:   7 / 2; 7 % 2
来源：http://ang.0kj1m.cn

Ruby: 7 / 2; 7 % 2
来源：http://oey.mhx1999.top

C#:   7 / 2; 7 % 2
来源：http://goi.jqgufenzy.top

[A06] 字符串转数字
来源：http://lyr.chenlongwang.top

Py:   int("42"); float("3.14")
来源：http://oky.c1oappe.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://omy.cashguo.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nbq.9152youxi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://etd.ivvv.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://iei.zhixingplan.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bzf.zhengqikj.top

Ruby: "42".to_i; "3.14".to_f
来源：http://poo.jqgfzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nqm.hywenlv.cn

[A07] 数字转字符串
来源：http://gyp.316326.xyz

Py:   str(42)
来源：http://yvb.jinqigfzy.top

PHP:  (string) 42; strval(42)
来源：http://yfl.yj20258888.top

JS:   String(42); (42).toString()
来源：http://ren.jqgfzy.top

TS:   String(42)
来源：http://bon.vqdsnc.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://esn.zhijiandao.cn

Go:   strconv.Itoa(42)
来源：http://vzc.feifeiyinyue.top


<!-- 参考信息 -->