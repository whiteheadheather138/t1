代发 wailian999

[U43] PHP：声明命名空间
来源：http://glb.zhiwuduotai.top

namespace App\Http;
来源：http://bul.zhiwuduotai.top

[U44] PHP：开启严格类型
来源：http://xaj.aizwys.cn

declare(strict_types=1);
来源：http://nlw.yuanzhike.top

[U45] PHP：类型声明与返回类型
来源：http://fxi.yuxming.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cvv.shzxlz.cn

[U46] PHP：可空类型
来源：http://ykb.tian-w.cn

?string $name = null
来源：http://xdi.chenzaomai.com

[U47] PHP：联合类型
来源：http://acz.zhijiandao.cn

int|string $id
来源：http://gdr.hywenlv.cn

[U48] PHP：纯枚举
来源：http://clc.gotoacloud.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jfp.fehbvm.com

[U49] PHP：只读属性
来源：http://vno.daxiang520.top

public readonly string $name
来源：http://omn.sweek.top

[U50] PHP：构造器属性提升
来源：http://rqu.yongpay.top

public function __construct(private int $id) {}
来源：http://rzu.yangfankeji.com

[U51] PHP：数组解构
来源：http://dyy.jqgufenzy.top

[$a, $b] = $arr;
来源：http://yje.andypj.xyz

[U52] PHP：箭头函数
来源：http://pcc.52xcode.cn

$double = fn($x) => $x * 2;
来源：http://err.sjlbkw.cn

[U53] PHP：空合并运算符
来源：http://mxx.daxiang520.top

$v = $a ?? $b ?? "default";
来源：http://uxi.ehwqpu.com

[U54] PHP：空安全调用
来源：http://vld.nwbrower.top

$obj?->method()
来源：http://soi.fehbvm.com

[U55] PHP：match 表达式
来源：http://ied.meibo888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://knp.hywenlv.cn

[U56] PHP：命名参数
来源：http://nar.wangshuangyany.cn

f(a: 1, b: 2)
来源：http://dkk.zdqjudy.top

[U57] PHP：字符串插值
来源：http://rxe.fktsv.cn

"值: {$a}"
来源：http://ukj.aizwys.cn

[U58] PHP：数组三件套
来源：http://bxc.cdnleiting.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sdd.jinqigufen.top

[U59] PHP：自定义排序
来源：http://lja.yangfankeji.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rtu.xinyue.icu

[U60] PHP：JSON 编解码
来源：http://icl.daria6918.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nth.fanxiaobao.xyz

[U61] PHP：正则
来源：http://nli.cdnleiting.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bpb.hfpthk.cn

[U62] PHP：日期对象
来源：http://exq.chenlongwang.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mvp.shzxlz.cn

[U63] PHP：文件读写
来源：http://cbs.fktsv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://olp.hongshengwenyu.top

[U64] PHP：目录遍历
来源：http://nmw.yj202588.top

glob("dir/*.php");  scandir("dir");
来源：http://mit.smart0.xyz

[U65] PHP：会话
来源：http://jvt.aibaodan.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://srs.ehwqpu.com

[U66] PHP：设置 Cookie
来源：http://fxt.sxryk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fvs.jiagoushi.top

[U67] PHP：处理文件上传
来源：http://dis.316326.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dxw.pengpengdd.cyou

[U68] PHP：PDO 连接
来源：http://ilv.sufxvd.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mow.quarkkingdee.top

[U69] PHP：PDO 预处理
来源：http://asf.gogol.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uwk.sjlbkw.cn

[U70] PHP：PDO 事务
来源：http://doh.xuanzx.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dph.jiagoushi.top

[U71] PHP：抛出异常
来源：http://oso.jinqigufen.top

throw new RuntimeException("失败", 500);
来源：http://cdt.jianghu66.top

[U72] PHP：写错误日志
来源：http://pdc.dianchejie.cn

error_log("失败: " . $e->getMessage());
来源：http://jyc.gzhubu.top

[U73] PHP：读取 ini 配置
来源：http://rmn.daria6918.cn

parse_ini_file("config.ini", true)
来源：http://ceo.cashguo.top

[U74] PHP：读取环境变量
来源：http://bnr.yonumen.top

getenv("APP_ENV") ?: "production"
来源：http://htr.c1oappe.top

[U75] PHP：依赖注入
来源：http://mlg.c1oappe.top

composer require psr/container
来源：http://kkc.svipenyu.cn

[U76] PHP：简单路由
来源：http://jmg.zycfv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qzk.zhiwuduotai.top

[U77] PHP：模板渲染
来源：http://xyw.jinqigfzy.top

composer require twig/twig
来源：http://ahr.hysaishi.cn

[U78] PHP：单元测试
来源：http://piw.svipenyu.cn

composer require --dev phpunit/phpunit
来源：http://mxz.ybcxt.top

[U79] PHP：静态分析
来源：http://hcf.xziqi.cn

composer require --dev phpstan/phpstan
来源：http://vkx.chenjidiqi.icu

[U80] PHP：代码规范修复
来源：http://okw.316326.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://vyo.jinqigfzy.top

[U81] JS：初始化项目
来源：http://brw.yj20258888.top

npm init -y;  npm i express
来源：http://bjj.gzhubu.top

[U82] JS：package.json 脚本
来源：http://ubr.bjfxy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qra.pycfn.com

[U83] JS：ES Module 导入导出
来源：http://ulf.tian-w.cn

export const a = 1;  import { a } from "./m.js";
来源：http://eob.fzhhl.top

[U84] JS：CommonJS 写法
来源：http://seb.sufxvd.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yoy.xylfe.cn

[U85] JS：可选链
来源：http://ppv.sxryk.cn

a?.b?.c
来源：http://ryb.xuetiantiany.cn

[U86] JS：空值合并
来源：http://lti.zhoulong.xyz

a ?? b
来源：http://cke.fehbvm.com

[U87] JS：解构默认值
来源：http://ape.jiagoushi.top

const { a = 1, b = 2 } = obj;
来源：http://ekz.chenlongwang.top

[U88] JS：对象展开合并
来源：http://fes.zhiwuduotai.top

{ ...a, ...b }
来源：http://hcw.zdbjq.cn

[U89] JS：数组去重
来源：http://uuk.aibaodan.cn

[...new Set(arr)]
来源：http://qxi.ydzc1.top

[U90] JS：数字数组排序
来源：http://pej.dianchejie.cn

[...arr].sort((a, b) => a - b)
来源：http://zuz.uphjek.com

[U91] JS：对象键值遍历
来源：http://jum.shzxlz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://izc.ivvv.top

[U92] JS：深拷贝
来源：http://kfn.hongshengwenyu.top

structuredClone(obj)
来源：http://cfw.hongshengwenyu.top

[U93] JS：模板字符串
来源：http://hww.yfazqb.com

`共 ${n} 条`
来源：http://nvo.sysykeji.top

[U94] JS：箭头函数
来源：http://yeo.vehdjk.com

const double = x => x * 2;
来源：http://ygj.hesvh.cn

[U95] JS：Promise 包装
来源：http://opm.aizwys.cn

new Promise((resolve, reject) => {})
来源：http://tys.yangfankeji.com

[U96] JS：async/await 与异常
来源：http://aft.fktsv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dyr.haohaochexian.top

[U97] JS：并发请求
来源：http://bre.shzxlz.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ouh.jinghuilouyu.cn

[U98] JS：fetch 带 JSON
来源：http://uka.jqgfzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ztp.nanxuanxn.top

[U99] JS：事件监听
来源：http://gzx.tianlin.xyz

el.addEventListener("click", e => {})
来源：http://rvw.c1oappe.top

[U100] JS：DOM 查询
来源：http://uuz.chenlongwang.top

document.querySelector(".item")
来源：http://mcv.bbcook.cn

[U101] JS：classList 操作
来源：http://kex.fengsongda.top

el.classList.toggle("active")
来源：http://clq.xinyue.icu

[U102] JS：本地存储
来源：http://men.yueranfly.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://qbr.yvedp.cn

[U103] JS：定时器
来源：http://bdt.jinqigfzy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ghn.jinghuilouyu.cn

[U104] JS：防抖
来源：http://riw.shzxlz.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wks.meibo888.top

[U105] JS：节流
来源：http://rdk.smart0.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hnj.yonumen.top

[U106] JS：日期格式化
来源：http://mkv.aizwys.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dmj.hnxiangtu.top

[U107] JS：数字千分位
来源：http://ouz.pycfn.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ugd.yfazqb.com

[U108] JS：随机整数
来源：http://scf.yj20258.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tam.jqgfzy.top

[U109] JS：数组分组
来源：http://oxi.gotoacloud.top

Object.groupBy(arr, x => x.type)
来源：http://yst.jinqigfzy.top

[U110] JS：数组分块
来源：http://fzp.jlsjyb.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uum.jinyuanbaomall.cn

[U111] JS：对象转 Map
来源：http://nua.tianlin.xyz

new Map(Object.entries(obj))
来源：http://qid.svipenyu.cn

[U112] JS：字符串补位
来源：http://vcr.birdmap.top

"7".padStart(3, "0")
来源：http://slw.zhengqikj.top

[U113] JS：正则替换全部
来源：http://bid.daxiang520.top

s.replaceAll("a", "b")
来源：http://xrp.c1oappe.top

[U114] JS：JSON 深比较
来源：http://dlz.dashuyun.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mve.hnxiangtu.top

[U115] JS：生成 UUID
来源：http://raz.zhongyouzk.top

crypto.randomUUID()
来源：http://qby.yj20258888.top

[U116] JS：类型检查（JSDoc）
来源：http://pbz.sufxvd.cn

/** @param {string} name */ function f(name) {}
来源：http://vyo.dashuyun.cn

[U117] JS：单元测试
来源：http://yrn.yuxming.cn

npm i -D vitest;  npx vitest
来源：http://nfl.yfazqb.com

[U118] JS：开发服务器
来源：http://stu.jyoumei.cn

npm i -D vite;  npx vite
来源：http://tyj.yj202588.top

[U119] JS：生产构建
来源：http://xlk.chenzaomai.com

npx vite build
来源：http://avw.dashuyun.cn

[U120] JS：读取环境变量（Vite）
来源：http://aut.jianghu66.top

import.meta.env.VITE_API_URL
来源：http://vif.sweek.top

================================================================================
来源：http://xsc.gzhubu.top

统计汇总
来源：http://utk.gotoacloud.top

================================================================================
来源：http://ell.kuanghao11.cn

按语言统计（条）：
来源：http://wsl.bbcook.cn

Python ......... 252
来源：http://fxk.hongshengwenyu.top

PHP ............ 252
来源：http://hwg.shangyingyoupin.top

JavaScript ..... 252
来源：http://nmc.tian-w.cn

TypeScript ..... 212
来源：http://qgr.tanke756.top

Java ........... 212
来源：http://wou.chenzaomai.com

Go ............. 212
来源：http://uac.pengpengdd.cyou

Ruby ........... 212
来源：http://ugf.nwbrower.top

C# ............. 212
来源：http://abk.smart0.xyz

C .............. 30
来源：http://yxz.tian-w.cn

C++ ............ 30
来源：http://ejt.jqgfzy.top

SQL ............ 90
来源：http://uxc.yonumen.top

Bash ........... 80
来源：http://erd.yongpay.top

Kotlin ......... 15
来源：http://miy.hfpthk.cn

Swift .......... 15
来源：http://azv.zhoulong.xyz

Lua ............ 10
来源：http://kjw.jinghuilouyu.cn

Perl ........... 10
来源：http://jwg.ppjwa.cn

Scala .......... 10
来源：http://qvx.redwolf501.top

------------------------------------
来源：http://rhg.hywenlv.cn

合计 ........... 2106 条
来源：http://vwa.nanxuanxn.top

按章节统计：
来源：http://eof.pycfn.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bpi.pengpengdd.cyou

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lwd.fehbvm.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mho.nwbrower.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hvk.birdmap.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mfy.chenzaomai.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uqd.daria6918.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mhu.meibo888.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jfp.jqgufenzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://npu.mhx1999.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wmr.chenlongwang.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tsb.316326.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lnl.ehwqpu.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://abc.xziqi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zvw.gzhubu.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ssb.cheryme.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gid.0kj1m.cn

Q SQL 专题                              90
来源：http://mip.xylfe.cn

R Bash 专题                             80
来源：http://sgk.smart0.xyz

S C / C++ 专题                          60
来源：http://tzo.yanxiufei.cn

T 其他语言补充                          60
来源：http://nwv.uphjek.com

U 高频实用片段                         120
来源：http://cti.zhengqikj.top

------------------------------------
来源：http://plw.bbcook.cn

合计                                  2106 条
来源：http://lpk.zhaomingkeji.xyz

--------------------------------------------------------------------------------
来源：http://fkw.zdqjudy.top

使用提醒
来源：http://rob.ctjpmb.com

--------------------------------------------------------------------------------
来源：http://fhw.ehwqpu.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://krr.hesvh.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xms.zdbjq.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nfw.birdmap.top

在旧版本上使用前请先确认语法支持情况。
来源：http://rqy.yuxming.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jfq.aibaodan.cn

—— 文件结束 ——
来源：http://vlj.bbcook.cn

================================================================================
来源：http://ngh.hnqzz.top

程序语言常见例子速查手册（2024 版）
来源：http://oxg.sysykeji.top

Common Programming Examples Cheat Book
来源：http://hgl.guowangkeji.top

================================================================================
来源：http://bbg.hnxiangtu.top

【收录内容】
来源：http://wwz.hesvh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pln.shanyushiyangtech.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hgp.dashuyun.cn

SQL · Bash · C · C++
来源：http://nzw.nanxinkj.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dye.cdnleiting.top

【使用说明】
来源：http://qgw.ivvv.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qox.shuidangran.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://itp.guannengcc.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cne.daria6918.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qca.xuanzx.com

Bash:  Shell         C:     C             C++:   C++
来源：http://wwj.fzhhl.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fer.daxiang520.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qjq.yj20258888.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cmf.aibaodan.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rmd.bbcook.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rmo.zhaomingkeji.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://esb.guowangkeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xch.yongpay.top

【文件统计】
来源：http://rnu.jqgfzy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ptp.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://avz.iojbl.cn

目  录
来源：http://kqk.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://eox.chenzaomai.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://knc.shangyingyoupin.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qbt.cqqwz.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uyt.yj20258888.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://phe.wangdashe.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dse.zhaomingkeji.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wlm.fanxiaobao.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wli.nanxinkj.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ojv.havefunace.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://oqf.zhongyouzk.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pzt.guannengcc.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bor.cashguo.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vii.havefunace.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ahg.epnwcf.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tpv.hysaishi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rjh.quarkkingdee.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nou.fktsv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gls.yj202588.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://eaf.yfazqb.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://klc.svipenyu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rwe.zhongyouzk.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bof.dashuyun.cn

================================================================================
来源：http://kln.chenjidiqi.icu

A. 基础语法与类型
来源：http://zbl.jiagoushi.top

================================================================================
来源：http://lbc.kuanghao11.cn

[A01] Hello World
来源：http://ruh.fehbvm.com

Py:   print("Hello, World!")
来源：http://hmj.xylfe.cn

PHP:  echo "Hello, World!";
来源：http://oqz.yj20258.top

JS:   console.log("Hello, World!");
来源：http://tva.hnqzz.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kph.sufxvd.cn

Java: System.out.println("Hello, World!");
来源：http://jpt.chenjidiqi.icu

Go:   fmt.Println("Hello, World!")
来源：http://imo.yj20258888.top

Ruby: puts "Hello, World!"
来源：http://apj.mhx1999.top

C#:   Console.WriteLine("Hello, World!");
来源：http://avk.yonumen.top

[A02] 变量声明与赋值
来源：http://uvh.jinghuilouyu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jyb.nanxinkj.top

PHP:  $name = "Alex"; $age = 20;
来源：http://cny.c1oappe.top

JS:   let name = "Alex"; const age = 20;
来源：http://bdf.hnqzz.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tct.shanyushiyangtech.top

Java: String name = "Alex"; int age = 20;
来源：http://oyc.xziqi.cn

Go:   name := "Alex"; age := 20
来源：http://wlv.bjfxy.top

Ruby: name = "Alex"; age = 20
来源：http://qwr.yj20258.top

C#:   string name = "Alex"; int age = 20;
来源：http://bon.0kj1m.cn

[A03] 常量定义
来源：http://jgt.zhoulong.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://svo.ybcxt.top

PHP:  const PI = 3.14159;
来源：http://vci.cucudq.cn

JS:   const PI = 3.14159;
来源：http://wro.snrcjt.cn

TS:   const PI: number = 3.14159;
来源：http://bvy.zhixingplan.top

Java: static final double PI = 3.14159;
来源：http://ffc.hfpthk.cn

Go:   const PI = 3.14159
来源：http://mxb.jqgfzy.top

Ruby: PI = 3.14159
来源：http://pgb.nanxinkj.top

C#:   const double PI = 3.14159;
来源：http://keo.ydzc1.top

[A04] 判断变量类型
来源：http://zbc.sufxvd.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gkj.cashguo.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://spp.hesvh.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lbw.cheryme.top

TS:   typeof x; x instanceof Date
来源：http://cis.ivvv.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qok.ybcxt.top

Go:   reflect.TypeOf(x).Name()
来源：http://oyv.cucudq.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://rdc.chenjidiqi.icu

C#:   x.GetType().Name; x is int
来源：http://eug.zycfv.cn

[A05] 整数除法与取模
来源：http://vwo.zhixingplan.top


<!-- 参考信息 -->