代发 wailian999

[U51] PHP：数组解构
来源：http://vrc.yfazqb.com

[$a, $b] = $arr;
来源：http://kos.cdnleiting.top

[U52] PHP：箭头函数
来源：http://jsp.jqgfzy.top

$double = fn($x) => $x * 2;
来源：http://xcd.yanxiufei.cn

[U53] PHP：空合并运算符
来源：http://ifv.svipenyu.cn

$v = $a ?? $b ?? "default";
来源：http://dbw.ybcxt.top

[U54] PHP：空安全调用
来源：http://hvh.sufxvd.cn

$obj?->method()
来源：http://dmr.wangshuangyany.cn

[U55] PHP：match 表达式
来源：http://mzo.hysaishi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wit.zdqjudy.top

[U56] PHP：命名参数
来源：http://aor.cashguo.top

f(a: 1, b: 2)
来源：http://hij.cdnleiting.top

[U57] PHP：字符串插值
来源：http://lvm.quarkkingdee.top

"值: {$a}"
来源：http://tqs.jinqigufen.top

[U58] PHP：数组三件套
来源：http://axj.yj20258888.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tdc.chenzaomai.com

[U59] PHP：自定义排序
来源：http://gec.jianghu66.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ben.yangfankeji.com

[U60] PHP：JSON 编解码
来源：http://sou.guowangkeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bit.bbcook.cn

[U61] PHP：正则
来源：http://cjx.uphjek.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wet.havefunace.top

[U62] PHP：日期对象
来源：http://bux.dianchejie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pyk.zhongyouzk.top

[U63] PHP：文件读写
来源：http://tzk.hywenlv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kxw.zhijiandao.cn

[U64] PHP：目录遍历
来源：http://clf.meibo888.top

glob("dir/*.php");  scandir("dir");
来源：http://zfw.fehbvm.com

[U65] PHP：会话
来源：http://qus.cucudq.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kpd.chenzaomai.com

[U66] PHP：设置 Cookie
来源：http://szh.redwolf501.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qqz.hnxiangtu.top

[U67] PHP：处理文件上传
来源：http://oqp.daxiang520.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wya.yueranfly.top

[U68] PHP：PDO 连接
来源：http://rzb.zhixingplan.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lig.gotoacloud.top

[U69] PHP：PDO 预处理
来源：http://hot.fanxiaobao.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xii.yongpay.top

[U70] PHP：PDO 事务
来源：http://soq.shangyingyoupin.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bqs.mhx1999.top

[U71] PHP：抛出异常
来源：http://ruu.pengpengdd.cyou

throw new RuntimeException("失败", 500);
来源：http://spp.yj202588.top

[U72] PHP：写错误日志
来源：http://dly.redwolf501.top

error_log("失败: " . $e->getMessage());
来源：http://dqp.cheryme.top

[U73] PHP：读取 ini 配置
来源：http://zuk.zycfv.cn

parse_ini_file("config.ini", true)
来源：http://wcx.mhx1999.top

[U74] PHP：读取环境变量
来源：http://lel.jlsjyb.cn

getenv("APP_ENV") ?: "production"
来源：http://jin.0kj1m.cn

[U75] PHP：依赖注入
来源：http://jea.zdbjq.cn

composer require psr/container
来源：http://hjs.chenjidiqi.icu

[U76] PHP：简单路由
来源：http://uvr.tianlin.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://szl.ybcxt.top

[U77] PHP：模板渲染
来源：http://rae.ydzc1.top

composer require twig/twig
来源：http://hgf.yj20258888.top

[U78] PHP：单元测试
来源：http://rtg.epnwcf.com

composer require --dev phpunit/phpunit
来源：http://ens.ctjpmb.com

[U79] PHP：静态分析
来源：http://qeu.daria6918.cn

composer require --dev phpstan/phpstan
来源：http://azp.ivvv.top

[U80] PHP：代码规范修复
来源：http://vmr.chenlongwang.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://xtd.zycfv.cn

[U81] JS：初始化项目
来源：http://tgd.gzhubu.top

npm init -y;  npm i express
来源：http://xdj.zhengqikj.top

[U82] JS：package.json 脚本
来源：http://okf.chenlongwang.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xpx.ctjpmb.com

[U83] JS：ES Module 导入导出
来源：http://aup.hysaishi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pbb.hammf.cn

[U84] JS：CommonJS 写法
来源：http://yzz.jqgufenzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://ykz.bbcook.cn

[U85] JS：可选链
来源：http://jff.cashguo.top

a?.b?.c
来源：http://pxc.pycfn.com

[U86] JS：空值合并
来源：http://pxo.52xcode.cn

a ?? b
来源：http://vkx.zhiwuduotai.top

[U87] JS：解构默认值
来源：http://uit.ydzc1.top

const { a = 1, b = 2 } = obj;
来源：http://jus.sxryk.cn

[U88] JS：对象展开合并
来源：http://ean.sjlbkw.cn

{ ...a, ...b }
来源：http://fom.guowangkeji.top

[U89] JS：数组去重
来源：http://bgf.tarul.cn

[...new Set(arr)]
来源：http://ovl.xylfe.cn

[U90] JS：数字数组排序
来源：http://wbu.nanxuanxn.top

[...arr].sort((a, b) => a - b)
来源：http://dkk.cucudq.cn

[U91] JS：对象键值遍历
来源：http://cve.yj20258.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vnn.daria6918.cn

[U92] JS：深拷贝
来源：http://ztp.zdbjq.cn

structuredClone(obj)
来源：http://jir.hfpthk.cn

[U93] JS：模板字符串
来源：http://dnz.andypj.xyz

`共 ${n} 条`
来源：http://qnj.yuxming.cn

[U94] JS：箭头函数
来源：http://buj.chenlongwang.top

const double = x => x * 2;
来源：http://ykl.ppjwa.cn

[U95] JS：Promise 包装
来源：http://ygs.sjlbkw.cn

new Promise((resolve, reject) => {})
来源：http://lht.fktsv.cn

[U96] JS：async/await 与异常
来源：http://xvt.fengsongda.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mji.xuetiantiany.cn

[U97] JS：并发请求
来源：http://ngr.vqdsnc.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cys.quarkkingdee.top

[U98] JS：fetch 带 JSON
来源：http://itx.cheryme.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kvy.52xcode.cn

[U99] JS：事件监听
来源：http://rbu.yueranfly.top

el.addEventListener("click", e => {})
来源：http://xpm.zdqjudy.top

[U100] JS：DOM 查询
来源：http://wig.tanke756.top

document.querySelector(".item")
来源：http://hhh.sufxvd.cn

[U101] JS：classList 操作
来源：http://jvh.fanxiaobao.xyz

el.classList.toggle("active")
来源：http://zfs.ehwqpu.com

[U102] JS：本地存储
来源：http://xns.andypj.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://hql.aibaodan.cn

[U103] JS：定时器
来源：http://jof.jlsjyb.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sxu.uphjek.com

[U104] JS：防抖
来源：http://aqi.shanyushiyangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fmu.vqdsnc.cn

[U105] JS：节流
来源：http://pwq.zhijiandao.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tvy.hysaishi.cn

[U106] JS：日期格式化
来源：http://nzh.yfazqb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kak.cashguo.top

[U107] JS：数字千分位
来源：http://dkh.yonumen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bnc.haohaochexian.top

[U108] JS：随机整数
来源：http://oud.cdnleiting.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wwz.zycfv.cn

[U109] JS：数组分组
来源：http://pco.feifeiyinyue.top

Object.groupBy(arr, x => x.type)
来源：http://swj.xuetiantiany.cn

[U110] JS：数组分块
来源：http://lvz.jlsjyb.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jkd.zdqjudy.top

[U111] JS：对象转 Map
来源：http://vsh.gaohongyu789.top

new Map(Object.entries(obj))
来源：http://uub.epnwcf.com

[U112] JS：字符串补位
来源：http://nip.jqgfzy.top

"7".padStart(3, "0")
来源：http://qjp.ctjpmb.com

[U113] JS：正则替换全部
来源：http://qve.chenlongwang.top

s.replaceAll("a", "b")
来源：http://hjq.yueranfly.top

[U114] JS：JSON 深比较
来源：http://guo.zdqjudy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rps.fktsv.cn

[U115] JS：生成 UUID
来源：http://oar.yvedp.cn

crypto.randomUUID()
来源：http://dtn.xylfe.cn

[U116] JS：类型检查（JSDoc）
来源：http://yfu.zhijiandao.cn

/** @param {string} name */ function f(name) {}
来源：http://wsc.52xcode.cn

[U117] JS：单元测试
来源：http://ses.shanyushiyangkeji.top

npm i -D vitest;  npx vitest
来源：http://lor.tian-w.cn

[U118] JS：开发服务器
来源：http://fmd.fanxiaobao.xyz

npm i -D vite;  npx vite
来源：http://fuw.meibo888.top

[U119] JS：生产构建
来源：http://tlh.hnxiangtu.top

npx vite build
来源：http://iwy.daxiang520.top

[U120] JS：读取环境变量（Vite）
来源：http://oit.cqqwz.cn

import.meta.env.VITE_API_URL
来源：http://vex.shuidangran.top

================================================================================
来源：http://eds.vehdjk.com

统计汇总
来源：http://ans.bjfxy.top

================================================================================
来源：http://ogb.hammf.cn

按语言统计（条）：
来源：http://rht.havefunace.top

Python ......... 252
来源：http://eon.jyoumei.cn

PHP ............ 252
来源：http://uho.yanxiufei.cn

JavaScript ..... 252
来源：http://zvn.hongshengwenyu.top

TypeScript ..... 212
来源：http://zoz.tianlin.xyz

Java ........... 212
来源：http://enm.xziqi.cn

Go ............. 212
来源：http://qpd.sweek.top

Ruby ........... 212
来源：http://kpz.ctjpmb.com

C# ............. 212
来源：http://lpm.meibo888.top

C .............. 30
来源：http://rvo.hfpthk.cn

C++ ............ 30
来源：http://fwl.feifeiyinyue.top

SQL ............ 90
来源：http://rib.cheryme.top

Bash ........... 80
来源：http://mxo.xuetiantiany.cn

Kotlin ......... 15
来源：http://ind.ivvv.top

Swift .......... 15
来源：http://etu.0kj1m.cn

Lua ............ 10
来源：http://ahu.zycfv.cn

Perl ........... 10
来源：http://irq.ppjwa.cn

Scala .......... 10
来源：http://yrt.sjlbkw.cn

------------------------------------
来源：http://sev.ydzc1.top

合计 ........... 2106 条
来源：http://fgh.daxiang520.top

按章节统计：
来源：http://zze.yfazqb.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://iaq.hfpthk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qno.shuidangran.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hgf.cucudq.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tyf.daria6918.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hsz.vehdjk.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://umo.fanxiaobao.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ytf.cqqwz.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qlq.jianghu66.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ozs.ppjwa.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://grp.c1oappe.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hkx.zhaomingkeji.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mav.nwbrower.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tdx.yuxming.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bko.jinyuanbaomall.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://iml.hammf.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wvy.gzhubu.top

Q SQL 专题                              90
来源：http://crx.chenjidiqi.icu

R Bash 专题                             80
来源：http://lbi.316326.xyz

S C / C++ 专题                          60
来源：http://qfd.xinyue.icu

T 其他语言补充                          60
来源：http://lyb.daria6918.cn

U 高频实用片段                         120
来源：http://hpy.jiagoushi.top

------------------------------------
来源：http://kwk.jlsjyb.cn

合计                                  2106 条
来源：http://dsh.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://bki.hcnkem.com

使用提醒
来源：http://xxy.yueranfly.top

--------------------------------------------------------------------------------
来源：http://hja.hcnkem.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rhs.zhongyouzk.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gty.feifeiyinyue.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mes.feifeiyinyue.top

在旧版本上使用前请先确认语法支持情况。
来源：http://hdk.gogol.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tey.ctjpmb.com

—— 文件结束 ——
来源：http://ufn.daria6918.cn

================================================================================
来源：http://jis.feifeiyinyue.top

程序语言常见例子速查手册（2024 版）
来源：http://zxt.yongpay.top

Common Programming Examples Cheat Book
来源：http://alv.dianchejie.cn

================================================================================
来源：http://aug.zhoulong.xyz

【收录内容】
来源：http://piz.snrcjt.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rit.chenjidiqi.icu

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gqs.nanxuanxn.top

SQL · Bash · C · C++
来源：http://nxj.zhaomingkeji.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qbq.nwbrower.top

【使用说明】
来源：http://xfz.hongshengwenyu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pia.ybcxt.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fsn.ydjk.org.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hpv.havefunace.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vgj.birdmap.top

Bash:  Shell         C:     C             C++:   C++
来源：http://xsv.tian-w.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://itn.shangyingyoupin.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yot.hnqzz.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gop.yanxiufei.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mbt.iojbl.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://czn.sxryk.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hrq.bjfxy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qwf.tanke756.top

【文件统计】
来源：http://lii.vehdjk.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xvq.jiagoushi.top

--------------------------------------------------------------------------------
来源：http://ydq.yuxming.cn

目  录
来源：http://gyo.hesvh.cn

--------------------------------------------------------------------------------
来源：http://cmy.snrcjt.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zot.zhijiandao.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dqt.fktsv.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jdq.kuanghao11.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jrq.wangdashe.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ehj.zhongyouzk.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pfx.sufxvd.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rwz.zhijiandao.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bcn.hcnkem.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zva.cucudq.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://uco.jinghuilouyu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://iju.ivvv.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cvb.nanxuanxn.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cxu.yj20258.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://djr.xylfe.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://grp.svipenyu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qsl.cucudq.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gpl.hfpthk.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gbo.jinyuanbaomall.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ggl.ydjk.org.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nsl.guowangkeji.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zxj.svipenyu.cn

================================================================================
来源：http://dxx.chenjidiqi.icu

A. 基础语法与类型
来源：http://mtq.jqgfzy.top

================================================================================
来源：http://nus.meibo888.top

[A01] Hello World
来源：http://oka.jinyuanbaomall.cn

Py:   print("Hello, World!")
来源：http://wvl.xylfe.cn

PHP:  echo "Hello, World!";
来源：http://zqv.316326.xyz

JS:   console.log("Hello, World!");
来源：http://bur.ivvv.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://his.9152youxi.cn

Java: System.out.println("Hello, World!");
来源：http://gpn.iojbl.cn

Go:   fmt.Println("Hello, World!")
来源：http://afw.zhiwuduotai.top

Ruby: puts "Hello, World!"
来源：http://jxx.nanxinkj.top

C#:   Console.WriteLine("Hello, World!");
来源：http://opy.yj20258888.top

[A02] 变量声明与赋值
来源：http://npp.chenlongwang.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xev.ppjwa.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mml.jinqigufen.top

JS:   let name = "Alex"; const age = 20;
来源：http://ask.sysykeji.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vhr.fengsongda.top

Java: String name = "Alex"; int age = 20;
来源：http://ped.cqqwz.cn

Go:   name := "Alex"; age := 20
来源：http://kva.jinqigfzy.top

Ruby: name = "Alex"; age = 20
来源：http://ssl.shangyingyoupin.top

C#:   string name = "Alex"; int age = 20;
来源：http://ksp.yvedp.cn

[A03] 常量定义
来源：http://mnz.c1oappe.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ebq.hnxiangtu.top

PHP:  const PI = 3.14159;
来源：http://meh.hfpthk.cn

JS:   const PI = 3.14159;
来源：http://uyu.daxiang520.top

TS:   const PI: number = 3.14159;
来源：http://hix.yueranfly.top

Java: static final double PI = 3.14159;
来源：http://opx.zhaomingkeji.xyz

Go:   const PI = 3.14159
来源：http://kbh.gaohongyu789.top

Ruby: PI = 3.14159
来源：http://qyu.redwolf501.top

C#:   const double PI = 3.14159;
来源：http://mik.yj20258.top

[A04] 判断变量类型
来源：http://qlm.svipenyu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://lyo.xziqi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://iac.nwbrower.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://uva.dianchejie.cn

TS:   typeof x; x instanceof Date
来源：http://nez.yj20258.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hit.mhx1999.top

Go:   reflect.TypeOf(x).Name()
来源：http://hak.xylfe.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://zvt.jlsjyb.cn

C#:   x.GetType().Name; x is int
来源：http://azl.redwolf501.top

[A05] 整数除法与取模
来源：http://dde.fengsongda.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lrt.ppjwa.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qcf.tianlin.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pyl.havefunace.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bma.bjfxy.top

Java: 7 / 2; 7 % 2
来源：http://ilv.daria6918.cn

Go:   7 / 2; 7 % 2
来源：http://wnq.meibo888.top

Ruby: 7 / 2; 7 % 2
来源：http://vlj.yonumen.top

C#:   7 / 2; 7 % 2
来源：http://wft.ehwqpu.com

[A06] 字符串转数字
来源：http://bik.pengpengdd.cyou

Py:   int("42"); float("3.14")
来源：http://gli.sweek.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dny.cqqwz.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cth.chenjidiqi.icu

TS:   parseInt("42", 10); Number("42")
来源：http://rvq.yuxming.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ntc.xuetiantiany.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fhq.daxiang520.top

Ruby: "42".to_i; "3.14".to_f
来源：http://spa.sjlbkw.cn


<!-- 参考信息 -->