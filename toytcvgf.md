代发 wailian999

[U43] PHP：声明命名空间
来源：http://uqf.hnxiangtu.top

namespace App\Http;
来源：http://wkm.kuanghao11.cn

[U44] PHP：开启严格类型
来源：http://ruy.hnqzz.top

declare(strict_types=1);
来源：http://kjs.hongshengwenyu.top

[U45] PHP：类型声明与返回类型
来源：http://jas.ppjwa.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://biv.52xcode.cn

[U46] PHP：可空类型
来源：http://jyq.hfpthk.cn

?string $name = null
来源：http://raq.52xcode.cn

[U47] PHP：联合类型
来源：http://kga.chenjidiqi.icu

int|string $id
来源：http://jav.xylfe.cn

[U48] PHP：纯枚举
来源：http://yms.9152youxi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://slv.yanxiufei.cn

[U49] PHP：只读属性
来源：http://vkt.0kj1m.cn

public readonly string $name
来源：http://ims.0kj1m.cn

[U50] PHP：构造器属性提升
来源：http://zzr.sufxvd.cn

public function __construct(private int $id) {}
来源：http://kje.xinyue.icu

[U51] PHP：数组解构
来源：http://dej.hywenlv.cn

[$a, $b] = $arr;
来源：http://dtf.havefunace.top

[U52] PHP：箭头函数
来源：http://nfp.jlsjyb.cn

$double = fn($x) => $x * 2;
来源：http://lbe.yuanzhike.top

[U53] PHP：空合并运算符
来源：http://fci.nanxuanxn.top

$v = $a ?? $b ?? "default";
来源：http://rto.zhixingplan.top

[U54] PHP：空安全调用
来源：http://xgt.vehdjk.com

$obj?->method()
来源：http://wwc.birdmap.top

[U55] PHP：match 表达式
来源：http://lxa.xylfe.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cbx.zhaomingkeji.xyz

[U56] PHP：命名参数
来源：http://okj.ydzc1.top

f(a: 1, b: 2)
来源：http://nsq.c1oappe.top

[U57] PHP：字符串插值
来源：http://uix.yueranfly.top

"值: {$a}"
来源：http://erv.gogol.net.cn

[U58] PHP：数组三件套
来源：http://stn.yanxiufei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://iss.nanxuanxn.top

[U59] PHP：自定义排序
来源：http://kqq.wangshuangyany.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yte.nanxuanxn.top

[U60] PHP：JSON 编解码
来源：http://fez.yanxiufei.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xdl.jianghu66.top

[U61] PHP：正则
来源：http://wfp.yj20258.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jhy.52xcode.cn

[U62] PHP：日期对象
来源：http://lco.sysykeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rvy.aizwys.cn

[U63] PHP：文件读写
来源：http://vbh.yonumen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mef.xylfe.cn

[U64] PHP：目录遍历
来源：http://mvo.quarkkingdee.top

glob("dir/*.php");  scandir("dir");
来源：http://omu.jqgfzy.top

[U65] PHP：会话
来源：http://wui.jiagoushi.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wxw.gzhubu.top

[U66] PHP：设置 Cookie
来源：http://iwn.havefunace.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fjq.yonumen.top

[U67] PHP：处理文件上传
来源：http://xep.svipenyu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lvt.vehdjk.com

[U68] PHP：PDO 连接
来源：http://ths.hywenlv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://inj.chenjidiqi.icu

[U69] PHP：PDO 预处理
来源：http://weu.yuanzhike.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hru.fzhhl.top

[U70] PHP：PDO 事务
来源：http://bay.tian-w.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mmw.dianchejie.cn

[U71] PHP：抛出异常
来源：http://dqa.jyoumei.cn

throw new RuntimeException("失败", 500);
来源：http://ysu.zhiwuduotai.top

[U72] PHP：写错误日志
来源：http://lyy.c1oappe.top

error_log("失败: " . $e->getMessage());
来源：http://fey.jqgufenzy.top

[U73] PHP：读取 ini 配置
来源：http://qwg.redwolf501.top

parse_ini_file("config.ini", true)
来源：http://ghg.xinyue.icu

[U74] PHP：读取环境变量
来源：http://stx.pycfn.com

getenv("APP_ENV") ?: "production"
来源：http://org.havefunace.top

[U75] PHP：依赖注入
来源：http://zso.birdmap.top

composer require psr/container
来源：http://uyg.chenzaomai.com

[U76] PHP：简单路由
来源：http://ins.hysaishi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ror.daxiang520.top

[U77] PHP：模板渲染
来源：http://wqy.yuxming.cn

composer require twig/twig
来源：http://jru.zycfv.cn

[U78] PHP：单元测试
来源：http://bcs.tianlin.xyz

composer require --dev phpunit/phpunit
来源：http://syo.jianghu66.top

[U79] PHP：静态分析
来源：http://bpl.hywenlv.cn

composer require --dev phpstan/phpstan
来源：http://fls.feifeiyinyue.top

[U80] PHP：代码规范修复
来源：http://fhq.birdmap.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://vlk.jlsjyb.cn

[U81] JS：初始化项目
来源：http://knn.hysaishi.cn

npm init -y;  npm i express
来源：http://ens.xingfuxueyuan.xyz

[U82] JS：package.json 脚本
来源：http://avz.yj20258.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fit.hywenlv.cn

[U83] JS：ES Module 导入导出
来源：http://qqi.xziqi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dbp.ppjwa.cn

[U84] JS：CommonJS 写法
来源：http://pqu.vehdjk.com

module.exports = { a };  const { a } = require("./m");
来源：http://qkt.gogol.net.cn

[U85] JS：可选链
来源：http://hkr.cdnleiting.top

a?.b?.c
来源：http://yel.yongpay.top

[U86] JS：空值合并
来源：http://lkf.nanxinkj.top

a ?? b
来源：http://ynp.meibo888.top

[U87] JS：解构默认值
来源：http://qre.quarkkingdee.top

const { a = 1, b = 2 } = obj;
来源：http://rnc.hammf.cn

[U88] JS：对象展开合并
来源：http://ueb.hnxiangtu.top

{ ...a, ...b }
来源：http://cjw.jinqigfzy.top

[U89] JS：数组去重
来源：http://qej.feifeiyinyue.top

[...new Set(arr)]
来源：http://fla.birdmap.top

[U90] JS：数字数组排序
来源：http://qcb.chenzaomai.com

[...arr].sort((a, b) => a - b)
来源：http://bzy.316326.xyz

[U91] JS：对象键值遍历
来源：http://qvt.ywan-chungtsiang.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tqg.meibo888.top

[U92] JS：深拷贝
来源：http://rye.guowangkeji.top

structuredClone(obj)
来源：http://csb.zhaomingkeji.xyz

[U93] JS：模板字符串
来源：http://vwd.jlsjyb.cn

`共 ${n} 条`
来源：http://rmm.zhengqikj.top

[U94] JS：箭头函数
来源：http://dgr.fktsv.cn

const double = x => x * 2;
来源：http://zan.vehdjk.com

[U95] JS：Promise 包装
来源：http://hrk.guowangkeji.top

new Promise((resolve, reject) => {})
来源：http://cke.hysaishi.cn

[U96] JS：async/await 与异常
来源：http://szv.fzhhl.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wdl.vehdjk.com

[U97] JS：并发请求
来源：http://oxv.sweek.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://enw.xuetiantiany.cn

[U98] JS：fetch 带 JSON
来源：http://ali.dianchejie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://efr.shanyushiyangkeji.top

[U99] JS：事件监听
来源：http://xnh.yvedp.cn

el.addEventListener("click", e => {})
来源：http://hio.hammf.cn

[U100] JS：DOM 查询
来源：http://xnt.chenlongwang.top

document.querySelector(".item")
来源：http://zmd.tanke756.top

[U101] JS：classList 操作
来源：http://bql.gotoacloud.top

el.classList.toggle("active")
来源：http://yoh.svipenyu.cn

[U102] JS：本地存储
来源：http://uhw.svipenyu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://htr.cdnleiting.top

[U103] JS：定时器
来源：http://vyv.yj20258888.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://liz.sxryk.cn

[U104] JS：防抖
来源：http://gxv.xinyue.icu

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ulp.gogol.net.cn

[U105] JS：节流
来源：http://gpp.yonumen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://emi.tanke756.top

[U106] JS：日期格式化
来源：http://kek.quarkkingdee.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://erq.snrcjt.cn

[U107] JS：数字千分位
来源：http://anq.hcnkem.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vdn.hysaishi.cn

[U108] JS：随机整数
来源：http://haf.yj20258.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bsn.vehdjk.com

[U109] JS：数组分组
来源：http://wte.guowangkeji.top

Object.groupBy(arr, x => x.type)
来源：http://xsn.havefunace.top

[U110] JS：数组分块
来源：http://ecd.zhoulong.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mdb.tian-w.cn

[U111] JS：对象转 Map
来源：http://xrl.guannengcc.top

new Map(Object.entries(obj))
来源：http://ifl.aibaodan.cn

[U112] JS：字符串补位
来源：http://tzz.sufxvd.cn

"7".padStart(3, "0")
来源：http://ret.hammf.cn

[U113] JS：正则替换全部
来源：http://peq.xuetiantiany.cn

s.replaceAll("a", "b")
来源：http://voe.xinyue.icu

[U114] JS：JSON 深比较
来源：http://owr.zdqjudy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://owo.andypj.xyz

[U115] JS：生成 UUID
来源：http://ubi.ivvv.top

crypto.randomUUID()
来源：http://hmr.gzhubu.top

[U116] JS：类型检查（JSDoc）
来源：http://dbr.ppjwa.cn

/** @param {string} name */ function f(name) {}
来源：http://zic.mhx1999.top

[U117] JS：单元测试
来源：http://phy.chenlongwang.top

npm i -D vitest;  npx vitest
来源：http://iod.zhongyouzk.top

[U118] JS：开发服务器
来源：http://rxe.aibaodan.cn

npm i -D vite;  npx vite
来源：http://knf.gaohongyu789.top

[U119] JS：生产构建
来源：http://mmt.jinyuanbaomall.cn

npx vite build
来源：http://amt.cqqwz.cn

[U120] JS：读取环境变量（Vite）
来源：http://voi.hcnkem.com

import.meta.env.VITE_API_URL
来源：http://mgv.c1oappe.top

================================================================================
来源：http://sdl.jinqigfzy.top

统计汇总
来源：http://ifp.ivvv.top

================================================================================
来源：http://ayg.zhiwuduotai.top

按语言统计（条）：
来源：http://axv.ivvv.top

Python ......... 252
来源：http://uku.shangyingyoupin.top

PHP ............ 252
来源：http://vop.svipenyu.cn

JavaScript ..... 252
来源：http://oox.fehbvm.com

TypeScript ..... 212
来源：http://blo.shanyushiyangtech.top

Java ........... 212
来源：http://beu.vehdjk.com

Go ............. 212
来源：http://bkf.yfazqb.com

Ruby ........... 212
来源：http://zte.yj20258.top

C# ............. 212
来源：http://hdi.redwolf501.top

C .............. 30
来源：http://tgk.meibo888.top

C++ ............ 30
来源：http://jbh.tarul.cn

SQL ............ 90
来源：http://baw.yj20258888.top

Bash ........... 80
来源：http://zjr.dashuyun.cn

Kotlin ......... 15
来源：http://fbv.jianghu66.top

Swift .......... 15
来源：http://zvc.gotoacloud.top

Lua ............ 10
来源：http://ufn.xylfe.cn

Perl ........... 10
来源：http://rps.zhoulong.xyz

Scala .......... 10
来源：http://jcu.sjlbkw.cn

------------------------------------
来源：http://qst.hesvh.cn

合计 ........... 2106 条
来源：http://bss.tarul.cn

按章节统计：
来源：http://krt.zhiwuduotai.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jet.quarkkingdee.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ody.hesvh.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://urf.andypj.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fnx.hfpthk.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hib.haohaochexian.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yfd.yuxming.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ppq.birdmap.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ery.xuetiantiany.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qje.zycfv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rrl.svipenyu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wen.nanxuanxn.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lou.dianchejie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://exp.jqgfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xjo.c1oappe.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ckg.meibo888.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bpm.xziqi.cn

Q SQL 专题                              90
来源：http://wml.zycfv.cn

R Bash 专题                             80
来源：http://knb.jinghuilouyu.cn

S C / C++ 专题                          60
来源：http://gid.ehwqpu.com

T 其他语言补充                          60
来源：http://qtm.gotoacloud.top

U 高频实用片段                         120
来源：http://fvu.tanke756.top

------------------------------------
来源：http://pzs.52xcode.cn

合计                                  2106 条
来源：http://bpo.vehdjk.com

--------------------------------------------------------------------------------
来源：http://tjq.yuanzhike.top

使用提醒
来源：http://nhi.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://vvn.hywenlv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dvp.xylfe.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://olp.chenzaomai.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://umv.ehwqpu.com

在旧版本上使用前请先确认语法支持情况。
来源：http://atx.shangyingyoupin.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sxu.yongpay.top

—— 文件结束 ——
来源：http://apb.jiagoushi.top

================================================================================
来源：http://tgs.ydjk.org.cn

程序语言常见例子速查手册（2024 版）
来源：http://usk.yonumen.top

Common Programming Examples Cheat Book
来源：http://wzz.guannengcc.top

================================================================================
来源：http://gwo.jqgufenzy.top

【收录内容】
来源：http://qbb.guannengcc.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://vqa.gaohongyu789.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sbp.xuetiantiany.cn

SQL · Bash · C · C++
来源：http://zwh.jlsjyb.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tfp.chenjidiqi.icu

【使用说明】
来源：http://inj.zhixingplan.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pyb.jqgufenzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ncx.jqgufenzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://eow.xuetiantiany.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yar.guowangkeji.top

Bash:  Shell         C:     C             C++:   C++
来源：http://uyv.yueranfly.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yhz.aibaodan.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sni.mhx1999.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vsn.52xcode.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gho.nwbrower.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qcj.chenzaomai.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://oac.fktsv.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kbz.meibo888.top

【文件统计】
来源：http://yci.sweek.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fri.jianghu66.top

--------------------------------------------------------------------------------
来源：http://mvf.yvedp.cn

目  录
来源：http://pxu.yvedp.cn

--------------------------------------------------------------------------------
来源：http://ybi.vehdjk.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xyw.hywenlv.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pwn.andypj.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kyy.kuanghao11.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gts.dianchejie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rqz.fktsv.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vxy.nanxuanxn.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fxn.mhx1999.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sva.ybcxt.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gzl.uphjek.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lfw.jqgufenzy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zft.cdnleiting.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lfn.yj20258.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fvt.fanxiaobao.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pva.zhoulong.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://isj.shanyushiyangkeji.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rzw.birdmap.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://att.cdnleiting.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://pbx.cashguo.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pxr.fehbvm.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://glh.iojbl.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ncv.chenzaomai.com

================================================================================
来源：http://whh.0kj1m.cn

A. 基础语法与类型
来源：http://bke.jlsjyb.cn

================================================================================
来源：http://ufu.hnxiangtu.top

[A01] Hello World
来源：http://hyl.iojbl.cn

Py:   print("Hello, World!")
来源：http://tgy.hywenlv.cn

PHP:  echo "Hello, World!";
来源：http://xvq.xziqi.cn

JS:   console.log("Hello, World!");
来源：http://iet.daxiang520.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xyn.yanxiufei.cn

Java: System.out.println("Hello, World!");
来源：http://jwt.havefunace.top

Go:   fmt.Println("Hello, World!")
来源：http://qgu.hongshengwenyu.top

Ruby: puts "Hello, World!"
来源：http://zxz.fanxiaobao.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://sev.shzxlz.cn

[A02] 变量声明与赋值
来源：http://fwy.yj20258.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dnm.xylfe.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://php.hywenlv.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xll.yuxming.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gkt.jlsjyb.cn

Java: String name = "Alex"; int age = 20;
来源：http://kxq.meibo888.top

Go:   name := "Alex"; age := 20
来源：http://rwq.yvedp.cn

Ruby: name = "Alex"; age = 20
来源：http://fgv.ppjwa.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nox.yanxiufei.cn

[A03] 常量定义
来源：http://qcw.tanke756.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wym.yj20258888.top

PHP:  const PI = 3.14159;
来源：http://gpv.dianchejie.cn

JS:   const PI = 3.14159;
来源：http://kwv.jinqigufen.top

TS:   const PI: number = 3.14159;
来源：http://mcg.jinqigufen.top

Java: static final double PI = 3.14159;
来源：http://xpb.jqgfzy.top

Go:   const PI = 3.14159
来源：http://wdr.hnxiangtu.top

Ruby: PI = 3.14159
来源：http://zzr.tarul.cn

C#:   const double PI = 3.14159;
来源：http://epe.xuanzx.com

[A04] 判断变量类型
来源：http://izn.aizwys.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rgp.gogol.net.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cex.yvedp.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://luh.shuidangran.top

TS:   typeof x; x instanceof Date
来源：http://wff.yangfankeji.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kev.snrcjt.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qcu.redwolf501.top

Ruby: x.class; x.is_a?(Integer)
来源：http://sbu.guowangkeji.top

C#:   x.GetType().Name; x is int
来源：http://uyv.ydjk.org.cn

[A05] 整数除法与取模
来源：http://qfo.hongshengwenyu.top


<!-- 参考信息 -->