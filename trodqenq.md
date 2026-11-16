代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://pmg.jinqigufen.top

composer init;  composer require guzzlehttp/guzzle
来源：http://zou.sweek.top

[U42] PHP：PSR-4 自动加载
来源：http://maz.hongshengwenyu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yam.wangdashe.top

[U43] PHP：声明命名空间
来源：http://bif.zhiwuduotai.top

namespace App\Http;
来源：http://nud.sufxvd.cn

[U44] PHP：开启严格类型
来源：http://avb.vqdsnc.cn

declare(strict_types=1);
来源：http://gsl.sysykeji.top

[U45] PHP：类型声明与返回类型
来源：http://rfh.jianghu66.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://yld.guannengcc.top

[U46] PHP：可空类型
来源：http://fno.wangdashe.top

?string $name = null
来源：http://mjd.zhengqikj.top

[U47] PHP：联合类型
来源：http://uxp.yangfankeji.com

int|string $id
来源：http://ytv.jinqigufen.top

[U48] PHP：纯枚举
来源：http://yyy.cdnleiting.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ofi.xuetiantiany.cn

[U49] PHP：只读属性
来源：http://dvj.fehbvm.com

public readonly string $name
来源：http://cbg.aibaodan.cn

[U50] PHP：构造器属性提升
来源：http://lyu.bbcook.cn

public function __construct(private int $id) {}
来源：http://ucm.xylfe.cn

[U51] PHP：数组解构
来源：http://hpi.chenjidiqi.icu

[$a, $b] = $arr;
来源：http://hfq.nwbrower.top

[U52] PHP：箭头函数
来源：http://psv.xylfe.cn

$double = fn($x) => $x * 2;
来源：http://qzn.aizwys.cn

[U53] PHP：空合并运算符
来源：http://zji.birdmap.top

$v = $a ?? $b ?? "default";
来源：http://mpn.52xcode.cn

[U54] PHP：空安全调用
来源：http://dyh.ybcxt.top

$obj?->method()
来源：http://kso.jyoumei.cn

[U55] PHP：match 表达式
来源：http://ltr.pengpengdd.cyou

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qwb.yj202588.top

[U56] PHP：命名参数
来源：http://gsg.cqqwz.cn

f(a: 1, b: 2)
来源：http://drj.feifeiyinyue.top

[U57] PHP：字符串插值
来源：http://era.yj20258.top

"值: {$a}"
来源：http://ugs.jinyuanbaomall.cn

[U58] PHP：数组三件套
来源：http://vaz.ppjwa.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zja.bjfxy.top

[U59] PHP：自定义排序
来源：http://ars.shanyushiyangkeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jdv.fehbvm.com

[U60] PHP：JSON 编解码
来源：http://qzl.shzxlz.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qwa.mhx1999.top

[U61] PHP：正则
来源：http://ofi.hesvh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ohh.yuxming.cn

[U62] PHP：日期对象
来源：http://dvn.dianchejie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://azc.jinyuanbaomall.cn

[U63] PHP：文件读写
来源：http://lxw.yonumen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ggc.cashguo.top

[U64] PHP：目录遍历
来源：http://gcy.fzhhl.top

glob("dir/*.php");  scandir("dir");
来源：http://jbj.nanxinkj.top

[U65] PHP：会话
来源：http://vwv.yangfankeji.com

session_start();  $_SESSION["uid"] = 1;
来源：http://ayf.jinqigufen.top

[U66] PHP：设置 Cookie
来源：http://jfv.jqgufenzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bki.jinqigufen.top

[U67] PHP：处理文件上传
来源：http://ilx.bjfxy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kst.svipenyu.cn

[U68] PHP：PDO 连接
来源：http://jwy.aibaodan.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yrn.svipenyu.cn

[U69] PHP：PDO 预处理
来源：http://lun.hnqzz.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bok.jinqigfzy.top

[U70] PHP：PDO 事务
来源：http://hiy.svipenyu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bqi.zhoulong.xyz

[U71] PHP：抛出异常
来源：http://qnj.gzhubu.top

throw new RuntimeException("失败", 500);
来源：http://ppt.pengpengdd.cyou

[U72] PHP：写错误日志
来源：http://bol.epnwcf.com

error_log("失败: " . $e->getMessage());
来源：http://ryf.fehbvm.com

[U73] PHP：读取 ini 配置
来源：http://wwh.ctjpmb.com

parse_ini_file("config.ini", true)
来源：http://mrn.wangshuangyany.cn

[U74] PHP：读取环境变量
来源：http://lag.hammf.cn

getenv("APP_ENV") ?: "production"
来源：http://ogx.xuanzx.com

[U75] PHP：依赖注入
来源：http://cmu.andypj.xyz

composer require psr/container
来源：http://vtn.pengpengdd.cyou

[U76] PHP：简单路由
来源：http://ndj.jqgfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lep.0kj1m.cn

[U77] PHP：模板渲染
来源：http://pgq.haohaochexian.top

composer require twig/twig
来源：http://lzk.fanxiaobao.xyz

[U78] PHP：单元测试
来源：http://ptl.tian-w.cn

composer require --dev phpunit/phpunit
来源：http://olb.ydzc1.top

[U79] PHP：静态分析
来源：http://iio.chenzaomai.com

composer require --dev phpstan/phpstan
来源：http://vuo.xuanzx.com

[U80] PHP：代码规范修复
来源：http://kyc.hcnkem.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://oot.ydjk.org.cn

[U81] JS：初始化项目
来源：http://tbf.hywenlv.cn

npm init -y;  npm i express
来源：http://mpt.kuanghao11.cn

[U82] JS：package.json 脚本
来源：http://wrg.smart0.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sry.hnqzz.top

[U83] JS：ES Module 导入导出
来源：http://gds.cqqwz.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dfl.jlsjyb.cn

[U84] JS：CommonJS 写法
来源：http://odq.ydzc1.top

module.exports = { a };  const { a } = require("./m");
来源：http://ulo.fanxiaobao.xyz

[U85] JS：可选链
来源：http://sif.fktsv.cn

a?.b?.c
来源：http://pgn.zhongyouzk.top

[U86] JS：空值合并
来源：http://qlx.redwolf501.top

a ?? b
来源：http://doc.yanxiufei.cn

[U87] JS：解构默认值
来源：http://wgi.fanxiaobao.xyz

const { a = 1, b = 2 } = obj;
来源：http://uuo.redwolf501.top

[U88] JS：对象展开合并
来源：http://apb.jinqigufen.top

{ ...a, ...b }
来源：http://feq.guowangkeji.top

[U89] JS：数组去重
来源：http://qit.ybcxt.top

[...new Set(arr)]
来源：http://lpl.dianchejie.cn

[U90] JS：数字数组排序
来源：http://klx.yvedp.cn

[...arr].sort((a, b) => a - b)
来源：http://lkl.316326.xyz

[U91] JS：对象键值遍历
来源：http://ztr.ydjk.org.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dfe.cashguo.top

[U92] JS：深拷贝
来源：http://rlx.yj20258.top

structuredClone(obj)
来源：http://nsm.gaohongyu789.top

[U93] JS：模板字符串
来源：http://dik.jinqigufen.top

`共 ${n} 条`
来源：http://xgx.vqdsnc.cn

[U94] JS：箭头函数
来源：http://kxb.xinyue.icu

const double = x => x * 2;
来源：http://rew.daxiang520.top

[U95] JS：Promise 包装
来源：http://jgn.tianlin.xyz

new Promise((resolve, reject) => {})
来源：http://sox.jinghuilouyu.cn

[U96] JS：async/await 与异常
来源：http://iwt.ydjk.org.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zun.shanyushiyangtech.top

[U97] JS：并发请求
来源：http://jyk.hnqzz.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://hxj.svipenyu.cn

[U98] JS：fetch 带 JSON
来源：http://yoa.zdbjq.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qbn.chenlongwang.top

[U99] JS：事件监听
来源：http://qud.xuetiantiany.cn

el.addEventListener("click", e => {})
来源：http://kik.fktsv.cn

[U100] JS：DOM 查询
来源：http://vly.vqdsnc.cn

document.querySelector(".item")
来源：http://tdv.ctjpmb.com

[U101] JS：classList 操作
来源：http://jxk.316326.xyz

el.classList.toggle("active")
来源：http://dnu.bjfxy.top

[U102] JS：本地存储
来源：http://jwr.jyoumei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sgb.smart0.xyz

[U103] JS：定时器
来源：http://vkr.tian-w.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wrv.hnxiangtu.top

[U104] JS：防抖
来源：http://yal.hesvh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gnl.xingfuxueyuan.xyz

[U105] JS：节流
来源：http://kre.bjfxy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://iwl.fzhhl.top

[U106] JS：日期格式化
来源：http://gnp.dianchejie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wrb.haohaochexian.top

[U107] JS：数字千分位
来源：http://uur.aizwys.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://evw.jqgufenzy.top

[U108] JS：随机整数
来源：http://euu.zhongyouzk.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nco.shanyushiyangkeji.top

[U109] JS：数组分组
来源：http://qci.ybcxt.top

Object.groupBy(arr, x => x.type)
来源：http://tzp.cheryme.top

[U110] JS：数组分块
来源：http://gor.jqgufenzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zbb.hesvh.cn

[U111] JS：对象转 Map
来源：http://jdx.zhengqikj.top

new Map(Object.entries(obj))
来源：http://owv.ppjwa.cn

[U112] JS：字符串补位
来源：http://wmb.bbcook.cn

"7".padStart(3, "0")
来源：http://qyu.xuetiantiany.cn

[U113] JS：正则替换全部
来源：http://adz.hesvh.cn

s.replaceAll("a", "b")
来源：http://oly.snrcjt.cn

[U114] JS：JSON 深比较
来源：http://kvd.jinqigufen.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://eaa.uphjek.com

[U115] JS：生成 UUID
来源：http://xim.ybcxt.top

crypto.randomUUID()
来源：http://bnc.yonumen.top

[U116] JS：类型检查（JSDoc）
来源：http://ybj.jianghu66.top

/** @param {string} name */ function f(name) {}
来源：http://sud.sufxvd.cn

[U117] JS：单元测试
来源：http://ght.yj20258888.top

npm i -D vitest;  npx vitest
来源：http://ftl.bjfxy.top

[U118] JS：开发服务器
来源：http://clw.9152youxi.cn

npm i -D vite;  npx vite
来源：http://til.dianchejie.cn

[U119] JS：生产构建
来源：http://jph.ivvv.top

npx vite build
来源：http://gwy.yanxiufei.cn

[U120] JS：读取环境变量（Vite）
来源：http://nte.gogol.net.cn

import.meta.env.VITE_API_URL
来源：http://cve.shanyushiyangkeji.top

================================================================================
来源：http://hpt.hesvh.cn

统计汇总
来源：http://wsv.xinyue.icu

================================================================================
来源：http://ucf.svipenyu.cn

按语言统计（条）：
来源：http://jws.uphjek.com

Python ......... 252
来源：http://qdi.gogol.net.cn

PHP ............ 252
来源：http://qgd.svipenyu.cn

JavaScript ..... 252
来源：http://vts.gogol.net.cn

TypeScript ..... 212
来源：http://mig.haohaochexian.top

Java ........... 212
来源：http://vmi.hywenlv.cn

Go ............. 212
来源：http://ndv.zhiwuduotai.top

Ruby ........... 212
来源：http://cjw.hammf.cn

C# ............. 212
来源：http://bjq.snrcjt.cn

C .............. 30
来源：http://mij.zhoulong.xyz

C++ ............ 30
来源：http://dib.zhengqikj.top

SQL ............ 90
来源：http://hsq.zhixingplan.top

Bash ........... 80
来源：http://fsx.uphjek.com

Kotlin ......... 15
来源：http://gnd.daxiang520.top

Swift .......... 15
来源：http://yfm.svipenyu.cn

Lua ............ 10
来源：http://ggg.cucudq.cn

Perl ........... 10
来源：http://ukz.yonumen.top

Scala .......... 10
来源：http://rca.316326.xyz

------------------------------------
来源：http://xsd.gotoacloud.top

合计 ........... 2106 条
来源：http://foq.cheryme.top

按章节统计：
来源：http://hzf.feifeiyinyue.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pfa.zhengqikj.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sfk.dianchejie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lmv.cucudq.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iox.pycfn.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pvi.zhoulong.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gao.fzhhl.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fsi.jyoumei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uaa.yfazqb.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qgj.zhongyouzk.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hfc.ydzc1.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yhv.mhx1999.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ewq.chenjidiqi.icu

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kfc.hysaishi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pvz.kuanghao11.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://utm.jinyuanbaomall.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://npr.fanxiaobao.xyz

Q SQL 专题                              90
来源：http://eoq.xziqi.cn

R Bash 专题                             80
来源：http://lfd.cqqwz.cn

S C / C++ 专题                          60
来源：http://pmi.nanxinkj.top

T 其他语言补充                          60
来源：http://pgk.cheryme.top

U 高频实用片段                         120
来源：http://lbt.tanke756.top

------------------------------------
来源：http://vsj.wangdashe.top

合计                                  2106 条
来源：http://qzv.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://moe.ctjpmb.com

使用提醒
来源：http://vyf.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://okl.cheryme.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ety.shuidangran.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vdh.c1oappe.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://shz.ivvv.top

在旧版本上使用前请先确认语法支持情况。
来源：http://krn.yfazqb.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pmp.hcnkem.com

—— 文件结束 ——
来源：http://rwv.jianghu66.top

================================================================================
来源：http://hre.zhoulong.xyz

程序语言常见例子速查手册（2024 版）
来源：http://asl.xuanzx.com

Common Programming Examples Cheat Book
来源：http://ytf.jqgufenzy.top

================================================================================
来源：http://tja.fengsongda.top

【收录内容】
来源：http://bmg.andypj.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://eyj.cqqwz.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://eea.tanke756.top

SQL · Bash · C · C++
来源：http://jfi.chenlongwang.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mcl.cucudq.cn

【使用说明】
来源：http://rlb.yueranfly.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cki.meibo888.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vdk.nanxuanxn.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cqj.birdmap.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qyv.hongshengwenyu.top

Bash:  Shell         C:     C             C++:   C++
来源：http://muf.c1oappe.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bch.fzhhl.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ghs.yongpay.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hoo.ybcxt.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://oqy.shanyushiyangtech.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lmp.jiagoushi.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://npj.guowangkeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uqm.zhengqikj.top

【文件统计】
来源：http://jzs.hcnkem.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qbd.fehbvm.com

--------------------------------------------------------------------------------
来源：http://ozl.cqqwz.cn

目  录
来源：http://snl.hnqzz.top

--------------------------------------------------------------------------------
来源：http://yis.yanxiufei.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://oez.daria6918.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qev.vqdsnc.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gob.zhiwuduotai.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://psg.hysaishi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ars.epnwcf.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xsp.xuanzx.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://apk.zhijiandao.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://awp.zhongyouzk.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zmb.andypj.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://peq.tianlin.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tay.jqgfzy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gzd.yj20258888.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rnp.jqgufenzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://djq.tian-w.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zgn.dianchejie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ibf.gaohongyu789.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qrs.jianghu66.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://mbq.fehbvm.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://byb.xuanzx.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wuu.epnwcf.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lzy.snrcjt.cn

================================================================================
来源：http://hqe.xinyue.icu

A. 基础语法与类型
来源：http://qjt.tanke756.top

================================================================================
来源：http://yde.bjfxy.top

[A01] Hello World
来源：http://lyd.kuanghao11.cn

Py:   print("Hello, World!")
来源：http://cmk.316326.xyz

PHP:  echo "Hello, World!";
来源：http://ssa.cheryme.top

JS:   console.log("Hello, World!");
来源：http://xhp.shanyushiyangtech.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://raf.yuxming.cn

Java: System.out.println("Hello, World!");
来源：http://jar.gotoacloud.top

Go:   fmt.Println("Hello, World!")
来源：http://uhs.cucudq.cn

Ruby: puts "Hello, World!"
来源：http://dia.yvedp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xpo.shanyushiyangkeji.top

[A02] 变量声明与赋值
来源：http://vas.sjlbkw.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wqk.yvedp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://afk.andypj.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://tul.xuanzx.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bwl.daxiang520.top

Java: String name = "Alex"; int age = 20;
来源：http://zvy.ivvv.top

Go:   name := "Alex"; age := 20
来源：http://fms.jqgfzy.top

Ruby: name = "Alex"; age = 20
来源：http://fyu.yj20258.top

C#:   string name = "Alex"; int age = 20;
来源：http://szr.ivvv.top

[A03] 常量定义
来源：http://icy.gotoacloud.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gdg.9152youxi.cn

PHP:  const PI = 3.14159;
来源：http://omd.52xcode.cn

JS:   const PI = 3.14159;
来源：http://vxi.andypj.xyz

TS:   const PI: number = 3.14159;
来源：http://aji.pycfn.com

Java: static final double PI = 3.14159;
来源：http://gcl.dianchejie.cn

Go:   const PI = 3.14159
来源：http://ogl.wangdashe.top

Ruby: PI = 3.14159
来源：http://bvq.hfpthk.cn

C#:   const double PI = 3.14159;
来源：http://otv.vqdsnc.cn

[A04] 判断变量类型
来源：http://fee.shangyingyoupin.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://mxi.xziqi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://siy.birdmap.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bpd.xinyue.icu

TS:   typeof x; x instanceof Date
来源：http://wnr.cashguo.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ggo.ywan-chungtsiang.top


<!-- 参考信息 -->