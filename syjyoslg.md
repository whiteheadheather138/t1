代发 wailian999

[U43] PHP：声明命名空间
来源：http://ktf.ehwqpu.com

namespace App\Http;
来源：http://vvm.zdbjq.cn

[U44] PHP：开启严格类型
来源：http://xvd.hammf.cn

declare(strict_types=1);
来源：http://znf.fanxiaobao.xyz

[U45] PHP：类型声明与返回类型
来源：http://uzg.hnqzz.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://kzi.aibaodan.cn

[U46] PHP：可空类型
来源：http://teu.ywan-chungtsiang.top

?string $name = null
来源：http://ufj.aizwys.cn

[U47] PHP：联合类型
来源：http://jpv.jinqigufen.top

int|string $id
来源：http://yla.jqgufenzy.top

[U48] PHP：纯枚举
来源：http://fts.hammf.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lph.cheryme.top

[U49] PHP：只读属性
来源：http://gqw.shzxlz.cn

public readonly string $name
来源：http://tnb.vehdjk.com

[U50] PHP：构造器属性提升
来源：http://vwz.jinghuilouyu.cn

public function __construct(private int $id) {}
来源：http://wau.hesvh.cn

[U51] PHP：数组解构
来源：http://ggn.cdnleiting.top

[$a, $b] = $arr;
来源：http://tgg.tianlin.xyz

[U52] PHP：箭头函数
来源：http://iwa.aibaodan.cn

$double = fn($x) => $x * 2;
来源：http://kib.shangyingyoupin.top

[U53] PHP：空合并运算符
来源：http://mun.zhaomingkeji.xyz

$v = $a ?? $b ?? "default";
来源：http://daz.vqdsnc.cn

[U54] PHP：空安全调用
来源：http://diu.uphjek.com

$obj?->method()
来源：http://gqy.kuanghao11.cn

[U55] PHP：match 表达式
来源：http://iwu.hcnkem.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hlw.zdqjudy.top

[U56] PHP：命名参数
来源：http://prw.zdqjudy.top

f(a: 1, b: 2)
来源：http://ihw.hesvh.cn

[U57] PHP：字符串插值
来源：http://jjo.epnwcf.com

"值: {$a}"
来源：http://dta.nanxinkj.top

[U58] PHP：数组三件套
来源：http://ddf.xylfe.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xfe.bbcook.cn

[U59] PHP：自定义排序
来源：http://ltv.zycfv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vvk.havefunace.top

[U60] PHP：JSON 编解码
来源：http://row.aizwys.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tmh.yj202588.top

[U61] PHP：正则
来源：http://hrt.shanyushiyangtech.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mgp.yj20258888.top

[U62] PHP：日期对象
来源：http://xux.hysaishi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jcc.cucudq.cn

[U63] PHP：文件读写
来源：http://dlc.fktsv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ccc.ctjpmb.com

[U64] PHP：目录遍历
来源：http://uca.haohaochexian.top

glob("dir/*.php");  scandir("dir");
来源：http://mmz.mhx1999.top

[U65] PHP：会话
来源：http://hfz.cashguo.top

session_start();  $_SESSION["uid"] = 1;
来源：http://lfw.bjfxy.top

[U66] PHP：设置 Cookie
来源：http://lef.mhx1999.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sfz.kuanghao11.cn

[U67] PHP：处理文件上传
来源：http://ucc.fzhhl.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ldx.yj20258888.top

[U68] PHP：PDO 连接
来源：http://uuv.yj20258.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hxv.zhijiandao.cn

[U69] PHP：PDO 预处理
来源：http://ojg.gzhubu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cjc.316326.xyz

[U70] PHP：PDO 事务
来源：http://tew.kuanghao11.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ktk.snrcjt.cn

[U71] PHP：抛出异常
来源：http://vha.jqgufenzy.top

throw new RuntimeException("失败", 500);
来源：http://gpx.xylfe.cn

[U72] PHP：写错误日志
来源：http://ooh.shzxlz.cn

error_log("失败: " . $e->getMessage());
来源：http://irw.bbcook.cn

[U73] PHP：读取 ini 配置
来源：http://pqi.jinghuilouyu.cn

parse_ini_file("config.ini", true)
来源：http://vol.0kj1m.cn

[U74] PHP：读取环境变量
来源：http://ess.xinyue.icu

getenv("APP_ENV") ?: "production"
来源：http://esf.hnxiangtu.top

[U75] PHP：依赖注入
来源：http://hdv.vehdjk.com

composer require psr/container
来源：http://ffc.snrcjt.cn

[U76] PHP：简单路由
来源：http://ihd.uphjek.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sfy.yj20258.top

[U77] PHP：模板渲染
来源：http://krh.zdbjq.cn

composer require twig/twig
来源：http://ren.hnqzz.top

[U78] PHP：单元测试
来源：http://lgt.aibaodan.cn

composer require --dev phpunit/phpunit
来源：http://rbg.chenjidiqi.icu

[U79] PHP：静态分析
来源：http://pol.c1oappe.top

composer require --dev phpstan/phpstan
来源：http://iar.nwbrower.top

[U80] PHP：代码规范修复
来源：http://egr.ydjk.org.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://isp.xingfuxueyuan.xyz

[U81] JS：初始化项目
来源：http://wht.andypj.xyz

npm init -y;  npm i express
来源：http://mvx.ydjk.org.cn

[U82] JS：package.json 脚本
来源：http://spy.yuxming.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qjp.sysykeji.top

[U83] JS：ES Module 导入导出
来源：http://oqy.yfazqb.com

export const a = 1;  import { a } from "./m.js";
来源：http://fig.dianchejie.cn

[U84] JS：CommonJS 写法
来源：http://xis.yvedp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zfq.zhoulong.xyz

[U85] JS：可选链
来源：http://xxb.fanxiaobao.xyz

a?.b?.c
来源：http://wfg.feifeiyinyue.top

[U86] JS：空值合并
来源：http://ffe.nanxinkj.top

a ?? b
来源：http://fmh.hywenlv.cn

[U87] JS：解构默认值
来源：http://udk.zhengqikj.top

const { a = 1, b = 2 } = obj;
来源：http://zca.quarkkingdee.top

[U88] JS：对象展开合并
来源：http://gvs.xinyue.icu

{ ...a, ...b }
来源：http://rbg.pengpengdd.cyou

[U89] JS：数组去重
来源：http://exp.jiagoushi.top

[...new Set(arr)]
来源：http://isv.xingfuxueyuan.xyz

[U90] JS：数字数组排序
来源：http://dwl.yj202588.top

[...arr].sort((a, b) => a - b)
来源：http://sel.cheryme.top

[U91] JS：对象键值遍历
来源：http://bjh.yueranfly.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ojp.hnqzz.top

[U92] JS：深拷贝
来源：http://frs.cdnleiting.top

structuredClone(obj)
来源：http://eqd.xylfe.cn

[U93] JS：模板字符串
来源：http://fxb.daxiang520.top

`共 ${n} 条`
来源：http://cqu.jlsjyb.cn

[U94] JS：箭头函数
来源：http://zio.ydzc1.top

const double = x => x * 2;
来源：http://tpv.fzhhl.top

[U95] JS：Promise 包装
来源：http://cxi.cdnleiting.top

new Promise((resolve, reject) => {})
来源：http://hmq.zycfv.cn

[U96] JS：async/await 与异常
来源：http://ncb.meibo888.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mcu.hywenlv.cn

[U97] JS：并发请求
来源：http://wug.ivvv.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://bko.cdnleiting.top

[U98] JS：fetch 带 JSON
来源：http://slt.jinyuanbaomall.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bel.jianghu66.top

[U99] JS：事件监听
来源：http://qtl.jiagoushi.top

el.addEventListener("click", e => {})
来源：http://pry.zhengqikj.top

[U100] JS：DOM 查询
来源：http://mvm.svipenyu.cn

document.querySelector(".item")
来源：http://mxt.zhixingplan.top

[U101] JS：classList 操作
来源：http://ixq.ydjk.org.cn

el.classList.toggle("active")
来源：http://xjl.cucudq.cn

[U102] JS：本地存储
来源：http://abw.chenjidiqi.icu

localStorage.setItem("k", JSON.stringify(v))
来源：http://psd.chenlongwang.top

[U103] JS：定时器
来源：http://wvi.fzhhl.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yjp.9152youxi.cn

[U104] JS：防抖
来源：http://gpf.guowangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nny.hnxiangtu.top

[U105] JS：节流
来源：http://isy.ehwqpu.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bye.zdbjq.cn

[U106] JS：日期格式化
来源：http://oay.aibaodan.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jog.bjfxy.top

[U107] JS：数字千分位
来源：http://qtx.epnwcf.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fjl.daria6918.cn

[U108] JS：随机整数
来源：http://svd.hfpthk.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jta.aibaodan.cn

[U109] JS：数组分组
来源：http://hjp.zhiwuduotai.top

Object.groupBy(arr, x => x.type)
来源：http://uys.sxryk.cn

[U110] JS：数组分块
来源：http://wdp.jiagoushi.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ert.xylfe.cn

[U111] JS：对象转 Map
来源：http://smu.shangyingyoupin.top

new Map(Object.entries(obj))
来源：http://scm.316326.xyz

[U112] JS：字符串补位
来源：http://mbl.chenlongwang.top

"7".padStart(3, "0")
来源：http://yll.gaohongyu789.top

[U113] JS：正则替换全部
来源：http://uqf.cqqwz.cn

s.replaceAll("a", "b")
来源：http://kql.hnxiangtu.top

[U114] JS：JSON 深比较
来源：http://npg.zhoulong.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://pqm.daria6918.cn

[U115] JS：生成 UUID
来源：http://wys.sxryk.cn

crypto.randomUUID()
来源：http://tzu.ybcxt.top

[U116] JS：类型检查（JSDoc）
来源：http://afi.zhixingplan.top

/** @param {string} name */ function f(name) {}
来源：http://ikt.cqqwz.cn

[U117] JS：单元测试
来源：http://snx.ydzc1.top

npm i -D vitest;  npx vitest
来源：http://uzi.nanxuanxn.top

[U118] JS：开发服务器
来源：http://sbs.yfazqb.com

npm i -D vite;  npx vite
来源：http://ttf.aizwys.cn

[U119] JS：生产构建
来源：http://ipw.havefunace.top

npx vite build
来源：http://dvi.gzhubu.top

[U120] JS：读取环境变量（Vite）
来源：http://csh.sysykeji.top

import.meta.env.VITE_API_URL
来源：http://eoh.cashguo.top

================================================================================
来源：http://csc.fengsongda.top

统计汇总
来源：http://sqr.cdnleiting.top

================================================================================
来源：http://upw.snrcjt.cn

按语言统计（条）：
来源：http://agw.yj20258888.top

Python ......... 252
来源：http://hqg.tianlin.xyz

PHP ............ 252
来源：http://dxp.cdnleiting.top

JavaScript ..... 252
来源：http://epo.yonumen.top

TypeScript ..... 212
来源：http://aeb.yj20258.top

Java ........... 212
来源：http://ehf.bbcook.cn

Go ............. 212
来源：http://ytx.zdqjudy.top

Ruby ........... 212
来源：http://efm.feifeiyinyue.top

C# ............. 212
来源：http://nkx.sjlbkw.cn

C .............. 30
来源：http://fuo.zhaomingkeji.xyz

C++ ............ 30
来源：http://pcq.kuanghao11.cn

SQL ............ 90
来源：http://qnq.guowangkeji.top

Bash ........... 80
来源：http://hqe.chenjidiqi.icu

Kotlin ......... 15
来源：http://ofz.haohaochexian.top

Swift .......... 15
来源：http://dal.tanke756.top

Lua ............ 10
来源：http://lak.tian-w.cn

Perl ........... 10
来源：http://zxd.316326.xyz

Scala .......... 10
来源：http://nra.haohaochexian.top

------------------------------------
来源：http://dvg.daxiang520.top

合计 ........... 2106 条
来源：http://bbc.tarul.cn

按章节统计：
来源：http://qep.tian-w.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tzs.tianlin.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cjs.ydzc1.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://edh.jianghu66.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://alo.hnxiangtu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xxs.jlsjyb.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yie.jyoumei.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qtx.jlsjyb.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mse.ppjwa.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nnc.wangdashe.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jbj.zhoulong.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://apu.sufxvd.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qoj.hnxiangtu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wjj.mhx1999.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ubj.ywan-chungtsiang.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://chh.fehbvm.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://awl.yanxiufei.cn

Q SQL 专题                              90
来源：http://ovd.iojbl.cn

R Bash 专题                             80
来源：http://wfe.zhongyouzk.top

S C / C++ 专题                          60
来源：http://yrl.hnqzz.top

T 其他语言补充                          60
来源：http://gbd.zdbjq.cn

U 高频实用片段                         120
来源：http://qad.gaohongyu789.top

------------------------------------
来源：http://neq.shangyingyoupin.top

合计                                  2106 条
来源：http://gar.cashguo.top

--------------------------------------------------------------------------------
来源：http://snc.ivvv.top

使用提醒
来源：http://hwt.wangdashe.top

--------------------------------------------------------------------------------
来源：http://rrr.daria6918.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tlg.yfazqb.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wup.nanxinkj.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mrb.316326.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://zld.guannengcc.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qtb.ybcxt.top

—— 文件结束 ——
来源：http://jmh.xuanzx.com

================================================================================
来源：http://eyd.zhixingplan.top

程序语言常见例子速查手册（2024 版）
来源：http://kox.shzxlz.cn

Common Programming Examples Cheat Book
来源：http://ygu.yvedp.cn

================================================================================
来源：http://lin.chenjidiqi.icu

【收录内容】
来源：http://epu.shangyingyoupin.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://uhs.birdmap.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jgd.daria6918.cn

SQL · Bash · C · C++
来源：http://xkt.jinyuanbaomall.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ozb.yvedp.cn

【使用说明】
来源：http://hzx.birdmap.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wpd.hysaishi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://flc.ehwqpu.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dmp.xinyue.icu

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mjx.yj20258.top

Bash:  Shell         C:     C             C++:   C++
来源：http://tcf.nanxuanxn.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hno.9152youxi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rmd.mhx1999.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://njd.shuidangran.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://eou.andypj.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://soi.ctjpmb.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pkr.yj202588.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ctp.cashguo.top

【文件统计】
来源：http://foc.hfpthk.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://luh.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://esn.ywan-chungtsiang.top

目  录
来源：http://ujo.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://jwn.fktsv.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sng.uphjek.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rmr.wangdashe.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://crv.zhixingplan.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kzp.shanyushiyangtech.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wkn.xinyue.icu

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zkk.cashguo.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xqi.jiagoushi.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mma.nanxuanxn.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://htq.yj20258888.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gkn.fengsongda.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vba.52xcode.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://snw.ybcxt.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://juj.birdmap.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ghc.redwolf501.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dfr.yfazqb.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://iun.hcnkem.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jxv.jianghu66.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://why.svipenyu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rty.jqgfzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ruj.dashuyun.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yia.fanxiaobao.xyz

================================================================================
来源：http://dsw.pycfn.com

A. 基础语法与类型
来源：http://jzc.cashguo.top

================================================================================
来源：http://bcn.dashuyun.cn

[A01] Hello World
来源：http://oum.9152youxi.cn

Py:   print("Hello, World!")
来源：http://eam.nwbrower.top

PHP:  echo "Hello, World!";
来源：http://vtp.yongpay.top

JS:   console.log("Hello, World!");
来源：http://txb.andypj.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rcu.tian-w.cn

Java: System.out.println("Hello, World!");
来源：http://aup.tian-w.cn

Go:   fmt.Println("Hello, World!")
来源：http://cnz.kuanghao11.cn

Ruby: puts "Hello, World!"
来源：http://pwl.c1oappe.top

C#:   Console.WriteLine("Hello, World!");
来源：http://cka.52xcode.cn

[A02] 变量声明与赋值
来源：http://ezt.jqgufenzy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hiy.fzhhl.top

PHP:  $name = "Alex"; $age = 20;
来源：http://pac.hnxiangtu.top

JS:   let name = "Alex"; const age = 20;
来源：http://ybw.cucudq.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wnw.kuanghao11.cn

Java: String name = "Alex"; int age = 20;
来源：http://zet.wangdashe.top

Go:   name := "Alex"; age := 20
来源：http://wye.yj20258888.top

Ruby: name = "Alex"; age = 20
来源：http://bcq.cucudq.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ntk.jiagoushi.top

[A03] 常量定义
来源：http://ydt.tianlin.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vwz.ybcxt.top

PHP:  const PI = 3.14159;
来源：http://gcj.xingfuxueyuan.xyz

JS:   const PI = 3.14159;
来源：http://rqi.fanxiaobao.xyz

TS:   const PI: number = 3.14159;
来源：http://urp.wangdashe.top

Java: static final double PI = 3.14159;
来源：http://nka.vqdsnc.cn

Go:   const PI = 3.14159
来源：http://bzq.tarul.cn

Ruby: PI = 3.14159
来源：http://ngc.xuetiantiany.cn

C#:   const double PI = 3.14159;
来源：http://wci.xuanzx.com

[A04] 判断变量类型
来源：http://nuk.pengpengdd.cyou

Py:   type(x).__name__; isinstance(x, int)
来源：http://jxu.sweek.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zdu.tarul.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://geo.hongshengwenyu.top

TS:   typeof x; x instanceof Date
来源：http://zlp.jyoumei.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yco.svipenyu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://epu.zdqjudy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ugt.yuxming.cn

C#:   x.GetType().Name; x is int
来源：http://fsc.9152youxi.cn

[A05] 整数除法与取模
来源：http://vgj.svipenyu.cn


<!-- 参考信息 -->