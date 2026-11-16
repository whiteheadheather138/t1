代发 wailian999

[U43] PHP：声明命名空间
来源：http://ueu.iojbl.cn

namespace App\Http;
来源：http://eek.hywenlv.cn

[U44] PHP：开启严格类型
来源：http://ssj.jinghuilouyu.cn

declare(strict_types=1);
来源：http://syj.nanxinkj.top

[U45] PHP：类型声明与返回类型
来源：http://qmc.xylfe.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rkx.jlsjyb.cn

[U46] PHP：可空类型
来源：http://txs.yj20258.top

?string $name = null
来源：http://hbu.yuanzhike.top

[U47] PHP：联合类型
来源：http://tps.zhiwuduotai.top

int|string $id
来源：http://wwu.sufxvd.cn

[U48] PHP：纯枚举
来源：http://qfd.yangfankeji.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gzl.hongshengwenyu.top

[U49] PHP：只读属性
来源：http://qfb.tian-w.cn

public readonly string $name
来源：http://unk.yonumen.top

[U50] PHP：构造器属性提升
来源：http://jsc.aibaodan.cn

public function __construct(private int $id) {}
来源：http://zkh.pycfn.com

[U51] PHP：数组解构
来源：http://tqe.jianghu66.top

[$a, $b] = $arr;
来源：http://saq.pengpengdd.cyou

[U52] PHP：箭头函数
来源：http://jyn.zycfv.cn

$double = fn($x) => $x * 2;
来源：http://wbb.sufxvd.cn

[U53] PHP：空合并运算符
来源：http://hom.guowangkeji.top

$v = $a ?? $b ?? "default";
来源：http://bjy.jinqigufen.top

[U54] PHP：空安全调用
来源：http://qmp.hesvh.cn

$obj?->method()
来源：http://ljz.zhoulong.xyz

[U55] PHP：match 表达式
来源：http://szd.hnxiangtu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://htu.ydjk.org.cn

[U56] PHP：命名参数
来源：http://sre.ydzc1.top

f(a: 1, b: 2)
来源：http://vev.daria6918.cn

[U57] PHP：字符串插值
来源：http://tno.epnwcf.com

"值: {$a}"
来源：http://lmu.gogol.net.cn

[U58] PHP：数组三件套
来源：http://idx.52xcode.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://utn.cashguo.top

[U59] PHP：自定义排序
来源：http://gsz.52xcode.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vdc.shangyingyoupin.top

[U60] PHP：JSON 编解码
来源：http://kzz.fehbvm.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hom.uphjek.com

[U61] PHP：正则
来源：http://nqh.yj20258888.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xum.daxiang520.top

[U62] PHP：日期对象
来源：http://uti.xinyue.icu

(new DateTimeImmutable())->format("Y-m-d");
来源：http://exo.gzhubu.top

[U63] PHP：文件读写
来源：http://vbx.yanxiufei.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jli.ivvv.top

[U64] PHP：目录遍历
来源：http://ljx.daxiang520.top

glob("dir/*.php");  scandir("dir");
来源：http://bjm.yonumen.top

[U65] PHP：会话
来源：http://tvq.haohaochexian.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ino.havefunace.top

[U66] PHP：设置 Cookie
来源：http://vrv.guowangkeji.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uyq.gaohongyu789.top

[U67] PHP：处理文件上传
来源：http://gyb.jyoumei.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sja.xziqi.cn

[U68] PHP：PDO 连接
来源：http://uwo.hcnkem.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bth.tianlin.xyz

[U69] PHP：PDO 预处理
来源：http://uip.fehbvm.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nkr.hesvh.cn

[U70] PHP：PDO 事务
来源：http://jcg.fanxiaobao.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://shf.hesvh.cn

[U71] PHP：抛出异常
来源：http://kbg.jianghu66.top

throw new RuntimeException("失败", 500);
来源：http://ebv.bjfxy.top

[U72] PHP：写错误日志
来源：http://cup.daria6918.cn

error_log("失败: " . $e->getMessage());
来源：http://iwp.pycfn.com

[U73] PHP：读取 ini 配置
来源：http://ozn.cucudq.cn

parse_ini_file("config.ini", true)
来源：http://xix.ehwqpu.com

[U74] PHP：读取环境变量
来源：http://cvq.mhx1999.top

getenv("APP_ENV") ?: "production"
来源：http://yih.yongpay.top

[U75] PHP：依赖注入
来源：http://oqs.sweek.top

composer require psr/container
来源：http://kqc.shuidangran.top

[U76] PHP：简单路由
来源：http://cxt.mhx1999.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://moq.dashuyun.cn

[U77] PHP：模板渲染
来源：http://hym.zhoulong.xyz

composer require twig/twig
来源：http://adt.mhx1999.top

[U78] PHP：单元测试
来源：http://uoc.guannengcc.top

composer require --dev phpunit/phpunit
来源：http://dac.yangfankeji.com

[U79] PHP：静态分析
来源：http://bhp.yj202588.top

composer require --dev phpstan/phpstan
来源：http://jfn.chenlongwang.top

[U80] PHP：代码规范修复
来源：http://lbn.hywenlv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nad.cdnleiting.top

[U81] JS：初始化项目
来源：http://pdo.andypj.xyz

npm init -y;  npm i express
来源：http://xee.hammf.cn

[U82] JS：package.json 脚本
来源：http://acs.yangfankeji.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kih.nwbrower.top

[U83] JS：ES Module 导入导出
来源：http://gcf.xinyue.icu

export const a = 1;  import { a } from "./m.js";
来源：http://cdl.andypj.xyz

[U84] JS：CommonJS 写法
来源：http://hsl.ydzc1.top

module.exports = { a };  const { a } = require("./m");
来源：http://kzs.xylfe.cn

[U85] JS：可选链
来源：http://cgy.ybcxt.top

a?.b?.c
来源：http://ckp.iojbl.cn

[U86] JS：空值合并
来源：http://gym.gaohongyu789.top

a ?? b
来源：http://ump.bbcook.cn

[U87] JS：解构默认值
来源：http://rhj.c1oappe.top

const { a = 1, b = 2 } = obj;
来源：http://sze.zhongyouzk.top

[U88] JS：对象展开合并
来源：http://pvf.havefunace.top

{ ...a, ...b }
来源：http://jmi.ppjwa.cn

[U89] JS：数组去重
来源：http://olk.xuanzx.com

[...new Set(arr)]
来源：http://fyb.nanxuanxn.top

[U90] JS：数字数组排序
来源：http://gpq.jqgufenzy.top

[...arr].sort((a, b) => a - b)
来源：http://dmj.wangshuangyany.cn

[U91] JS：对象键值遍历
来源：http://zka.chenlongwang.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zfh.iojbl.cn

[U92] JS：深拷贝
来源：http://ofl.cheryme.top

structuredClone(obj)
来源：http://maz.cheryme.top

[U93] JS：模板字符串
来源：http://hon.jqgfzy.top

`共 ${n} 条`
来源：http://qae.jiagoushi.top

[U94] JS：箭头函数
来源：http://jiq.pengpengdd.cyou

const double = x => x * 2;
来源：http://xkk.svipenyu.cn

[U95] JS：Promise 包装
来源：http://uqq.shangyingyoupin.top

new Promise((resolve, reject) => {})
来源：http://lph.fehbvm.com

[U96] JS：async/await 与异常
来源：http://hia.aizwys.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://iuz.ctjpmb.com

[U97] JS：并发请求
来源：http://vln.wangshuangyany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sml.sjlbkw.cn

[U98] JS：fetch 带 JSON
来源：http://kmu.shangyingyoupin.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vvr.jiagoushi.top

[U99] JS：事件监听
来源：http://xcn.zhongyouzk.top

el.addEventListener("click", e => {})
来源：http://jyg.bjfxy.top

[U100] JS：DOM 查询
来源：http://zvj.bjfxy.top

document.querySelector(".item")
来源：http://afg.jinqigfzy.top

[U101] JS：classList 操作
来源：http://zxb.xuanzx.com

el.classList.toggle("active")
来源：http://naq.hammf.cn

[U102] JS：本地存储
来源：http://mfk.yongpay.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://fea.dianchejie.cn

[U103] JS：定时器
来源：http://uoy.aizwys.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://juc.yj202588.top

[U104] JS：防抖
来源：http://rtt.sjlbkw.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uvx.jyoumei.cn

[U105] JS：节流
来源：http://kdn.sweek.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qhq.ydzc1.top

[U106] JS：日期格式化
来源：http://vue.c1oappe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jms.tarul.cn

[U107] JS：数字千分位
来源：http://gpr.daxiang520.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wkb.pengpengdd.cyou

[U108] JS：随机整数
来源：http://vum.hcnkem.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iat.hesvh.cn

[U109] JS：数组分组
来源：http://dbb.sweek.top

Object.groupBy(arr, x => x.type)
来源：http://gcp.vqdsnc.cn

[U110] JS：数组分块
来源：http://nab.sxryk.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ihw.hnqzz.top

[U111] JS：对象转 Map
来源：http://rhj.nanxuanxn.top

new Map(Object.entries(obj))
来源：http://hgl.snrcjt.cn

[U112] JS：字符串补位
来源：http://tvr.yj20258888.top

"7".padStart(3, "0")
来源：http://hbg.kuanghao11.cn

[U113] JS：正则替换全部
来源：http://uty.yonumen.top

s.replaceAll("a", "b")
来源：http://uqc.shuidangran.top

[U114] JS：JSON 深比较
来源：http://kkj.uphjek.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://mte.uphjek.com

[U115] JS：生成 UUID
来源：http://mfj.guannengcc.top

crypto.randomUUID()
来源：http://ysg.ctjpmb.com

[U116] JS：类型检查（JSDoc）
来源：http://vnx.aizwys.cn

/** @param {string} name */ function f(name) {}
来源：http://exz.yonumen.top

[U117] JS：单元测试
来源：http://qlp.shangyingyoupin.top

npm i -D vitest;  npx vitest
来源：http://xsz.vehdjk.com

[U118] JS：开发服务器
来源：http://qjh.jiagoushi.top

npm i -D vite;  npx vite
来源：http://zkr.sjlbkw.cn

[U119] JS：生产构建
来源：http://uff.xziqi.cn

npx vite build
来源：http://omm.gzhubu.top

[U120] JS：读取环境变量（Vite）
来源：http://bts.sweek.top

import.meta.env.VITE_API_URL
来源：http://upk.zdbjq.cn

================================================================================
来源：http://dcm.yj202588.top

统计汇总
来源：http://gul.jyoumei.cn

================================================================================
来源：http://ltd.cqqwz.cn

按语言统计（条）：
来源：http://fvc.xingfuxueyuan.xyz

Python ......... 252
来源：http://mon.tarul.cn

PHP ............ 252
来源：http://cpp.shangyingyoupin.top

JavaScript ..... 252
来源：http://rnk.shanyushiyangkeji.top

TypeScript ..... 212
来源：http://qdb.zhongyouzk.top

Java ........... 212
来源：http://ilc.uphjek.com

Go ............. 212
来源：http://ivu.tanke756.top

Ruby ........... 212
来源：http://ujv.yfazqb.com

C# ............. 212
来源：http://cxb.wangshuangyany.cn

C .............. 30
来源：http://vdc.ehwqpu.com

C++ ............ 30
来源：http://kcn.cucudq.cn

SQL ............ 90
来源：http://rqa.nwbrower.top

Bash ........... 80
来源：http://slr.daxiang520.top

Kotlin ......... 15
来源：http://npb.pycfn.com

Swift .......... 15
来源：http://vhv.mhx1999.top

Lua ............ 10
来源：http://hil.hongshengwenyu.top

Perl ........... 10
来源：http://wzr.ppjwa.cn

Scala .......... 10
来源：http://faa.guowangkeji.top

------------------------------------
来源：http://onr.dashuyun.cn

合计 ........... 2106 条
来源：http://dtv.9152youxi.cn

按章节统计：
来源：http://rhs.meibo888.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hfw.ydzc1.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ila.feifeiyinyue.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xxx.zhixingplan.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://okv.dianchejie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tzq.xuetiantiany.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wlv.yonumen.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ukr.xziqi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pyn.ydjk.org.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hnc.zhiwuduotai.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hch.shuidangran.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uup.hammf.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://czw.shanyushiyangtech.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sbp.xinyue.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ycz.yj20258.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://axl.dashuyun.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://peh.smart0.xyz

Q SQL 专题                              90
来源：http://day.jlsjyb.cn

R Bash 专题                             80
来源：http://iiz.hammf.cn

S C / C++ 专题                          60
来源：http://xzd.cucudq.cn

T 其他语言补充                          60
来源：http://sbs.tarul.cn

U 高频实用片段                         120
来源：http://evz.aibaodan.cn

------------------------------------
来源：http://cuv.xuetiantiany.cn

合计                                  2106 条
来源：http://lbk.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://szn.yj20258888.top

使用提醒
来源：http://btd.yfazqb.com

--------------------------------------------------------------------------------
来源：http://kvq.jinqigufen.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ytz.quarkkingdee.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tus.shzxlz.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uxq.yj202588.top

在旧版本上使用前请先确认语法支持情况。
来源：http://dls.kuanghao11.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qbf.fengsongda.top

—— 文件结束 ——
来源：http://bbo.ywan-chungtsiang.top

================================================================================
来源：http://kqq.ppjwa.cn

程序语言常见例子速查手册（2024 版）
来源：http://eiy.guowangkeji.top

Common Programming Examples Cheat Book
来源：http://pjv.hnxiangtu.top

================================================================================
来源：http://phz.yonumen.top

【收录内容】
来源：http://ake.vqdsnc.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zta.bbcook.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jvi.xziqi.cn

SQL · Bash · C · C++
来源：http://okn.shuidangran.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qhg.quarkkingdee.top

【使用说明】
来源：http://cxk.hnqzz.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://spx.yangfankeji.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ckq.yuxming.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wij.cqqwz.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kqv.aizwys.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://bgu.zhixingplan.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vxb.0kj1m.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jow.wangshuangyany.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tev.jqgufenzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xwe.guannengcc.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gvs.sweek.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yam.xingfuxueyuan.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hcx.iojbl.cn

【文件统计】
来源：http://dzw.yonumen.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hax.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://lse.hammf.cn

目  录
来源：http://yyb.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://irk.cdnleiting.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yow.daxiang520.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fhc.shanyushiyangkeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://clb.dianchejie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rqn.iojbl.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xje.haohaochexian.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vzb.snrcjt.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://our.gotoacloud.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dqr.hysaishi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ztk.pycfn.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ivn.sxryk.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uwu.guowangkeji.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xza.guowangkeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gwe.chenjidiqi.icu

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://naz.52xcode.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kqt.c1oappe.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://atm.zhengqikj.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cpj.daria6918.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ktw.aizwys.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xsm.gotoacloud.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gdv.hcnkem.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gmt.vqdsnc.cn

================================================================================
来源：http://mca.guowangkeji.top

A. 基础语法与类型
来源：http://inw.shangyingyoupin.top

================================================================================
来源：http://lfu.jyoumei.cn

[A01] Hello World
来源：http://krd.sxryk.cn

Py:   print("Hello, World!")
来源：http://ese.yvedp.cn

PHP:  echo "Hello, World!";
来源：http://djd.daria6918.cn

JS:   console.log("Hello, World!");
来源：http://gdu.yuxming.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pcv.cheryme.top

Java: System.out.println("Hello, World!");
来源：http://flh.aibaodan.cn

Go:   fmt.Println("Hello, World!")
来源：http://gho.shanyushiyangtech.top

Ruby: puts "Hello, World!"
来源：http://uag.9152youxi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wsa.yuxming.cn

[A02] 变量声明与赋值
来源：http://ayg.svipenyu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pjr.wangshuangyany.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dlj.jinghuilouyu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://svn.birdmap.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bhk.zhoulong.xyz

Java: String name = "Alex"; int age = 20;
来源：http://ytv.xingfuxueyuan.xyz

Go:   name := "Alex"; age := 20
来源：http://oea.yj20258888.top

Ruby: name = "Alex"; age = 20
来源：http://khw.xingfuxueyuan.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://vns.smart0.xyz

[A03] 常量定义
来源：http://odb.redwolf501.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qwr.tianlin.xyz

PHP:  const PI = 3.14159;
来源：http://jrp.zhiwuduotai.top

JS:   const PI = 3.14159;
来源：http://ohe.snrcjt.cn

TS:   const PI: number = 3.14159;
来源：http://kin.snrcjt.cn

Java: static final double PI = 3.14159;
来源：http://wcp.wangdashe.top

Go:   const PI = 3.14159
来源：http://mxz.guannengcc.top

Ruby: PI = 3.14159
来源：http://acv.xylfe.cn

C#:   const double PI = 3.14159;
来源：http://tpv.shanyushiyangtech.top

[A04] 判断变量类型
来源：http://hsc.mhx1999.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://dpn.andypj.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hdw.hcnkem.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dfb.xuanzx.com

TS:   typeof x; x instanceof Date
来源：http://hts.dashuyun.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vts.xziqi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://gci.ppjwa.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://upr.sjlbkw.cn

C#:   x.GetType().Name; x is int
来源：http://yoe.xuetiantiany.cn

[A05] 整数除法与取模
来源：http://ggd.jyoumei.cn


<!-- 参考信息 -->