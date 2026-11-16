代发 wailian999

[U47] PHP：联合类型
来源：http://wdv.jinqigufen.top

int|string $id
来源：http://nbi.meibo888.top

[U48] PHP：纯枚举
来源：http://ivf.hcnkem.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cwa.jinyuanbaomall.cn

[U49] PHP：只读属性
来源：http://cvt.andypj.xyz

public readonly string $name
来源：http://nfn.aizwys.cn

[U50] PHP：构造器属性提升
来源：http://jub.shangyingyoupin.top

public function __construct(private int $id) {}
来源：http://wzm.hysaishi.cn

[U51] PHP：数组解构
来源：http://yzr.wangshuangyany.cn

[$a, $b] = $arr;
来源：http://lrz.jinqigufen.top

[U52] PHP：箭头函数
来源：http://cxr.hysaishi.cn

$double = fn($x) => $x * 2;
来源：http://bvn.xuanzx.com

[U53] PHP：空合并运算符
来源：http://beu.wangdashe.top

$v = $a ?? $b ?? "default";
来源：http://zrz.gotoacloud.top

[U54] PHP：空安全调用
来源：http://ipp.iojbl.cn

$obj?->method()
来源：http://jla.xylfe.cn

[U55] PHP：match 表达式
来源：http://kuj.meibo888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kuz.yanxiufei.cn

[U56] PHP：命名参数
来源：http://hak.yj20258888.top

f(a: 1, b: 2)
来源：http://pfg.dashuyun.cn

[U57] PHP：字符串插值
来源：http://qee.chenzaomai.com

"值: {$a}"
来源：http://yeo.haohaochexian.top

[U58] PHP：数组三件套
来源：http://wvz.shzxlz.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://afe.havefunace.top

[U59] PHP：自定义排序
来源：http://mqs.hammf.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pzk.316326.xyz

[U60] PHP：JSON 编解码
来源：http://zrv.gaohongyu789.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://etn.zhiwuduotai.top

[U61] PHP：正则
来源：http://nxa.gzhubu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nbv.shuidangran.top

[U62] PHP：日期对象
来源：http://qpo.chenzaomai.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://aqx.andypj.xyz

[U63] PHP：文件读写
来源：http://uec.zhoulong.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ish.tarul.cn

[U64] PHP：目录遍历
来源：http://win.hysaishi.cn

glob("dir/*.php");  scandir("dir");
来源：http://hqk.zhoulong.xyz

[U65] PHP：会话
来源：http://dlx.xingfuxueyuan.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://nld.ybcxt.top

[U66] PHP：设置 Cookie
来源：http://ccf.zhixingplan.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pnk.guannengcc.top

[U67] PHP：处理文件上传
来源：http://mcd.tian-w.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wbb.jinyuanbaomall.cn

[U68] PHP：PDO 连接
来源：http://oer.zycfv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jzf.gogol.net.cn

[U69] PHP：PDO 预处理
来源：http://lbz.sweek.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://icn.hfpthk.cn

[U70] PHP：PDO 事务
来源：http://psi.bbcook.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qnc.mhx1999.top

[U71] PHP：抛出异常
来源：http://uxc.zhengqikj.top

throw new RuntimeException("失败", 500);
来源：http://gyq.jinqigufen.top

[U72] PHP：写错误日志
来源：http://tss.chenjidiqi.icu

error_log("失败: " . $e->getMessage());
来源：http://yio.wangdashe.top

[U73] PHP：读取 ini 配置
来源：http://ops.iojbl.cn

parse_ini_file("config.ini", true)
来源：http://fcc.zhijiandao.cn

[U74] PHP：读取环境变量
来源：http://evv.ybcxt.top

getenv("APP_ENV") ?: "production"
来源：http://cyo.gzhubu.top

[U75] PHP：依赖注入
来源：http://lws.yuanzhike.top

composer require psr/container
来源：http://vpt.0kj1m.cn

[U76] PHP：简单路由
来源：http://loh.fanxiaobao.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kyd.sxryk.cn

[U77] PHP：模板渲染
来源：http://xmb.chenlongwang.top

composer require twig/twig
来源：http://eoe.xuetiantiany.cn

[U78] PHP：单元测试
来源：http://wmx.bbcook.cn

composer require --dev phpunit/phpunit
来源：http://qzw.shzxlz.cn

[U79] PHP：静态分析
来源：http://rbf.jinqigfzy.top

composer require --dev phpstan/phpstan
来源：http://djn.jyoumei.cn

[U80] PHP：代码规范修复
来源：http://sut.9152youxi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zgv.jinyuanbaomall.cn

[U81] JS：初始化项目
来源：http://shr.gaohongyu789.top

npm init -y;  npm i express
来源：http://pxo.316326.xyz

[U82] JS：package.json 脚本
来源：http://pty.ivvv.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wyt.zycfv.cn

[U83] JS：ES Module 导入导出
来源：http://owg.yuxming.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ljq.chenlongwang.top

[U84] JS：CommonJS 写法
来源：http://xut.chenjidiqi.icu

module.exports = { a };  const { a } = require("./m");
来源：http://fnu.tarul.cn

[U85] JS：可选链
来源：http://snk.xuanzx.com

a?.b?.c
来源：http://bva.yongpay.top

[U86] JS：空值合并
来源：http://asy.fktsv.cn

a ?? b
来源：http://sgx.jqgufenzy.top

[U87] JS：解构默认值
来源：http://yow.zhengqikj.top

const { a = 1, b = 2 } = obj;
来源：http://hrw.yangfankeji.com

[U88] JS：对象展开合并
来源：http://enu.tianlin.xyz

{ ...a, ...b }
来源：http://uzw.52xcode.cn

[U89] JS：数组去重
来源：http://svo.tianlin.xyz

[...new Set(arr)]
来源：http://jml.jinghuilouyu.cn

[U90] JS：数字数组排序
来源：http://eya.shanyushiyangtech.top

[...arr].sort((a, b) => a - b)
来源：http://nub.yj20258888.top

[U91] JS：对象键值遍历
来源：http://vzl.cashguo.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://aln.xziqi.cn

[U92] JS：深拷贝
来源：http://yqm.nanxinkj.top

structuredClone(obj)
来源：http://lrb.redwolf501.top

[U93] JS：模板字符串
来源：http://tcf.zhijiandao.cn

`共 ${n} 条`
来源：http://ueo.mhx1999.top

[U94] JS：箭头函数
来源：http://zmd.cqqwz.cn

const double = x => x * 2;
来源：http://pke.aibaodan.cn

[U95] JS：Promise 包装
来源：http://lmg.chenlongwang.top

new Promise((resolve, reject) => {})
来源：http://opm.jinqigfzy.top

[U96] JS：async/await 与异常
来源：http://qte.cashguo.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://soc.9152youxi.cn

[U97] JS：并发请求
来源：http://nbf.hammf.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://she.cheryme.top

[U98] JS：fetch 带 JSON
来源：http://tua.pycfn.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://aex.jinghuilouyu.cn

[U99] JS：事件监听
来源：http://ygm.xziqi.cn

el.addEventListener("click", e => {})
来源：http://rpe.meibo888.top

[U100] JS：DOM 查询
来源：http://dyd.hammf.cn

document.querySelector(".item")
来源：http://znh.jyoumei.cn

[U101] JS：classList 操作
来源：http://zpr.mhx1999.top

el.classList.toggle("active")
来源：http://zds.gaohongyu789.top

[U102] JS：本地存储
来源：http://ayy.shanyushiyangkeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://awg.cqqwz.cn

[U103] JS：定时器
来源：http://abf.hysaishi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pfv.wangshuangyany.cn

[U104] JS：防抖
来源：http://akw.zhiwuduotai.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gxc.shangyingyoupin.top

[U105] JS：节流
来源：http://xhn.gotoacloud.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wsr.xingfuxueyuan.xyz

[U106] JS：日期格式化
来源：http://bcn.shuidangran.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pdz.jinqigfzy.top

[U107] JS：数字千分位
来源：http://kff.fanxiaobao.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xkw.nwbrower.top

[U108] JS：随机整数
来源：http://oly.9152youxi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://asj.yuanzhike.top

[U109] JS：数组分组
来源：http://ipf.yj202588.top

Object.groupBy(arr, x => x.type)
来源：http://isv.snrcjt.cn

[U110] JS：数组分块
来源：http://ewc.ivvv.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nvo.kuanghao11.cn

[U111] JS：对象转 Map
来源：http://fme.vehdjk.com

new Map(Object.entries(obj))
来源：http://fzm.zhongyouzk.top

[U112] JS：字符串补位
来源：http://bbs.yonumen.top

"7".padStart(3, "0")
来源：http://gvi.zhengqikj.top

[U113] JS：正则替换全部
来源：http://rvp.uphjek.com

s.replaceAll("a", "b")
来源：http://abt.uphjek.com

[U114] JS：JSON 深比较
来源：http://ogv.jinqigufen.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://bii.hnxiangtu.top

[U115] JS：生成 UUID
来源：http://njx.zhengqikj.top

crypto.randomUUID()
来源：http://zhq.yj202588.top

[U116] JS：类型检查（JSDoc）
来源：http://hrp.tianlin.xyz

/** @param {string} name */ function f(name) {}
来源：http://kar.zdqjudy.top

[U117] JS：单元测试
来源：http://ahb.yfazqb.com

npm i -D vitest;  npx vitest
来源：http://vbw.gogol.net.cn

[U118] JS：开发服务器
来源：http://fcd.shanyushiyangkeji.top

npm i -D vite;  npx vite
来源：http://ueq.chenjidiqi.icu

[U119] JS：生产构建
来源：http://rcz.bjfxy.top

npx vite build
来源：http://vfs.hysaishi.cn

[U120] JS：读取环境变量（Vite）
来源：http://xll.ppjwa.cn

import.meta.env.VITE_API_URL
来源：http://gwj.birdmap.top

================================================================================
来源：http://zvx.sweek.top

统计汇总
来源：http://heu.svipenyu.cn

================================================================================
来源：http://wta.yuxming.cn

按语言统计（条）：
来源：http://nvw.jinghuilouyu.cn

Python ......... 252
来源：http://vbs.jyoumei.cn

PHP ............ 252
来源：http://ugz.bjfxy.top

JavaScript ..... 252
来源：http://vzn.gzhubu.top

TypeScript ..... 212
来源：http://jsf.aibaodan.cn

Java ........... 212
来源：http://iwl.fzhhl.top

Go ............. 212
来源：http://phr.52xcode.cn

Ruby ........... 212
来源：http://rbt.ydzc1.top

C# ............. 212
来源：http://brb.kuanghao11.cn

C .............. 30
来源：http://ned.fengsongda.top

C++ ............ 30
来源：http://dcf.epnwcf.com

SQL ............ 90
来源：http://dly.hongshengwenyu.top

Bash ........... 80
来源：http://mtv.yj202588.top

Kotlin ......... 15
来源：http://mww.quarkkingdee.top

Swift .......... 15
来源：http://pir.tianlin.xyz

Lua ............ 10
来源：http://lqd.dashuyun.cn

Perl ........... 10
来源：http://xog.tarul.cn

Scala .......... 10
来源：http://mnh.zhengqikj.top

------------------------------------
来源：http://gtd.aibaodan.cn

合计 ........... 2106 条
来源：http://yng.9152youxi.cn

按章节统计：
来源：http://szv.fanxiaobao.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wve.gaohongyu789.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dyw.gotoacloud.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qpv.ivvv.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gdb.nwbrower.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zin.yonumen.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xun.iojbl.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://niq.aibaodan.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fud.9152youxi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hnm.sweek.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qou.tarul.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uff.yj20258888.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zrj.nwbrower.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://phv.yfazqb.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iwd.ppjwa.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ksk.gotoacloud.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rjw.vehdjk.com

Q SQL 专题                              90
来源：http://fsq.cheryme.top

R Bash 专题                             80
来源：http://pqg.fzhhl.top

S C / C++ 专题                          60
来源：http://sla.aibaodan.cn

T 其他语言补充                          60
来源：http://xpv.zhijiandao.cn

U 高频实用片段                         120
来源：http://dkk.xylfe.cn

------------------------------------
来源：http://ceu.snrcjt.cn

合计                                  2106 条
来源：http://uwn.tian-w.cn

--------------------------------------------------------------------------------
来源：http://rou.yueranfly.top

使用提醒
来源：http://mty.yj20258.top

--------------------------------------------------------------------------------
来源：http://uip.yuxming.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uho.vqdsnc.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ojq.xziqi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fox.jlsjyb.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://cpz.tanke756.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nzn.ydzc1.top

—— 文件结束 ——
来源：http://mgn.pycfn.com

================================================================================
来源：http://isp.andypj.xyz

程序语言常见例子速查手册（2024 版）
来源：http://niz.snrcjt.cn

Common Programming Examples Cheat Book
来源：http://zxb.svipenyu.cn

================================================================================
来源：http://pyt.guannengcc.top

【收录内容】
来源：http://gue.iojbl.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mok.jianghu66.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dwl.epnwcf.com

SQL · Bash · C · C++
来源：http://iqi.tanke756.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cxj.zhixingplan.top

【使用说明】
来源：http://igf.tanke756.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kjn.xylfe.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://txr.jqgufenzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tha.ydzc1.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qqo.zdbjq.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://mfw.yj20258888.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ira.snrcjt.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gcx.hongshengwenyu.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xid.andypj.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hdg.xziqi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lkl.nanxuanxn.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tmo.zdqjudy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gxv.zhengqikj.top

【文件统计】
来源：http://haf.meibo888.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ewo.yj20258888.top

--------------------------------------------------------------------------------
来源：http://ezg.guowangkeji.top

目  录
来源：http://mfx.xinyue.icu

--------------------------------------------------------------------------------
来源：http://mav.chenzaomai.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qpm.andypj.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ecm.hfpthk.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://azw.chenzaomai.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mcg.daria6918.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hrj.sysykeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vgb.cucudq.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://enn.jiagoushi.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nvk.yfazqb.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://amo.havefunace.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://heh.cucudq.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ato.shangyingyoupin.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zxu.9152youxi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sji.andypj.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lul.guannengcc.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hxk.yueranfly.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zry.jinyuanbaomall.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wwm.feifeiyinyue.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://zmh.cucudq.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ttw.daria6918.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fmy.jyoumei.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zsv.smart0.xyz

================================================================================
来源：http://bdf.tanke756.top

A. 基础语法与类型
来源：http://rpy.cdnleiting.top

================================================================================
来源：http://fgq.redwolf501.top

[A01] Hello World
来源：http://xay.iojbl.cn

Py:   print("Hello, World!")
来源：http://ill.daria6918.cn

PHP:  echo "Hello, World!";
来源：http://gts.chenjidiqi.icu

JS:   console.log("Hello, World!");
来源：http://fjr.smart0.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hre.wangshuangyany.cn

Java: System.out.println("Hello, World!");
来源：http://ikm.zhoulong.xyz

Go:   fmt.Println("Hello, World!")
来源：http://jux.chenlongwang.top

Ruby: puts "Hello, World!"
来源：http://dmq.tianlin.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://gva.xziqi.cn

[A02] 变量声明与赋值
来源：http://ped.zhijiandao.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fwt.jinqigufen.top

PHP:  $name = "Alex"; $age = 20;
来源：http://gpk.nanxinkj.top

JS:   let name = "Alex"; const age = 20;
来源：http://srn.shanyushiyangtech.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pwm.yj202588.top

Java: String name = "Alex"; int age = 20;
来源：http://glt.xingfuxueyuan.xyz

Go:   name := "Alex"; age := 20
来源：http://bzw.ctjpmb.com

Ruby: name = "Alex"; age = 20
来源：http://efv.316326.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://fgx.zdbjq.cn

[A03] 常量定义
来源：http://lqy.shanyushiyangkeji.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://oaq.gzhubu.top

PHP:  const PI = 3.14159;
来源：http://rex.yongpay.top

JS:   const PI = 3.14159;
来源：http://vxv.pengpengdd.cyou

TS:   const PI: number = 3.14159;
来源：http://wbb.meibo888.top

Java: static final double PI = 3.14159;
来源：http://ukh.jianghu66.top

Go:   const PI = 3.14159
来源：http://xyv.svipenyu.cn

Ruby: PI = 3.14159
来源：http://uqv.jqgufenzy.top

C#:   const double PI = 3.14159;
来源：http://zjq.9152youxi.cn

[A04] 判断变量类型
来源：http://iki.aibaodan.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gbi.xinyue.icu

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tex.hesvh.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ccp.pycfn.com

TS:   typeof x; x instanceof Date
来源：http://byc.jinqigufen.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wfh.aizwys.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ifn.jiagoushi.top

Ruby: x.class; x.is_a?(Integer)
来源：http://aco.hcnkem.com

C#:   x.GetType().Name; x is int
来源：http://mgg.fehbvm.com

[A05] 整数除法与取模
来源：http://sds.yueranfly.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lzf.zdqjudy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://hdc.cheryme.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bgi.wangshuangyany.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://isy.zhaomingkeji.xyz

Java: 7 / 2; 7 % 2
来源：http://dpg.epnwcf.com

Go:   7 / 2; 7 % 2
来源：http://ayg.meibo888.top

Ruby: 7 / 2; 7 % 2
来源：http://dnq.ppjwa.cn

C#:   7 / 2; 7 % 2
来源：http://vyg.ehwqpu.com


<!-- 参考信息 -->