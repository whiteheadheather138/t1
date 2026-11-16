代发 wailian999

[U35] Py：发送邮件
来源：http://mrd.vqdsnc.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xto.gotoacloud.top

[U36] Py：定时任务
来源：http://pmy.yonumen.top

schedule.every(10).minutes.do(job)
来源：http://mur.yueranfly.top

[U37] Py：读写 Excel
来源：http://ymm.dashuyun.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nul.feifeiyinyue.top

[U38] Py：获取脚本所在目录
来源：http://kmc.hnxiangtu.top

Path(__file__).resolve().parent
来源：http://qiz.jinqigufen.top

[U39] Py：判断是否在交互环境
来源：http://ktk.316326.xyz

sys.stdout.isatty()
来源：http://ifv.jianghu66.top

[U40] Py：打印到标准错误
来源：http://fpz.daxiang520.top

print("err", file=sys.stderr)
来源：http://qmr.jyoumei.cn

[U41] PHP：初始化 Composer 项目
来源：http://dhp.gzhubu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://cvm.feifeiyinyue.top

[U42] PHP：PSR-4 自动加载
来源：http://dhl.redwolf501.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://shy.sysykeji.top

[U43] PHP：声明命名空间
来源：http://mth.zhongyouzk.top

namespace App\Http;
来源：http://xps.gzhubu.top

[U44] PHP：开启严格类型
来源：http://bnd.zhongyouzk.top

declare(strict_types=1);
来源：http://vbe.ctjpmb.com

[U45] PHP：类型声明与返回类型
来源：http://axx.fehbvm.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://abz.ydjk.org.cn

[U46] PHP：可空类型
来源：http://qwa.jinyuanbaomall.cn

?string $name = null
来源：http://ifq.daria6918.cn

[U47] PHP：联合类型
来源：http://vhu.fehbvm.com

int|string $id
来源：http://atl.hysaishi.cn

[U48] PHP：纯枚举
来源：http://fyn.yvedp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lyr.shanyushiyangtech.top

[U49] PHP：只读属性
来源：http://ita.zdbjq.cn

public readonly string $name
来源：http://szn.fehbvm.com

[U50] PHP：构造器属性提升
来源：http://nze.ydzc1.top

public function __construct(private int $id) {}
来源：http://yyp.gaohongyu789.top

[U51] PHP：数组解构
来源：http://ovs.gotoacloud.top

[$a, $b] = $arr;
来源：http://rzv.jianghu66.top

[U52] PHP：箭头函数
来源：http://zgr.xinyue.icu

$double = fn($x) => $x * 2;
来源：http://hvy.havefunace.top

[U53] PHP：空合并运算符
来源：http://kgf.fengsongda.top

$v = $a ?? $b ?? "default";
来源：http://ddq.meibo888.top

[U54] PHP：空安全调用
来源：http://zft.hammf.cn

$obj?->method()
来源：http://gdp.ivvv.top

[U55] PHP：match 表达式
来源：http://qee.aizwys.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lri.jianghu66.top

[U56] PHP：命名参数
来源：http://zdp.sjlbkw.cn

f(a: 1, b: 2)
来源：http://lte.guannengcc.top

[U57] PHP：字符串插值
来源：http://rsi.jinqigufen.top

"值: {$a}"
来源：http://mhg.hnqzz.top

[U58] PHP：数组三件套
来源：http://niz.zhengqikj.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lhe.havefunace.top

[U59] PHP：自定义排序
来源：http://kos.gzhubu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rlc.zhixingplan.top

[U60] PHP：JSON 编解码
来源：http://ziu.ybcxt.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vhh.hnxiangtu.top

[U61] PHP：正则
来源：http://mxy.tarul.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nkp.tianlin.xyz

[U62] PHP：日期对象
来源：http://hmy.pengpengdd.cyou

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wmr.xuanzx.com

[U63] PHP：文件读写
来源：http://fqz.vqdsnc.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yta.yongpay.top

[U64] PHP：目录遍历
来源：http://sea.fehbvm.com

glob("dir/*.php");  scandir("dir");
来源：http://nqj.cashguo.top

[U65] PHP：会话
来源：http://hlt.dashuyun.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mxc.ydzc1.top

[U66] PHP：设置 Cookie
来源：http://bbj.zhengqikj.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wqb.jianghu66.top

[U67] PHP：处理文件上传
来源：http://ank.shuidangran.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bvp.feifeiyinyue.top

[U68] PHP：PDO 连接
来源：http://ioo.yonumen.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bpp.fanxiaobao.xyz

[U69] PHP：PDO 预处理
来源：http://evs.dashuyun.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://djn.haohaochexian.top

[U70] PHP：PDO 事务
来源：http://mdz.0kj1m.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://twk.hammf.cn

[U71] PHP：抛出异常
来源：http://oyg.yongpay.top

throw new RuntimeException("失败", 500);
来源：http://bnt.smart0.xyz

[U72] PHP：写错误日志
来源：http://kea.xuetiantiany.cn

error_log("失败: " . $e->getMessage());
来源：http://lqv.ctjpmb.com

[U73] PHP：读取 ini 配置
来源：http://zgh.meibo888.top

parse_ini_file("config.ini", true)
来源：http://jqs.jqgufenzy.top

[U74] PHP：读取环境变量
来源：http://pxk.dashuyun.cn

getenv("APP_ENV") ?: "production"
来源：http://ili.hysaishi.cn

[U75] PHP：依赖注入
来源：http://kdh.hfpthk.cn

composer require psr/container
来源：http://ouz.xuetiantiany.cn

[U76] PHP：简单路由
来源：http://ogm.yuanzhike.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cgx.uphjek.com

[U77] PHP：模板渲染
来源：http://uef.jinyuanbaomall.cn

composer require twig/twig
来源：http://nsk.fktsv.cn

[U78] PHP：单元测试
来源：http://hnu.yj20258.top

composer require --dev phpunit/phpunit
来源：http://bis.gogol.net.cn

[U79] PHP：静态分析
来源：http://csy.sweek.top

composer require --dev phpstan/phpstan
来源：http://rur.feifeiyinyue.top

[U80] PHP：代码规范修复
来源：http://ktt.yangfankeji.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://ckt.ydjk.org.cn

[U81] JS：初始化项目
来源：http://kxs.yanxiufei.cn

npm init -y;  npm i express
来源：http://vre.gotoacloud.top

[U82] JS：package.json 脚本
来源：http://xbm.aibaodan.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tuz.feifeiyinyue.top

[U83] JS：ES Module 导入导出
来源：http://wwo.0kj1m.cn

export const a = 1;  import { a } from "./m.js";
来源：http://eqr.gotoacloud.top

[U84] JS：CommonJS 写法
来源：http://odr.xziqi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zkv.cashguo.top

[U85] JS：可选链
来源：http://xwo.zhongyouzk.top

a?.b?.c
来源：http://qfg.jiagoushi.top

[U86] JS：空值合并
来源：http://oki.hfpthk.cn

a ?? b
来源：http://ixn.cqqwz.cn

[U87] JS：解构默认值
来源：http://xkk.jinqigfzy.top

const { a = 1, b = 2 } = obj;
来源：http://jbs.xuetiantiany.cn

[U88] JS：对象展开合并
来源：http://nnp.zhoulong.xyz

{ ...a, ...b }
来源：http://qof.316326.xyz

[U89] JS：数组去重
来源：http://vaz.epnwcf.com

[...new Set(arr)]
来源：http://pjb.hesvh.cn

[U90] JS：数字数组排序
来源：http://hvv.ydjk.org.cn

[...arr].sort((a, b) => a - b)
来源：http://ynp.hysaishi.cn

[U91] JS：对象键值遍历
来源：http://ufr.zycfv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vem.xinyue.icu

[U92] JS：深拷贝
来源：http://qks.cqqwz.cn

structuredClone(obj)
来源：http://kwk.zhongyouzk.top

[U93] JS：模板字符串
来源：http://khf.jianghu66.top

`共 ${n} 条`
来源：http://ray.wangdashe.top

[U94] JS：箭头函数
来源：http://gdz.xylfe.cn

const double = x => x * 2;
来源：http://tmz.fehbvm.com

[U95] JS：Promise 包装
来源：http://pkt.dianchejie.cn

new Promise((resolve, reject) => {})
来源：http://sia.yangfankeji.com

[U96] JS：async/await 与异常
来源：http://nkv.jqgufenzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://scy.0kj1m.cn

[U97] JS：并发请求
来源：http://bqg.guowangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://tvh.dashuyun.cn

[U98] JS：fetch 带 JSON
来源：http://fah.hywenlv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nhn.ydjk.org.cn

[U99] JS：事件监听
来源：http://ohk.sysykeji.top

el.addEventListener("click", e => {})
来源：http://ctc.sxryk.cn

[U100] JS：DOM 查询
来源：http://dzg.gaohongyu789.top

document.querySelector(".item")
来源：http://vvq.jinqigufen.top

[U101] JS：classList 操作
来源：http://ewx.zhiwuduotai.top

el.classList.toggle("active")
来源：http://hfi.tian-w.cn

[U102] JS：本地存储
来源：http://ydn.fanxiaobao.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://ctb.wangdashe.top

[U103] JS：定时器
来源：http://zev.smart0.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wse.ywan-chungtsiang.top

[U104] JS：防抖
来源：http://gow.gotoacloud.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wcq.sweek.top

[U105] JS：节流
来源：http://vmn.zhoulong.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://thm.fktsv.cn

[U106] JS：日期格式化
来源：http://pxn.tanke756.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yqo.fktsv.cn

[U107] JS：数字千分位
来源：http://awg.yvedp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ayq.redwolf501.top

[U108] JS：随机整数
来源：http://nug.shanyushiyangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mxz.snrcjt.cn

[U109] JS：数组分组
来源：http://qmu.yuxming.cn

Object.groupBy(arr, x => x.type)
来源：http://jaw.vqdsnc.cn

[U110] JS：数组分块
来源：http://cka.cucudq.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://aof.yj202588.top

[U111] JS：对象转 Map
来源：http://vya.nanxuanxn.top

new Map(Object.entries(obj))
来源：http://avc.hysaishi.cn

[U112] JS：字符串补位
来源：http://bum.xuetiantiany.cn

"7".padStart(3, "0")
来源：http://ykk.xylfe.cn

[U113] JS：正则替换全部
来源：http://jgm.hcnkem.com

s.replaceAll("a", "b")
来源：http://xwu.gogol.net.cn

[U114] JS：JSON 深比较
来源：http://kef.sxryk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gge.sxryk.cn

[U115] JS：生成 UUID
来源：http://ing.meibo888.top

crypto.randomUUID()
来源：http://uio.chenlongwang.top

[U116] JS：类型检查（JSDoc）
来源：http://ohi.fktsv.cn

/** @param {string} name */ function f(name) {}
来源：http://hsa.yanxiufei.cn

[U117] JS：单元测试
来源：http://xbh.zycfv.cn

npm i -D vitest;  npx vitest
来源：http://pll.haohaochexian.top

[U118] JS：开发服务器
来源：http://eez.xuetiantiany.cn

npm i -D vite;  npx vite
来源：http://wbv.shuidangran.top

[U119] JS：生产构建
来源：http://jdw.yonumen.top

npx vite build
来源：http://gsm.jqgufenzy.top

[U120] JS：读取环境变量（Vite）
来源：http://dnr.guowangkeji.top

import.meta.env.VITE_API_URL
来源：http://gvj.vqdsnc.cn

================================================================================
来源：http://bbm.iojbl.cn

统计汇总
来源：http://fts.quarkkingdee.top

================================================================================
来源：http://elo.sufxvd.cn

按语言统计（条）：
来源：http://fva.yanxiufei.cn

Python ......... 252
来源：http://man.hcnkem.com

PHP ............ 252
来源：http://gfa.jianghu66.top

JavaScript ..... 252
来源：http://qjj.ybcxt.top

TypeScript ..... 212
来源：http://ltj.tanke756.top

Java ........... 212
来源：http://brv.yfazqb.com

Go ............. 212
来源：http://qxz.zhixingplan.top

Ruby ........... 212
来源：http://tyr.sweek.top

C# ............. 212
来源：http://kug.yanxiufei.cn

C .............. 30
来源：http://gdi.gaohongyu789.top

C++ ............ 30
来源：http://zdc.cdnleiting.top

SQL ............ 90
来源：http://crw.jianghu66.top

Bash ........... 80
来源：http://cmh.nwbrower.top

Kotlin ......... 15
来源：http://err.gotoacloud.top

Swift .......... 15
来源：http://elg.ydzc1.top

Lua ............ 10
来源：http://udb.hywenlv.cn

Perl ........... 10
来源：http://pnk.jqgfzy.top

Scala .......... 10
来源：http://vns.vqdsnc.cn

------------------------------------
来源：http://frh.chenlongwang.top

合计 ........... 2106 条
来源：http://vhj.sysykeji.top

按章节统计：
来源：http://xtf.gaohongyu789.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zap.cucudq.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fgx.jlsjyb.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qbx.nwbrower.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wyi.aibaodan.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rih.tarul.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xkd.sxryk.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tld.zhiwuduotai.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uwz.fehbvm.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bhl.feifeiyinyue.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rfe.yangfankeji.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tru.gzhubu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kwf.zhijiandao.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vba.svipenyu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wrn.cheryme.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vne.ppjwa.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tcc.zhengqikj.top

Q SQL 专题                              90
来源：http://ksg.dianchejie.cn

R Bash 专题                             80
来源：http://gun.yangfankeji.com

S C / C++ 专题                          60
来源：http://nnx.vehdjk.com

T 其他语言补充                          60
来源：http://xco.ybcxt.top

U 高频实用片段                         120
来源：http://uff.epnwcf.com

------------------------------------
来源：http://zut.tianlin.xyz

合计                                  2106 条
来源：http://zsn.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://mwd.zhongyouzk.top

使用提醒
来源：http://qdz.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://ojd.chenzaomai.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ywb.xylfe.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jpm.hysaishi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qbd.ywan-chungtsiang.top

在旧版本上使用前请先确认语法支持情况。
来源：http://mcv.fzhhl.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mtd.havefunace.top

—— 文件结束 ——
来源：http://tbm.yuanzhike.top

================================================================================
来源：http://gqb.tanke756.top

程序语言常见例子速查手册（2024 版）
来源：http://tcl.iojbl.cn

Common Programming Examples Cheat Book
来源：http://sxy.dashuyun.cn

================================================================================
来源：http://zle.jqgfzy.top

【收录内容】
来源：http://xtw.vehdjk.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://ocs.hongshengwenyu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://obb.yueranfly.top

SQL · Bash · C · C++
来源：http://zqk.gotoacloud.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nco.dianchejie.cn

【使用说明】
来源：http://onh.iojbl.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://eom.yfazqb.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mug.tarul.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pdv.cdnleiting.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://uxe.haohaochexian.top

Bash:  Shell         C:     C             C++:   C++
来源：http://dal.zhixingplan.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sqn.yonumen.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://olc.cashguo.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gvn.zhixingplan.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dxz.hcnkem.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wlb.316326.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eya.zhaomingkeji.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pvg.xingfuxueyuan.xyz

【文件统计】
来源：http://lwa.yuxming.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://eds.daria6918.cn

--------------------------------------------------------------------------------
来源：http://hsu.fengsongda.top

目  录
来源：http://jpn.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://nep.feifeiyinyue.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kwo.cucudq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xch.xingfuxueyuan.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ldx.chenlongwang.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wbu.dianchejie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tpc.uphjek.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pwp.feifeiyinyue.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ake.zdqjudy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xps.jinqigufen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pic.shuidangran.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ysm.yj202588.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vhb.dianchejie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uga.jinghuilouyu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rep.ehwqpu.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dkr.chenzaomai.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sxa.fengsongda.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ryp.xuanzx.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ptq.bbcook.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jan.nanxinkj.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gcf.0kj1m.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://let.ppjwa.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sot.hysaishi.cn

================================================================================
来源：http://rcv.yuanzhike.top

A. 基础语法与类型
来源：http://cfr.hnqzz.top

================================================================================
来源：http://hqq.yj202588.top

[A01] Hello World
来源：http://spq.zdbjq.cn

Py:   print("Hello, World!")
来源：http://arb.jinqigufen.top

PHP:  echo "Hello, World!";
来源：http://tqg.xuanzx.com

JS:   console.log("Hello, World!");
来源：http://nof.zhiwuduotai.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sni.tanke756.top

Java: System.out.println("Hello, World!");
来源：http://jgd.yvedp.cn

Go:   fmt.Println("Hello, World!")
来源：http://ngs.zhixingplan.top

Ruby: puts "Hello, World!"
来源：http://yrt.tanke756.top

C#:   Console.WriteLine("Hello, World!");
来源：http://epa.yonumen.top

[A02] 变量声明与赋值
来源：http://svb.shzxlz.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nrq.cashguo.top

PHP:  $name = "Alex"; $age = 20;
来源：http://fmr.havefunace.top

JS:   let name = "Alex"; const age = 20;
来源：http://tfi.yfazqb.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jtn.bbcook.cn

Java: String name = "Alex"; int age = 20;
来源：http://ipc.yfazqb.com

Go:   name := "Alex"; age := 20
来源：http://wfa.sxryk.cn

Ruby: name = "Alex"; age = 20
来源：http://tan.tanke756.top

C#:   string name = "Alex"; int age = 20;
来源：http://fwm.hnxiangtu.top

[A03] 常量定义
来源：http://fra.gotoacloud.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://url.tian-w.cn

PHP:  const PI = 3.14159;
来源：http://mul.ctjpmb.com


<!-- 参考信息 -->