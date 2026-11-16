代发 wailian999

[U37] Py：读写 Excel
来源：http://tig.tarul.cn

pandas.read_excel / DataFrame.to_excel
来源：http://thf.bbcook.cn

[U38] Py：获取脚本所在目录
来源：http://nkf.yfazqb.com

Path(__file__).resolve().parent
来源：http://jrr.haohaochexian.top

[U39] Py：判断是否在交互环境
来源：http://cab.hfpthk.cn

sys.stdout.isatty()
来源：http://mwq.wangdashe.top

[U40] Py：打印到标准错误
来源：http://fge.hywenlv.cn

print("err", file=sys.stderr)
来源：http://ucn.ywan-chungtsiang.top

[U41] PHP：初始化 Composer 项目
来源：http://eis.0kj1m.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://weq.xuanzx.com

[U42] PHP：PSR-4 自动加载
来源：http://okf.guowangkeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hgh.yvedp.cn

[U43] PHP：声明命名空间
来源：http://yvt.ydjk.org.cn

namespace App\Http;
来源：http://edb.chenjidiqi.icu

[U44] PHP：开启严格类型
来源：http://zud.yuxming.cn

declare(strict_types=1);
来源：http://spm.gzhubu.top

[U45] PHP：类型声明与返回类型
来源：http://unz.hfpthk.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dsc.sysykeji.top

[U46] PHP：可空类型
来源：http://nns.aibaodan.cn

?string $name = null
来源：http://erx.yj202588.top

[U47] PHP：联合类型
来源：http://ozf.zhiwuduotai.top

int|string $id
来源：http://xoq.0kj1m.cn

[U48] PHP：纯枚举
来源：http://oug.hesvh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zku.andypj.xyz

[U49] PHP：只读属性
来源：http://rhn.zhongyouzk.top

public readonly string $name
来源：http://bkh.snrcjt.cn

[U50] PHP：构造器属性提升
来源：http://mab.havefunace.top

public function __construct(private int $id) {}
来源：http://grj.daria6918.cn

[U51] PHP：数组解构
来源：http://rka.xylfe.cn

[$a, $b] = $arr;
来源：http://syl.vehdjk.com

[U52] PHP：箭头函数
来源：http://twc.zycfv.cn

$double = fn($x) => $x * 2;
来源：http://zmp.zhiwuduotai.top

[U53] PHP：空合并运算符
来源：http://gpc.zhijiandao.cn

$v = $a ?? $b ?? "default";
来源：http://hwp.zhengqikj.top

[U54] PHP：空安全调用
来源：http://wbf.cqqwz.cn

$obj?->method()
来源：http://itb.zhijiandao.cn

[U55] PHP：match 表达式
来源：http://bnf.svipenyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://trd.yj20258.top

[U56] PHP：命名参数
来源：http://kxi.aizwys.cn

f(a: 1, b: 2)
来源：http://xed.sxryk.cn

[U57] PHP：字符串插值
来源：http://dnq.wangdashe.top

"值: {$a}"
来源：http://naq.shanyushiyangtech.top

[U58] PHP：数组三件套
来源：http://vyh.fanxiaobao.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kxn.jiagoushi.top

[U59] PHP：自定义排序
来源：http://gnm.52xcode.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wwb.cdnleiting.top

[U60] PHP：JSON 编解码
来源：http://oyx.quarkkingdee.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kzf.tianlin.xyz

[U61] PHP：正则
来源：http://xql.sjlbkw.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://icv.zhixingplan.top

[U62] PHP：日期对象
来源：http://euq.tianlin.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kqi.sweek.top

[U63] PHP：文件读写
来源：http://rcv.hywenlv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zio.sweek.top

[U64] PHP：目录遍历
来源：http://fra.shanyushiyangtech.top

glob("dir/*.php");  scandir("dir");
来源：http://bdc.xziqi.cn

[U65] PHP：会话
来源：http://hjf.shanyushiyangtech.top

session_start();  $_SESSION["uid"] = 1;
来源：http://kmd.ehwqpu.com

[U66] PHP：设置 Cookie
来源：http://hlt.316326.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sty.meibo888.top

[U67] PHP：处理文件上传
来源：http://cvm.wangshuangyany.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kgd.meibo888.top

[U68] PHP：PDO 连接
来源：http://ejx.guowangkeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://txp.ybcxt.top

[U69] PHP：PDO 预处理
来源：http://pxc.sysykeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yax.chenjidiqi.icu

[U70] PHP：PDO 事务
来源：http://grs.vqdsnc.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://csl.yfazqb.com

[U71] PHP：抛出异常
来源：http://fat.ctjpmb.com

throw new RuntimeException("失败", 500);
来源：http://qne.wangshuangyany.cn

[U72] PHP：写错误日志
来源：http://efn.feifeiyinyue.top

error_log("失败: " . $e->getMessage());
来源：http://pkj.daxiang520.top

[U73] PHP：读取 ini 配置
来源：http://ieg.hongshengwenyu.top

parse_ini_file("config.ini", true)
来源：http://ayt.mhx1999.top

[U74] PHP：读取环境变量
来源：http://fcj.nanxuanxn.top

getenv("APP_ENV") ?: "production"
来源：http://bkf.yuxming.cn

[U75] PHP：依赖注入
来源：http://uvq.zhaomingkeji.xyz

composer require psr/container
来源：http://kly.vehdjk.com

[U76] PHP：简单路由
来源：http://grq.sysykeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://adb.chenlongwang.top

[U77] PHP：模板渲染
来源：http://tnv.jqgfzy.top

composer require twig/twig
来源：http://fgs.xuanzx.com

[U78] PHP：单元测试
来源：http://fwn.zhongyouzk.top

composer require --dev phpunit/phpunit
来源：http://gjg.snrcjt.cn

[U79] PHP：静态分析
来源：http://nwj.redwolf501.top

composer require --dev phpstan/phpstan
来源：http://rcn.fehbvm.com

[U80] PHP：代码规范修复
来源：http://mui.316326.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://qxe.jinyuanbaomall.cn

[U81] JS：初始化项目
来源：http://ywz.quarkkingdee.top

npm init -y;  npm i express
来源：http://wjw.sweek.top

[U82] JS：package.json 脚本
来源：http://cqm.yonumen.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rwe.guannengcc.top

[U83] JS：ES Module 导入导出
来源：http://tly.bbcook.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dik.gaohongyu789.top

[U84] JS：CommonJS 写法
来源：http://xjb.9152youxi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ndz.ctjpmb.com

[U85] JS：可选链
来源：http://gat.daria6918.cn

a?.b?.c
来源：http://tax.jiagoushi.top

[U86] JS：空值合并
来源：http://vxb.dianchejie.cn

a ?? b
来源：http://lmg.zhongyouzk.top

[U87] JS：解构默认值
来源：http://hvg.hammf.cn

const { a = 1, b = 2 } = obj;
来源：http://tdd.wangshuangyany.cn

[U88] JS：对象展开合并
来源：http://kmc.haohaochexian.top

{ ...a, ...b }
来源：http://ndm.vehdjk.com

[U89] JS：数组去重
来源：http://dqi.cashguo.top

[...new Set(arr)]
来源：http://yqk.xingfuxueyuan.xyz

[U90] JS：数字数组排序
来源：http://osv.kuanghao11.cn

[...arr].sort((a, b) => a - b)
来源：http://ynk.cqqwz.cn

[U91] JS：对象键值遍历
来源：http://iqc.pengpengdd.cyou

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jgz.bjfxy.top

[U92] JS：深拷贝
来源：http://ege.zdqjudy.top

structuredClone(obj)
来源：http://opm.shuidangran.top

[U93] JS：模板字符串
来源：http://ekc.shzxlz.cn

`共 ${n} 条`
来源：http://yka.yj202588.top

[U94] JS：箭头函数
来源：http://fep.yj20258888.top

const double = x => x * 2;
来源：http://urt.dianchejie.cn

[U95] JS：Promise 包装
来源：http://uog.ivvv.top

new Promise((resolve, reject) => {})
来源：http://fkg.zdqjudy.top

[U96] JS：async/await 与异常
来源：http://xed.cashguo.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mqt.hysaishi.cn

[U97] JS：并发请求
来源：http://rub.zdqjudy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://qyd.chenlongwang.top

[U98] JS：fetch 带 JSON
来源：http://cdp.yvedp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xzc.zdbjq.cn

[U99] JS：事件监听
来源：http://zft.jiagoushi.top

el.addEventListener("click", e => {})
来源：http://ecy.shzxlz.cn

[U100] JS：DOM 查询
来源：http://crp.guowangkeji.top

document.querySelector(".item")
来源：http://wmb.nwbrower.top

[U101] JS：classList 操作
来源：http://ltb.hammf.cn

el.classList.toggle("active")
来源：http://tlo.c1oappe.top

[U102] JS：本地存储
来源：http://abz.yfazqb.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://fnq.sysykeji.top

[U103] JS：定时器
来源：http://kwb.zdbjq.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eyf.yanxiufei.cn

[U104] JS：防抖
来源：http://bos.316326.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pea.ppjwa.cn

[U105] JS：节流
来源：http://ywk.haohaochexian.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tli.hysaishi.cn

[U106] JS：日期格式化
来源：http://mst.jiagoushi.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xiz.hesvh.cn

[U107] JS：数字千分位
来源：http://env.fengsongda.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://shb.0kj1m.cn

[U108] JS：随机整数
来源：http://alt.zhiwuduotai.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://oud.cdnleiting.top

[U109] JS：数组分组
来源：http://wia.zdbjq.cn

Object.groupBy(arr, x => x.type)
来源：http://zee.yj20258888.top

[U110] JS：数组分块
来源：http://iuk.ehwqpu.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xti.hnqzz.top

[U111] JS：对象转 Map
来源：http://cmv.yueranfly.top

new Map(Object.entries(obj))
来源：http://epq.yfazqb.com

[U112] JS：字符串补位
来源：http://wll.yuanzhike.top

"7".padStart(3, "0")
来源：http://iyf.haohaochexian.top

[U113] JS：正则替换全部
来源：http://cwk.sysykeji.top

s.replaceAll("a", "b")
来源：http://ujg.uphjek.com

[U114] JS：JSON 深比较
来源：http://dkn.fktsv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qsb.yueranfly.top

[U115] JS：生成 UUID
来源：http://nvk.jyoumei.cn

crypto.randomUUID()
来源：http://mcz.ybcxt.top

[U116] JS：类型检查（JSDoc）
来源：http://vcl.zhaomingkeji.xyz

/** @param {string} name */ function f(name) {}
来源：http://etj.tianlin.xyz

[U117] JS：单元测试
来源：http://voh.snrcjt.cn

npm i -D vitest;  npx vitest
来源：http://ycj.sjlbkw.cn

[U118] JS：开发服务器
来源：http://boi.yangfankeji.com

npm i -D vite;  npx vite
来源：http://mbl.zhaomingkeji.xyz

[U119] JS：生产构建
来源：http://esi.jyoumei.cn

npx vite build
来源：http://wxd.ctjpmb.com

[U120] JS：读取环境变量（Vite）
来源：http://tdu.fktsv.cn

import.meta.env.VITE_API_URL
来源：http://dzb.nanxinkj.top

================================================================================
来源：http://lmn.yj20258.top

统计汇总
来源：http://ymw.ydzc1.top

================================================================================
来源：http://ygq.wangshuangyany.cn

按语言统计（条）：
来源：http://maw.guannengcc.top

Python ......... 252
来源：http://xby.hnqzz.top

PHP ............ 252
来源：http://uhx.hcnkem.com

JavaScript ..... 252
来源：http://zei.aizwys.cn

TypeScript ..... 212
来源：http://now.redwolf501.top

Java ........... 212
来源：http://tjn.hfpthk.cn

Go ............. 212
来源：http://aqt.yuanzhike.top

Ruby ........... 212
来源：http://utz.zhijiandao.cn

C# ............. 212
来源：http://gfg.0kj1m.cn

C .............. 30
来源：http://civ.sweek.top

C++ ............ 30
来源：http://kol.jinghuilouyu.cn

SQL ............ 90
来源：http://dzl.chenzaomai.com

Bash ........... 80
来源：http://uxh.gogol.net.cn

Kotlin ......... 15
来源：http://pis.fanxiaobao.xyz

Swift .......... 15
来源：http://xwy.feifeiyinyue.top

Lua ............ 10
来源：http://srt.chenjidiqi.icu

Perl ........... 10
来源：http://lqt.xziqi.cn

Scala .......... 10
来源：http://pil.hnxiangtu.top

------------------------------------
来源：http://tku.0kj1m.cn

合计 ........... 2106 条
来源：http://pyq.guowangkeji.top

按章节统计：
来源：http://fgw.yvedp.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mhz.hywenlv.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bfj.jinqigufen.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cnd.fanxiaobao.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wyy.yj202588.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ssc.dashuyun.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vdu.fanxiaobao.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ywp.yj20258.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cnc.ydzc1.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wzz.cheryme.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fhk.yongpay.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cyh.nwbrower.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qoc.iojbl.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lqt.pengpengdd.cyou

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kuv.xuanzx.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://otg.zdbjq.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mnl.dashuyun.cn

Q SQL 专题                              90
来源：http://cmh.sysykeji.top

R Bash 专题                             80
来源：http://lto.dashuyun.cn

S C / C++ 专题                          60
来源：http://icz.tarul.cn

T 其他语言补充                          60
来源：http://qae.zhijiandao.cn

U 高频实用片段                         120
来源：http://upp.sweek.top

------------------------------------
来源：http://onq.yfazqb.com

合计                                  2106 条
来源：http://tnd.iojbl.cn

--------------------------------------------------------------------------------
来源：http://iii.chenlongwang.top

使用提醒
来源：http://kno.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://prg.xuanzx.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://znr.tian-w.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xno.bjfxy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nfn.bjfxy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://xae.jianghu66.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ymb.fehbvm.com

—— 文件结束 ——
来源：http://qyi.zdqjudy.top

================================================================================
来源：http://dgg.yangfankeji.com

程序语言常见例子速查手册（2024 版）
来源：http://oae.jianghu66.top

Common Programming Examples Cheat Book
来源：http://xfh.jqgfzy.top

================================================================================
来源：http://zfe.chenlongwang.top

【收录内容】
来源：http://wid.nanxinkj.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://dcl.xylfe.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://toa.shanyushiyangkeji.top

SQL · Bash · C · C++
来源：http://ttw.sysykeji.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://btm.jlsjyb.cn

【使用说明】
来源：http://ndn.yj20258.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rur.daria6918.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://oos.guowangkeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ijn.fehbvm.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://uii.316326.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://pbk.yfazqb.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://szn.0kj1m.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ija.ppjwa.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sjc.yj202588.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://oxg.shuidangran.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://osv.andypj.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wmp.dianchejie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vbj.xylfe.cn

【文件统计】
来源：http://vbd.ppjwa.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ode.yj20258888.top

--------------------------------------------------------------------------------
来源：http://zhc.zhaomingkeji.xyz

目  录
来源：http://wya.daxiang520.top

--------------------------------------------------------------------------------
来源：http://ymy.fengsongda.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mcg.sufxvd.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gqd.ydjk.org.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cgn.jiagoushi.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vch.smart0.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bcg.fehbvm.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://egi.meibo888.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cup.sysykeji.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tmt.feifeiyinyue.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tln.kuanghao11.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fgm.havefunace.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ive.daxiang520.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://twb.hnxiangtu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lqn.jinqigfzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://amm.snrcjt.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cva.fzhhl.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pyy.c1oappe.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kng.svipenyu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bma.ppjwa.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jak.daria6918.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://esu.xziqi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vsc.gogol.net.cn

================================================================================
来源：http://ndf.zhijiandao.cn

A. 基础语法与类型
来源：http://vaj.yueranfly.top

================================================================================
来源：http://vec.tarul.cn

[A01] Hello World
来源：http://aig.hnxiangtu.top

Py:   print("Hello, World!")
来源：http://xjt.c1oappe.top

PHP:  echo "Hello, World!";
来源：http://dts.daxiang520.top

JS:   console.log("Hello, World!");
来源：http://uyp.zhaomingkeji.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://olh.hammf.cn

Java: System.out.println("Hello, World!");
来源：http://feu.tian-w.cn

Go:   fmt.Println("Hello, World!")
来源：http://fvk.hongshengwenyu.top

Ruby: puts "Hello, World!"
来源：http://uke.shangyingyoupin.top

C#:   Console.WriteLine("Hello, World!");
来源：http://vwa.jqgfzy.top

[A02] 变量声明与赋值
来源：http://ypq.guowangkeji.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://juy.hongshengwenyu.top

PHP:  $name = "Alex"; $age = 20;
来源：http://dgs.ctjpmb.com

JS:   let name = "Alex"; const age = 20;
来源：http://ayt.sxryk.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qca.jinghuilouyu.cn

Java: String name = "Alex"; int age = 20;
来源：http://jtn.gogol.net.cn

Go:   name := "Alex"; age := 20
来源：http://qws.yfazqb.com

Ruby: name = "Alex"; age = 20
来源：http://vfg.yongpay.top

C#:   string name = "Alex"; int age = 20;
来源：http://ili.tian-w.cn

[A03] 常量定义
来源：http://vkw.dianchejie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://okg.xingfuxueyuan.xyz

PHP:  const PI = 3.14159;
来源：http://rmy.yanxiufei.cn

JS:   const PI = 3.14159;
来源：http://ubb.nanxuanxn.top

TS:   const PI: number = 3.14159;
来源：http://hnc.zhoulong.xyz

Java: static final double PI = 3.14159;
来源：http://som.gotoacloud.top

Go:   const PI = 3.14159
来源：http://kxf.shuidangran.top


<!-- 参考信息 -->