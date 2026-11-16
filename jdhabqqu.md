代发 wailian999

[U43] PHP：声明命名空间
来源：http://pfb.ivvv.top

namespace App\Http;
来源：http://prx.xinyue.icu

[U44] PHP：开启严格类型
来源：http://ryg.guowangkeji.top

declare(strict_types=1);
来源：http://lbj.hongshengwenyu.top

[U45] PHP：类型声明与返回类型
来源：http://zjo.daria6918.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fgm.shanyushiyangkeji.top

[U46] PHP：可空类型
来源：http://udr.ydjk.org.cn

?string $name = null
来源：http://zoz.yfazqb.com

[U47] PHP：联合类型
来源：http://bhn.dashuyun.cn

int|string $id
来源：http://iej.tianlin.xyz

[U48] PHP：纯枚举
来源：http://cta.hammf.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tvo.jinghuilouyu.cn

[U49] PHP：只读属性
来源：http://tib.xingfuxueyuan.xyz

public readonly string $name
来源：http://tbx.svipenyu.cn

[U50] PHP：构造器属性提升
来源：http://ooh.jqgfzy.top

public function __construct(private int $id) {}
来源：http://mgv.hfpthk.cn

[U51] PHP：数组解构
来源：http://ivv.jinyuanbaomall.cn

[$a, $b] = $arr;
来源：http://ksv.feifeiyinyue.top

[U52] PHP：箭头函数
来源：http://sgm.xziqi.cn

$double = fn($x) => $x * 2;
来源：http://shp.yj20258.top

[U53] PHP：空合并运算符
来源：http://mye.shuidangran.top

$v = $a ?? $b ?? "default";
来源：http://qrq.feifeiyinyue.top

[U54] PHP：空安全调用
来源：http://gwo.cucudq.cn

$obj?->method()
来源：http://nje.0kj1m.cn

[U55] PHP：match 表达式
来源：http://erj.9152youxi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bgd.yongpay.top

[U56] PHP：命名参数
来源：http://mxf.shanyushiyangkeji.top

f(a: 1, b: 2)
来源：http://pck.svipenyu.cn

[U57] PHP：字符串插值
来源：http://swq.tian-w.cn

"值: {$a}"
来源：http://wvd.fzhhl.top

[U58] PHP：数组三件套
来源：http://oed.xylfe.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://btu.zhixingplan.top

[U59] PHP：自定义排序
来源：http://com.chenzaomai.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wai.dashuyun.cn

[U60] PHP：JSON 编解码
来源：http://cen.chenlongwang.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vdw.yongpay.top

[U61] PHP：正则
来源：http://zst.tianlin.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lah.andypj.xyz

[U62] PHP：日期对象
来源：http://xvc.zdbjq.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pgc.fanxiaobao.xyz

[U63] PHP：文件读写
来源：http://udu.yuxming.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lnc.zdqjudy.top

[U64] PHP：目录遍历
来源：http://fpm.yj20258888.top

glob("dir/*.php");  scandir("dir");
来源：http://srr.zycfv.cn

[U65] PHP：会话
来源：http://hjv.guannengcc.top

session_start();  $_SESSION["uid"] = 1;
来源：http://goh.jinqigufen.top

[U66] PHP：设置 Cookie
来源：http://saj.hysaishi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hpb.daria6918.cn

[U67] PHP：处理文件上传
来源：http://mrc.sxryk.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://krl.jinghuilouyu.cn

[U68] PHP：PDO 连接
来源：http://hkz.hysaishi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://scd.jianghu66.top

[U69] PHP：PDO 预处理
来源：http://icz.nanxuanxn.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yfz.tian-w.cn

[U70] PHP：PDO 事务
来源：http://lwg.daxiang520.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jan.zhijiandao.cn

[U71] PHP：抛出异常
来源：http://huf.yonumen.top

throw new RuntimeException("失败", 500);
来源：http://rxh.fzhhl.top

[U72] PHP：写错误日志
来源：http://ihc.sxryk.cn

error_log("失败: " . $e->getMessage());
来源：http://jww.daria6918.cn

[U73] PHP：读取 ini 配置
来源：http://xav.ybcxt.top

parse_ini_file("config.ini", true)
来源：http://rqq.hesvh.cn

[U74] PHP：读取环境变量
来源：http://dre.cheryme.top

getenv("APP_ENV") ?: "production"
来源：http://vtq.fehbvm.com

[U75] PHP：依赖注入
来源：http://gmp.gzhubu.top

composer require psr/container
来源：http://zay.cucudq.cn

[U76] PHP：简单路由
来源：http://rxk.zdbjq.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yfa.gaohongyu789.top

[U77] PHP：模板渲染
来源：http://snc.mhx1999.top

composer require twig/twig
来源：http://uot.hesvh.cn

[U78] PHP：单元测试
来源：http://cxh.ppjwa.cn

composer require --dev phpunit/phpunit
来源：http://kcn.jianghu66.top

[U79] PHP：静态分析
来源：http://agv.hongshengwenyu.top

composer require --dev phpstan/phpstan
来源：http://bxj.fzhhl.top

[U80] PHP：代码规范修复
来源：http://rml.jianghu66.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rzl.zhaomingkeji.xyz

[U81] JS：初始化项目
来源：http://xal.xinyue.icu

npm init -y;  npm i express
来源：http://jof.yj20258888.top

[U82] JS：package.json 脚本
来源：http://lqw.zdbjq.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fun.wangdashe.top

[U83] JS：ES Module 导入导出
来源：http://ewa.ivvv.top

export const a = 1;  import { a } from "./m.js";
来源：http://pyi.ydzc1.top

[U84] JS：CommonJS 写法
来源：http://lcm.gaohongyu789.top

module.exports = { a };  const { a } = require("./m");
来源：http://ylb.yanxiufei.cn

[U85] JS：可选链
来源：http://hmy.ppjwa.cn

a?.b?.c
来源：http://xvm.hysaishi.cn

[U86] JS：空值合并
来源：http://hcz.meibo888.top

a ?? b
来源：http://trw.xinyue.icu

[U87] JS：解构默认值
来源：http://ory.hongshengwenyu.top

const { a = 1, b = 2 } = obj;
来源：http://xaw.cheryme.top

[U88] JS：对象展开合并
来源：http://lgs.cucudq.cn

{ ...a, ...b }
来源：http://hlj.cashguo.top

[U89] JS：数组去重
来源：http://sir.fehbvm.com

[...new Set(arr)]
来源：http://mny.yj202588.top

[U90] JS：数字数组排序
来源：http://qqu.sufxvd.cn

[...arr].sort((a, b) => a - b)
来源：http://syv.jinqigfzy.top

[U91] JS：对象键值遍历
来源：http://gdj.tian-w.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://egx.ybcxt.top

[U92] JS：深拷贝
来源：http://ako.yj202588.top

structuredClone(obj)
来源：http://xbv.daxiang520.top

[U93] JS：模板字符串
来源：http://kjq.316326.xyz

`共 ${n} 条`
来源：http://uhq.fehbvm.com

[U94] JS：箭头函数
来源：http://ven.jinqigfzy.top

const double = x => x * 2;
来源：http://pmm.xylfe.cn

[U95] JS：Promise 包装
来源：http://jrm.xuetiantiany.cn

new Promise((resolve, reject) => {})
来源：http://gux.fehbvm.com

[U96] JS：async/await 与异常
来源：http://myq.hysaishi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qtr.chenzaomai.com

[U97] JS：并发请求
来源：http://ukc.nanxuanxn.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://txe.ehwqpu.com

[U98] JS：fetch 带 JSON
来源：http://iuk.yj202588.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rzt.jianghu66.top

[U99] JS：事件监听
来源：http://yxn.pycfn.com

el.addEventListener("click", e => {})
来源：http://oxw.gaohongyu789.top

[U100] JS：DOM 查询
来源：http://lsz.sjlbkw.cn

document.querySelector(".item")
来源：http://enh.xinyue.icu

[U101] JS：classList 操作
来源：http://otu.shangyingyoupin.top

el.classList.toggle("active")
来源：http://uyb.zhengqikj.top

[U102] JS：本地存储
来源：http://aew.nwbrower.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://lke.yonumen.top

[U103] JS：定时器
来源：http://dtk.52xcode.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wbw.aibaodan.cn

[U104] JS：防抖
来源：http://gns.9152youxi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://clp.hfpthk.cn

[U105] JS：节流
来源：http://vyb.zhaomingkeji.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mnv.bjfxy.top

[U106] JS：日期格式化
来源：http://rof.guannengcc.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mek.bjfxy.top

[U107] JS：数字千分位
来源：http://jzn.tarul.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rxz.wangshuangyany.cn

[U108] JS：随机整数
来源：http://mvp.zhoulong.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bde.vqdsnc.cn

[U109] JS：数组分组
来源：http://cri.birdmap.top

Object.groupBy(arr, x => x.type)
来源：http://mpy.dianchejie.cn

[U110] JS：数组分块
来源：http://pan.hysaishi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jco.bjfxy.top

[U111] JS：对象转 Map
来源：http://cry.shangyingyoupin.top

new Map(Object.entries(obj))
来源：http://esj.ywan-chungtsiang.top

[U112] JS：字符串补位
来源：http://aag.sjlbkw.cn

"7".padStart(3, "0")
来源：http://abz.birdmap.top

[U113] JS：正则替换全部
来源：http://jan.jqgfzy.top

s.replaceAll("a", "b")
来源：http://wxb.yangfankeji.com

[U114] JS：JSON 深比较
来源：http://ffc.daria6918.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wdo.bbcook.cn

[U115] JS：生成 UUID
来源：http://hmh.zhoulong.xyz

crypto.randomUUID()
来源：http://mee.meibo888.top

[U116] JS：类型检查（JSDoc）
来源：http://njm.jinqigfzy.top

/** @param {string} name */ function f(name) {}
来源：http://xgb.xingfuxueyuan.xyz

[U117] JS：单元测试
来源：http://pyn.gaohongyu789.top

npm i -D vitest;  npx vitest
来源：http://puo.havefunace.top

[U118] JS：开发服务器
来源：http://omq.zycfv.cn

npm i -D vite;  npx vite
来源：http://brg.pengpengdd.cyou

[U119] JS：生产构建
来源：http://pym.jinqigufen.top

npx vite build
来源：http://hlh.nwbrower.top

[U120] JS：读取环境变量（Vite）
来源：http://kav.jinqigfzy.top

import.meta.env.VITE_API_URL
来源：http://gte.yangfankeji.com

================================================================================
来源：http://wgx.havefunace.top

统计汇总
来源：http://rwh.guannengcc.top

================================================================================
来源：http://cap.sweek.top

按语言统计（条）：
来源：http://ywa.aizwys.cn

Python ......... 252
来源：http://hcm.smart0.xyz

PHP ............ 252
来源：http://bmd.havefunace.top

JavaScript ..... 252
来源：http://pgf.hongshengwenyu.top

TypeScript ..... 212
来源：http://bza.wangdashe.top

Java ........... 212
来源：http://dpw.nwbrower.top

Go ............. 212
来源：http://rzj.bbcook.cn

Ruby ........... 212
来源：http://jhw.ybcxt.top

C# ............. 212
来源：http://inb.birdmap.top

C .............. 30
来源：http://gso.snrcjt.cn

C++ ............ 30
来源：http://wnf.wangdashe.top

SQL ............ 90
来源：http://man.hywenlv.cn

Bash ........... 80
来源：http://kqv.sjlbkw.cn

Kotlin ......... 15
来源：http://utp.zhijiandao.cn

Swift .......... 15
来源：http://mtz.jinyuanbaomall.cn

Lua ............ 10
来源：http://dqx.daxiang520.top

Perl ........... 10
来源：http://flo.aizwys.cn

Scala .......... 10
来源：http://fex.ctjpmb.com

------------------------------------
来源：http://prx.sjlbkw.cn

合计 ........... 2106 条
来源：http://ryo.hongshengwenyu.top

按章节统计：
来源：http://vlg.dashuyun.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://coe.yanxiufei.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vlt.zdbjq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nbz.xuanzx.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tbq.sweek.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pnf.sysykeji.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://izo.hfpthk.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yfz.cheryme.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sov.zhixingplan.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nlh.gzhubu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ass.316326.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yhh.fengsongda.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lfp.cqqwz.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zth.shanyushiyangkeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://swy.chenzaomai.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tzx.hesvh.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dio.birdmap.top

Q SQL 专题                              90
来源：http://rqh.yj202588.top

R Bash 专题                             80
来源：http://cgk.gzhubu.top

S C / C++ 专题                          60
来源：http://nae.jinyuanbaomall.cn

T 其他语言补充                          60
来源：http://acs.shanyushiyangkeji.top

U 高频实用片段                         120
来源：http://jdr.dianchejie.cn

------------------------------------
来源：http://vuj.ydjk.org.cn

合计                                  2106 条
来源：http://dul.jianghu66.top

--------------------------------------------------------------------------------
来源：http://xxk.yanxiufei.cn

使用提醒
来源：http://kwd.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://cts.0kj1m.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dxd.fehbvm.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zim.sufxvd.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sjy.ppjwa.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bmm.svipenyu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pzt.yongpay.top

—— 文件结束 ——
来源：http://ryn.nwbrower.top

================================================================================
来源：http://zgx.xuanzx.com

程序语言常见例子速查手册（2024 版）
来源：http://kxn.zhiwuduotai.top

Common Programming Examples Cheat Book
来源：http://ifi.chenjidiqi.icu

================================================================================
来源：http://rjy.chenlongwang.top

【收录内容】
来源：http://nvi.guowangkeji.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ker.yuxming.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pbv.zhengqikj.top

SQL · Bash · C · C++
来源：http://mhx.ivvv.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pqu.chenjidiqi.icu

【使用说明】
来源：http://onz.quarkkingdee.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yae.kuanghao11.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sft.iojbl.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pcv.nanxuanxn.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zfz.hnxiangtu.top

Bash:  Shell         C:     C             C++:   C++
来源：http://urz.sjlbkw.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://foc.bbcook.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://juf.0kj1m.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nbh.nwbrower.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zgf.yuxming.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qwv.zhoulong.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://aov.chenzaomai.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gnb.ywan-chungtsiang.top

【文件统计】
来源：http://ioi.aibaodan.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://htf.havefunace.top

--------------------------------------------------------------------------------
来源：http://whl.zhoulong.xyz

目  录
来源：http://vzl.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://zyj.cucudq.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://eku.tianlin.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nke.ydzc1.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xas.hammf.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://krx.cqqwz.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nqx.shzxlz.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uhf.haohaochexian.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jwr.gogol.net.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zxo.meibo888.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jcf.fktsv.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hyx.uphjek.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ggl.gzhubu.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://azc.xziqi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zca.cqqwz.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fem.zycfv.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cer.shangyingyoupin.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kfs.gogol.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dzq.sysykeji.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://mrv.havefunace.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jud.zhiwuduotai.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xpj.jqgfzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fmn.fengsongda.top

================================================================================
来源：http://gdn.epnwcf.com

A. 基础语法与类型
来源：http://njx.jinqigufen.top

================================================================================
来源：http://uaq.fehbvm.com

[A01] Hello World
来源：http://gar.vehdjk.com

Py:   print("Hello, World!")
来源：http://cru.fktsv.cn

PHP:  echo "Hello, World!";
来源：http://dlt.dashuyun.cn

JS:   console.log("Hello, World!");
来源：http://wrk.yj20258.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://awc.meibo888.top

Java: System.out.println("Hello, World!");
来源：http://cui.yueranfly.top

Go:   fmt.Println("Hello, World!")
来源：http://xdh.jinghuilouyu.cn

Ruby: puts "Hello, World!"
来源：http://jtm.tanke756.top

C#:   Console.WriteLine("Hello, World!");
来源：http://soe.cucudq.cn

[A02] 变量声明与赋值
来源：http://ksa.nanxuanxn.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://byj.gzhubu.top

PHP:  $name = "Alex"; $age = 20;
来源：http://bhu.vqdsnc.cn

JS:   let name = "Alex"; const age = 20;
来源：http://nfh.xinyue.icu

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bcm.snrcjt.cn

Java: String name = "Alex"; int age = 20;
来源：http://xzt.aibaodan.cn

Go:   name := "Alex"; age := 20
来源：http://owi.ywan-chungtsiang.top

Ruby: name = "Alex"; age = 20
来源：http://kbk.nanxinkj.top

C#:   string name = "Alex"; int age = 20;
来源：http://nny.nanxinkj.top

[A03] 常量定义
来源：http://sdv.yj202588.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yqd.wangshuangyany.cn

PHP:  const PI = 3.14159;
来源：http://wyu.pycfn.com

JS:   const PI = 3.14159;
来源：http://rxk.ydzc1.top

TS:   const PI: number = 3.14159;
来源：http://mnz.cdnleiting.top

Java: static final double PI = 3.14159;
来源：http://wpy.kuanghao11.cn

Go:   const PI = 3.14159
来源：http://unj.hnxiangtu.top

Ruby: PI = 3.14159
来源：http://uin.ydzc1.top

C#:   const double PI = 3.14159;
来源：http://bhe.52xcode.cn

[A04] 判断变量类型
来源：http://wai.jlsjyb.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://imx.cashguo.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://frz.yanxiufei.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rfa.shzxlz.cn

TS:   typeof x; x instanceof Date
来源：http://jeq.tanke756.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tlt.hfpthk.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ruu.feifeiyinyue.top

Ruby: x.class; x.is_a?(Integer)
来源：http://idw.shzxlz.cn

C#:   x.GetType().Name; x is int
来源：http://dmw.nanxuanxn.top

[A05] 整数除法与取模
来源：http://pna.jyoumei.cn


<!-- 参考信息 -->