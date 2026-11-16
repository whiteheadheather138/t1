代发 wailian999

[U43] PHP：声明命名空间
来源：http://ocw.xinyue.icu

namespace App\Http;
来源：http://sqk.zhongyouzk.top

[U44] PHP：开启严格类型
来源：http://oyk.sysykeji.top

declare(strict_types=1);
来源：http://rqn.pycfn.com

[U45] PHP：类型声明与返回类型
来源：http://igg.yuanzhike.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vtc.pycfn.com

[U46] PHP：可空类型
来源：http://njq.hammf.cn

?string $name = null
来源：http://udt.52xcode.cn

[U47] PHP：联合类型
来源：http://dss.yj202588.top

int|string $id
来源：http://kxh.xuetiantiany.cn

[U48] PHP：纯枚举
来源：http://vgj.nanxuanxn.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ivw.hcnkem.com

[U49] PHP：只读属性
来源：http://byk.yfazqb.com

public readonly string $name
来源：http://tfs.yuanzhike.top

[U50] PHP：构造器属性提升
来源：http://ktw.fanxiaobao.xyz

public function __construct(private int $id) {}
来源：http://dqt.zhijiandao.cn

[U51] PHP：数组解构
来源：http://qid.fehbvm.com

[$a, $b] = $arr;
来源：http://hvh.jqgufenzy.top

[U52] PHP：箭头函数
来源：http://khh.fanxiaobao.xyz

$double = fn($x) => $x * 2;
来源：http://vjk.xylfe.cn

[U53] PHP：空合并运算符
来源：http://bux.nanxinkj.top

$v = $a ?? $b ?? "default";
来源：http://jwp.cdnleiting.top

[U54] PHP：空安全调用
来源：http://xbz.birdmap.top

$obj?->method()
来源：http://mkh.zhiwuduotai.top

[U55] PHP：match 表达式
来源：http://rgp.haohaochexian.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qpq.pycfn.com

[U56] PHP：命名参数
来源：http://ipu.chenzaomai.com

f(a: 1, b: 2)
来源：http://uda.vehdjk.com

[U57] PHP：字符串插值
来源：http://feb.yonumen.top

"值: {$a}"
来源：http://ost.ydzc1.top

[U58] PHP：数组三件套
来源：http://rcp.xingfuxueyuan.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rom.hammf.cn

[U59] PHP：自定义排序
来源：http://gba.daxiang520.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zdz.hnxiangtu.top

[U60] PHP：JSON 编解码
来源：http://guv.yonumen.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yhm.316326.xyz

[U61] PHP：正则
来源：http://dff.xinyue.icu

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qhv.jianghu66.top

[U62] PHP：日期对象
来源：http://oiy.xuanzx.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://upo.bbcook.cn

[U63] PHP：文件读写
来源：http://vck.hongshengwenyu.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zqt.epnwcf.com

[U64] PHP：目录遍历
来源：http://vnc.tian-w.cn

glob("dir/*.php");  scandir("dir");
来源：http://uig.yvedp.cn

[U65] PHP：会话
来源：http://ijp.hammf.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wui.bbcook.cn

[U66] PHP：设置 Cookie
来源：http://uiu.316326.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ury.ivvv.top

[U67] PHP：处理文件上传
来源：http://gap.wangdashe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://foj.xinyue.icu

[U68] PHP：PDO 连接
来源：http://xjx.ydzc1.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://irz.cqqwz.cn

[U69] PHP：PDO 预处理
来源：http://kxx.shanyushiyangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dpb.aibaodan.cn

[U70] PHP：PDO 事务
来源：http://nar.sjlbkw.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hwf.52xcode.cn

[U71] PHP：抛出异常
来源：http://qws.jqgufenzy.top

throw new RuntimeException("失败", 500);
来源：http://sji.316326.xyz

[U72] PHP：写错误日志
来源：http://arn.aizwys.cn

error_log("失败: " . $e->getMessage());
来源：http://jew.tian-w.cn

[U73] PHP：读取 ini 配置
来源：http://ouu.xingfuxueyuan.xyz

parse_ini_file("config.ini", true)
来源：http://qbe.ydzc1.top

[U74] PHP：读取环境变量
来源：http://thu.xinyue.icu

getenv("APP_ENV") ?: "production"
来源：http://dsi.chenlongwang.top

[U75] PHP：依赖注入
来源：http://wuf.yangfankeji.com

composer require psr/container
来源：http://vzi.daria6918.cn

[U76] PHP：简单路由
来源：http://muz.haohaochexian.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rle.cdnleiting.top

[U77] PHP：模板渲染
来源：http://srw.quarkkingdee.top

composer require twig/twig
来源：http://don.kuanghao11.cn

[U78] PHP：单元测试
来源：http://vfu.hcnkem.com

composer require --dev phpunit/phpunit
来源：http://zpm.zhaomingkeji.xyz

[U79] PHP：静态分析
来源：http://rqk.smart0.xyz

composer require --dev phpstan/phpstan
来源：http://kkc.zhijiandao.cn

[U80] PHP：代码规范修复
来源：http://amw.fehbvm.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://esf.kuanghao11.cn

[U81] JS：初始化项目
来源：http://pzm.zhongyouzk.top

npm init -y;  npm i express
来源：http://ziq.havefunace.top

[U82] JS：package.json 脚本
来源：http://jmo.daxiang520.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jlf.hongshengwenyu.top

[U83] JS：ES Module 导入导出
来源：http://taq.hysaishi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ndj.sweek.top

[U84] JS：CommonJS 写法
来源：http://evg.9152youxi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://chc.fehbvm.com

[U85] JS：可选链
来源：http://mmm.vqdsnc.cn

a?.b?.c
来源：http://bay.yanxiufei.cn

[U86] JS：空值合并
来源：http://urd.jlsjyb.cn

a ?? b
来源：http://cmf.jinqigufen.top

[U87] JS：解构默认值
来源：http://qtl.52xcode.cn

const { a = 1, b = 2 } = obj;
来源：http://vph.0kj1m.cn

[U88] JS：对象展开合并
来源：http://kpp.daria6918.cn

{ ...a, ...b }
来源：http://efr.pengpengdd.cyou

[U89] JS：数组去重
来源：http://cxh.zhongyouzk.top

[...new Set(arr)]
来源：http://bjm.yueranfly.top

[U90] JS：数字数组排序
来源：http://llt.yj20258.top

[...arr].sort((a, b) => a - b)
来源：http://dkx.aibaodan.cn

[U91] JS：对象键值遍历
来源：http://pgs.hywenlv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gan.zhixingplan.top

[U92] JS：深拷贝
来源：http://npk.ivvv.top

structuredClone(obj)
来源：http://bbu.sufxvd.cn

[U93] JS：模板字符串
来源：http://uzo.fktsv.cn

`共 ${n} 条`
来源：http://smv.ppjwa.cn

[U94] JS：箭头函数
来源：http://nxt.svipenyu.cn

const double = x => x * 2;
来源：http://wyq.gotoacloud.top

[U95] JS：Promise 包装
来源：http://slg.sweek.top

new Promise((resolve, reject) => {})
来源：http://mby.aizwys.cn

[U96] JS：async/await 与异常
来源：http://dux.gaohongyu789.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pad.yuanzhike.top

[U97] JS：并发请求
来源：http://rpz.zhongyouzk.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://yys.birdmap.top

[U98] JS：fetch 带 JSON
来源：http://iaw.hongshengwenyu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mnq.pycfn.com

[U99] JS：事件监听
来源：http://tzs.wangdashe.top

el.addEventListener("click", e => {})
来源：http://fbl.andypj.xyz

[U100] JS：DOM 查询
来源：http://geg.cdnleiting.top

document.querySelector(".item")
来源：http://dfj.sysykeji.top

[U101] JS：classList 操作
来源：http://cke.uphjek.com

el.classList.toggle("active")
来源：http://jnm.hcnkem.com

[U102] JS：本地存储
来源：http://tqq.fktsv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ufi.tarul.cn

[U103] JS：定时器
来源：http://kys.gaohongyu789.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nlm.zhiwuduotai.top

[U104] JS：防抖
来源：http://npx.fktsv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://twb.yonumen.top

[U105] JS：节流
来源：http://cua.guowangkeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ziw.jqgfzy.top

[U106] JS：日期格式化
来源：http://ufl.nanxinkj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ucs.xinyue.icu

[U107] JS：数字千分位
来源：http://vmo.gaohongyu789.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jdi.hysaishi.cn

[U108] JS：随机整数
来源：http://rtk.hnxiangtu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qoj.feifeiyinyue.top

[U109] JS：数组分组
来源：http://hrq.tian-w.cn

Object.groupBy(arr, x => x.type)
来源：http://xco.hammf.cn

[U110] JS：数组分块
来源：http://fem.zdbjq.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nor.hnxiangtu.top

[U111] JS：对象转 Map
来源：http://pua.cucudq.cn

new Map(Object.entries(obj))
来源：http://izw.hnqzz.top

[U112] JS：字符串补位
来源：http://tlq.yongpay.top

"7".padStart(3, "0")
来源：http://cjd.hesvh.cn

[U113] JS：正则替换全部
来源：http://avw.hammf.cn

s.replaceAll("a", "b")
来源：http://qot.0kj1m.cn

[U114] JS：JSON 深比较
来源：http://oio.iojbl.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qnh.birdmap.top

[U115] JS：生成 UUID
来源：http://rkt.dashuyun.cn

crypto.randomUUID()
来源：http://mam.ybcxt.top

[U116] JS：类型检查（JSDoc）
来源：http://umv.yfazqb.com

/** @param {string} name */ function f(name) {}
来源：http://mlu.guowangkeji.top

[U117] JS：单元测试
来源：http://qlx.yj202588.top

npm i -D vitest;  npx vitest
来源：http://toq.uphjek.com

[U118] JS：开发服务器
来源：http://eeg.zhengqikj.top

npm i -D vite;  npx vite
来源：http://zwr.quarkkingdee.top

[U119] JS：生产构建
来源：http://bzk.zhaomingkeji.xyz

npx vite build
来源：http://xbv.ybcxt.top

[U120] JS：读取环境变量（Vite）
来源：http://jif.cqqwz.cn

import.meta.env.VITE_API_URL
来源：http://zbi.yvedp.cn

================================================================================
来源：http://pbo.gotoacloud.top

统计汇总
来源：http://odj.quarkkingdee.top

================================================================================
来源：http://mzi.zhaomingkeji.xyz

按语言统计（条）：
来源：http://vch.haohaochexian.top

Python ......... 252
来源：http://pyt.jiagoushi.top

PHP ............ 252
来源：http://ttq.hesvh.cn

JavaScript ..... 252
来源：http://hak.cqqwz.cn

TypeScript ..... 212
来源：http://yyk.iojbl.cn

Java ........... 212
来源：http://cch.zhixingplan.top

Go ............. 212
来源：http://ltu.9152youxi.cn

Ruby ........... 212
来源：http://qhm.meibo888.top

C# ............. 212
来源：http://asa.jinyuanbaomall.cn

C .............. 30
来源：http://dzw.dashuyun.cn

C++ ............ 30
来源：http://bed.wangdashe.top

SQL ............ 90
来源：http://cpy.ywan-chungtsiang.top

Bash ........... 80
来源：http://ids.gotoacloud.top

Kotlin ......... 15
来源：http://umi.yongpay.top

Swift .......... 15
来源：http://chp.chenlongwang.top

Lua ............ 10
来源：http://hlw.pycfn.com

Perl ........... 10
来源：http://suo.redwolf501.top

Scala .......... 10
来源：http://vlu.yueranfly.top

------------------------------------
来源：http://lhf.yanxiufei.cn

合计 ........... 2106 条
来源：http://zxy.yanxiufei.cn

按章节统计：
来源：http://xwt.dianchejie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lel.jqgfzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uyc.sxryk.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ank.shanyushiyangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wnb.hesvh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lko.yvedp.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kpz.hysaishi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bqc.0kj1m.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cfo.ydjk.org.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xua.smart0.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mpb.ydjk.org.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cge.yonumen.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yyh.hysaishi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://csg.gaohongyu789.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ybw.zdqjudy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cqe.hysaishi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://chb.aizwys.cn

Q SQL 专题                              90
来源：http://xcg.snrcjt.cn

R Bash 专题                             80
来源：http://fit.yj20258888.top

S C / C++ 专题                          60
来源：http://cys.pengpengdd.cyou

T 其他语言补充                          60
来源：http://iwd.fehbvm.com

U 高频实用片段                         120
来源：http://rhz.hfpthk.cn

------------------------------------
来源：http://xvg.aizwys.cn

合计                                  2106 条
来源：http://wdb.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://nth.xuanzx.com

使用提醒
来源：http://paz.yongpay.top

--------------------------------------------------------------------------------
来源：http://cav.bbcook.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wqw.cashguo.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://uav.dianchejie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://huo.vqdsnc.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://euy.feifeiyinyue.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fna.epnwcf.com

—— 文件结束 ——
来源：http://pey.zhijiandao.cn

================================================================================
来源：http://hcn.yonumen.top

程序语言常见例子速查手册（2024 版）
来源：http://ewq.jianghu66.top

Common Programming Examples Cheat Book
来源：http://bih.zhijiandao.cn

================================================================================
来源：http://zzk.9152youxi.cn

【收录内容】
来源：http://mlq.jinqigfzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://xpx.nwbrower.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://iyo.zhiwuduotai.top

SQL · Bash · C · C++
来源：http://ljj.nanxinkj.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://eje.ehwqpu.com

【使用说明】
来源：http://bog.tian-w.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xov.sysykeji.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://eie.vqdsnc.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dvd.haohaochexian.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://aeu.zhongyouzk.top

Bash:  Shell         C:     C             C++:   C++
来源：http://vea.shzxlz.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xep.zhengqikj.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fhg.birdmap.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hju.svipenyu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://het.yuanzhike.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://snd.zhiwuduotai.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kfv.sufxvd.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uds.316326.xyz

【文件统计】
来源：http://wwp.fzhhl.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zwu.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://eyh.pengpengdd.cyou

目  录
来源：http://iap.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://uex.gogol.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yfj.zdbjq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lyl.xuanzx.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bbe.hammf.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cdr.jiagoushi.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bti.316326.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mkz.gaohongyu789.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xsc.ybcxt.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ibe.daxiang520.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://een.yj20258.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cvu.uphjek.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ynq.sweek.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lql.hcnkem.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bta.316326.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tgz.wangdashe.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vuf.ivvv.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tdl.wangshuangyany.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gdp.sysykeji.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://hcd.jlsjyb.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wxe.bjfxy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://smp.jinqigfzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jcp.gogol.net.cn

================================================================================
来源：http://eoq.guowangkeji.top

A. 基础语法与类型
来源：http://ojh.mhx1999.top

================================================================================
来源：http://tbp.vehdjk.com

[A01] Hello World
来源：http://ioo.cdnleiting.top

Py:   print("Hello, World!")
来源：http://bpy.cqqwz.cn

PHP:  echo "Hello, World!";
来源：http://baj.daria6918.cn

JS:   console.log("Hello, World!");
来源：http://rjb.zhixingplan.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://djm.yuanzhike.top

Java: System.out.println("Hello, World!");
来源：http://mir.zhengqikj.top

Go:   fmt.Println("Hello, World!")
来源：http://ljy.jqgufenzy.top

Ruby: puts "Hello, World!"
来源：http://rkk.guowangkeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://lbw.tanke756.top

[A02] 变量声明与赋值
来源：http://mhq.gaohongyu789.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://eco.dianchejie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://vei.nanxuanxn.top

JS:   let name = "Alex"; const age = 20;
来源：http://duf.nwbrower.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cjk.yueranfly.top

Java: String name = "Alex"; int age = 20;
来源：http://pfv.0kj1m.cn

Go:   name := "Alex"; age := 20
来源：http://vwi.tianlin.xyz

Ruby: name = "Alex"; age = 20
来源：http://ymn.c1oappe.top

C#:   string name = "Alex"; int age = 20;
来源：http://hua.zhengqikj.top

[A03] 常量定义
来源：http://wgg.jlsjyb.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tuo.aizwys.cn

PHP:  const PI = 3.14159;
来源：http://tba.haohaochexian.top

JS:   const PI = 3.14159;
来源：http://enc.nanxuanxn.top

TS:   const PI: number = 3.14159;
来源：http://ado.zdbjq.cn

Java: static final double PI = 3.14159;
来源：http://jat.yonumen.top

Go:   const PI = 3.14159
来源：http://bis.xziqi.cn

Ruby: PI = 3.14159
来源：http://lqq.sxryk.cn

C#:   const double PI = 3.14159;
来源：http://yvj.mhx1999.top

[A04] 判断变量类型
来源：http://ulf.zhongyouzk.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ela.zhengqikj.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bls.ppjwa.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ldk.yfazqb.com

TS:   typeof x; x instanceof Date
来源：http://kyi.smart0.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://czr.cheryme.top

Go:   reflect.TypeOf(x).Name()
来源：http://ujv.guannengcc.top

Ruby: x.class; x.is_a?(Integer)
来源：http://tbc.sweek.top

C#:   x.GetType().Name; x is int
来源：http://mgb.guowangkeji.top

[A05] 整数除法与取模
来源：http://uhk.mhx1999.top


<!-- 参考信息 -->