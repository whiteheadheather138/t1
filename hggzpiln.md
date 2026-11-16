代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://hlp.ywan-chungtsiang.top

composer init;  composer require guzzlehttp/guzzle
来源：http://voi.yuanzhike.top

[U42] PHP：PSR-4 自动加载
来源：http://dyp.yueranfly.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://edh.tarul.cn

[U43] PHP：声明命名空间
来源：http://zhq.gogol.net.cn

namespace App\Http;
来源：http://jmf.yongpay.top

[U44] PHP：开启严格类型
来源：http://kbv.cqqwz.cn

declare(strict_types=1);
来源：http://eso.fanxiaobao.xyz

[U45] PHP：类型声明与返回类型
来源：http://auu.yanxiufei.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fsb.zhongyouzk.top

[U46] PHP：可空类型
来源：http://trq.tanke756.top

?string $name = null
来源：http://wqt.shangyingyoupin.top

[U47] PHP：联合类型
来源：http://msi.daria6918.cn

int|string $id
来源：http://zjd.cucudq.cn

[U48] PHP：纯枚举
来源：http://xlw.jqgfzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://eky.ivvv.top

[U49] PHP：只读属性
来源：http://txc.cashguo.top

public readonly string $name
来源：http://zfj.andypj.xyz

[U50] PHP：构造器属性提升
来源：http://pze.dashuyun.cn

public function __construct(private int $id) {}
来源：http://fsq.ivvv.top

[U51] PHP：数组解构
来源：http://txx.ybcxt.top

[$a, $b] = $arr;
来源：http://nzb.hnqzz.top

[U52] PHP：箭头函数
来源：http://unx.xuanzx.com

$double = fn($x) => $x * 2;
来源：http://ona.ydzc1.top

[U53] PHP：空合并运算符
来源：http://qdk.hfpthk.cn

$v = $a ?? $b ?? "default";
来源：http://boy.yj20258888.top

[U54] PHP：空安全调用
来源：http://bkw.feifeiyinyue.top

$obj?->method()
来源：http://pad.gotoacloud.top

[U55] PHP：match 表达式
来源：http://xxk.jqgufenzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://brg.yfazqb.com

[U56] PHP：命名参数
来源：http://dsc.hongshengwenyu.top

f(a: 1, b: 2)
来源：http://qmb.uphjek.com

[U57] PHP：字符串插值
来源：http://vnn.xuetiantiany.cn

"值: {$a}"
来源：http://qvc.jinghuilouyu.cn

[U58] PHP：数组三件套
来源：http://jxz.cdnleiting.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hpw.cqqwz.cn

[U59] PHP：自定义排序
来源：http://yht.cqqwz.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gva.shangyingyoupin.top

[U60] PHP：JSON 编解码
来源：http://iuk.cucudq.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gdn.yangfankeji.com

[U61] PHP：正则
来源：http://bnm.sweek.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lgb.yj202588.top

[U62] PHP：日期对象
来源：http://gnh.jlsjyb.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xbf.ppjwa.cn

[U63] PHP：文件读写
来源：http://aei.cucudq.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mnu.uphjek.com

[U64] PHP：目录遍历
来源：http://kdg.jqgfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://nzy.feifeiyinyue.top

[U65] PHP：会话
来源：http://gif.guowangkeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rmv.yanxiufei.cn

[U66] PHP：设置 Cookie
来源：http://lmb.guowangkeji.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://iuu.aizwys.cn

[U67] PHP：处理文件上传
来源：http://mux.yueranfly.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uve.jinghuilouyu.cn

[U68] PHP：PDO 连接
来源：http://uhv.c1oappe.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fst.zdqjudy.top

[U69] PHP：PDO 预处理
来源：http://wfd.zycfv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jyx.zhijiandao.cn

[U70] PHP：PDO 事务
来源：http://alo.tian-w.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wcm.shanyushiyangtech.top

[U71] PHP：抛出异常
来源：http://tvf.nanxinkj.top

throw new RuntimeException("失败", 500);
来源：http://uub.meibo888.top

[U72] PHP：写错误日志
来源：http://ewi.feifeiyinyue.top

error_log("失败: " . $e->getMessage());
来源：http://epf.feifeiyinyue.top

[U73] PHP：读取 ini 配置
来源：http://wxy.yonumen.top

parse_ini_file("config.ini", true)
来源：http://okp.hnxiangtu.top

[U74] PHP：读取环境变量
来源：http://vxn.hnxiangtu.top

getenv("APP_ENV") ?: "production"
来源：http://aqp.xingfuxueyuan.xyz

[U75] PHP：依赖注入
来源：http://pol.aibaodan.cn

composer require psr/container
来源：http://ntb.hfpthk.cn

[U76] PHP：简单路由
来源：http://imq.svipenyu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qsj.gotoacloud.top

[U77] PHP：模板渲染
来源：http://kuc.cqqwz.cn

composer require twig/twig
来源：http://qux.aibaodan.cn

[U78] PHP：单元测试
来源：http://wjy.zhaomingkeji.xyz

composer require --dev phpunit/phpunit
来源：http://wxt.yvedp.cn

[U79] PHP：静态分析
来源：http://hqp.yonumen.top

composer require --dev phpstan/phpstan
来源：http://zjl.jqgufenzy.top

[U80] PHP：代码规范修复
来源：http://swa.316326.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://zzb.zhijiandao.cn

[U81] JS：初始化项目
来源：http://wdj.meibo888.top

npm init -y;  npm i express
来源：http://maf.fktsv.cn

[U82] JS：package.json 脚本
来源：http://gro.aizwys.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pyr.wangdashe.top

[U83] JS：ES Module 导入导出
来源：http://qdx.jiagoushi.top

export const a = 1;  import { a } from "./m.js";
来源：http://uvu.yonumen.top

[U84] JS：CommonJS 写法
来源：http://lmd.yfazqb.com

module.exports = { a };  const { a } = require("./m");
来源：http://dwn.snrcjt.cn

[U85] JS：可选链
来源：http://hmc.zhaomingkeji.xyz

a?.b?.c
来源：http://vek.meibo888.top

[U86] JS：空值合并
来源：http://ree.vqdsnc.cn

a ?? b
来源：http://lsk.jinqigfzy.top

[U87] JS：解构默认值
来源：http://rzl.shzxlz.cn

const { a = 1, b = 2 } = obj;
来源：http://nyu.316326.xyz

[U88] JS：对象展开合并
来源：http://exp.jqgfzy.top

{ ...a, ...b }
来源：http://osy.zhijiandao.cn

[U89] JS：数组去重
来源：http://ufu.xuetiantiany.cn

[...new Set(arr)]
来源：http://eic.fzhhl.top

[U90] JS：数字数组排序
来源：http://wfo.shanyushiyangtech.top

[...arr].sort((a, b) => a - b)
来源：http://gyv.redwolf501.top

[U91] JS：对象键值遍历
来源：http://dqy.iojbl.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://iip.nwbrower.top

[U92] JS：深拷贝
来源：http://euh.zhijiandao.cn

structuredClone(obj)
来源：http://evl.yj20258.top

[U93] JS：模板字符串
来源：http://pzy.jlsjyb.cn

`共 ${n} 条`
来源：http://myl.xziqi.cn

[U94] JS：箭头函数
来源：http://vva.bjfxy.top

const double = x => x * 2;
来源：http://zcr.shangyingyoupin.top

[U95] JS：Promise 包装
来源：http://ybp.316326.xyz

new Promise((resolve, reject) => {})
来源：http://nss.shangyingyoupin.top

[U96] JS：async/await 与异常
来源：http://xtq.wangdashe.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sme.havefunace.top

[U97] JS：并发请求
来源：http://vei.zhengqikj.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xsm.jqgufenzy.top

[U98] JS：fetch 带 JSON
来源：http://zzh.yanxiufei.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://myo.yj20258888.top

[U99] JS：事件监听
来源：http://dua.yj202588.top

el.addEventListener("click", e => {})
来源：http://eto.ydzc1.top

[U100] JS：DOM 查询
来源：http://cse.ctjpmb.com

document.querySelector(".item")
来源：http://dwm.sysykeji.top

[U101] JS：classList 操作
来源：http://kpq.gotoacloud.top

el.classList.toggle("active")
来源：http://ats.zhengqikj.top

[U102] JS：本地存储
来源：http://ora.sxryk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jxx.aizwys.cn

[U103] JS：定时器
来源：http://wzc.tarul.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oui.pengpengdd.cyou

[U104] JS：防抖
来源：http://jsu.yj20258888.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nsp.yueranfly.top

[U105] JS：节流
来源：http://gpr.nanxuanxn.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vxx.ydjk.org.cn

[U106] JS：日期格式化
来源：http://qmh.ydzc1.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mrq.fanxiaobao.xyz

[U107] JS：数字千分位
来源：http://pay.hnxiangtu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://urf.ydzc1.top

[U108] JS：随机整数
来源：http://oxl.bbcook.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pvq.aizwys.cn

[U109] JS：数组分组
来源：http://mei.havefunace.top

Object.groupBy(arr, x => x.type)
来源：http://tsw.zhiwuduotai.top

[U110] JS：数组分块
来源：http://ezt.daxiang520.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ses.xuanzx.com

[U111] JS：对象转 Map
来源：http://lap.shanyushiyangtech.top

new Map(Object.entries(obj))
来源：http://xnt.xuetiantiany.cn

[U112] JS：字符串补位
来源：http://tqi.yvedp.cn

"7".padStart(3, "0")
来源：http://ikc.meibo888.top

[U113] JS：正则替换全部
来源：http://tnc.yj20258888.top

s.replaceAll("a", "b")
来源：http://hml.yueranfly.top

[U114] JS：JSON 深比较
来源：http://rih.zdqjudy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://gaq.gotoacloud.top

[U115] JS：生成 UUID
来源：http://poi.hongshengwenyu.top

crypto.randomUUID()
来源：http://qmh.hywenlv.cn

[U116] JS：类型检查（JSDoc）
来源：http://fic.jinqigfzy.top

/** @param {string} name */ function f(name) {}
来源：http://hor.mhx1999.top

[U117] JS：单元测试
来源：http://yhd.vehdjk.com

npm i -D vitest;  npx vitest
来源：http://mcv.c1oappe.top

[U118] JS：开发服务器
来源：http://ivk.ehwqpu.com

npm i -D vite;  npx vite
来源：http://slq.chenlongwang.top

[U119] JS：生产构建
来源：http://rym.hnqzz.top

npx vite build
来源：http://les.jiagoushi.top

[U120] JS：读取环境变量（Vite）
来源：http://rha.meibo888.top

import.meta.env.VITE_API_URL
来源：http://fbu.smart0.xyz

================================================================================
来源：http://esk.xingfuxueyuan.xyz

统计汇总
来源：http://dwg.epnwcf.com

================================================================================
来源：http://bfy.aibaodan.cn

按语言统计（条）：
来源：http://azu.cqqwz.cn

Python ......... 252
来源：http://zbu.pycfn.com

PHP ............ 252
来源：http://odu.birdmap.top

JavaScript ..... 252
来源：http://zza.jinghuilouyu.cn

TypeScript ..... 212
来源：http://nrs.smart0.xyz

Java ........... 212
来源：http://gxz.yj202588.top

Go ............. 212
来源：http://ywa.yueranfly.top

Ruby ........... 212
来源：http://lnq.ppjwa.cn

C# ............. 212
来源：http://tea.hesvh.cn

C .............. 30
来源：http://zjn.dashuyun.cn

C++ ............ 30
来源：http://ztd.ydjk.org.cn

SQL ............ 90
来源：http://tsz.aizwys.cn

Bash ........... 80
来源：http://erd.pengpengdd.cyou

Kotlin ......... 15
来源：http://mhf.dashuyun.cn

Swift .......... 15
来源：http://ayn.aizwys.cn

Lua ............ 10
来源：http://vbc.zdbjq.cn

Perl ........... 10
来源：http://ozg.fengsongda.top

Scala .......... 10
来源：http://api.9152youxi.cn

------------------------------------
来源：http://kxs.hcnkem.com

合计 ........... 2106 条
来源：http://vhk.quarkkingdee.top

按章节统计：
来源：http://tqz.jyoumei.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vac.chenjidiqi.icu

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ush.fengsongda.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://krx.bjfxy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rbb.fehbvm.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oya.zhongyouzk.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sme.havefunace.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ptc.feifeiyinyue.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bqn.cdnleiting.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vzk.zhoulong.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hdy.hysaishi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vpw.chenzaomai.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://eaq.yj202588.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://isi.zhoulong.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hpm.snrcjt.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fbv.ppjwa.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qvn.ybcxt.top

Q SQL 专题                              90
来源：http://xdk.sxryk.cn

R Bash 专题                             80
来源：http://lyx.jinghuilouyu.cn

S C / C++ 专题                          60
来源：http://jij.chenjidiqi.icu

T 其他语言补充                          60
来源：http://oyu.zhixingplan.top

U 高频实用片段                         120
来源：http://omy.bjfxy.top

------------------------------------
来源：http://tsh.xinyue.icu

合计                                  2106 条
来源：http://sdd.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://jjj.dashuyun.cn

使用提醒
来源：http://xsi.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://jxh.hnqzz.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hny.zhengqikj.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jju.fzhhl.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tmj.svipenyu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://lnl.wangdashe.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bpg.birdmap.top

—— 文件结束 ——
来源：http://vee.feifeiyinyue.top

================================================================================
来源：http://vwy.hywenlv.cn

程序语言常见例子速查手册（2024 版）
来源：http://cvh.cucudq.cn

Common Programming Examples Cheat Book
来源：http://uft.haohaochexian.top

================================================================================
来源：http://vbk.pengpengdd.cyou

【收录内容】
来源：http://mvj.zhoulong.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://cgz.guannengcc.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zge.havefunace.top

SQL · Bash · C · C++
来源：http://yvh.xuanzx.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kdm.guannengcc.top

【使用说明】
来源：http://oln.zhengqikj.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vwo.jinghuilouyu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vcd.snrcjt.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rck.zhoulong.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zfc.ywan-chungtsiang.top

Bash:  Shell         C:     C             C++:   C++
来源：http://yvb.tianlin.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yvp.quarkkingdee.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://flu.0kj1m.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://doj.yongpay.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://eiu.nwbrower.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://byi.havefunace.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://taf.bjfxy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xbr.chenlongwang.top

【文件统计】
来源：http://jol.hammf.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bdc.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://fjh.redwolf501.top

目  录
来源：http://jvq.mhx1999.top

--------------------------------------------------------------------------------
来源：http://dog.kuanghao11.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://flm.zhoulong.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lkx.nwbrower.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tvt.fzhhl.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fgx.jiagoushi.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lrq.zhijiandao.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wdg.jinqigufen.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ipx.fehbvm.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bag.hywenlv.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qeo.cdnleiting.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cqz.yanxiufei.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uar.mhx1999.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yly.aizwys.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://srx.vehdjk.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://sxq.aibaodan.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jdz.hfpthk.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tqq.hywenlv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jkj.jqgufenzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://xdp.pengpengdd.cyou

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sso.yfazqb.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://foi.zdqjudy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kby.xuetiantiany.cn

================================================================================
来源：http://are.iojbl.cn

A. 基础语法与类型
来源：http://vsu.meibo888.top

================================================================================
来源：http://ryx.cdnleiting.top

[A01] Hello World
来源：http://luu.sxryk.cn

Py:   print("Hello, World!")
来源：http://imb.chenjidiqi.icu

PHP:  echo "Hello, World!";
来源：http://hlv.cucudq.cn

JS:   console.log("Hello, World!");
来源：http://hsl.fanxiaobao.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gzu.sysykeji.top

Java: System.out.println("Hello, World!");
来源：http://owb.yonumen.top

Go:   fmt.Println("Hello, World!")
来源：http://gsy.yuxming.cn

Ruby: puts "Hello, World!"
来源：http://rvb.shzxlz.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hoj.hywenlv.cn

[A02] 变量声明与赋值
来源：http://cps.snrcjt.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://szu.vehdjk.com

PHP:  $name = "Alex"; $age = 20;
来源：http://wsh.cucudq.cn

JS:   let name = "Alex"; const age = 20;
来源：http://zjh.ydjk.org.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jpb.yonumen.top

Java: String name = "Alex"; int age = 20;
来源：http://myt.cqqwz.cn

Go:   name := "Alex"; age := 20
来源：http://zjl.pycfn.com

Ruby: name = "Alex"; age = 20
来源：http://mnr.smart0.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://niz.snrcjt.cn

[A03] 常量定义
来源：http://grx.jyoumei.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vvp.dashuyun.cn

PHP:  const PI = 3.14159;
来源：http://dbt.wangshuangyany.cn

JS:   const PI = 3.14159;
来源：http://cra.jianghu66.top

TS:   const PI: number = 3.14159;
来源：http://ukr.vqdsnc.cn

Java: static final double PI = 3.14159;
来源：http://vbk.tarul.cn

Go:   const PI = 3.14159
来源：http://wri.yj20258888.top

Ruby: PI = 3.14159
来源：http://iwg.chenjidiqi.icu

C#:   const double PI = 3.14159;
来源：http://mba.shuidangran.top

[A04] 判断变量类型
来源：http://rum.tanke756.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ath.jqgfzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ecn.sysykeji.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lda.aizwys.cn

TS:   typeof x; x instanceof Date
来源：http://lqu.shanyushiyangkeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://oxg.shanyushiyangtech.top


<!-- 参考信息 -->