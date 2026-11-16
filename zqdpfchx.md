代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://qrl.yanxiufei.cn

sys.stdout.isatty()
来源：http://poe.hnqzz.top

[U40] Py：打印到标准错误
来源：http://ujj.sxryk.cn

print("err", file=sys.stderr)
来源：http://idz.zycfv.cn

[U41] PHP：初始化 Composer 项目
来源：http://mty.yj202588.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qij.jqgfzy.top

[U42] PHP：PSR-4 自动加载
来源：http://mpw.xziqi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vdr.hammf.cn

[U43] PHP：声明命名空间
来源：http://gfi.yj202588.top

namespace App\Http;
来源：http://zfv.zhaomingkeji.xyz

[U44] PHP：开启严格类型
来源：http://kuu.dashuyun.cn

declare(strict_types=1);
来源：http://nsp.smart0.xyz

[U45] PHP：类型声明与返回类型
来源：http://ykc.sxryk.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://abk.yuanzhike.top

[U46] PHP：可空类型
来源：http://mtt.nanxinkj.top

?string $name = null
来源：http://xsk.hesvh.cn

[U47] PHP：联合类型
来源：http://gkb.tarul.cn

int|string $id
来源：http://ait.xuanzx.com

[U48] PHP：纯枚举
来源：http://noo.gotoacloud.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pbq.guowangkeji.top

[U49] PHP：只读属性
来源：http://fjf.havefunace.top

public readonly string $name
来源：http://fdg.c1oappe.top

[U50] PHP：构造器属性提升
来源：http://dgz.cdnleiting.top

public function __construct(private int $id) {}
来源：http://sqz.quarkkingdee.top

[U51] PHP：数组解构
来源：http://fos.hfpthk.cn

[$a, $b] = $arr;
来源：http://wxu.smart0.xyz

[U52] PHP：箭头函数
来源：http://xyx.vqdsnc.cn

$double = fn($x) => $x * 2;
来源：http://zqe.hnxiangtu.top

[U53] PHP：空合并运算符
来源：http://hxd.zhongyouzk.top

$v = $a ?? $b ?? "default";
来源：http://ahu.sweek.top

[U54] PHP：空安全调用
来源：http://zxk.chenjidiqi.icu

$obj?->method()
来源：http://hiw.jinghuilouyu.cn

[U55] PHP：match 表达式
来源：http://aoy.ivvv.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://abv.chenlongwang.top

[U56] PHP：命名参数
来源：http://ple.yonumen.top

f(a: 1, b: 2)
来源：http://vcb.ppjwa.cn

[U57] PHP：字符串插值
来源：http://lku.jyoumei.cn

"值: {$a}"
来源：http://bst.sjlbkw.cn

[U58] PHP：数组三件套
来源：http://wbf.fanxiaobao.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pbm.jqgfzy.top

[U59] PHP：自定义排序
来源：http://tqq.gaohongyu789.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hhf.kuanghao11.cn

[U60] PHP：JSON 编解码
来源：http://cou.aibaodan.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nqj.ctjpmb.com

[U61] PHP：正则
来源：http://zer.smart0.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fzi.yuxming.cn

[U62] PHP：日期对象
来源：http://ttv.aizwys.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://iny.nanxuanxn.top

[U63] PHP：文件读写
来源：http://lkq.nanxuanxn.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xyw.guowangkeji.top

[U64] PHP：目录遍历
来源：http://xgy.gaohongyu789.top

glob("dir/*.php");  scandir("dir");
来源：http://ipx.sxryk.cn

[U65] PHP：会话
来源：http://imw.vehdjk.com

session_start();  $_SESSION["uid"] = 1;
来源：http://jrj.cqqwz.cn

[U66] PHP：设置 Cookie
来源：http://dsm.jyoumei.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jbe.jqgfzy.top

[U67] PHP：处理文件上传
来源：http://crb.nwbrower.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://clh.fengsongda.top

[U68] PHP：PDO 连接
来源：http://fzh.hcnkem.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bld.hysaishi.cn

[U69] PHP：PDO 预处理
来源：http://jcs.ppjwa.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://roj.jinghuilouyu.cn

[U70] PHP：PDO 事务
来源：http://gcf.ydzc1.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://utc.birdmap.top

[U71] PHP：抛出异常
来源：http://euf.snrcjt.cn

throw new RuntimeException("失败", 500);
来源：http://zta.xuanzx.com

[U72] PHP：写错误日志
来源：http://wnx.sysykeji.top

error_log("失败: " . $e->getMessage());
来源：http://wmy.yvedp.cn

[U73] PHP：读取 ini 配置
来源：http://mgc.yfazqb.com

parse_ini_file("config.ini", true)
来源：http://zsw.hammf.cn

[U74] PHP：读取环境变量
来源：http://som.tianlin.xyz

getenv("APP_ENV") ?: "production"
来源：http://veu.jinyuanbaomall.cn

[U75] PHP：依赖注入
来源：http://lic.smart0.xyz

composer require psr/container
来源：http://psl.yanxiufei.cn

[U76] PHP：简单路由
来源：http://lic.ivvv.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dix.pengpengdd.cyou

[U77] PHP：模板渲染
来源：http://mzj.cdnleiting.top

composer require twig/twig
来源：http://psm.jqgfzy.top

[U78] PHP：单元测试
来源：http://yxg.ydjk.org.cn

composer require --dev phpunit/phpunit
来源：http://xdh.gogol.net.cn

[U79] PHP：静态分析
来源：http://fbk.sjlbkw.cn

composer require --dev phpstan/phpstan
来源：http://ucm.fengsongda.top

[U80] PHP：代码规范修复
来源：http://dxx.yanxiufei.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qnf.316326.xyz

[U81] JS：初始化项目
来源：http://hjh.0kj1m.cn

npm init -y;  npm i express
来源：http://clx.dianchejie.cn

[U82] JS：package.json 脚本
来源：http://ais.havefunace.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fwx.ctjpmb.com

[U83] JS：ES Module 导入导出
来源：http://tcv.zycfv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bxr.yvedp.cn

[U84] JS：CommonJS 写法
来源：http://wes.yuanzhike.top

module.exports = { a };  const { a } = require("./m");
来源：http://tvq.yfazqb.com

[U85] JS：可选链
来源：http://uho.9152youxi.cn

a?.b?.c
来源：http://une.yangfankeji.com

[U86] JS：空值合并
来源：http://pqo.ywan-chungtsiang.top

a ?? b
来源：http://ybz.uphjek.com

[U87] JS：解构默认值
来源：http://bor.0kj1m.cn

const { a = 1, b = 2 } = obj;
来源：http://zmt.9152youxi.cn

[U88] JS：对象展开合并
来源：http://wzg.9152youxi.cn

{ ...a, ...b }
来源：http://fle.cdnleiting.top

[U89] JS：数组去重
来源：http://klt.meibo888.top

[...new Set(arr)]
来源：http://sbj.ehwqpu.com

[U90] JS：数字数组排序
来源：http://qut.ywan-chungtsiang.top

[...arr].sort((a, b) => a - b)
来源：http://mjn.xingfuxueyuan.xyz

[U91] JS：对象键值遍历
来源：http://loi.zhoulong.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://quh.yongpay.top

[U92] JS：深拷贝
来源：http://spn.nanxinkj.top

structuredClone(obj)
来源：http://scv.hnxiangtu.top

[U93] JS：模板字符串
来源：http://bck.jiagoushi.top

`共 ${n} 条`
来源：http://abd.zdbjq.cn

[U94] JS：箭头函数
来源：http://obs.bbcook.cn

const double = x => x * 2;
来源：http://eij.yj20258888.top

[U95] JS：Promise 包装
来源：http://vnj.yfazqb.com

new Promise((resolve, reject) => {})
来源：http://oyc.daria6918.cn

[U96] JS：async/await 与异常
来源：http://wdx.dianchejie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hff.havefunace.top

[U97] JS：并发请求
来源：http://uok.shzxlz.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qvn.guowangkeji.top

[U98] JS：fetch 带 JSON
来源：http://sel.jinyuanbaomall.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ghr.pycfn.com

[U99] JS：事件监听
来源：http://mej.chenlongwang.top

el.addEventListener("click", e => {})
来源：http://noz.zhixingplan.top

[U100] JS：DOM 查询
来源：http://qff.quarkkingdee.top

document.querySelector(".item")
来源：http://dmd.wangdashe.top

[U101] JS：classList 操作
来源：http://ssr.xziqi.cn

el.classList.toggle("active")
来源：http://ngb.fktsv.cn

[U102] JS：本地存储
来源：http://zcj.birdmap.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://yjl.yuanzhike.top

[U103] JS：定时器
来源：http://yit.zhiwuduotai.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hbn.aizwys.cn

[U104] JS：防抖
来源：http://bqr.tian-w.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wht.jinyuanbaomall.cn

[U105] JS：节流
来源：http://iiu.smart0.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vyz.yuxming.cn

[U106] JS：日期格式化
来源：http://emg.shanyushiyangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bow.cheryme.top

[U107] JS：数字千分位
来源：http://qme.sjlbkw.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://aoc.dashuyun.cn

[U108] JS：随机整数
来源：http://uvh.shanyushiyangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zpy.uphjek.com

[U109] JS：数组分组
来源：http://meg.sysykeji.top

Object.groupBy(arr, x => x.type)
来源：http://xll.vehdjk.com

[U110] JS：数组分块
来源：http://pgg.ctjpmb.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://efk.ywan-chungtsiang.top

[U111] JS：对象转 Map
来源：http://upw.wangshuangyany.cn

new Map(Object.entries(obj))
来源：http://avx.hesvh.cn

[U112] JS：字符串补位
来源：http://pax.shzxlz.cn

"7".padStart(3, "0")
来源：http://kvw.yonumen.top

[U113] JS：正则替换全部
来源：http://nmp.yanxiufei.cn

s.replaceAll("a", "b")
来源：http://idu.jianghu66.top

[U114] JS：JSON 深比较
来源：http://uzw.sjlbkw.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://les.jianghu66.top

[U115] JS：生成 UUID
来源：http://yaj.ehwqpu.com

crypto.randomUUID()
来源：http://sfj.birdmap.top

[U116] JS：类型检查（JSDoc）
来源：http://uwp.ywan-chungtsiang.top

/** @param {string} name */ function f(name) {}
来源：http://zbi.cqqwz.cn

[U117] JS：单元测试
来源：http://kqp.guowangkeji.top

npm i -D vitest;  npx vitest
来源：http://qex.ehwqpu.com

[U118] JS：开发服务器
来源：http://hnh.gotoacloud.top

npm i -D vite;  npx vite
来源：http://ctf.hcnkem.com

[U119] JS：生产构建
来源：http://unf.hcnkem.com

npx vite build
来源：http://clg.xuanzx.com

[U120] JS：读取环境变量（Vite）
来源：http://xmv.yuxming.cn

import.meta.env.VITE_API_URL
来源：http://atc.jinyuanbaomall.cn

================================================================================
来源：http://kel.snrcjt.cn

统计汇总
来源：http://cee.hcnkem.com

================================================================================
来源：http://wvy.zhengqikj.top

按语言统计（条）：
来源：http://bml.shzxlz.cn

Python ......... 252
来源：http://sfz.epnwcf.com

PHP ............ 252
来源：http://pbo.ppjwa.cn

JavaScript ..... 252
来源：http://wkv.quarkkingdee.top

TypeScript ..... 212
来源：http://dso.zhaomingkeji.xyz

Java ........... 212
来源：http://npv.cdnleiting.top

Go ............. 212
来源：http://kpp.quarkkingdee.top

Ruby ........... 212
来源：http://ixk.sweek.top

C# ............. 212
来源：http://gol.jqgfzy.top

C .............. 30
来源：http://ehu.wangshuangyany.cn

C++ ............ 30
来源：http://tfj.vqdsnc.cn

SQL ............ 90
来源：http://uby.shuidangran.top

Bash ........... 80
来源：http://arc.yvedp.cn

Kotlin ......... 15
来源：http://fbz.epnwcf.com

Swift .......... 15
来源：http://wta.sxryk.cn

Lua ............ 10
来源：http://lix.cashguo.top

Perl ........... 10
来源：http://cjz.hesvh.cn

Scala .......... 10
来源：http://sgd.xziqi.cn

------------------------------------
来源：http://tjq.sjlbkw.cn

合计 ........... 2106 条
来源：http://nan.shzxlz.cn

按章节统计：
来源：http://dqs.tarul.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qmw.9152youxi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://glq.kuanghao11.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wmg.316326.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://prf.sjlbkw.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://piv.zhaomingkeji.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dyd.yangfankeji.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cfp.daria6918.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ezt.jianghu66.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ndt.cucudq.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kfw.meibo888.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ylf.guannengcc.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wiv.sjlbkw.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kjd.gotoacloud.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://okw.hcnkem.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dja.jlsjyb.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bze.zhaomingkeji.xyz

Q SQL 专题                              90
来源：http://rgx.hnxiangtu.top

R Bash 专题                             80
来源：http://xgx.ehwqpu.com

S C / C++ 专题                          60
来源：http://swz.jianghu66.top

T 其他语言补充                          60
来源：http://xtw.daxiang520.top

U 高频实用片段                         120
来源：http://stm.gotoacloud.top

------------------------------------
来源：http://vuf.yongpay.top

合计                                  2106 条
来源：http://igv.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://tqc.jinqigufen.top

使用提醒
来源：http://rqz.hammf.cn

--------------------------------------------------------------------------------
来源：http://unf.tian-w.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vdg.shanyushiyangkeji.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zmu.shanyushiyangkeji.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wlo.hnxiangtu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://pko.andypj.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kfo.zhijiandao.cn

—— 文件结束 ——
来源：http://ptj.cucudq.cn

================================================================================
来源：http://yqk.yuxming.cn

程序语言常见例子速查手册（2024 版）
来源：http://tsc.bbcook.cn

Common Programming Examples Cheat Book
来源：http://azg.bbcook.cn

================================================================================
来源：http://eyg.zhaomingkeji.xyz

【收录内容】
来源：http://sig.0kj1m.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fhb.aibaodan.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ecc.shanyushiyangtech.top

SQL · Bash · C · C++
来源：http://ahw.shangyingyoupin.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dfm.yj20258.top

【使用说明】
来源：http://rer.9152youxi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vgr.cashguo.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gli.yuanzhike.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pse.fktsv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tcd.zhijiandao.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://uyk.yj202588.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cbb.shangyingyoupin.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wba.fehbvm.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vtc.jinghuilouyu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://odz.ydzc1.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yua.bbcook.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zto.hongshengwenyu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://loa.ivvv.top

【文件统计】
来源：http://wnq.sweek.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kff.ybcxt.top

--------------------------------------------------------------------------------
来源：http://wke.yueranfly.top

目  录
来源：http://dmw.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://hli.snrcjt.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mie.hammf.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hwq.epnwcf.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gqc.vehdjk.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uta.hongshengwenyu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pas.yuxming.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ryq.jianghu66.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://emj.pengpengdd.cyou

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zhy.yanxiufei.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jgn.jiagoushi.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nsq.xinyue.icu

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rij.sxryk.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jpp.haohaochexian.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jsb.fzhhl.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fte.cqqwz.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://twn.yj202588.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lxi.52xcode.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vff.xuanzx.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://bjx.epnwcf.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ljb.dianchejie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cva.jlsjyb.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vlh.sweek.top

================================================================================
来源：http://kdq.hongshengwenyu.top

A. 基础语法与类型
来源：http://fog.jinqigufen.top

================================================================================
来源：http://dbm.9152youxi.cn

[A01] Hello World
来源：http://ltz.chenzaomai.com

Py:   print("Hello, World!")
来源：http://gky.yuxming.cn

PHP:  echo "Hello, World!";
来源：http://dnf.nanxinkj.top

JS:   console.log("Hello, World!");
来源：http://twd.andypj.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://miq.bbcook.cn

Java: System.out.println("Hello, World!");
来源：http://gpj.yj20258.top

Go:   fmt.Println("Hello, World!")
来源：http://qjt.quarkkingdee.top

Ruby: puts "Hello, World!"
来源：http://eza.pengpengdd.cyou

C#:   Console.WriteLine("Hello, World!");
来源：http://czk.yvedp.cn

[A02] 变量声明与赋值
来源：http://ikh.yueranfly.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://aoq.hnqzz.top

PHP:  $name = "Alex"; $age = 20;
来源：http://kxr.pycfn.com

JS:   let name = "Alex"; const age = 20;
来源：http://zwx.fehbvm.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://iro.bjfxy.top

Java: String name = "Alex"; int age = 20;
来源：http://gni.vehdjk.com

Go:   name := "Alex"; age := 20
来源：http://yal.aizwys.cn

Ruby: name = "Alex"; age = 20
来源：http://yfy.kuanghao11.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ebj.wangdashe.top

[A03] 常量定义
来源：http://psi.yj20258.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sor.yfazqb.com

PHP:  const PI = 3.14159;
来源：http://fec.tarul.cn

JS:   const PI = 3.14159;
来源：http://xff.smart0.xyz

TS:   const PI: number = 3.14159;
来源：http://zqq.zdbjq.cn

Java: static final double PI = 3.14159;
来源：http://ztu.zycfv.cn

Go:   const PI = 3.14159
来源：http://qjw.daria6918.cn

Ruby: PI = 3.14159
来源：http://gyi.daxiang520.top

C#:   const double PI = 3.14159;
来源：http://eww.sxryk.cn

[A04] 判断变量类型
来源：http://hyg.jqgfzy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://mrp.aizwys.cn


<!-- 参考信息 -->