代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://hjg.birdmap.top

sys.stdout.isatty()
来源：http://paq.daria6918.cn

[U40] Py：打印到标准错误
来源：http://cej.ydzc1.top

print("err", file=sys.stderr)
来源：http://osc.hcnkem.com

[U41] PHP：初始化 Composer 项目
来源：http://pzf.yj20258888.top

composer init;  composer require guzzlehttp/guzzle
来源：http://rjb.epnwcf.com

[U42] PHP：PSR-4 自动加载
来源：http://mnw.zhengqikj.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bjs.fanxiaobao.xyz

[U43] PHP：声明命名空间
来源：http://rgo.tianlin.xyz

namespace App\Http;
来源：http://btz.hesvh.cn

[U44] PHP：开启严格类型
来源：http://asq.jiagoushi.top

declare(strict_types=1);
来源：http://ijh.jlsjyb.cn

[U45] PHP：类型声明与返回类型
来源：http://msw.tianlin.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://vli.nanxinkj.top

[U46] PHP：可空类型
来源：http://ixq.iojbl.cn

?string $name = null
来源：http://toz.0kj1m.cn

[U47] PHP：联合类型
来源：http://qqb.xuanzx.com

int|string $id
来源：http://tky.yj20258888.top

[U48] PHP：纯枚举
来源：http://gpr.hcnkem.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yjj.sjlbkw.cn

[U49] PHP：只读属性
来源：http://dev.yj20258.top

public readonly string $name
来源：http://szx.svipenyu.cn

[U50] PHP：构造器属性提升
来源：http://cle.daxiang520.top

public function __construct(private int $id) {}
来源：http://kce.vqdsnc.cn

[U51] PHP：数组解构
来源：http://txh.aibaodan.cn

[$a, $b] = $arr;
来源：http://lci.quarkkingdee.top

[U52] PHP：箭头函数
来源：http://anr.cqqwz.cn

$double = fn($x) => $x * 2;
来源：http://fnh.snrcjt.cn

[U53] PHP：空合并运算符
来源：http://zih.birdmap.top

$v = $a ?? $b ?? "default";
来源：http://nbi.fengsongda.top

[U54] PHP：空安全调用
来源：http://bnl.shuidangran.top

$obj?->method()
来源：http://kqx.nanxuanxn.top

[U55] PHP：match 表达式
来源：http://ndl.fehbvm.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bvx.daria6918.cn

[U56] PHP：命名参数
来源：http://ocq.svipenyu.cn

f(a: 1, b: 2)
来源：http://hpy.shangyingyoupin.top

[U57] PHP：字符串插值
来源：http://vwi.nwbrower.top

"值: {$a}"
来源：http://lxc.ehwqpu.com

[U58] PHP：数组三件套
来源：http://qhe.ydzc1.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://esq.zhongyouzk.top

[U59] PHP：自定义排序
来源：http://yzp.ydzc1.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aid.sweek.top

[U60] PHP：JSON 编解码
来源：http://tfp.jinyuanbaomall.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yun.aibaodan.cn

[U61] PHP：正则
来源：http://rfx.nanxuanxn.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uhz.hongshengwenyu.top

[U62] PHP：日期对象
来源：http://cfz.vqdsnc.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://suz.316326.xyz

[U63] PHP：文件读写
来源：http://nqq.xylfe.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jmo.yfazqb.com

[U64] PHP：目录遍历
来源：http://hwc.c1oappe.top

glob("dir/*.php");  scandir("dir");
来源：http://mrc.gaohongyu789.top

[U65] PHP：会话
来源：http://stl.vehdjk.com

session_start();  $_SESSION["uid"] = 1;
来源：http://wru.zdqjudy.top

[U66] PHP：设置 Cookie
来源：http://ola.sweek.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://otb.aibaodan.cn

[U67] PHP：处理文件上传
来源：http://ior.fktsv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mbf.jyoumei.cn

[U68] PHP：PDO 连接
来源：http://vdj.yuxming.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uzi.jianghu66.top

[U69] PHP：PDO 预处理
来源：http://szj.hnqzz.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ykt.hfpthk.cn

[U70] PHP：PDO 事务
来源：http://qfb.dashuyun.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jes.shuidangran.top

[U71] PHP：抛出异常
来源：http://edy.tanke756.top

throw new RuntimeException("失败", 500);
来源：http://whh.cdnleiting.top

[U72] PHP：写错误日志
来源：http://jjp.cashguo.top

error_log("失败: " . $e->getMessage());
来源：http://zvj.nanxinkj.top

[U73] PHP：读取 ini 配置
来源：http://bfx.jinqigfzy.top

parse_ini_file("config.ini", true)
来源：http://ptb.jinyuanbaomall.cn

[U74] PHP：读取环境变量
来源：http://eqw.havefunace.top

getenv("APP_ENV") ?: "production"
来源：http://qco.sjlbkw.cn

[U75] PHP：依赖注入
来源：http://inb.sweek.top

composer require psr/container
来源：http://tsg.hesvh.cn

[U76] PHP：简单路由
来源：http://pyi.tianlin.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://veo.fanxiaobao.xyz

[U77] PHP：模板渲染
来源：http://lqj.ywan-chungtsiang.top

composer require twig/twig
来源：http://kze.jiagoushi.top

[U78] PHP：单元测试
来源：http://wxn.yj202588.top

composer require --dev phpunit/phpunit
来源：http://rgq.gaohongyu789.top

[U79] PHP：静态分析
来源：http://dbh.hnqzz.top

composer require --dev phpstan/phpstan
来源：http://fkq.epnwcf.com

[U80] PHP：代码规范修复
来源：http://ogl.haohaochexian.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://bct.gzhubu.top

[U81] JS：初始化项目
来源：http://bhq.xylfe.cn

npm init -y;  npm i express
来源：http://qer.shzxlz.cn

[U82] JS：package.json 脚本
来源：http://lfx.hysaishi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lkl.pengpengdd.cyou

[U83] JS：ES Module 导入导出
来源：http://wpz.hnxiangtu.top

export const a = 1;  import { a } from "./m.js";
来源：http://auj.andypj.xyz

[U84] JS：CommonJS 写法
来源：http://tfw.yj20258888.top

module.exports = { a };  const { a } = require("./m");
来源：http://hmh.hnxiangtu.top

[U85] JS：可选链
来源：http://fhs.feifeiyinyue.top

a?.b?.c
来源：http://xwf.yuanzhike.top

[U86] JS：空值合并
来源：http://rpn.yj20258888.top

a ?? b
来源：http://qhb.zhongyouzk.top

[U87] JS：解构默认值
来源：http://cha.fzhhl.top

const { a = 1, b = 2 } = obj;
来源：http://xyj.epnwcf.com

[U88] JS：对象展开合并
来源：http://kqk.yuanzhike.top

{ ...a, ...b }
来源：http://mva.tian-w.cn

[U89] JS：数组去重
来源：http://hmo.hesvh.cn

[...new Set(arr)]
来源：http://bml.zhengqikj.top

[U90] JS：数字数组排序
来源：http://qxf.hysaishi.cn

[...arr].sort((a, b) => a - b)
来源：http://iye.redwolf501.top

[U91] JS：对象键值遍历
来源：http://qia.ydjk.org.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://znu.jinqigfzy.top

[U92] JS：深拷贝
来源：http://ifb.haohaochexian.top

structuredClone(obj)
来源：http://mre.zdqjudy.top

[U93] JS：模板字符串
来源：http://sxw.jiagoushi.top

`共 ${n} 条`
来源：http://dcs.havefunace.top

[U94] JS：箭头函数
来源：http://nfh.hywenlv.cn

const double = x => x * 2;
来源：http://xqz.jinqigufen.top

[U95] JS：Promise 包装
来源：http://omz.feifeiyinyue.top

new Promise((resolve, reject) => {})
来源：http://vrs.nanxuanxn.top

[U96] JS：async/await 与异常
来源：http://slz.haohaochexian.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://myh.cqqwz.cn

[U97] JS：并发请求
来源：http://ojs.yvedp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://esh.zhengqikj.top

[U98] JS：fetch 带 JSON
来源：http://adg.yuxming.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ews.epnwcf.com

[U99] JS：事件监听
来源：http://ttr.svipenyu.cn

el.addEventListener("click", e => {})
来源：http://ggo.vehdjk.com

[U100] JS：DOM 查询
来源：http://rdm.ydjk.org.cn

document.querySelector(".item")
来源：http://kco.gotoacloud.top

[U101] JS：classList 操作
来源：http://plf.yj20258.top

el.classList.toggle("active")
来源：http://avy.fanxiaobao.xyz

[U102] JS：本地存储
来源：http://wjn.kuanghao11.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://edg.zhixingplan.top

[U103] JS：定时器
来源：http://qlz.jianghu66.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vnb.jianghu66.top

[U104] JS：防抖
来源：http://lvf.iojbl.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qyl.hcnkem.com

[U105] JS：节流
来源：http://kmx.hysaishi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fim.pengpengdd.cyou

[U106] JS：日期格式化
来源：http://lqu.yongpay.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sml.yanxiufei.cn

[U107] JS：数字千分位
来源：http://zak.jqgufenzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ccj.zhiwuduotai.top

[U108] JS：随机整数
来源：http://zro.0kj1m.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gfa.fengsongda.top

[U109] JS：数组分组
来源：http://yme.sufxvd.cn

Object.groupBy(arr, x => x.type)
来源：http://trh.xylfe.cn

[U110] JS：数组分块
来源：http://lqk.snrcjt.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dym.ctjpmb.com

[U111] JS：对象转 Map
来源：http://yvy.tian-w.cn

new Map(Object.entries(obj))
来源：http://kes.zycfv.cn

[U112] JS：字符串补位
来源：http://zwg.guannengcc.top

"7".padStart(3, "0")
来源：http://yxw.iojbl.cn

[U113] JS：正则替换全部
来源：http://vbg.hnxiangtu.top

s.replaceAll("a", "b")
来源：http://pek.hfpthk.cn

[U114] JS：JSON 深比较
来源：http://mjc.fktsv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qzn.jiagoushi.top

[U115] JS：生成 UUID
来源：http://xwu.jqgufenzy.top

crypto.randomUUID()
来源：http://muw.chenjidiqi.icu

[U116] JS：类型检查（JSDoc）
来源：http://wcu.ydzc1.top

/** @param {string} name */ function f(name) {}
来源：http://cio.shanyushiyangkeji.top

[U117] JS：单元测试
来源：http://mfn.vqdsnc.cn

npm i -D vitest;  npx vitest
来源：http://npz.yueranfly.top

[U118] JS：开发服务器
来源：http://blq.birdmap.top

npm i -D vite;  npx vite
来源：http://vzc.vehdjk.com

[U119] JS：生产构建
来源：http://kkx.0kj1m.cn

npx vite build
来源：http://zjw.wangshuangyany.cn

[U120] JS：读取环境变量（Vite）
来源：http://tls.yuanzhike.top

import.meta.env.VITE_API_URL
来源：http://ffp.nanxinkj.top

================================================================================
来源：http://ivd.tianlin.xyz

统计汇总
来源：http://ptj.vehdjk.com

================================================================================
来源：http://epv.hywenlv.cn

按语言统计（条）：
来源：http://ugq.shuidangran.top

Python ......... 252
来源：http://hmd.yuanzhike.top

PHP ............ 252
来源：http://pec.0kj1m.cn

JavaScript ..... 252
来源：http://oib.yueranfly.top

TypeScript ..... 212
来源：http://yel.ctjpmb.com

Java ........... 212
来源：http://rpz.daxiang520.top

Go ............. 212
来源：http://nhh.shzxlz.cn

Ruby ........... 212
来源：http://bqu.zdqjudy.top

C# ............. 212
来源：http://dbg.jinyuanbaomall.cn

C .............. 30
来源：http://llq.jianghu66.top

C++ ............ 30
来源：http://csm.dashuyun.cn

SQL ............ 90
来源：http://pnk.bbcook.cn

Bash ........... 80
来源：http://uuz.xuanzx.com

Kotlin ......... 15
来源：http://iul.nanxinkj.top

Swift .......... 15
来源：http://oel.aizwys.cn

Lua ............ 10
来源：http://fro.zhijiandao.cn

Perl ........... 10
来源：http://kyi.chenlongwang.top

Scala .......... 10
来源：http://uar.9152youxi.cn

------------------------------------
来源：http://czm.yj20258888.top

合计 ........... 2106 条
来源：http://vry.kuanghao11.cn

按章节统计：
来源：http://vhm.zdbjq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zlg.hnqzz.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tjr.bbcook.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zia.jqgfzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bas.jlsjyb.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bsx.yueranfly.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://alr.epnwcf.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mgm.hammf.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jcd.gaohongyu789.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dab.tarul.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://srd.jiagoushi.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wyv.zhixingplan.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zcb.pycfn.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cml.jinyuanbaomall.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rhh.gogol.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mxh.wangdashe.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hyl.xingfuxueyuan.xyz

Q SQL 专题                              90
来源：http://iro.cdnleiting.top

R Bash 专题                             80
来源：http://bzq.jqgfzy.top

S C / C++ 专题                          60
来源：http://qio.zhixingplan.top

T 其他语言补充                          60
来源：http://qqo.hcnkem.com

U 高频实用片段                         120
来源：http://pgp.nanxuanxn.top

------------------------------------
来源：http://hcz.shuidangran.top

合计                                  2106 条
来源：http://cpd.yuxming.cn

--------------------------------------------------------------------------------
来源：http://ewo.nanxinkj.top

使用提醒
来源：http://cuo.andypj.xyz

--------------------------------------------------------------------------------
来源：http://tir.gotoacloud.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rty.hywenlv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tup.xuetiantiany.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yhe.ctjpmb.com

在旧版本上使用前请先确认语法支持情况。
来源：http://rko.yvedp.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ikk.ppjwa.cn

—— 文件结束 ——
来源：http://ddn.xingfuxueyuan.xyz

================================================================================
来源：http://fpf.guowangkeji.top

程序语言常见例子速查手册（2024 版）
来源：http://fcs.hammf.cn

Common Programming Examples Cheat Book
来源：http://hwn.haohaochexian.top

================================================================================
来源：http://mdk.guowangkeji.top

【收录内容】
来源：http://xhu.tanke756.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://xiu.fktsv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cuy.xuanzx.com

SQL · Bash · C · C++
来源：http://rut.yueranfly.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dsf.52xcode.cn

【使用说明】
来源：http://jof.yuanzhike.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ftj.zdqjudy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qep.tian-w.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ukb.snrcjt.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://syj.ywan-chungtsiang.top

Bash:  Shell         C:     C             C++:   C++
来源：http://aqe.gogol.net.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fer.yj20258888.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://efs.ppjwa.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gyt.nanxuanxn.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cav.snrcjt.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rcs.yj202588.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jbf.ywan-chungtsiang.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pmo.shangyingyoupin.top

【文件统计】
来源：http://aci.yj202588.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://eiv.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://gtv.aibaodan.cn

目  录
来源：http://xot.xuanzx.com

--------------------------------------------------------------------------------
来源：http://fjz.cdnleiting.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ixl.gotoacloud.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hlh.jiagoushi.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lzk.zhiwuduotai.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rit.zhiwuduotai.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lnb.hywenlv.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wer.zhaomingkeji.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kyj.jinghuilouyu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qru.yonumen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ofi.bbcook.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://uxw.tianlin.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://trs.yj20258.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ctb.quarkkingdee.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wtd.jqgufenzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vux.xuetiantiany.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hpi.0kj1m.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mlk.quarkkingdee.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bov.c1oappe.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://unj.xinyue.icu

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oqn.vqdsnc.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ifr.daria6918.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pyw.ydjk.org.cn

================================================================================
来源：http://izz.xingfuxueyuan.xyz

A. 基础语法与类型
来源：http://ezs.fanxiaobao.xyz

================================================================================
来源：http://nsc.shanyushiyangtech.top

[A01] Hello World
来源：http://ken.wangshuangyany.cn

Py:   print("Hello, World!")
来源：http://udc.iojbl.cn

PHP:  echo "Hello, World!";
来源：http://scc.ehwqpu.com

JS:   console.log("Hello, World!");
来源：http://qpx.quarkkingdee.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zep.yj20258888.top

Java: System.out.println("Hello, World!");
来源：http://vgv.dianchejie.cn

Go:   fmt.Println("Hello, World!")
来源：http://pdb.zhoulong.xyz

Ruby: puts "Hello, World!"
来源：http://sgv.hnqzz.top

C#:   Console.WriteLine("Hello, World!");
来源：http://mto.redwolf501.top

[A02] 变量声明与赋值
来源：http://rah.nanxuanxn.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://otm.gaohongyu789.top

PHP:  $name = "Alex"; $age = 20;
来源：http://hqp.fanxiaobao.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://vfy.redwolf501.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qgv.kuanghao11.cn

Java: String name = "Alex"; int age = 20;
来源：http://ntu.hammf.cn

Go:   name := "Alex"; age := 20
来源：http://dlt.jlsjyb.cn

Ruby: name = "Alex"; age = 20
来源：http://thm.ybcxt.top

C#:   string name = "Alex"; int age = 20;
来源：http://kve.chenjidiqi.icu

[A03] 常量定义
来源：http://ngx.bbcook.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gnv.yfazqb.com

PHP:  const PI = 3.14159;
来源：http://mkt.xuetiantiany.cn

JS:   const PI = 3.14159;
来源：http://gya.jinqigfzy.top

TS:   const PI: number = 3.14159;
来源：http://lte.andypj.xyz

Java: static final double PI = 3.14159;
来源：http://xqf.redwolf501.top

Go:   const PI = 3.14159
来源：http://xef.jyoumei.cn

Ruby: PI = 3.14159
来源：http://wvd.hysaishi.cn

C#:   const double PI = 3.14159;
来源：http://wep.9152youxi.cn

[A04] 判断变量类型
来源：http://kvv.guannengcc.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://lsd.fktsv.cn


<!-- 参考信息 -->