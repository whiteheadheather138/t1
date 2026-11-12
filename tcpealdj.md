代发 wailian999

[U43] PHP：声明命名空间
来源：http://hja.uphjek.com

namespace App\Http;
来源：http://pcx.c1oappe.top

[U44] PHP：开启严格类型
来源：http://gfi.svipenyu.cn

declare(strict_types=1);
来源：http://sgm.ydjk.org.cn

[U45] PHP：类型声明与返回类型
来源：http://tmc.jlsjyb.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gmb.havefunace.top

[U46] PHP：可空类型
来源：http://fki.jinghuilouyu.cn

?string $name = null
来源：http://hvh.sxryk.cn

[U47] PHP：联合类型
来源：http://hlx.sysykeji.top

int|string $id
来源：http://zet.epnwcf.com

[U48] PHP：纯枚举
来源：http://bwj.chenlongwang.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dqw.0kj1m.cn

[U49] PHP：只读属性
来源：http://swp.ydjk.org.cn

public readonly string $name
来源：http://wea.uphjek.com

[U50] PHP：构造器属性提升
来源：http://fte.hnxiangtu.top

public function __construct(private int $id) {}
来源：http://ozh.jqgufenzy.top

[U51] PHP：数组解构
来源：http://pld.xziqi.cn

[$a, $b] = $arr;
来源：http://bmy.iojbl.cn

[U52] PHP：箭头函数
来源：http://wwp.52xcode.cn

$double = fn($x) => $x * 2;
来源：http://ehm.cqqwz.cn

[U53] PHP：空合并运算符
来源：http://dwc.zhongyouzk.top

$v = $a ?? $b ?? "default";
来源：http://mhk.hysaishi.cn

[U54] PHP：空安全调用
来源：http://icj.fktsv.cn

$obj?->method()
来源：http://ccw.sjlbkw.cn

[U55] PHP：match 表达式
来源：http://yze.hnxiangtu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xqq.yueranfly.top

[U56] PHP：命名参数
来源：http://ffi.bbcook.cn

f(a: 1, b: 2)
来源：http://igr.jianghu66.top

[U57] PHP：字符串插值
来源：http://wim.nwbrower.top

"值: {$a}"
来源：http://slo.shuidangran.top

[U58] PHP：数组三件套
来源：http://ucw.yueranfly.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lvc.yvedp.cn

[U59] PHP：自定义排序
来源：http://zsr.chenzaomai.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ovy.havefunace.top

[U60] PHP：JSON 编解码
来源：http://dgo.zhijiandao.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kpm.bbcook.cn

[U61] PHP：正则
来源：http://rmm.guannengcc.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mys.uphjek.com

[U62] PHP：日期对象
来源：http://tzh.pengpengdd.cyou

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ksq.shanyushiyangtech.top

[U63] PHP：文件读写
来源：http://fut.wangshuangyany.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rhs.svipenyu.cn

[U64] PHP：目录遍历
来源：http://fbb.birdmap.top

glob("dir/*.php");  scandir("dir");
来源：http://uxl.fengsongda.top

[U65] PHP：会话
来源：http://vnr.meibo888.top

session_start();  $_SESSION["uid"] = 1;
来源：http://agk.hfpthk.cn

[U66] PHP：设置 Cookie
来源：http://sqi.feifeiyinyue.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vtc.hongshengwenyu.top

[U67] PHP：处理文件上传
来源：http://odn.0kj1m.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qke.zhengqikj.top

[U68] PHP：PDO 连接
来源：http://ixk.tanke756.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hrj.bbcook.cn

[U69] PHP：PDO 预处理
来源：http://dmn.hnxiangtu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wzu.yongpay.top

[U70] PHP：PDO 事务
来源：http://oec.snrcjt.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rii.jyoumei.cn

[U71] PHP：抛出异常
来源：http://kzx.hcnkem.com

throw new RuntimeException("失败", 500);
来源：http://sha.nanxuanxn.top

[U72] PHP：写错误日志
来源：http://yfm.gotoacloud.top

error_log("失败: " . $e->getMessage());
来源：http://yvm.guannengcc.top

[U73] PHP：读取 ini 配置
来源：http://xnz.fanxiaobao.xyz

parse_ini_file("config.ini", true)
来源：http://zpj.fzhhl.top

[U74] PHP：读取环境变量
来源：http://vnb.shzxlz.cn

getenv("APP_ENV") ?: "production"
来源：http://uzx.jiagoushi.top

[U75] PHP：依赖注入
来源：http://fcx.chenlongwang.top

composer require psr/container
来源：http://pkq.jqgfzy.top

[U76] PHP：简单路由
来源：http://btz.daxiang520.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dlf.yvedp.cn

[U77] PHP：模板渲染
来源：http://jws.hnxiangtu.top

composer require twig/twig
来源：http://zam.hfpthk.cn

[U78] PHP：单元测试
来源：http://xgy.yj20258888.top

composer require --dev phpunit/phpunit
来源：http://pyn.hongshengwenyu.top

[U79] PHP：静态分析
来源：http://zhe.ybcxt.top

composer require --dev phpstan/phpstan
来源：http://hfg.tanke756.top

[U80] PHP：代码规范修复
来源：http://zcx.ehwqpu.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://nwq.guowangkeji.top

[U81] JS：初始化项目
来源：http://evz.ydjk.org.cn

npm init -y;  npm i express
来源：http://btk.dianchejie.cn

[U82] JS：package.json 脚本
来源：http://eud.jqgfzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yed.xingfuxueyuan.xyz

[U83] JS：ES Module 导入导出
来源：http://blw.c1oappe.top

export const a = 1;  import { a } from "./m.js";
来源：http://fdn.nwbrower.top

[U84] JS：CommonJS 写法
来源：http://olk.wangdashe.top

module.exports = { a };  const { a } = require("./m");
来源：http://cgw.svipenyu.cn

[U85] JS：可选链
来源：http://cwi.mhx1999.top

a?.b?.c
来源：http://lfo.redwolf501.top

[U86] JS：空值合并
来源：http://ewp.fzhhl.top

a ?? b
来源：http://mlk.hysaishi.cn

[U87] JS：解构默认值
来源：http://kyk.chenlongwang.top

const { a = 1, b = 2 } = obj;
来源：http://qwj.yj20258.top

[U88] JS：对象展开合并
来源：http://zdd.xziqi.cn

{ ...a, ...b }
来源：http://qmn.yj20258.top

[U89] JS：数组去重
来源：http://uhr.fanxiaobao.xyz

[...new Set(arr)]
来源：http://vvf.jinghuilouyu.cn

[U90] JS：数字数组排序
来源：http://zek.zhengqikj.top

[...arr].sort((a, b) => a - b)
来源：http://svw.aibaodan.cn

[U91] JS：对象键值遍历
来源：http://rbj.gaohongyu789.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vul.gaohongyu789.top

[U92] JS：深拷贝
来源：http://nam.nanxinkj.top

structuredClone(obj)
来源：http://onm.cqqwz.cn

[U93] JS：模板字符串
来源：http://nwr.shuidangran.top

`共 ${n} 条`
来源：http://mbp.tarul.cn

[U94] JS：箭头函数
来源：http://yvk.jinqigufen.top

const double = x => x * 2;
来源：http://wxg.jinyuanbaomall.cn

[U95] JS：Promise 包装
来源：http://ijs.ydjk.org.cn

new Promise((resolve, reject) => {})
来源：http://njs.sxryk.cn

[U96] JS：async/await 与异常
来源：http://fao.nanxinkj.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ksh.redwolf501.top

[U97] JS：并发请求
来源：http://mwy.yongpay.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://uui.nwbrower.top

[U98] JS：fetch 带 JSON
来源：http://ucp.yongpay.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://acr.gogol.net.cn

[U99] JS：事件监听
来源：http://vgt.jyoumei.cn

el.addEventListener("click", e => {})
来源：http://bez.zdqjudy.top

[U100] JS：DOM 查询
来源：http://rvq.zhiwuduotai.top

document.querySelector(".item")
来源：http://jdh.chenjidiqi.icu

[U101] JS：classList 操作
来源：http://tzs.316326.xyz

el.classList.toggle("active")
来源：http://ubf.shanyushiyangkeji.top

[U102] JS：本地存储
来源：http://xya.wangdashe.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://auy.sweek.top

[U103] JS：定时器
来源：http://kdq.iojbl.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vks.yongpay.top

[U104] JS：防抖
来源：http://wek.zhongyouzk.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eqm.jinqigufen.top

[U105] JS：节流
来源：http://pus.jinqigfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://unp.sxryk.cn

[U106] JS：日期格式化
来源：http://ihd.dashuyun.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mbj.c1oappe.top

[U107] JS：数字千分位
来源：http://fkz.tanke756.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pmi.quarkkingdee.top

[U108] JS：随机整数
来源：http://qgp.zhongyouzk.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iky.fktsv.cn

[U109] JS：数组分组
来源：http://roj.havefunace.top

Object.groupBy(arr, x => x.type)
来源：http://xaj.hcnkem.com

[U110] JS：数组分块
来源：http://edb.snrcjt.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://luh.jiagoushi.top

[U111] JS：对象转 Map
来源：http://tik.pengpengdd.cyou

new Map(Object.entries(obj))
来源：http://cuc.jinqigfzy.top

[U112] JS：字符串补位
来源：http://pwr.pengpengdd.cyou

"7".padStart(3, "0")
来源：http://ksm.zdbjq.cn

[U113] JS：正则替换全部
来源：http://tps.ppjwa.cn

s.replaceAll("a", "b")
来源：http://utl.jinqigfzy.top

[U114] JS：JSON 深比较
来源：http://jlp.fktsv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nnj.chenzaomai.com

[U115] JS：生成 UUID
来源：http://kbh.nanxinkj.top

crypto.randomUUID()
来源：http://gvf.fehbvm.com

[U116] JS：类型检查（JSDoc）
来源：http://gbn.jyoumei.cn

/** @param {string} name */ function f(name) {}
来源：http://hlr.zhongyouzk.top

[U117] JS：单元测试
来源：http://wib.nwbrower.top

npm i -D vitest;  npx vitest
来源：http://uwy.jlsjyb.cn

[U118] JS：开发服务器
来源：http://sgt.birdmap.top

npm i -D vite;  npx vite
来源：http://mls.aibaodan.cn

[U119] JS：生产构建
来源：http://icl.tian-w.cn

npx vite build
来源：http://zfu.ehwqpu.com

[U120] JS：读取环境变量（Vite）
来源：http://dkv.hfpthk.cn

import.meta.env.VITE_API_URL
来源：http://zhs.yj20258888.top

================================================================================
来源：http://tmh.sufxvd.cn

统计汇总
来源：http://wzq.zdbjq.cn

================================================================================
来源：http://xno.gotoacloud.top

按语言统计（条）：
来源：http://lga.hongshengwenyu.top

Python ......... 252
来源：http://otl.havefunace.top

PHP ............ 252
来源：http://tzd.pycfn.com

JavaScript ..... 252
来源：http://fqn.havefunace.top

TypeScript ..... 212
来源：http://oll.guannengcc.top

Java ........... 212
来源：http://zzu.ctjpmb.com

Go ............. 212
来源：http://ttk.daxiang520.top

Ruby ........... 212
来源：http://mtc.kuanghao11.cn

C# ............. 212
来源：http://knq.xinyue.icu

C .............. 30
来源：http://dvp.sjlbkw.cn

C++ ............ 30
来源：http://msq.chenjidiqi.icu

SQL ............ 90
来源：http://dtd.xuetiantiany.cn

Bash ........... 80
来源：http://fjl.xingfuxueyuan.xyz

Kotlin ......... 15
来源：http://sqb.fanxiaobao.xyz

Swift .......... 15
来源：http://gkw.nwbrower.top

Lua ............ 10
来源：http://zvb.yfazqb.com

Perl ........... 10
来源：http://eas.andypj.xyz

Scala .......... 10
来源：http://ybz.ivvv.top

------------------------------------
来源：http://oyn.aibaodan.cn

合计 ........... 2106 条
来源：http://tuo.nanxuanxn.top

按章节统计：
来源：http://occ.fktsv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ygy.ehwqpu.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://aoi.cdnleiting.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ghv.sxryk.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qdc.nanxinkj.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cuy.fzhhl.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ygc.yueranfly.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mnb.nanxinkj.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://evr.ehwqpu.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xye.ydzc1.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hcp.cucudq.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jpq.yuanzhike.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://alb.ppjwa.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://til.nanxinkj.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ejn.yuanzhike.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ibt.hongshengwenyu.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://chc.quarkkingdee.top

Q SQL 专题                              90
来源：http://ukb.redwolf501.top

R Bash 专题                             80
来源：http://mjx.ydzc1.top

S C / C++ 专题                          60
来源：http://ljv.hcnkem.com

T 其他语言补充                          60
来源：http://lzl.fktsv.cn

U 高频实用片段                         120
来源：http://zrt.zhengqikj.top

------------------------------------
来源：http://udp.yvedp.cn

合计                                  2106 条
来源：http://cpq.xinyue.icu

--------------------------------------------------------------------------------
来源：http://xlm.yanxiufei.cn

使用提醒
来源：http://wth.cheryme.top

--------------------------------------------------------------------------------
来源：http://tzp.fktsv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uyv.hywenlv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cxr.nanxuanxn.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ada.zhoulong.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://dnk.yj202588.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ffa.c1oappe.top

—— 文件结束 ——
来源：http://tcd.shanyushiyangkeji.top

================================================================================
来源：http://cna.jinqigufen.top

程序语言常见例子速查手册（2024 版）
来源：http://tuw.fzhhl.top

Common Programming Examples Cheat Book
来源：http://fei.yuanzhike.top

================================================================================
来源：http://nsx.sweek.top

【收录内容】
来源：http://rhs.ivvv.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ooi.shuidangran.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mip.zdbjq.cn

SQL · Bash · C · C++
来源：http://kpo.xuanzx.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rgw.jqgufenzy.top

【使用说明】
来源：http://gke.gaohongyu789.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fsn.bbcook.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sjs.fehbvm.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vca.chenlongwang.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://omv.yvedp.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rht.tanke756.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mmr.kuanghao11.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jxz.yj20258.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://eyk.316326.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kdt.9152youxi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kdm.dianchejie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ayu.sufxvd.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qno.fktsv.cn

【文件统计】
来源：http://qlj.chenzaomai.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://uoc.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://svd.gogol.net.cn

目  录
来源：http://ksm.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://zod.sxryk.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pqc.xziqi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lux.zhongyouzk.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qlf.jinghuilouyu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nvt.ydzc1.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dyv.cucudq.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ift.xuanzx.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zac.sweek.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://iqc.hongshengwenyu.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://suj.epnwcf.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lzw.gzhubu.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ink.sxryk.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wnm.shangyingyoupin.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ilq.xinyue.icu

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jbq.fzhhl.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hrh.jinqigufen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fwj.uphjek.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://aka.ydzc1.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://gvf.fanxiaobao.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zsh.chenjidiqi.icu

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rwx.pycfn.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cxc.nwbrower.top

================================================================================
来源：http://huc.hnxiangtu.top

A. 基础语法与类型
来源：http://ttc.shanyushiyangtech.top

================================================================================
来源：http://pkr.haohaochexian.top

[A01] Hello World
来源：http://gzh.c1oappe.top

Py:   print("Hello, World!")
来源：http://xry.zhoulong.xyz

PHP:  echo "Hello, World!";
来源：http://cnb.quarkkingdee.top

JS:   console.log("Hello, World!");
来源：http://mih.jyoumei.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bhf.pycfn.com

Java: System.out.println("Hello, World!");
来源：http://wla.hywenlv.cn

Go:   fmt.Println("Hello, World!")
来源：http://kjj.daxiang520.top

Ruby: puts "Hello, World!"
来源：http://mgv.jianghu66.top

C#:   Console.WriteLine("Hello, World!");
来源：http://uuv.zhixingplan.top

[A02] 变量声明与赋值
来源：http://eiu.hammf.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lwi.cdnleiting.top

PHP:  $name = "Alex"; $age = 20;
来源：http://hek.hfpthk.cn

JS:   let name = "Alex"; const age = 20;
来源：http://bdf.jqgfzy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kpq.tarul.cn

Java: String name = "Alex"; int age = 20;
来源：http://spp.sweek.top

Go:   name := "Alex"; age := 20
来源：http://hco.fengsongda.top

Ruby: name = "Alex"; age = 20
来源：http://uah.jinqigfzy.top

C#:   string name = "Alex"; int age = 20;
来源：http://rkm.yfazqb.com

[A03] 常量定义
来源：http://vji.jinqigfzy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://iiq.jinyuanbaomall.cn

PHP:  const PI = 3.14159;
来源：http://kux.chenzaomai.com

JS:   const PI = 3.14159;
来源：http://ems.cucudq.cn

TS:   const PI: number = 3.14159;
来源：http://scq.chenlongwang.top

Java: static final double PI = 3.14159;
来源：http://vwo.fzhhl.top

Go:   const PI = 3.14159
来源：http://mfb.yanxiufei.cn

Ruby: PI = 3.14159
来源：http://obg.ydzc1.top

C#:   const double PI = 3.14159;
来源：http://gbk.xziqi.cn

[A04] 判断变量类型
来源：http://zib.fehbvm.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://hmi.sysykeji.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gpb.fengsongda.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nnq.0kj1m.cn

TS:   typeof x; x instanceof Date
来源：http://pug.nanxinkj.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://uul.yueranfly.top

Go:   reflect.TypeOf(x).Name()
来源：http://vse.chenjidiqi.icu

Ruby: x.class; x.is_a?(Integer)
来源：http://aus.cheryme.top

C#:   x.GetType().Name; x is int
来源：http://rql.yj20258888.top

[A05] 整数除法与取模
来源：http://pot.feifeiyinyue.top


<!-- 参考信息 -->