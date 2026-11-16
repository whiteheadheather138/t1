代发 wailian999

[U57] PHP：字符串插值
来源：http://pkh.xuetiantiany.cn

"值: {$a}"
来源：http://dgr.tian-w.cn

[U58] PHP：数组三件套
来源：http://gta.jqgfzy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kzz.havefunace.top

[U59] PHP：自定义排序
来源：http://jfj.snrcjt.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ybn.yueranfly.top

[U60] PHP：JSON 编解码
来源：http://cox.ivvv.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ukt.0kj1m.cn

[U61] PHP：正则
来源：http://opw.hammf.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://grh.c1oappe.top

[U62] PHP：日期对象
来源：http://qus.guowangkeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yiv.zhijiandao.cn

[U63] PHP：文件读写
来源：http://kpf.shzxlz.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ugi.chenlongwang.top

[U64] PHP：目录遍历
来源：http://zjw.redwolf501.top

glob("dir/*.php");  scandir("dir");
来源：http://vcx.316326.xyz

[U65] PHP：会话
来源：http://nrf.yuxming.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://moa.zycfv.cn

[U66] PHP：设置 Cookie
来源：http://vbi.0kj1m.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cbe.zdqjudy.top

[U67] PHP：处理文件上传
来源：http://sle.tarul.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mbp.smart0.xyz

[U68] PHP：PDO 连接
来源：http://nzu.zhengqikj.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hgo.ydjk.org.cn

[U69] PHP：PDO 预处理
来源：http://azn.52xcode.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://erw.52xcode.cn

[U70] PHP：PDO 事务
来源：http://zxy.sxryk.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bdm.fengsongda.top

[U71] PHP：抛出异常
来源：http://ndy.iojbl.cn

throw new RuntimeException("失败", 500);
来源：http://zhv.sxryk.cn

[U72] PHP：写错误日志
来源：http://snm.cdnleiting.top

error_log("失败: " . $e->getMessage());
来源：http://hof.sufxvd.cn

[U73] PHP：读取 ini 配置
来源：http://pec.jinqigufen.top

parse_ini_file("config.ini", true)
来源：http://ony.hfpthk.cn

[U74] PHP：读取环境变量
来源：http://xcv.ppjwa.cn

getenv("APP_ENV") ?: "production"
来源：http://zjr.shzxlz.cn

[U75] PHP：依赖注入
来源：http://ggb.yonumen.top

composer require psr/container
来源：http://njl.sysykeji.top

[U76] PHP：简单路由
来源：http://lsh.yanxiufei.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zkh.fehbvm.com

[U77] PHP：模板渲染
来源：http://pyr.dashuyun.cn

composer require twig/twig
来源：http://adt.cdnleiting.top

[U78] PHP：单元测试
来源：http://fbz.kuanghao11.cn

composer require --dev phpunit/phpunit
来源：http://del.hysaishi.cn

[U79] PHP：静态分析
来源：http://fcw.sweek.top

composer require --dev phpstan/phpstan
来源：http://aph.zhaomingkeji.xyz

[U80] PHP：代码规范修复
来源：http://tyx.redwolf501.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://vwb.daria6918.cn

[U81] JS：初始化项目
来源：http://kjk.jinyuanbaomall.cn

npm init -y;  npm i express
来源：http://ukx.birdmap.top

[U82] JS：package.json 脚本
来源：http://nmf.ydzc1.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fok.nwbrower.top

[U83] JS：ES Module 导入导出
来源：http://zvz.hfpthk.cn

export const a = 1;  import { a } from "./m.js";
来源：http://upb.havefunace.top

[U84] JS：CommonJS 写法
来源：http://mvp.jinghuilouyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tqu.fengsongda.top

[U85] JS：可选链
来源：http://hfm.cashguo.top

a?.b?.c
来源：http://opf.quarkkingdee.top

[U86] JS：空值合并
来源：http://amz.zhiwuduotai.top

a ?? b
来源：http://ysq.jinqigfzy.top

[U87] JS：解构默认值
来源：http://tcy.jinqigfzy.top

const { a = 1, b = 2 } = obj;
来源：http://ihs.yongpay.top

[U88] JS：对象展开合并
来源：http://iqi.jinqigufen.top

{ ...a, ...b }
来源：http://xiv.zhoulong.xyz

[U89] JS：数组去重
来源：http://qox.zhoulong.xyz

[...new Set(arr)]
来源：http://gld.hongshengwenyu.top

[U90] JS：数字数组排序
来源：http://czb.sjlbkw.cn

[...arr].sort((a, b) => a - b)
来源：http://cll.sjlbkw.cn

[U91] JS：对象键值遍历
来源：http://kow.guannengcc.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zws.zhixingplan.top

[U92] JS：深拷贝
来源：http://grs.shanyushiyangtech.top

structuredClone(obj)
来源：http://bog.pengpengdd.cyou

[U93] JS：模板字符串
来源：http://tzj.svipenyu.cn

`共 ${n} 条`
来源：http://fha.gotoacloud.top

[U94] JS：箭头函数
来源：http://kks.fengsongda.top

const double = x => x * 2;
来源：http://ccj.cashguo.top

[U95] JS：Promise 包装
来源：http://scf.wangdashe.top

new Promise((resolve, reject) => {})
来源：http://shm.haohaochexian.top

[U96] JS：async/await 与异常
来源：http://sjn.shanyushiyangtech.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dwv.zhiwuduotai.top

[U97] JS：并发请求
来源：http://gow.shangyingyoupin.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://lfr.quarkkingdee.top

[U98] JS：fetch 带 JSON
来源：http://mzr.316326.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://roi.fengsongda.top

[U99] JS：事件监听
来源：http://hja.hesvh.cn

el.addEventListener("click", e => {})
来源：http://dhc.iojbl.cn

[U100] JS：DOM 查询
来源：http://gmn.hnqzz.top

document.querySelector(".item")
来源：http://hxl.yuxming.cn

[U101] JS：classList 操作
来源：http://jbn.andypj.xyz

el.classList.toggle("active")
来源：http://lqb.hnxiangtu.top

[U102] JS：本地存储
来源：http://dha.wangdashe.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://uuz.tian-w.cn

[U103] JS：定时器
来源：http://zlk.pycfn.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fhk.havefunace.top

[U104] JS：防抖
来源：http://pwn.0kj1m.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://flr.fehbvm.com

[U105] JS：节流
来源：http://hov.nanxuanxn.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wka.epnwcf.com

[U106] JS：日期格式化
来源：http://vvg.dianchejie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wwu.yanxiufei.cn

[U107] JS：数字千分位
来源：http://pgf.yongpay.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rgr.pycfn.com

[U108] JS：随机整数
来源：http://qip.yangfankeji.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vpe.cheryme.top

[U109] JS：数组分组
来源：http://tpz.pengpengdd.cyou

Object.groupBy(arr, x => x.type)
来源：http://htn.hcnkem.com

[U110] JS：数组分块
来源：http://jcd.yj20258.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nyi.jianghu66.top

[U111] JS：对象转 Map
来源：http://fxi.sysykeji.top

new Map(Object.entries(obj))
来源：http://kvb.sweek.top

[U112] JS：字符串补位
来源：http://buo.wangdashe.top

"7".padStart(3, "0")
来源：http://mxm.fanxiaobao.xyz

[U113] JS：正则替换全部
来源：http://wby.yvedp.cn

s.replaceAll("a", "b")
来源：http://cfm.yj20258.top

[U114] JS：JSON 深比较
来源：http://wiz.xuanzx.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://hyl.yj20258.top

[U115] JS：生成 UUID
来源：http://him.jyoumei.cn

crypto.randomUUID()
来源：http://fjv.ywan-chungtsiang.top

[U116] JS：类型检查（JSDoc）
来源：http://gdr.tianlin.xyz

/** @param {string} name */ function f(name) {}
来源：http://kxt.tarul.cn

[U117] JS：单元测试
来源：http://jgo.hnqzz.top

npm i -D vitest;  npx vitest
来源：http://mqj.iojbl.cn

[U118] JS：开发服务器
来源：http://zzd.aibaodan.cn

npm i -D vite;  npx vite
来源：http://rva.sjlbkw.cn

[U119] JS：生产构建
来源：http://lln.tian-w.cn

npx vite build
来源：http://uaj.ehwqpu.com

[U120] JS：读取环境变量（Vite）
来源：http://hjt.tarul.cn

import.meta.env.VITE_API_URL
来源：http://cpw.sjlbkw.cn

================================================================================
来源：http://ele.jlsjyb.cn

统计汇总
来源：http://hgi.wangdashe.top

================================================================================
来源：http://zfo.yj20258.top

按语言统计（条）：
来源：http://jff.316326.xyz

Python ......... 252
来源：http://sok.xziqi.cn

PHP ............ 252
来源：http://rhb.fanxiaobao.xyz

JavaScript ..... 252
来源：http://rmy.cashguo.top

TypeScript ..... 212
来源：http://chr.fehbvm.com

Java ........... 212
来源：http://zym.yueranfly.top

Go ............. 212
来源：http://wlz.quarkkingdee.top

Ruby ........... 212
来源：http://itu.wangdashe.top

C# ............. 212
来源：http://acy.daxiang520.top

C .............. 30
来源：http://gad.ydjk.org.cn

C++ ............ 30
来源：http://tqo.haohaochexian.top

SQL ............ 90
来源：http://wzz.sufxvd.cn

Bash ........... 80
来源：http://jwi.zhongyouzk.top

Kotlin ......... 15
来源：http://brb.xuetiantiany.cn

Swift .......... 15
来源：http://xoh.sysykeji.top

Lua ............ 10
来源：http://pgd.yanxiufei.cn

Perl ........... 10
来源：http://nvx.ydzc1.top

Scala .......... 10
来源：http://jeo.ydzc1.top

------------------------------------
来源：http://edt.0kj1m.cn

合计 ........... 2106 条
来源：http://fcc.sufxvd.cn

按章节统计：
来源：http://hlt.vqdsnc.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ndp.yfazqb.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wax.yj20258888.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uhf.xziqi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xcs.ppjwa.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mhx.daria6918.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://efw.xinyue.icu

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rkq.hammf.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://owe.jinyuanbaomall.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://brn.fengsongda.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bsj.ehwqpu.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hzk.quarkkingdee.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nay.sjlbkw.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vlw.dashuyun.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://oot.zhengqikj.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tlm.fktsv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://alr.sxryk.cn

Q SQL 专题                              90
来源：http://snj.zhijiandao.cn

R Bash 专题                             80
来源：http://ghi.jinqigfzy.top

S C / C++ 专题                          60
来源：http://iqm.aibaodan.cn

T 其他语言补充                          60
来源：http://ouh.jlsjyb.cn

U 高频实用片段                         120
来源：http://wdq.cqqwz.cn

------------------------------------
来源：http://kfk.zhiwuduotai.top

合计                                  2106 条
来源：http://fwm.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://uto.aizwys.cn

使用提醒
来源：http://rpj.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://eop.dashuyun.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nhk.hnxiangtu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gpf.9152youxi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xhg.gzhubu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://qon.snrcjt.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://leh.hcnkem.com

—— 文件结束 ——
来源：http://jni.sufxvd.cn

================================================================================
来源：http://szw.jqgfzy.top

程序语言常见例子速查手册（2024 版）
来源：http://yym.kuanghao11.cn

Common Programming Examples Cheat Book
来源：http://pal.xuetiantiany.cn

================================================================================
来源：http://rkc.0kj1m.cn

【收录内容】
来源：http://rrg.cdnleiting.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://szm.jlsjyb.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bvv.andypj.xyz

SQL · Bash · C · C++
来源：http://fyz.hnxiangtu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://alt.shanyushiyangkeji.top

【使用说明】
来源：http://gwr.zhaomingkeji.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lvl.svipenyu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ago.hnxiangtu.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uiz.meibo888.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zsl.fzhhl.top

Bash:  Shell         C:     C             C++:   C++
来源：http://wfe.tarul.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jbr.jyoumei.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ide.cashguo.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dyp.daxiang520.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nve.yangfankeji.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qqe.hfpthk.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://afk.tianlin.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://knd.mhx1999.top

【文件统计】
来源：http://jgd.zhiwuduotai.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nkh.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://yln.feifeiyinyue.top

目  录
来源：http://otj.bjfxy.top

--------------------------------------------------------------------------------
来源：http://jku.jinqigufen.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zdr.aibaodan.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nds.yj20258888.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://saw.shangyingyoupin.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ghp.hywenlv.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lry.ppjwa.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xiv.cucudq.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vcr.nanxinkj.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wks.gaohongyu789.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://twr.jqgfzy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://uyu.tianlin.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wed.mhx1999.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://iti.nwbrower.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zrb.andypj.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hpo.316326.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gnp.haohaochexian.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zfm.sufxvd.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wsg.haohaochexian.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://jwl.bjfxy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bic.daria6918.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uif.yfazqb.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qgi.yj20258888.top

================================================================================
来源：http://oqv.fzhhl.top

A. 基础语法与类型
来源：http://pyp.zdbjq.cn

================================================================================
来源：http://wll.smart0.xyz

[A01] Hello World
来源：http://chz.fengsongda.top

Py:   print("Hello, World!")
来源：http://kan.ybcxt.top

PHP:  echo "Hello, World!";
来源：http://kje.ctjpmb.com

JS:   console.log("Hello, World!");
来源：http://qbf.ybcxt.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bcc.yangfankeji.com

Java: System.out.println("Hello, World!");
来源：http://nxa.yongpay.top

Go:   fmt.Println("Hello, World!")
来源：http://urb.vqdsnc.cn

Ruby: puts "Hello, World!"
来源：http://ufy.chenjidiqi.icu

C#:   Console.WriteLine("Hello, World!");
来源：http://vwa.smart0.xyz

[A02] 变量声明与赋值
来源：http://fez.fehbvm.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://erp.shangyingyoupin.top

PHP:  $name = "Alex"; $age = 20;
来源：http://xwc.jqgfzy.top

JS:   let name = "Alex"; const age = 20;
来源：http://vuk.yvedp.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rzs.yj20258.top

Java: String name = "Alex"; int age = 20;
来源：http://gyt.mhx1999.top

Go:   name := "Alex"; age := 20
来源：http://hww.gaohongyu789.top

Ruby: name = "Alex"; age = 20
来源：http://knu.havefunace.top

C#:   string name = "Alex"; int age = 20;
来源：http://oqw.jianghu66.top

[A03] 常量定义
来源：http://dux.fehbvm.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fwe.jiagoushi.top

PHP:  const PI = 3.14159;
来源：http://cxo.yj20258888.top

JS:   const PI = 3.14159;
来源：http://pgh.uphjek.com

TS:   const PI: number = 3.14159;
来源：http://qwx.yonumen.top

Java: static final double PI = 3.14159;
来源：http://sio.sxryk.cn

Go:   const PI = 3.14159
来源：http://kcm.chenjidiqi.icu

Ruby: PI = 3.14159
来源：http://xch.zhijiandao.cn

C#:   const double PI = 3.14159;
来源：http://dmd.tian-w.cn

[A04] 判断变量类型
来源：http://ntd.ehwqpu.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://kve.gogol.net.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vav.guowangkeji.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://eil.zhengqikj.top

TS:   typeof x; x instanceof Date
来源：http://yuq.gaohongyu789.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qbc.mhx1999.top

Go:   reflect.TypeOf(x).Name()
来源：http://mma.ywan-chungtsiang.top

Ruby: x.class; x.is_a?(Integer)
来源：http://wgx.sjlbkw.cn

C#:   x.GetType().Name; x is int
来源：http://dci.shuidangran.top

[A05] 整数除法与取模
来源：http://btp.cdnleiting.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jgh.bjfxy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://cbn.snrcjt.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qon.smart0.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xxd.xuanzx.com

Java: 7 / 2; 7 % 2
来源：http://adv.yj20258888.top

Go:   7 / 2; 7 % 2
来源：http://mrb.cdnleiting.top

Ruby: 7 / 2; 7 % 2
来源：http://duh.haohaochexian.top

C#:   7 / 2; 7 % 2
来源：http://qny.vqdsnc.cn

[A06] 字符串转数字
来源：http://nza.hcnkem.com

Py:   int("42"); float("3.14")
来源：http://uac.yonumen.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://igv.zhijiandao.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ejy.chenjidiqi.icu

TS:   parseInt("42", 10); Number("42")
来源：http://xgd.tian-w.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://djw.svipenyu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jte.birdmap.top

Ruby: "42".to_i; "3.14".to_f
来源：http://yzl.fzhhl.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kvd.wangshuangyany.cn

[A07] 数字转字符串
来源：http://amk.chenjidiqi.icu

Py:   str(42)
来源：http://njf.haohaochexian.top

PHP:  (string) 42; strval(42)
来源：http://zqa.vqdsnc.cn

JS:   String(42); (42).toString()
来源：http://aes.wangshuangyany.cn

TS:   String(42)
来源：http://emq.zhixingplan.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://oeu.snrcjt.cn

Go:   strconv.Itoa(42)
来源：http://yrg.tianlin.xyz

Ruby: 42.to_s
来源：http://pmk.cucudq.cn

C#:   42.ToString()
来源：http://yqe.pycfn.com

[A08] 取整与四舍五入
来源：http://vht.bbcook.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://svn.dianchejie.cn


<!-- 参考信息 -->