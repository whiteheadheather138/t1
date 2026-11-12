代发 wailian999

[U43] PHP：声明命名空间
来源：http://zof.tanke756.top

namespace App\Http;
来源：http://jxk.gaohongyu789.top

[U44] PHP：开启严格类型
来源：http://uyc.uphjek.com

declare(strict_types=1);
来源：http://azj.sjlbkw.cn

[U45] PHP：类型声明与返回类型
来源：http://mlr.tian-w.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mpc.gzhubu.top

[U46] PHP：可空类型
来源：http://yhd.hnxiangtu.top

?string $name = null
来源：http://bqp.yfazqb.com

[U47] PHP：联合类型
来源：http://aft.feifeiyinyue.top

int|string $id
来源：http://dde.ydzc1.top

[U48] PHP：纯枚举
来源：http://ubq.zhaomingkeji.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hsd.c1oappe.top

[U49] PHP：只读属性
来源：http://lva.ydzc1.top

public readonly string $name
来源：http://jmo.cashguo.top

[U50] PHP：构造器属性提升
来源：http://lkq.hnqzz.top

public function __construct(private int $id) {}
来源：http://zcg.yfazqb.com

[U51] PHP：数组解构
来源：http://hke.fehbvm.com

[$a, $b] = $arr;
来源：http://rub.havefunace.top

[U52] PHP：箭头函数
来源：http://lqp.sweek.top

$double = fn($x) => $x * 2;
来源：http://mmv.svipenyu.cn

[U53] PHP：空合并运算符
来源：http://iwq.fzhhl.top

$v = $a ?? $b ?? "default";
来源：http://uuk.hcnkem.com

[U54] PHP：空安全调用
来源：http://maj.zhengqikj.top

$obj?->method()
来源：http://wgk.fengsongda.top

[U55] PHP：match 表达式
来源：http://gem.aibaodan.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fgf.shangyingyoupin.top

[U56] PHP：命名参数
来源：http://klc.hammf.cn

f(a: 1, b: 2)
来源：http://vhn.guannengcc.top

[U57] PHP：字符串插值
来源：http://zny.nanxuanxn.top

"值: {$a}"
来源：http://bbg.ybcxt.top

[U58] PHP：数组三件套
来源：http://ywu.gaohongyu789.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zta.jqgufenzy.top

[U59] PHP：自定义排序
来源：http://ndh.jinyuanbaomall.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mkc.c1oappe.top

[U60] PHP：JSON 编解码
来源：http://frg.zhongyouzk.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bui.iojbl.cn

[U61] PHP：正则
来源：http://ukl.fktsv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qfb.c1oappe.top

[U62] PHP：日期对象
来源：http://kmv.daria6918.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://oiz.yuanzhike.top

[U63] PHP：文件读写
来源：http://klo.pycfn.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tkr.hnxiangtu.top

[U64] PHP：目录遍历
来源：http://pdx.zhengqikj.top

glob("dir/*.php");  scandir("dir");
来源：http://vcd.chenjidiqi.icu

[U65] PHP：会话
来源：http://ntv.dashuyun.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://eee.yvedp.cn

[U66] PHP：设置 Cookie
来源：http://rof.jinyuanbaomall.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lpr.yvedp.cn

[U67] PHP：处理文件上传
来源：http://rhj.svipenyu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zwy.xingfuxueyuan.xyz

[U68] PHP：PDO 连接
来源：http://ytm.gotoacloud.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://udr.snrcjt.cn

[U69] PHP：PDO 预处理
来源：http://zao.guowangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qlf.feifeiyinyue.top

[U70] PHP：PDO 事务
来源：http://ecx.zhaomingkeji.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://giv.hnqzz.top

[U71] PHP：抛出异常
来源：http://qxk.dianchejie.cn

throw new RuntimeException("失败", 500);
来源：http://tgw.zhongyouzk.top

[U72] PHP：写错误日志
来源：http://niu.daria6918.cn

error_log("失败: " . $e->getMessage());
来源：http://kce.haohaochexian.top

[U73] PHP：读取 ini 配置
来源：http://bhm.andypj.xyz

parse_ini_file("config.ini", true)
来源：http://ebo.daria6918.cn

[U74] PHP：读取环境变量
来源：http://iko.daria6918.cn

getenv("APP_ENV") ?: "production"
来源：http://ief.cdnleiting.top

[U75] PHP：依赖注入
来源：http://yoc.aibaodan.cn

composer require psr/container
来源：http://cvu.zhongyouzk.top

[U76] PHP：简单路由
来源：http://omc.gaohongyu789.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ski.nanxinkj.top

[U77] PHP：模板渲染
来源：http://mbl.hywenlv.cn

composer require twig/twig
来源：http://zkp.sjlbkw.cn

[U78] PHP：单元测试
来源：http://mdf.jinqigfzy.top

composer require --dev phpunit/phpunit
来源：http://paq.pycfn.com

[U79] PHP：静态分析
来源：http://ddm.316326.xyz

composer require --dev phpstan/phpstan
来源：http://mth.jinqigfzy.top

[U80] PHP：代码规范修复
来源：http://uzf.xylfe.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fwj.xuanzx.com

[U81] JS：初始化项目
来源：http://crp.fanxiaobao.xyz

npm init -y;  npm i express
来源：http://nxe.shuidangran.top

[U82] JS：package.json 脚本
来源：http://osp.tanke756.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://goy.xziqi.cn

[U83] JS：ES Module 导入导出
来源：http://lbd.hysaishi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dtg.sweek.top

[U84] JS：CommonJS 写法
来源：http://dka.zhiwuduotai.top

module.exports = { a };  const { a } = require("./m");
来源：http://pjk.fktsv.cn

[U85] JS：可选链
来源：http://cuv.fanxiaobao.xyz

a?.b?.c
来源：http://mmx.meibo888.top

[U86] JS：空值合并
来源：http://nwk.52xcode.cn

a ?? b
来源：http://oix.daxiang520.top

[U87] JS：解构默认值
来源：http://dno.zhaomingkeji.xyz

const { a = 1, b = 2 } = obj;
来源：http://hsd.zhiwuduotai.top

[U88] JS：对象展开合并
来源：http://tqi.wangshuangyany.cn

{ ...a, ...b }
来源：http://fbk.9152youxi.cn

[U89] JS：数组去重
来源：http://vjr.kuanghao11.cn

[...new Set(arr)]
来源：http://ikc.jinghuilouyu.cn

[U90] JS：数字数组排序
来源：http://gfo.pycfn.com

[...arr].sort((a, b) => a - b)
来源：http://wvb.fktsv.cn

[U91] JS：对象键值遍历
来源：http://bfd.chenzaomai.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://iva.yj202588.top

[U92] JS：深拷贝
来源：http://nas.0kj1m.cn

structuredClone(obj)
来源：http://fxe.feifeiyinyue.top

[U93] JS：模板字符串
来源：http://kpg.yongpay.top

`共 ${n} 条`
来源：http://rad.vehdjk.com

[U94] JS：箭头函数
来源：http://ziz.dianchejie.cn

const double = x => x * 2;
来源：http://jji.hnqzz.top

[U95] JS：Promise 包装
来源：http://vyc.zhongyouzk.top

new Promise((resolve, reject) => {})
来源：http://uwz.wangshuangyany.cn

[U96] JS：async/await 与异常
来源：http://jhq.tianlin.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://snm.yuxming.cn

[U97] JS：并发请求
来源：http://jtz.chenjidiqi.icu

await Promise.all(urls.map(u => fetch(u)))
来源：http://txh.gaohongyu789.top

[U98] JS：fetch 带 JSON
来源：http://rnr.jinqigfzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://odc.jinghuilouyu.cn

[U99] JS：事件监听
来源：http://cvw.ydzc1.top

el.addEventListener("click", e => {})
来源：http://egt.cdnleiting.top

[U100] JS：DOM 查询
来源：http://pqd.svipenyu.cn

document.querySelector(".item")
来源：http://ifz.vqdsnc.cn

[U101] JS：classList 操作
来源：http://lfm.ywan-chungtsiang.top

el.classList.toggle("active")
来源：http://qja.vqdsnc.cn

[U102] JS：本地存储
来源：http://wft.yj20258.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://esl.iojbl.cn

[U103] JS：定时器
来源：http://jdj.aizwys.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dof.c1oappe.top

[U104] JS：防抖
来源：http://opb.gotoacloud.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dti.chenjidiqi.icu

[U105] JS：节流
来源：http://enp.hysaishi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://giw.tarul.cn

[U106] JS：日期格式化
来源：http://ptn.daxiang520.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://aif.tarul.cn

[U107] JS：数字千分位
来源：http://yfz.yj20258888.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ejl.jlsjyb.cn

[U108] JS：随机整数
来源：http://jvv.nanxuanxn.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yrn.pengpengdd.cyou

[U109] JS：数组分组
来源：http://mop.zhixingplan.top

Object.groupBy(arr, x => x.type)
来源：http://rbg.vqdsnc.cn

[U110] JS：数组分块
来源：http://bme.zhengqikj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lhv.sweek.top

[U111] JS：对象转 Map
来源：http://zag.ydzc1.top

new Map(Object.entries(obj))
来源：http://vaq.jinqigufen.top

[U112] JS：字符串补位
来源：http://uzb.ctjpmb.com

"7".padStart(3, "0")
来源：http://lgw.hammf.cn

[U113] JS：正则替换全部
来源：http://zto.nwbrower.top

s.replaceAll("a", "b")
来源：http://egx.sweek.top

[U114] JS：JSON 深比较
来源：http://ukv.cheryme.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://xdy.chenjidiqi.icu

[U115] JS：生成 UUID
来源：http://zro.xingfuxueyuan.xyz

crypto.randomUUID()
来源：http://jgj.snrcjt.cn

[U116] JS：类型检查（JSDoc）
来源：http://miz.jiagoushi.top

/** @param {string} name */ function f(name) {}
来源：http://ink.quarkkingdee.top

[U117] JS：单元测试
来源：http://ozl.chenlongwang.top

npm i -D vitest;  npx vitest
来源：http://emz.cdnleiting.top

[U118] JS：开发服务器
来源：http://vzh.shanyushiyangkeji.top

npm i -D vite;  npx vite
来源：http://aid.havefunace.top

[U119] JS：生产构建
来源：http://thu.c1oappe.top

npx vite build
来源：http://pcp.tianlin.xyz

[U120] JS：读取环境变量（Vite）
来源：http://rpb.bbcook.cn

import.meta.env.VITE_API_URL
来源：http://hbf.fehbvm.com

================================================================================
来源：http://yzx.bbcook.cn

统计汇总
来源：http://bvc.cqqwz.cn

================================================================================
来源：http://pib.zycfv.cn

按语言统计（条）：
来源：http://web.hongshengwenyu.top

Python ......... 252
来源：http://nyx.xziqi.cn

PHP ............ 252
来源：http://yoe.xingfuxueyuan.xyz

JavaScript ..... 252
来源：http://gex.pycfn.com

TypeScript ..... 212
来源：http://tka.fktsv.cn

Java ........... 212
来源：http://akk.xziqi.cn

Go ............. 212
来源：http://qhe.tian-w.cn

Ruby ........... 212
来源：http://jtj.hywenlv.cn

C# ............. 212
来源：http://oee.zdbjq.cn

C .............. 30
来源：http://ick.fengsongda.top

C++ ............ 30
来源：http://tql.316326.xyz

SQL ............ 90
来源：http://ulb.gzhubu.top

Bash ........... 80
来源：http://pyz.kuanghao11.cn

Kotlin ......... 15
来源：http://rqi.birdmap.top

Swift .......... 15
来源：http://wgw.ydzc1.top

Lua ............ 10
来源：http://yuv.guowangkeji.top

Perl ........... 10
来源：http://esw.hnxiangtu.top

Scala .......... 10
来源：http://xnx.fanxiaobao.xyz

------------------------------------
来源：http://lgx.52xcode.cn

合计 ........... 2106 条
来源：http://rtd.cashguo.top

按章节统计：
来源：http://zdt.zdqjudy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dio.yongpay.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://csw.hnqzz.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://azx.yuanzhike.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jsk.hcnkem.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zec.gaohongyu789.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bed.pycfn.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rkm.jianghu66.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xhc.jqgfzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wws.tanke756.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cfg.xziqi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://spz.chenlongwang.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sck.hfpthk.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dkw.gotoacloud.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vzu.jlsjyb.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rue.jinghuilouyu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ilv.meibo888.top

Q SQL 专题                              90
来源：http://fok.shanyushiyangkeji.top

R Bash 专题                             80
来源：http://jij.chenjidiqi.icu

S C / C++ 专题                          60
来源：http://juf.nanxinkj.top

T 其他语言补充                          60
来源：http://dfz.zhengqikj.top

U 高频实用片段                         120
来源：http://nal.jinqigfzy.top

------------------------------------
来源：http://wby.hysaishi.cn

合计                                  2106 条
来源：http://fii.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://yzw.jinqigfzy.top

使用提醒
来源：http://thr.cucudq.cn

--------------------------------------------------------------------------------
来源：http://zfn.epnwcf.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ocy.daria6918.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fdp.jinqigufen.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uhs.jyoumei.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fem.mhx1999.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qdz.gaohongyu789.top

—— 文件结束 ——
来源：http://awa.xuanzx.com

================================================================================
来源：http://qsy.pycfn.com

程序语言常见例子速查手册（2024 版）
来源：http://iek.jinqigufen.top

Common Programming Examples Cheat Book
来源：http://enu.birdmap.top

================================================================================
来源：http://wio.dashuyun.cn

【收录内容】
来源：http://kvb.nanxinkj.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://cao.haohaochexian.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cua.ybcxt.top

SQL · Bash · C · C++
来源：http://zyf.jyoumei.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gte.zhiwuduotai.top

【使用说明】
来源：http://zfk.shuidangran.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://eax.daxiang520.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mkz.jyoumei.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://iey.pycfn.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://oqd.wangdashe.top

Bash:  Shell         C:     C             C++:   C++
来源：http://jqq.snrcjt.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gsn.xinyue.icu

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vbd.zhiwuduotai.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wiy.cucudq.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ijl.jqgufenzy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hwb.bjfxy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gle.guowangkeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jom.hesvh.cn

【文件统计】
来源：http://ghc.yuxming.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://elb.hcnkem.com

--------------------------------------------------------------------------------
来源：http://jrn.zhongyouzk.top

目  录
来源：http://gkg.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://zfc.bbcook.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sue.ybcxt.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fzj.pengpengdd.cyou

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://son.yonumen.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://meu.xylfe.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wnf.yfazqb.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hkj.ydjk.org.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://eue.vehdjk.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nsx.xuanzx.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mef.aibaodan.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://iet.aizwys.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bit.ydzc1.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://iaf.zycfv.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qdl.havefunace.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://off.hongshengwenyu.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yjy.aizwys.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dli.zhoulong.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://txq.zhijiandao.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xwe.yj20258888.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zgu.fanxiaobao.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fyc.gzhubu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ehd.iojbl.cn

================================================================================
来源：http://eof.andypj.xyz

A. 基础语法与类型
来源：http://msy.daxiang520.top

================================================================================
来源：http://znr.iojbl.cn

[A01] Hello World
来源：http://vyu.gotoacloud.top

Py:   print("Hello, World!")
来源：http://kec.guannengcc.top

PHP:  echo "Hello, World!";
来源：http://dng.zycfv.cn

JS:   console.log("Hello, World!");
来源：http://gvm.fzhhl.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mag.tanke756.top

Java: System.out.println("Hello, World!");
来源：http://joq.hcnkem.com

Go:   fmt.Println("Hello, World!")
来源：http://cav.xziqi.cn

Ruby: puts "Hello, World!"
来源：http://tzt.fktsv.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jmo.fzhhl.top

[A02] 变量声明与赋值
来源：http://ynp.tarul.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://odo.mhx1999.top

PHP:  $name = "Alex"; $age = 20;
来源：http://nqu.tanke756.top

JS:   let name = "Alex"; const age = 20;
来源：http://hjo.ivvv.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ecw.birdmap.top

Java: String name = "Alex"; int age = 20;
来源：http://mcz.tanke756.top

Go:   name := "Alex"; age := 20
来源：http://pyx.tian-w.cn

Ruby: name = "Alex"; age = 20
来源：http://pfi.dashuyun.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ath.sjlbkw.cn

[A03] 常量定义
来源：http://nbz.zhixingplan.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://aeg.zhaomingkeji.xyz

PHP:  const PI = 3.14159;
来源：http://raf.daria6918.cn

JS:   const PI = 3.14159;
来源：http://gyd.gzhubu.top

TS:   const PI: number = 3.14159;
来源：http://kge.yvedp.cn

Java: static final double PI = 3.14159;
来源：http://url.52xcode.cn

Go:   const PI = 3.14159
来源：http://bjz.nanxuanxn.top

Ruby: PI = 3.14159
来源：http://pqq.ppjwa.cn

C#:   const double PI = 3.14159;
来源：http://hgp.zhaomingkeji.xyz

[A04] 判断变量类型
来源：http://utc.sjlbkw.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://nnm.zdbjq.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ytd.zdbjq.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wqo.daria6918.cn

TS:   typeof x; x instanceof Date
来源：http://tdt.jqgfzy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://noj.c1oappe.top

Go:   reflect.TypeOf(x).Name()
来源：http://hcf.vehdjk.com

Ruby: x.class; x.is_a?(Integer)
来源：http://dbt.aizwys.cn

C#:   x.GetType().Name; x is int
来源：http://geb.fktsv.cn

[A05] 整数除法与取模
来源：http://ovz.316326.xyz


<!-- 参考信息 -->