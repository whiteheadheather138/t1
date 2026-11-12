代发 wailian999

[U55] PHP：match 表达式
来源：http://euo.vehdjk.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ngq.jqgufenzy.top

[U56] PHP：命名参数
来源：http://wwg.zhongyouzk.top

f(a: 1, b: 2)
来源：http://fcm.haohaochexian.top

[U57] PHP：字符串插值
来源：http://aye.xinyue.icu

"值: {$a}"
来源：http://njf.zhiwuduotai.top

[U58] PHP：数组三件套
来源：http://xhq.bjfxy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mzf.pycfn.com

[U59] PHP：自定义排序
来源：http://auz.fanxiaobao.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xoo.cqqwz.cn

[U60] PHP：JSON 编解码
来源：http://tjj.jiagoushi.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yzu.xuetiantiany.cn

[U61] PHP：正则
来源：http://cxp.52xcode.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dzj.hywenlv.cn

[U62] PHP：日期对象
来源：http://rog.ivvv.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://igs.yj202588.top

[U63] PHP：文件读写
来源：http://flh.hesvh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kac.xinyue.icu

[U64] PHP：目录遍历
来源：http://eoo.ivvv.top

glob("dir/*.php");  scandir("dir");
来源：http://tfz.xziqi.cn

[U65] PHP：会话
来源：http://uyv.shangyingyoupin.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ivt.hnxiangtu.top

[U66] PHP：设置 Cookie
来源：http://lcs.nanxinkj.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cit.ctjpmb.com

[U67] PHP：处理文件上传
来源：http://lim.wangshuangyany.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://abb.yvedp.cn

[U68] PHP：PDO 连接
来源：http://amd.xuetiantiany.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vlx.vqdsnc.cn

[U69] PHP：PDO 预处理
来源：http://wwt.hnxiangtu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qyz.nanxuanxn.top

[U70] PHP：PDO 事务
来源：http://von.ehwqpu.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vdp.zdbjq.cn

[U71] PHP：抛出异常
来源：http://zuk.hywenlv.cn

throw new RuntimeException("失败", 500);
来源：http://qoa.zhengqikj.top

[U72] PHP：写错误日志
来源：http://fgb.tian-w.cn

error_log("失败: " . $e->getMessage());
来源：http://tis.ywan-chungtsiang.top

[U73] PHP：读取 ini 配置
来源：http://byu.daria6918.cn

parse_ini_file("config.ini", true)
来源：http://nmg.jianghu66.top

[U74] PHP：读取环境变量
来源：http://mey.fanxiaobao.xyz

getenv("APP_ENV") ?: "production"
来源：http://drl.9152youxi.cn

[U75] PHP：依赖注入
来源：http://ibo.vqdsnc.cn

composer require psr/container
来源：http://ipy.ehwqpu.com

[U76] PHP：简单路由
来源：http://nxb.zhixingplan.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lmt.fengsongda.top

[U77] PHP：模板渲染
来源：http://hkt.sweek.top

composer require twig/twig
来源：http://hbs.xuanzx.com

[U78] PHP：单元测试
来源：http://qnz.hesvh.cn

composer require --dev phpunit/phpunit
来源：http://uok.meibo888.top

[U79] PHP：静态分析
来源：http://dns.fzhhl.top

composer require --dev phpstan/phpstan
来源：http://atx.cdnleiting.top

[U80] PHP：代码规范修复
来源：http://zgn.hnqzz.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://sgc.zhengqikj.top

[U81] JS：初始化项目
来源：http://vzk.redwolf501.top

npm init -y;  npm i express
来源：http://srx.yonumen.top

[U82] JS：package.json 脚本
来源：http://nja.jinqigufen.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cwr.zhijiandao.cn

[U83] JS：ES Module 导入导出
来源：http://iwu.cucudq.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wpw.hongshengwenyu.top

[U84] JS：CommonJS 写法
来源：http://yai.zhaomingkeji.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://nbh.chenlongwang.top

[U85] JS：可选链
来源：http://ubl.snrcjt.cn

a?.b?.c
来源：http://zks.ctjpmb.com

[U86] JS：空值合并
来源：http://hnw.xuetiantiany.cn

a ?? b
来源：http://htl.zhijiandao.cn

[U87] JS：解构默认值
来源：http://xul.kuanghao11.cn

const { a = 1, b = 2 } = obj;
来源：http://ojl.aibaodan.cn

[U88] JS：对象展开合并
来源：http://htg.wangdashe.top

{ ...a, ...b }
来源：http://jww.c1oappe.top

[U89] JS：数组去重
来源：http://lqo.jqgfzy.top

[...new Set(arr)]
来源：http://cvp.aibaodan.cn

[U90] JS：数字数组排序
来源：http://var.wangdashe.top

[...arr].sort((a, b) => a - b)
来源：http://gvk.gzhubu.top

[U91] JS：对象键值遍历
来源：http://rjq.jyoumei.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ozk.sysykeji.top

[U92] JS：深拷贝
来源：http://xsw.52xcode.cn

structuredClone(obj)
来源：http://xmv.yvedp.cn

[U93] JS：模板字符串
来源：http://qkc.zhongyouzk.top

`共 ${n} 条`
来源：http://sgb.daxiang520.top

[U94] JS：箭头函数
来源：http://hhy.zhaomingkeji.xyz

const double = x => x * 2;
来源：http://tuf.sjlbkw.cn

[U95] JS：Promise 包装
来源：http://pab.jianghu66.top

new Promise((resolve, reject) => {})
来源：http://wfl.shangyingyoupin.top

[U96] JS：async/await 与异常
来源：http://ohb.zhongyouzk.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oct.tianlin.xyz

[U97] JS：并发请求
来源：http://ivo.hongshengwenyu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://itq.zhaomingkeji.xyz

[U98] JS：fetch 带 JSON
来源：http://smn.jyoumei.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ihl.wangdashe.top

[U99] JS：事件监听
来源：http://cpc.feifeiyinyue.top

el.addEventListener("click", e => {})
来源：http://wox.fengsongda.top

[U100] JS：DOM 查询
来源：http://lmq.jiagoushi.top

document.querySelector(".item")
来源：http://rxy.chenzaomai.com

[U101] JS：classList 操作
来源：http://gdb.zhiwuduotai.top

el.classList.toggle("active")
来源：http://hmc.hongshengwenyu.top

[U102] JS：本地存储
来源：http://blm.hongshengwenyu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://dxd.iojbl.cn

[U103] JS：定时器
来源：http://vfj.52xcode.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ujv.zhoulong.xyz

[U104] JS：防抖
来源：http://nnm.hfpthk.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xqm.jianghu66.top

[U105] JS：节流
来源：http://xpp.chenjidiqi.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rsb.yonumen.top

[U106] JS：日期格式化
来源：http://znw.shangyingyoupin.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sva.ctjpmb.com

[U107] JS：数字千分位
来源：http://uob.zhengqikj.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kcx.hcnkem.com

[U108] JS：随机整数
来源：http://auh.zhaomingkeji.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zqb.hnxiangtu.top

[U109] JS：数组分组
来源：http://yci.mhx1999.top

Object.groupBy(arr, x => x.type)
来源：http://gkw.jinqigufen.top

[U110] JS：数组分块
来源：http://pcp.fengsongda.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://eym.yuanzhike.top

[U111] JS：对象转 Map
来源：http://jxr.yfazqb.com

new Map(Object.entries(obj))
来源：http://ibm.guowangkeji.top

[U112] JS：字符串补位
来源：http://rfo.hesvh.cn

"7".padStart(3, "0")
来源：http://wds.chenjidiqi.icu

[U113] JS：正则替换全部
来源：http://kov.hfpthk.cn

s.replaceAll("a", "b")
来源：http://mec.yonumen.top

[U114] JS：JSON 深比较
来源：http://qpv.tian-w.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ooh.nwbrower.top

[U115] JS：生成 UUID
来源：http://clu.jiagoushi.top

crypto.randomUUID()
来源：http://bmd.zhoulong.xyz

[U116] JS：类型检查（JSDoc）
来源：http://mrc.ppjwa.cn

/** @param {string} name */ function f(name) {}
来源：http://jfk.ivvv.top

[U117] JS：单元测试
来源：http://ucc.guannengcc.top

npm i -D vitest;  npx vitest
来源：http://uuu.fanxiaobao.xyz

[U118] JS：开发服务器
来源：http://pbn.fzhhl.top

npm i -D vite;  npx vite
来源：http://vif.vqdsnc.cn

[U119] JS：生产构建
来源：http://pjg.chenzaomai.com

npx vite build
来源：http://pkm.hnxiangtu.top

[U120] JS：读取环境变量（Vite）
来源：http://dnv.havefunace.top

import.meta.env.VITE_API_URL
来源：http://juk.quarkkingdee.top

================================================================================
来源：http://mdq.sweek.top

统计汇总
来源：http://akt.hnqzz.top

================================================================================
来源：http://zay.andypj.xyz

按语言统计（条）：
来源：http://lim.jqgufenzy.top

Python ......... 252
来源：http://bpj.jinghuilouyu.cn

PHP ............ 252
来源：http://yhc.jianghu66.top

JavaScript ..... 252
来源：http://bgh.fktsv.cn

TypeScript ..... 212
来源：http://stz.uphjek.com

Java ........... 212
来源：http://hbi.shanyushiyangkeji.top

Go ............. 212
来源：http://uzu.xuetiantiany.cn

Ruby ........... 212
来源：http://aad.316326.xyz

C# ............. 212
来源：http://uxr.zhoulong.xyz

C .............. 30
来源：http://koz.yueranfly.top

C++ ............ 30
来源：http://ffy.xuanzx.com

SQL ............ 90
来源：http://naw.vqdsnc.cn

Bash ........... 80
来源：http://fbw.xuetiantiany.cn

Kotlin ......... 15
来源：http://dcu.cdnleiting.top

Swift .......... 15
来源：http://qgd.ehwqpu.com

Lua ............ 10
来源：http://seb.316326.xyz

Perl ........... 10
来源：http://mrh.jqgufenzy.top

Scala .......... 10
来源：http://wzn.jiagoushi.top

------------------------------------
来源：http://lzu.tanke756.top

合计 ........... 2106 条
来源：http://fae.jlsjyb.cn

按章节统计：
来源：http://phr.guannengcc.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tbg.guannengcc.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dpp.svipenyu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pyx.fengsongda.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blg.epnwcf.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rvk.zycfv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kxm.hfpthk.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cot.tian-w.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vrz.guowangkeji.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://odz.aizwys.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ely.birdmap.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sns.fanxiaobao.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://eyq.svipenyu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kzc.xziqi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bzw.hongshengwenyu.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lvs.ybcxt.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://czj.ybcxt.top

Q SQL 专题                              90
来源：http://wzw.ivvv.top

R Bash 专题                             80
来源：http://msb.xziqi.cn

S C / C++ 专题                          60
来源：http://ewy.cheryme.top

T 其他语言补充                          60
来源：http://faq.xuetiantiany.cn

U 高频实用片段                         120
来源：http://czw.shuidangran.top

------------------------------------
来源：http://mzv.shanyushiyangkeji.top

合计                                  2106 条
来源：http://qdi.xuanzx.com

--------------------------------------------------------------------------------
来源：http://asd.shangyingyoupin.top

使用提醒
来源：http://vob.yueranfly.top

--------------------------------------------------------------------------------
来源：http://mtp.guowangkeji.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jpc.fzhhl.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nev.fzhhl.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mdw.ybcxt.top

在旧版本上使用前请先确认语法支持情况。
来源：http://cxx.shanyushiyangkeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pmk.ydjk.org.cn

—— 文件结束 ——
来源：http://scc.jinghuilouyu.cn

================================================================================
来源：http://cgq.fzhhl.top

程序语言常见例子速查手册（2024 版）
来源：http://hir.epnwcf.com

Common Programming Examples Cheat Book
来源：http://cwi.sufxvd.cn

================================================================================
来源：http://ekb.chenzaomai.com

【收录内容】
来源：http://cha.guowangkeji.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://uor.daria6918.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bfh.guowangkeji.top

SQL · Bash · C · C++
来源：http://hah.fzhhl.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://iuk.xuanzx.com

【使用说明】
来源：http://etm.aibaodan.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qkn.cucudq.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hui.hesvh.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zbp.tarul.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ukr.shanyushiyangtech.top

Bash:  Shell         C:     C             C++:   C++
来源：http://phg.bbcook.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tpx.haohaochexian.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jqo.zhixingplan.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://him.hcnkem.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jxd.cashguo.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rud.wangdashe.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yxt.yuanzhike.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gfh.ivvv.top

【文件统计】
来源：http://abf.gaohongyu789.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cke.fengsongda.top

--------------------------------------------------------------------------------
来源：http://evc.shanyushiyangkeji.top

目  录
来源：http://xsv.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://enh.dianchejie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uak.zhongyouzk.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://brt.xylfe.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gae.nanxinkj.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rbx.snrcjt.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ucl.316326.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bhv.hammf.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://oce.zhijiandao.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wzw.ydzc1.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nyt.sxryk.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bxy.zhixingplan.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nqw.iojbl.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ewg.shangyingyoupin.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://iwi.tanke756.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://uyz.daria6918.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xdg.uphjek.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jqq.ppjwa.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lmq.hcnkem.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://lyp.vehdjk.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nhv.guowangkeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yai.shuidangran.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://irc.meibo888.top

================================================================================
来源：http://phn.xuanzx.com

A. 基础语法与类型
来源：http://luz.bbcook.cn

================================================================================
来源：http://wcf.zhaomingkeji.xyz

[A01] Hello World
来源：http://aec.sweek.top

Py:   print("Hello, World!")
来源：http://wnp.feifeiyinyue.top

PHP:  echo "Hello, World!";
来源：http://kzy.zhixingplan.top

JS:   console.log("Hello, World!");
来源：http://dqz.redwolf501.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nmp.shanyushiyangtech.top

Java: System.out.println("Hello, World!");
来源：http://ent.hnxiangtu.top

Go:   fmt.Println("Hello, World!")
来源：http://ket.andypj.xyz

Ruby: puts "Hello, World!"
来源：http://peg.hnqzz.top

C#:   Console.WriteLine("Hello, World!");
来源：http://gwg.jinqigufen.top

[A02] 变量声明与赋值
来源：http://ipd.yueranfly.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qrs.chenjidiqi.icu

PHP:  $name = "Alex"; $age = 20;
来源：http://qhc.fzhhl.top

JS:   let name = "Alex"; const age = 20;
来源：http://cje.hysaishi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oyn.hywenlv.cn

Java: String name = "Alex"; int age = 20;
来源：http://yrt.shanyushiyangkeji.top

Go:   name := "Alex"; age := 20
来源：http://max.gaohongyu789.top

Ruby: name = "Alex"; age = 20
来源：http://vxu.xuanzx.com

C#:   string name = "Alex"; int age = 20;
来源：http://zhd.aizwys.cn

[A03] 常量定义
来源：http://sng.gaohongyu789.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hqz.tianlin.xyz

PHP:  const PI = 3.14159;
来源：http://oaf.ybcxt.top

JS:   const PI = 3.14159;
来源：http://pod.xingfuxueyuan.xyz

TS:   const PI: number = 3.14159;
来源：http://cbx.xinyue.icu

Java: static final double PI = 3.14159;
来源：http://hmy.cucudq.cn

Go:   const PI = 3.14159
来源：http://kty.316326.xyz

Ruby: PI = 3.14159
来源：http://bhr.guannengcc.top

C#:   const double PI = 3.14159;
来源：http://ina.gzhubu.top

[A04] 判断变量类型
来源：http://brk.sysykeji.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://vqx.vehdjk.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://siy.wangdashe.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lvp.hfpthk.cn

TS:   typeof x; x instanceof Date
来源：http://lem.cheryme.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lde.cashguo.top

Go:   reflect.TypeOf(x).Name()
来源：http://bpl.xuanzx.com

Ruby: x.class; x.is_a?(Integer)
来源：http://nlz.tarul.cn

C#:   x.GetType().Name; x is int
来源：http://zww.sysykeji.top

[A05] 整数除法与取模
来源：http://qyb.ehwqpu.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pse.guowangkeji.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://spw.vehdjk.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xyx.xylfe.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vyr.gzhubu.top

Java: 7 / 2; 7 % 2
来源：http://tqv.sysykeji.top

Go:   7 / 2; 7 % 2
来源：http://xcz.yuxming.cn

Ruby: 7 / 2; 7 % 2
来源：http://thn.wangdashe.top

C#:   7 / 2; 7 % 2
来源：http://dvz.hnxiangtu.top

[A06] 字符串转数字
来源：http://mln.bbcook.cn

Py:   int("42"); float("3.14")
来源：http://nft.yueranfly.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://krl.jiagoushi.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xxt.fehbvm.com

TS:   parseInt("42", 10); Number("42")
来源：http://yah.havefunace.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xqy.dashuyun.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://osv.hesvh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://uif.shangyingyoupin.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fja.tarul.cn

[A07] 数字转字符串
来源：http://dyh.ctjpmb.com

Py:   str(42)
来源：http://lou.gogol.net.cn

PHP:  (string) 42; strval(42)
来源：http://jgj.cdnleiting.top

JS:   String(42); (42).toString()
来源：http://szk.yongpay.top

TS:   String(42)
来源：http://xqy.shanyushiyangtech.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://tln.yfazqb.com

Go:   strconv.Itoa(42)
来源：http://ldd.ywan-chungtsiang.top


<!-- 参考信息 -->