代发 wailian999

[U47] PHP：联合类型
来源：http://jqm.zhixingplan.top

int|string $id
来源：http://raw.dashuyun.cn

[U48] PHP：纯枚举
来源：http://zzq.gogol.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yyz.tarul.cn

[U49] PHP：只读属性
来源：http://dsa.tian-w.cn

public readonly string $name
来源：http://cbr.vqdsnc.cn

[U50] PHP：构造器属性提升
来源：http://xsa.jqgfzy.top

public function __construct(private int $id) {}
来源：http://dww.zhixingplan.top

[U51] PHP：数组解构
来源：http://euw.guannengcc.top

[$a, $b] = $arr;
来源：http://osr.zdbjq.cn

[U52] PHP：箭头函数
来源：http://edd.ydzc1.top

$double = fn($x) => $x * 2;
来源：http://wlg.yanxiufei.cn

[U53] PHP：空合并运算符
来源：http://fcj.kuanghao11.cn

$v = $a ?? $b ?? "default";
来源：http://yzh.yj20258888.top

[U54] PHP：空安全调用
来源：http://ztv.cashguo.top

$obj?->method()
来源：http://cfk.zdbjq.cn

[U55] PHP：match 表达式
来源：http://prs.vqdsnc.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qxs.zdbjq.cn

[U56] PHP：命名参数
来源：http://yhu.hammf.cn

f(a: 1, b: 2)
来源：http://kyf.jqgufenzy.top

[U57] PHP：字符串插值
来源：http://rzv.hnxiangtu.top

"值: {$a}"
来源：http://ghe.sweek.top

[U58] PHP：数组三件套
来源：http://aul.hysaishi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xji.yonumen.top

[U59] PHP：自定义排序
来源：http://cjd.ctjpmb.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jnf.yj20258888.top

[U60] PHP：JSON 编解码
来源：http://mzd.jinqigfzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hbs.xuetiantiany.cn

[U61] PHP：正则
来源：http://jxr.mhx1999.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ekm.guowangkeji.top

[U62] PHP：日期对象
来源：http://bbw.fanxiaobao.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://aie.zdqjudy.top

[U63] PHP：文件读写
来源：http://fyv.zhixingplan.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bdo.fengsongda.top

[U64] PHP：目录遍历
来源：http://gft.ivvv.top

glob("dir/*.php");  scandir("dir");
来源：http://hbe.nwbrower.top

[U65] PHP：会话
来源：http://tvg.nwbrower.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ixa.zycfv.cn

[U66] PHP：设置 Cookie
来源：http://lhe.fzhhl.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zat.zhengqikj.top

[U67] PHP：处理文件上传
来源：http://ynk.yvedp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hfx.guowangkeji.top

[U68] PHP：PDO 连接
来源：http://ijr.jlsjyb.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kmd.zycfv.cn

[U69] PHP：PDO 预处理
来源：http://wfc.yvedp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gzw.xinyue.icu

[U70] PHP：PDO 事务
来源：http://zpl.jinyuanbaomall.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dnd.zhiwuduotai.top

[U71] PHP：抛出异常
来源：http://bmb.meibo888.top

throw new RuntimeException("失败", 500);
来源：http://vkn.guowangkeji.top

[U72] PHP：写错误日志
来源：http://rau.gotoacloud.top

error_log("失败: " . $e->getMessage());
来源：http://ikf.yj20258888.top

[U73] PHP：读取 ini 配置
来源：http://kdg.yuanzhike.top

parse_ini_file("config.ini", true)
来源：http://zmg.bbcook.cn

[U74] PHP：读取环境变量
来源：http://bvb.kuanghao11.cn

getenv("APP_ENV") ?: "production"
来源：http://gsy.zhongyouzk.top

[U75] PHP：依赖注入
来源：http://bxs.hysaishi.cn

composer require psr/container
来源：http://odk.hfpthk.cn

[U76] PHP：简单路由
来源：http://gwg.nanxinkj.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mzi.ybcxt.top

[U77] PHP：模板渲染
来源：http://jxu.hammf.cn

composer require twig/twig
来源：http://cys.hammf.cn

[U78] PHP：单元测试
来源：http://rca.sufxvd.cn

composer require --dev phpunit/phpunit
来源：http://rfn.wangdashe.top

[U79] PHP：静态分析
来源：http://bwr.kuanghao11.cn

composer require --dev phpstan/phpstan
来源：http://qoh.zhaomingkeji.xyz

[U80] PHP：代码规范修复
来源：http://wbh.cucudq.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qla.hnqzz.top

[U81] JS：初始化项目
来源：http://opp.jyoumei.cn

npm init -y;  npm i express
来源：http://ueo.hywenlv.cn

[U82] JS：package.json 脚本
来源：http://tgz.shanyushiyangtech.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gho.jyoumei.cn

[U83] JS：ES Module 导入导出
来源：http://thc.vqdsnc.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zwz.yuxming.cn

[U84] JS：CommonJS 写法
来源：http://ppp.redwolf501.top

module.exports = { a };  const { a } = require("./m");
来源：http://ujj.meibo888.top

[U85] JS：可选链
来源：http://dlr.iojbl.cn

a?.b?.c
来源：http://dhu.jiagoushi.top

[U86] JS：空值合并
来源：http://ipr.xuanzx.com

a ?? b
来源：http://tkj.gogol.net.cn

[U87] JS：解构默认值
来源：http://bhh.fzhhl.top

const { a = 1, b = 2 } = obj;
来源：http://yda.hnxiangtu.top

[U88] JS：对象展开合并
来源：http://yhv.aibaodan.cn

{ ...a, ...b }
来源：http://iyq.sxryk.cn

[U89] JS：数组去重
来源：http://jjo.c1oappe.top

[...new Set(arr)]
来源：http://efd.mhx1999.top

[U90] JS：数字数组排序
来源：http://exx.guowangkeji.top

[...arr].sort((a, b) => a - b)
来源：http://ppf.0kj1m.cn

[U91] JS：对象键值遍历
来源：http://ucr.xingfuxueyuan.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gsq.hfpthk.cn

[U92] JS：深拷贝
来源：http://smv.cqqwz.cn

structuredClone(obj)
来源：http://pfv.xuanzx.com

[U93] JS：模板字符串
来源：http://lon.meibo888.top

`共 ${n} 条`
来源：http://vme.jinqigfzy.top

[U94] JS：箭头函数
来源：http://gnm.fzhhl.top

const double = x => x * 2;
来源：http://smr.tianlin.xyz

[U95] JS：Promise 包装
来源：http://fnu.wangdashe.top

new Promise((resolve, reject) => {})
来源：http://nol.ctjpmb.com

[U96] JS：async/await 与异常
来源：http://qpe.shangyingyoupin.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rep.fengsongda.top

[U97] JS：并发请求
来源：http://ehg.yvedp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lmc.xingfuxueyuan.xyz

[U98] JS：fetch 带 JSON
来源：http://xyx.tanke756.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bzk.zdqjudy.top

[U99] JS：事件监听
来源：http://pqe.uphjek.com

el.addEventListener("click", e => {})
来源：http://zhx.havefunace.top

[U100] JS：DOM 查询
来源：http://utw.fktsv.cn

document.querySelector(".item")
来源：http://exv.sweek.top

[U101] JS：classList 操作
来源：http://dku.dianchejie.cn

el.classList.toggle("active")
来源：http://ghn.tanke756.top

[U102] JS：本地存储
来源：http://asx.zhiwuduotai.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://pje.nanxinkj.top

[U103] JS：定时器
来源：http://uwt.ehwqpu.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tyn.yvedp.cn

[U104] JS：防抖
来源：http://lxz.aibaodan.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qqi.yj20258.top

[U105] JS：节流
来源：http://jcn.hcnkem.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dow.ivvv.top

[U106] JS：日期格式化
来源：http://cgo.wangdashe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ypd.chenzaomai.com

[U107] JS：数字千分位
来源：http://ulx.daxiang520.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nov.ydjk.org.cn

[U108] JS：随机整数
来源：http://osf.quarkkingdee.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tde.yuxming.cn

[U109] JS：数组分组
来源：http://lpu.quarkkingdee.top

Object.groupBy(arr, x => x.type)
来源：http://yyq.pengpengdd.cyou

[U110] JS：数组分块
来源：http://scm.wangdashe.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lfj.9152youxi.cn

[U111] JS：对象转 Map
来源：http://rnh.redwolf501.top

new Map(Object.entries(obj))
来源：http://tlg.cheryme.top

[U112] JS：字符串补位
来源：http://aim.xingfuxueyuan.xyz

"7".padStart(3, "0")
来源：http://nhi.zdbjq.cn

[U113] JS：正则替换全部
来源：http://pqf.jinyuanbaomall.cn

s.replaceAll("a", "b")
来源：http://ive.meibo888.top

[U114] JS：JSON 深比较
来源：http://cmi.ppjwa.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xgd.havefunace.top

[U115] JS：生成 UUID
来源：http://ubw.vqdsnc.cn

crypto.randomUUID()
来源：http://jnj.gaohongyu789.top

[U116] JS：类型检查（JSDoc）
来源：http://rlx.pycfn.com

/** @param {string} name */ function f(name) {}
来源：http://vwe.9152youxi.cn

[U117] JS：单元测试
来源：http://sbf.jlsjyb.cn

npm i -D vitest;  npx vitest
来源：http://qzp.sweek.top

[U118] JS：开发服务器
来源：http://fia.nwbrower.top

npm i -D vite;  npx vite
来源：http://cim.jqgfzy.top

[U119] JS：生产构建
来源：http://hvn.meibo888.top

npx vite build
来源：http://qgo.jinqigufen.top

[U120] JS：读取环境变量（Vite）
来源：http://avl.fehbvm.com

import.meta.env.VITE_API_URL
来源：http://bhn.yonumen.top

================================================================================
来源：http://hlr.zhiwuduotai.top

统计汇总
来源：http://zaq.tian-w.cn

================================================================================
来源：http://nxr.xziqi.cn

按语言统计（条）：
来源：http://xop.epnwcf.com

Python ......... 252
来源：http://abf.wangshuangyany.cn

PHP ............ 252
来源：http://fyn.zhengqikj.top

JavaScript ..... 252
来源：http://fti.gaohongyu789.top

TypeScript ..... 212
来源：http://bhz.jqgufenzy.top

Java ........... 212
来源：http://fiu.zhoulong.xyz

Go ............. 212
来源：http://mlc.sysykeji.top

Ruby ........... 212
来源：http://fyu.daria6918.cn

C# ............. 212
来源：http://mva.yongpay.top

C .............. 30
来源：http://lee.ehwqpu.com

C++ ............ 30
来源：http://bjc.jqgufenzy.top

SQL ............ 90
来源：http://rtk.yfazqb.com

Bash ........... 80
来源：http://vmu.zhaomingkeji.xyz

Kotlin ......... 15
来源：http://ybk.ehwqpu.com

Swift .......... 15
来源：http://rdd.ybcxt.top

Lua ............ 10
来源：http://lxi.cashguo.top

Perl ........... 10
来源：http://grn.snrcjt.cn

Scala .......... 10
来源：http://adr.sysykeji.top

------------------------------------
来源：http://nnt.jyoumei.cn

合计 ........... 2106 条
来源：http://jkc.sufxvd.cn

按章节统计：
来源：http://ggg.epnwcf.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tsk.fengsongda.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ufi.yfazqb.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://iuu.ehwqpu.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://twg.vehdjk.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zfb.hnqzz.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rlo.dashuyun.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wmq.tian-w.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zhb.gzhubu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nhj.snrcjt.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jsb.sufxvd.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fhx.gogol.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kud.yj20258888.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://acq.andypj.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://poo.redwolf501.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://viq.meibo888.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://luw.wangshuangyany.cn

Q SQL 专题                              90
来源：http://ldq.jinghuilouyu.cn

R Bash 专题                             80
来源：http://tkh.hywenlv.cn

S C / C++ 专题                          60
来源：http://jij.fzhhl.top

T 其他语言补充                          60
来源：http://uok.gaohongyu789.top

U 高频实用片段                         120
来源：http://obb.snrcjt.cn

------------------------------------
来源：http://aoy.aizwys.cn

合计                                  2106 条
来源：http://sct.gaohongyu789.top

--------------------------------------------------------------------------------
来源：http://pgt.zdqjudy.top

使用提醒
来源：http://jmq.316326.xyz

--------------------------------------------------------------------------------
来源：http://iei.daxiang520.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://okx.fanxiaobao.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fhy.guannengcc.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vpx.xuetiantiany.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ala.wangshuangyany.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://byz.zhoulong.xyz

—— 文件结束 ——
来源：http://amb.dashuyun.cn

================================================================================
来源：http://lbn.shangyingyoupin.top

程序语言常见例子速查手册（2024 版）
来源：http://ziy.xingfuxueyuan.xyz

Common Programming Examples Cheat Book
来源：http://nlt.yanxiufei.cn

================================================================================
来源：http://qwo.zhiwuduotai.top

【收录内容】
来源：http://pdn.jyoumei.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ucm.redwolf501.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://aes.yuxming.cn

SQL · Bash · C · C++
来源：http://gfc.pengpengdd.cyou

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uvp.yonumen.top

【使用说明】
来源：http://pne.yvedp.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://biz.epnwcf.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mhi.zycfv.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://oyx.daxiang520.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://oba.gogol.net.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zdr.jlsjyb.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yyb.fzhhl.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dud.vehdjk.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qtv.shangyingyoupin.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cvi.quarkkingdee.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fkb.yfazqb.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cpy.vehdjk.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mgo.xinyue.icu

【文件统计】
来源：http://ixj.pycfn.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xmj.wangdashe.top

--------------------------------------------------------------------------------
来源：http://iia.hongshengwenyu.top

目  录
来源：http://skd.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://iir.cucudq.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tjn.chenzaomai.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tuc.uphjek.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jtp.nanxinkj.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gir.hongshengwenyu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tai.wangdashe.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tmo.chenlongwang.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://knz.52xcode.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qdz.ydjk.org.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hkp.hesvh.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lqv.chenjidiqi.icu

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vaj.yueranfly.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hrf.zhongyouzk.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rwu.hesvh.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://sed.yj20258.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://clq.pengpengdd.cyou

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kwv.zhijiandao.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cyf.havefunace.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://efp.jyoumei.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://apv.sysykeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hsy.cqqwz.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mtg.ppjwa.cn

================================================================================
来源：http://wgm.hnqzz.top

A. 基础语法与类型
来源：http://ebd.nwbrower.top

================================================================================
来源：http://pwy.yj202588.top

[A01] Hello World
来源：http://yaw.fanxiaobao.xyz

Py:   print("Hello, World!")
来源：http://bhm.ydjk.org.cn

PHP:  echo "Hello, World!";
来源：http://lac.havefunace.top

JS:   console.log("Hello, World!");
来源：http://dgs.fktsv.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uys.gogol.net.cn

Java: System.out.println("Hello, World!");
来源：http://hum.9152youxi.cn

Go:   fmt.Println("Hello, World!")
来源：http://nyp.svipenyu.cn

Ruby: puts "Hello, World!"
来源：http://eas.jqgfzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://wou.hammf.cn

[A02] 变量声明与赋值
来源：http://ucb.chenjidiqi.icu

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dwk.52xcode.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zkm.tianlin.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://mei.gotoacloud.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ixa.hywenlv.cn

Java: String name = "Alex"; int age = 20;
来源：http://zxv.zhiwuduotai.top

Go:   name := "Alex"; age := 20
来源：http://kkp.gzhubu.top

Ruby: name = "Alex"; age = 20
来源：http://mcl.pengpengdd.cyou

C#:   string name = "Alex"; int age = 20;
来源：http://tpc.svipenyu.cn

[A03] 常量定义
来源：http://yja.yongpay.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qdc.zhaomingkeji.xyz

PHP:  const PI = 3.14159;
来源：http://but.chenlongwang.top

JS:   const PI = 3.14159;
来源：http://nim.jianghu66.top

TS:   const PI: number = 3.14159;
来源：http://rmp.yvedp.cn

Java: static final double PI = 3.14159;
来源：http://cuz.feifeiyinyue.top

Go:   const PI = 3.14159
来源：http://tkf.bbcook.cn

Ruby: PI = 3.14159
来源：http://wyw.sufxvd.cn

C#:   const double PI = 3.14159;
来源：http://uke.tarul.cn

[A04] 判断变量类型
来源：http://vvi.chenlongwang.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://bga.gzhubu.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ocu.haohaochexian.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rgt.snrcjt.cn

TS:   typeof x; x instanceof Date
来源：http://djr.ehwqpu.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ttc.shanyushiyangkeji.top

Go:   reflect.TypeOf(x).Name()
来源：http://ujm.zdbjq.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qim.xziqi.cn

C#:   x.GetType().Name; x is int
来源：http://cuq.yj20258888.top

[A05] 整数除法与取模
来源：http://dht.ctjpmb.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vjq.xuetiantiany.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://leh.dashuyun.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bxd.zhixingplan.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fxk.sjlbkw.cn

Java: 7 / 2; 7 % 2
来源：http://ecu.shangyingyoupin.top

Go:   7 / 2; 7 % 2
来源：http://jsz.hfpthk.cn

Ruby: 7 / 2; 7 % 2
来源：http://ndm.gaohongyu789.top

C#:   7 / 2; 7 % 2
来源：http://qhn.xuanzx.com


<!-- 参考信息 -->