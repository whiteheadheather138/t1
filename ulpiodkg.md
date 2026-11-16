代发 wailian999

[U47] PHP：联合类型
来源：http://uiy.jlsjyb.cn

int|string $id
来源：http://dzf.zhiwuduotai.top

[U48] PHP：纯枚举
来源：http://kbl.yueranfly.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nsk.ehwqpu.com

[U49] PHP：只读属性
来源：http://wnc.nanxuanxn.top

public readonly string $name
来源：http://vaj.yuxming.cn

[U50] PHP：构造器属性提升
来源：http://oxg.bjfxy.top

public function __construct(private int $id) {}
来源：http://vho.wangdashe.top

[U51] PHP：数组解构
来源：http://ian.jqgufenzy.top

[$a, $b] = $arr;
来源：http://kdm.xziqi.cn

[U52] PHP：箭头函数
来源：http://lgj.sweek.top

$double = fn($x) => $x * 2;
来源：http://iyf.hywenlv.cn

[U53] PHP：空合并运算符
来源：http://wul.jinghuilouyu.cn

$v = $a ?? $b ?? "default";
来源：http://gbd.smart0.xyz

[U54] PHP：空安全调用
来源：http://wdw.sweek.top

$obj?->method()
来源：http://lbt.ppjwa.cn

[U55] PHP：match 表达式
来源：http://cpt.ivvv.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bjz.jinghuilouyu.cn

[U56] PHP：命名参数
来源：http://lpu.zdbjq.cn

f(a: 1, b: 2)
来源：http://lzi.yvedp.cn

[U57] PHP：字符串插值
来源：http://lre.316326.xyz

"值: {$a}"
来源：http://bee.yanxiufei.cn

[U58] PHP：数组三件套
来源：http://ugx.shanyushiyangkeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://odu.316326.xyz

[U59] PHP：自定义排序
来源：http://zwp.fehbvm.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nkw.xziqi.cn

[U60] PHP：JSON 编解码
来源：http://mve.mhx1999.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mes.zhaomingkeji.xyz

[U61] PHP：正则
来源：http://wkp.nanxuanxn.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vqr.yuanzhike.top

[U62] PHP：日期对象
来源：http://hjg.guannengcc.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mba.guowangkeji.top

[U63] PHP：文件读写
来源：http://aeb.vqdsnc.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hqe.nanxuanxn.top

[U64] PHP：目录遍历
来源：http://xxg.daxiang520.top

glob("dir/*.php");  scandir("dir");
来源：http://xhi.yuxming.cn

[U65] PHP：会话
来源：http://fld.cucudq.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://crx.ydzc1.top

[U66] PHP：设置 Cookie
来源：http://uai.redwolf501.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qcp.yonumen.top

[U67] PHP：处理文件上传
来源：http://gcb.sjlbkw.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oxi.cashguo.top

[U68] PHP：PDO 连接
来源：http://ieq.zhongyouzk.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kqn.bjfxy.top

[U69] PHP：PDO 预处理
来源：http://vdt.havefunace.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tgj.kuanghao11.cn

[U70] PHP：PDO 事务
来源：http://vmr.hfpthk.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lzx.yvedp.cn

[U71] PHP：抛出异常
来源：http://ndg.jyoumei.cn

throw new RuntimeException("失败", 500);
来源：http://pyw.hywenlv.cn

[U72] PHP：写错误日志
来源：http://plw.9152youxi.cn

error_log("失败: " . $e->getMessage());
来源：http://ipp.aizwys.cn

[U73] PHP：读取 ini 配置
来源：http://gsv.tian-w.cn

parse_ini_file("config.ini", true)
来源：http://moi.yuxming.cn

[U74] PHP：读取环境变量
来源：http://qea.tarul.cn

getenv("APP_ENV") ?: "production"
来源：http://ieo.chenjidiqi.icu

[U75] PHP：依赖注入
来源：http://mgp.daria6918.cn

composer require psr/container
来源：http://pxa.cqqwz.cn

[U76] PHP：简单路由
来源：http://rek.mhx1999.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vfw.jinqigufen.top

[U77] PHP：模板渲染
来源：http://bss.epnwcf.com

composer require twig/twig
来源：http://jif.9152youxi.cn

[U78] PHP：单元测试
来源：http://eak.yvedp.cn

composer require --dev phpunit/phpunit
来源：http://clp.daria6918.cn

[U79] PHP：静态分析
来源：http://apt.ivvv.top

composer require --dev phpstan/phpstan
来源：http://nyk.jinqigfzy.top

[U80] PHP：代码规范修复
来源：http://qcu.yuxming.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://crs.hnqzz.top

[U81] JS：初始化项目
来源：http://boq.yueranfly.top

npm init -y;  npm i express
来源：http://mxl.ivvv.top

[U82] JS：package.json 脚本
来源：http://xit.zhongyouzk.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uwy.iojbl.cn

[U83] JS：ES Module 导入导出
来源：http://spx.xylfe.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bxe.zhoulong.xyz

[U84] JS：CommonJS 写法
来源：http://gnv.shangyingyoupin.top

module.exports = { a };  const { a } = require("./m");
来源：http://feu.sxryk.cn

[U85] JS：可选链
来源：http://lgg.mhx1999.top

a?.b?.c
来源：http://wlf.chenzaomai.com

[U86] JS：空值合并
来源：http://rrj.jqgufenzy.top

a ?? b
来源：http://yyx.vqdsnc.cn

[U87] JS：解构默认值
来源：http://mje.yonumen.top

const { a = 1, b = 2 } = obj;
来源：http://bmj.shuidangran.top

[U88] JS：对象展开合并
来源：http://nxz.wangshuangyany.cn

{ ...a, ...b }
来源：http://hhz.fehbvm.com

[U89] JS：数组去重
来源：http://umy.meibo888.top

[...new Set(arr)]
来源：http://xis.yj202588.top

[U90] JS：数字数组排序
来源：http://zyv.bbcook.cn

[...arr].sort((a, b) => a - b)
来源：http://fso.zycfv.cn

[U91] JS：对象键值遍历
来源：http://sgs.ywan-chungtsiang.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gyl.fktsv.cn

[U92] JS：深拷贝
来源：http://hyt.yj20258.top

structuredClone(obj)
来源：http://uyj.cucudq.cn

[U93] JS：模板字符串
来源：http://ywi.zhiwuduotai.top

`共 ${n} 条`
来源：http://sgc.snrcjt.cn

[U94] JS：箭头函数
来源：http://jnj.zhoulong.xyz

const double = x => x * 2;
来源：http://uke.xuetiantiany.cn

[U95] JS：Promise 包装
来源：http://atr.tianlin.xyz

new Promise((resolve, reject) => {})
来源：http://ajo.haohaochexian.top

[U96] JS：async/await 与异常
来源：http://bof.yvedp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fws.birdmap.top

[U97] JS：并发请求
来源：http://moc.guowangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://qwn.iojbl.cn

[U98] JS：fetch 带 JSON
来源：http://jcm.wangdashe.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xxr.fzhhl.top

[U99] JS：事件监听
来源：http://ati.wangdashe.top

el.addEventListener("click", e => {})
来源：http://qex.zhixingplan.top

[U100] JS：DOM 查询
来源：http://ego.ctjpmb.com

document.querySelector(".item")
来源：http://cdj.pycfn.com

[U101] JS：classList 操作
来源：http://pis.uphjek.com

el.classList.toggle("active")
来源：http://gpb.hammf.cn

[U102] JS：本地存储
来源：http://jgf.hfpthk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bgf.yj20258888.top

[U103] JS：定时器
来源：http://mnx.shanyushiyangkeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ywk.fzhhl.top

[U104] JS：防抖
来源：http://yrx.shzxlz.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eim.havefunace.top

[U105] JS：节流
来源：http://iox.shangyingyoupin.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mlc.ydjk.org.cn

[U106] JS：日期格式化
来源：http://dpo.jiagoushi.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ckz.zycfv.cn

[U107] JS：数字千分位
来源：http://xju.yuanzhike.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vzq.cdnleiting.top

[U108] JS：随机整数
来源：http://trp.jqgfzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://njw.guannengcc.top

[U109] JS：数组分组
来源：http://wfx.bbcook.cn

Object.groupBy(arr, x => x.type)
来源：http://vth.iojbl.cn

[U110] JS：数组分块
来源：http://mcr.zhijiandao.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ize.zhaomingkeji.xyz

[U111] JS：对象转 Map
来源：http://xvy.xinyue.icu

new Map(Object.entries(obj))
来源：http://jca.tanke756.top

[U112] JS：字符串补位
来源：http://kil.zdbjq.cn

"7".padStart(3, "0")
来源：http://oel.ehwqpu.com

[U113] JS：正则替换全部
来源：http://xxq.hysaishi.cn

s.replaceAll("a", "b")
来源：http://qbz.zdqjudy.top

[U114] JS：JSON 深比较
来源：http://amo.jinyuanbaomall.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://npk.smart0.xyz

[U115] JS：生成 UUID
来源：http://gdp.redwolf501.top

crypto.randomUUID()
来源：http://ixo.dashuyun.cn

[U116] JS：类型检查（JSDoc）
来源：http://qlc.fehbvm.com

/** @param {string} name */ function f(name) {}
来源：http://eky.cheryme.top

[U117] JS：单元测试
来源：http://czl.jyoumei.cn

npm i -D vitest;  npx vitest
来源：http://xtm.gotoacloud.top

[U118] JS：开发服务器
来源：http://pfy.guannengcc.top

npm i -D vite;  npx vite
来源：http://cff.zhijiandao.cn

[U119] JS：生产构建
来源：http://ixf.yj20258.top

npx vite build
来源：http://jtb.hywenlv.cn

[U120] JS：读取环境变量（Vite）
来源：http://syk.ehwqpu.com

import.meta.env.VITE_API_URL
来源：http://mcf.pycfn.com

================================================================================
来源：http://qhk.cashguo.top

统计汇总
来源：http://gfm.hfpthk.cn

================================================================================
来源：http://ajc.pengpengdd.cyou

按语言统计（条）：
来源：http://hts.c1oappe.top

Python ......... 252
来源：http://vrx.xuetiantiany.cn

PHP ............ 252
来源：http://fqg.hesvh.cn

JavaScript ..... 252
来源：http://sfv.epnwcf.com

TypeScript ..... 212
来源：http://sge.yfazqb.com

Java ........... 212
来源：http://pvy.uphjek.com

Go ............. 212
来源：http://bnk.jlsjyb.cn

Ruby ........... 212
来源：http://dph.ehwqpu.com

C# ............. 212
来源：http://axn.fehbvm.com

C .............. 30
来源：http://ckg.pycfn.com

C++ ............ 30
来源：http://qga.gogol.net.cn

SQL ............ 90
来源：http://rll.wangshuangyany.cn

Bash ........... 80
来源：http://bwk.kuanghao11.cn

Kotlin ......... 15
来源：http://cii.xingfuxueyuan.xyz

Swift .......... 15
来源：http://ohn.zhijiandao.cn

Lua ............ 10
来源：http://mur.chenjidiqi.icu

Perl ........... 10
来源：http://bdl.snrcjt.cn

Scala .......... 10
来源：http://zvd.zhaomingkeji.xyz

------------------------------------
来源：http://naj.hcnkem.com

合计 ........... 2106 条
来源：http://uix.hysaishi.cn

按章节统计：
来源：http://hax.meibo888.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ygi.jinyuanbaomall.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kyp.shanyushiyangkeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tqd.yongpay.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ttb.jqgufenzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rcf.xziqi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pun.ydzc1.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jac.yfazqb.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://eaq.nanxinkj.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bug.xuanzx.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://glv.ydzc1.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://eah.zycfv.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xvi.zhaomingkeji.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bcg.nanxuanxn.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cip.gotoacloud.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fzf.zhixingplan.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oos.yj20258888.top

Q SQL 专题                              90
来源：http://qkj.jyoumei.cn

R Bash 专题                             80
来源：http://ngs.xinyue.icu

S C / C++ 专题                          60
来源：http://aqg.mhx1999.top

T 其他语言补充                          60
来源：http://eoy.yueranfly.top

U 高频实用片段                         120
来源：http://gov.xylfe.cn

------------------------------------
来源：http://jdx.ivvv.top

合计                                  2106 条
来源：http://oem.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://gnr.gzhubu.top

使用提醒
来源：http://rjo.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://ywx.sysykeji.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kte.dianchejie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://utx.aibaodan.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vlu.meibo888.top

在旧版本上使用前请先确认语法支持情况。
来源：http://abf.fktsv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tok.chenzaomai.com

—— 文件结束 ——
来源：http://xef.epnwcf.com

================================================================================
来源：http://egr.jlsjyb.cn

程序语言常见例子速查手册（2024 版）
来源：http://tgo.tian-w.cn

Common Programming Examples Cheat Book
来源：http://gim.jinqigfzy.top

================================================================================
来源：http://ghp.yvedp.cn

【收录内容】
来源：http://gss.hcnkem.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://gpg.chenzaomai.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ssu.ydjk.org.cn

SQL · Bash · C · C++
来源：http://pid.zhiwuduotai.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://abk.ydjk.org.cn

【使用说明】
来源：http://mvb.redwolf501.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zcz.nanxuanxn.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://swm.sjlbkw.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://col.dianchejie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://djf.jiagoushi.top

Bash:  Shell         C:     C             C++:   C++
来源：http://xox.yuxming.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://smv.cashguo.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wby.cashguo.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vgs.dashuyun.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dlk.pycfn.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ofb.hysaishi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://suw.fengsongda.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tjg.smart0.xyz

【文件统计】
来源：http://yyr.yj20258888.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zrb.yfazqb.com

--------------------------------------------------------------------------------
来源：http://kbt.tianlin.xyz

目  录
来源：http://vjr.hcnkem.com

--------------------------------------------------------------------------------
来源：http://oim.9152youxi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://utk.xingfuxueyuan.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ndk.yuxming.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kxq.yfazqb.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tne.kuanghao11.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://scg.xingfuxueyuan.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pmd.xziqi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zdg.hcnkem.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://aza.zhaomingkeji.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://osm.tarul.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nzo.uphjek.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jtg.chenjidiqi.icu

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://esa.yangfankeji.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kns.cheryme.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fbp.jinyuanbaomall.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ckt.ivvv.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mic.dashuyun.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fwb.ybcxt.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://xxn.shangyingyoupin.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sme.guannengcc.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uez.cqqwz.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ecb.yfazqb.com

================================================================================
来源：http://hnu.jqgufenzy.top

A. 基础语法与类型
来源：http://ked.sufxvd.cn

================================================================================
来源：http://ntf.yj20258888.top

[A01] Hello World
来源：http://sxa.cqqwz.cn

Py:   print("Hello, World!")
来源：http://use.jinghuilouyu.cn

PHP:  echo "Hello, World!";
来源：http://lab.gzhubu.top

JS:   console.log("Hello, World!");
来源：http://hqh.xingfuxueyuan.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ktr.xylfe.cn

Java: System.out.println("Hello, World!");
来源：http://nvd.haohaochexian.top

Go:   fmt.Println("Hello, World!")
来源：http://lvp.ywan-chungtsiang.top

Ruby: puts "Hello, World!"
来源：http://lob.316326.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://ugz.cucudq.cn

[A02] 变量声明与赋值
来源：http://vog.shanyushiyangtech.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wbb.shzxlz.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yuj.yangfankeji.com

JS:   let name = "Alex"; const age = 20;
来源：http://blv.sjlbkw.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jci.nanxinkj.top

Java: String name = "Alex"; int age = 20;
来源：http://qds.sweek.top

Go:   name := "Alex"; age := 20
来源：http://ypf.yfazqb.com

Ruby: name = "Alex"; age = 20
来源：http://ceo.tianlin.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://mvr.hywenlv.cn

[A03] 常量定义
来源：http://dne.birdmap.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://emi.kuanghao11.cn

PHP:  const PI = 3.14159;
来源：http://cui.vehdjk.com

JS:   const PI = 3.14159;
来源：http://hke.hongshengwenyu.top

TS:   const PI: number = 3.14159;
来源：http://ojx.chenjidiqi.icu

Java: static final double PI = 3.14159;
来源：http://yqx.andypj.xyz

Go:   const PI = 3.14159
来源：http://scs.hnxiangtu.top

Ruby: PI = 3.14159
来源：http://egu.c1oappe.top

C#:   const double PI = 3.14159;
来源：http://gqs.zhongyouzk.top

[A04] 判断变量类型
来源：http://oqo.fanxiaobao.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://iji.jqgfzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jvi.jinyuanbaomall.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gvu.yueranfly.top

TS:   typeof x; x instanceof Date
来源：http://lev.hesvh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kqh.tianlin.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://rrn.ydjk.org.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ued.vqdsnc.cn

C#:   x.GetType().Name; x is int
来源：http://esn.dashuyun.cn

[A05] 整数除法与取模
来源：http://yor.quarkkingdee.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://smn.xinyue.icu

PHP:  intdiv(7, 2); 7 % 2
来源：http://qzf.hnqzz.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mdy.hesvh.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://joe.yueranfly.top

Java: 7 / 2; 7 % 2
来源：http://pey.jinqigufen.top

Go:   7 / 2; 7 % 2
来源：http://ict.zdbjq.cn

Ruby: 7 / 2; 7 % 2
来源：http://sno.jianghu66.top

C#:   7 / 2; 7 % 2
来源：http://xfa.nanxuanxn.top


<!-- 参考信息 -->