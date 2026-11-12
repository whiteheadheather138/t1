代发 wailian999

[U35] Py：发送邮件
来源：http://bew.xuetiantiany.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nvu.xinyue.icu

[U36] Py：定时任务
来源：http://mjm.nanxinkj.top

schedule.every(10).minutes.do(job)
来源：http://rnp.chenjidiqi.icu

[U37] Py：读写 Excel
来源：http://gbd.xuetiantiany.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nws.jinqigfzy.top

[U38] Py：获取脚本所在目录
来源：http://irh.zhiwuduotai.top

Path(__file__).resolve().parent
来源：http://wsn.zhixingplan.top

[U39] Py：判断是否在交互环境
来源：http://ylr.pycfn.com

sys.stdout.isatty()
来源：http://vrz.nanxinkj.top

[U40] Py：打印到标准错误
来源：http://ami.hfpthk.cn

print("err", file=sys.stderr)
来源：http://tid.xingfuxueyuan.xyz

[U41] PHP：初始化 Composer 项目
来源：http://frc.daria6918.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qnq.jianghu66.top

[U42] PHP：PSR-4 自动加载
来源：http://zcd.chenjidiqi.icu

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://onz.hesvh.cn

[U43] PHP：声明命名空间
来源：http://oyp.52xcode.cn

namespace App\Http;
来源：http://ejs.yj20258888.top

[U44] PHP：开启严格类型
来源：http://tkg.yj20258888.top

declare(strict_types=1);
来源：http://mou.hcnkem.com

[U45] PHP：类型声明与返回类型
来源：http://uly.yj20258888.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://gur.fengsongda.top

[U46] PHP：可空类型
来源：http://kqy.zhaomingkeji.xyz

?string $name = null
来源：http://svw.ybcxt.top

[U47] PHP：联合类型
来源：http://bdo.sxryk.cn

int|string $id
来源：http://yxm.yonumen.top

[U48] PHP：纯枚举
来源：http://okx.ybcxt.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kzo.yuxming.cn

[U49] PHP：只读属性
来源：http://pbj.ydzc1.top

public readonly string $name
来源：http://vpy.shzxlz.cn

[U50] PHP：构造器属性提升
来源：http://qtu.jinghuilouyu.cn

public function __construct(private int $id) {}
来源：http://jsp.dianchejie.cn

[U51] PHP：数组解构
来源：http://oyb.nanxinkj.top

[$a, $b] = $arr;
来源：http://qku.guowangkeji.top

[U52] PHP：箭头函数
来源：http://ywt.pengpengdd.cyou

$double = fn($x) => $x * 2;
来源：http://yvp.zhiwuduotai.top

[U53] PHP：空合并运算符
来源：http://bkd.zdbjq.cn

$v = $a ?? $b ?? "default";
来源：http://ven.zhaomingkeji.xyz

[U54] PHP：空安全调用
来源：http://nmv.andypj.xyz

$obj?->method()
来源：http://vnb.gaohongyu789.top

[U55] PHP：match 表达式
来源：http://rzj.hfpthk.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vjt.fehbvm.com

[U56] PHP：命名参数
来源：http://qrh.yj20258.top

f(a: 1, b: 2)
来源：http://ksx.0kj1m.cn

[U57] PHP：字符串插值
来源：http://ish.gotoacloud.top

"值: {$a}"
来源：http://oyb.fengsongda.top

[U58] PHP：数组三件套
来源：http://jos.smart0.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ovc.0kj1m.cn

[U59] PHP：自定义排序
来源：http://bds.c1oappe.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://icv.cucudq.cn

[U60] PHP：JSON 编解码
来源：http://mmd.shzxlz.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hin.fktsv.cn

[U61] PHP：正则
来源：http://npx.daria6918.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sqr.sjlbkw.cn

[U62] PHP：日期对象
来源：http://hyb.mhx1999.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lcl.9152youxi.cn

[U63] PHP：文件读写
来源：http://qoy.jinqigfzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://auv.aibaodan.cn

[U64] PHP：目录遍历
来源：http://gwo.ydjk.org.cn

glob("dir/*.php");  scandir("dir");
来源：http://gji.shanyushiyangkeji.top

[U65] PHP：会话
来源：http://ade.shanyushiyangtech.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vln.9152youxi.cn

[U66] PHP：设置 Cookie
来源：http://zdv.yvedp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vtb.jinghuilouyu.cn

[U67] PHP：处理文件上传
来源：http://ygu.ydzc1.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ggo.sysykeji.top

[U68] PHP：PDO 连接
来源：http://zzr.0kj1m.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yqw.yanxiufei.cn

[U69] PHP：PDO 预处理
来源：http://amm.tanke756.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pwy.gogol.net.cn

[U70] PHP：PDO 事务
来源：http://dso.fzhhl.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wnb.ybcxt.top

[U71] PHP：抛出异常
来源：http://pmr.cheryme.top

throw new RuntimeException("失败", 500);
来源：http://tio.jianghu66.top

[U72] PHP：写错误日志
来源：http://crw.andypj.xyz

error_log("失败: " . $e->getMessage());
来源：http://yta.tarul.cn

[U73] PHP：读取 ini 配置
来源：http://jrg.fzhhl.top

parse_ini_file("config.ini", true)
来源：http://ycl.gotoacloud.top

[U74] PHP：读取环境变量
来源：http://ofm.tianlin.xyz

getenv("APP_ENV") ?: "production"
来源：http://lyn.ivvv.top

[U75] PHP：依赖注入
来源：http://jrn.daria6918.cn

composer require psr/container
来源：http://tiz.sxryk.cn

[U76] PHP：简单路由
来源：http://kxb.kuanghao11.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lkv.zhixingplan.top

[U77] PHP：模板渲染
来源：http://lso.cheryme.top

composer require twig/twig
来源：http://gfi.ybcxt.top

[U78] PHP：单元测试
来源：http://did.xuanzx.com

composer require --dev phpunit/phpunit
来源：http://qoj.ydzc1.top

[U79] PHP：静态分析
来源：http://fki.wangdashe.top

composer require --dev phpstan/phpstan
来源：http://iyl.zhaomingkeji.xyz

[U80] PHP：代码规范修复
来源：http://lqq.cucudq.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sgk.mhx1999.top

[U81] JS：初始化项目
来源：http://vbp.chenjidiqi.icu

npm init -y;  npm i express
来源：http://tau.quarkkingdee.top

[U82] JS：package.json 脚本
来源：http://ber.fengsongda.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fol.tarul.cn

[U83] JS：ES Module 导入导出
来源：http://euh.yj202588.top

export const a = 1;  import { a } from "./m.js";
来源：http://vvc.hnqzz.top

[U84] JS：CommonJS 写法
来源：http://skb.fzhhl.top

module.exports = { a };  const { a } = require("./m");
来源：http://lhf.jyoumei.cn

[U85] JS：可选链
来源：http://xxj.tianlin.xyz

a?.b?.c
来源：http://mmx.cdnleiting.top

[U86] JS：空值合并
来源：http://nhx.9152youxi.cn

a ?? b
来源：http://ryr.dianchejie.cn

[U87] JS：解构默认值
来源：http://tnp.zhiwuduotai.top

const { a = 1, b = 2 } = obj;
来源：http://uhs.yueranfly.top

[U88] JS：对象展开合并
来源：http://sis.hongshengwenyu.top

{ ...a, ...b }
来源：http://rgo.yfazqb.com

[U89] JS：数组去重
来源：http://dqo.hongshengwenyu.top

[...new Set(arr)]
来源：http://jkg.guannengcc.top

[U90] JS：数字数组排序
来源：http://occ.yuxming.cn

[...arr].sort((a, b) => a - b)
来源：http://mze.sufxvd.cn

[U91] JS：对象键值遍历
来源：http://fod.ybcxt.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://aer.iojbl.cn

[U92] JS：深拷贝
来源：http://thi.fehbvm.com

structuredClone(obj)
来源：http://tya.daria6918.cn

[U93] JS：模板字符串
来源：http://oqd.shanyushiyangkeji.top

`共 ${n} 条`
来源：http://jtn.jinghuilouyu.cn

[U94] JS：箭头函数
来源：http://yxm.jqgufenzy.top

const double = x => x * 2;
来源：http://smk.ivvv.top

[U95] JS：Promise 包装
来源：http://xir.hnxiangtu.top

new Promise((resolve, reject) => {})
来源：http://ewu.jinqigfzy.top

[U96] JS：async/await 与异常
来源：http://ooa.ivvv.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yoq.hysaishi.cn

[U97] JS：并发请求
来源：http://ciq.iojbl.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cyo.daxiang520.top

[U98] JS：fetch 带 JSON
来源：http://lkp.zhoulong.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://odo.wangdashe.top

[U99] JS：事件监听
来源：http://cbp.cqqwz.cn

el.addEventListener("click", e => {})
来源：http://bta.yfazqb.com

[U100] JS：DOM 查询
来源：http://jxr.hnqzz.top

document.querySelector(".item")
来源：http://mbn.cdnleiting.top

[U101] JS：classList 操作
来源：http://hik.jinghuilouyu.cn

el.classList.toggle("active")
来源：http://kcl.ydzc1.top

[U102] JS：本地存储
来源：http://tbo.ywan-chungtsiang.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://pct.hammf.cn

[U103] JS：定时器
来源：http://zgz.havefunace.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nff.chenzaomai.com

[U104] JS：防抖
来源：http://csp.yonumen.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fbc.hammf.cn

[U105] JS：节流
来源：http://snw.smart0.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hpi.xuetiantiany.cn

[U106] JS：日期格式化
来源：http://nxt.jinqigufen.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sxh.ybcxt.top

[U107] JS：数字千分位
来源：http://joc.tian-w.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://foy.cucudq.cn

[U108] JS：随机整数
来源：http://jfx.jinyuanbaomall.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hom.feifeiyinyue.top

[U109] JS：数组分组
来源：http://dnq.kuanghao11.cn

Object.groupBy(arr, x => x.type)
来源：http://hoe.yangfankeji.com

[U110] JS：数组分块
来源：http://gyr.zhoulong.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bbp.meibo888.top

[U111] JS：对象转 Map
来源：http://fwz.jqgfzy.top

new Map(Object.entries(obj))
来源：http://iwz.zhijiandao.cn

[U112] JS：字符串补位
来源：http://onj.fzhhl.top

"7".padStart(3, "0")
来源：http://wju.uphjek.com

[U113] JS：正则替换全部
来源：http://ugb.nanxuanxn.top

s.replaceAll("a", "b")
来源：http://mfh.zhoulong.xyz

[U114] JS：JSON 深比较
来源：http://xle.gotoacloud.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://mjs.ivvv.top

[U115] JS：生成 UUID
来源：http://tjr.tianlin.xyz

crypto.randomUUID()
来源：http://lmz.tanke756.top

[U116] JS：类型检查（JSDoc）
来源：http://uym.hongshengwenyu.top

/** @param {string} name */ function f(name) {}
来源：http://yrs.bjfxy.top

[U117] JS：单元测试
来源：http://szu.yj202588.top

npm i -D vitest;  npx vitest
来源：http://qhn.chenlongwang.top

[U118] JS：开发服务器
来源：http://mxx.hammf.cn

npm i -D vite;  npx vite
来源：http://rgl.yonumen.top

[U119] JS：生产构建
来源：http://ysi.uphjek.com

npx vite build
来源：http://uqc.gzhubu.top

[U120] JS：读取环境变量（Vite）
来源：http://uxj.zhengqikj.top

import.meta.env.VITE_API_URL
来源：http://scj.daria6918.cn

================================================================================
来源：http://svl.chenzaomai.com

统计汇总
来源：http://pns.hnqzz.top

================================================================================
来源：http://etp.sxryk.cn

按语言统计（条）：
来源：http://ofz.hfpthk.cn

Python ......... 252
来源：http://vpn.nanxuanxn.top

PHP ............ 252
来源：http://bnf.ehwqpu.com

JavaScript ..... 252
来源：http://nkf.ivvv.top

TypeScript ..... 212
来源：http://vyf.iojbl.cn

Java ........... 212
来源：http://qyk.epnwcf.com

Go ............. 212
来源：http://rwf.yj20258888.top

Ruby ........... 212
来源：http://ygo.zdqjudy.top

C# ............. 212
来源：http://pxs.gzhubu.top

C .............. 30
来源：http://byz.jinyuanbaomall.cn

C++ ............ 30
来源：http://pqj.smart0.xyz

SQL ............ 90
来源：http://dro.jinghuilouyu.cn

Bash ........... 80
来源：http://ggz.jlsjyb.cn

Kotlin ......... 15
来源：http://aew.ydzc1.top

Swift .......... 15
来源：http://xap.xuetiantiany.cn

Lua ............ 10
来源：http://alf.yueranfly.top

Perl ........... 10
来源：http://evl.redwolf501.top

Scala .......... 10
来源：http://sjo.hywenlv.cn

------------------------------------
来源：http://foi.jiagoushi.top

合计 ........... 2106 条
来源：http://plt.ywan-chungtsiang.top

按章节统计：
来源：http://aez.svipenyu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://acs.zhongyouzk.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yga.tarul.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cnu.hcnkem.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nlb.guannengcc.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gzf.52xcode.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://glc.yfazqb.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zcp.feifeiyinyue.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tzi.zhoulong.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xlr.havefunace.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kzn.fehbvm.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mge.feifeiyinyue.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ttm.sjlbkw.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mpl.shanyushiyangtech.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ggy.jinghuilouyu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bvb.yangfankeji.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pdz.zhixingplan.top

Q SQL 专题                              90
来源：http://pdz.zdbjq.cn

R Bash 专题                             80
来源：http://afi.hesvh.cn

S C / C++ 专题                          60
来源：http://wya.wangdashe.top

T 其他语言补充                          60
来源：http://voy.zhixingplan.top

U 高频实用片段                         120
来源：http://dgj.shzxlz.cn

------------------------------------
来源：http://rrn.quarkkingdee.top

合计                                  2106 条
来源：http://waj.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://ajv.nwbrower.top

使用提醒
来源：http://whk.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://riz.epnwcf.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uzd.andypj.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://oks.hywenlv.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mmu.gzhubu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ibi.xylfe.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pdo.sxryk.cn

—— 文件结束 ——
来源：http://udt.cdnleiting.top

================================================================================
来源：http://mnb.yanxiufei.cn

程序语言常见例子速查手册（2024 版）
来源：http://cnd.hammf.cn

Common Programming Examples Cheat Book
来源：http://rvm.chenlongwang.top

================================================================================
来源：http://exa.hcnkem.com

【收录内容】
来源：http://xhj.gaohongyu789.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ydc.316326.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wmo.hysaishi.cn

SQL · Bash · C · C++
来源：http://lha.ydjk.org.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nzg.zhiwuduotai.top

【使用说明】
来源：http://kmz.kuanghao11.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://moy.yonumen.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ldt.tian-w.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yhq.zhixingplan.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://oww.fanxiaobao.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://ixg.yangfankeji.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ayz.yueranfly.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qut.mhx1999.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ylm.cashguo.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cum.tianlin.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qwn.hnxiangtu.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://atw.fzhhl.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pju.chenlongwang.top

【文件统计】
来源：http://njh.sweek.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qeu.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://iwm.shangyingyoupin.top

目  录
来源：http://ata.uphjek.com

--------------------------------------------------------------------------------
来源：http://qjc.ydjk.org.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zkm.zhengqikj.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gvq.0kj1m.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bkb.yuxming.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hac.aizwys.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bjo.hongshengwenyu.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wlq.ydjk.org.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qim.yangfankeji.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sdm.zhaomingkeji.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mai.tianlin.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pgj.xuanzx.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mgn.shanyushiyangtech.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uxx.pycfn.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ber.zdbjq.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ors.jlsjyb.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jic.shangyingyoupin.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cyc.ehwqpu.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ija.zdbjq.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ktz.pycfn.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bsm.sufxvd.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rbp.tanke756.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://veo.cashguo.top

================================================================================
来源：http://smy.yfazqb.com

A. 基础语法与类型
来源：http://khl.zdbjq.cn

================================================================================
来源：http://rda.sjlbkw.cn

[A01] Hello World
来源：http://clc.yuanzhike.top

Py:   print("Hello, World!")
来源：http://err.guannengcc.top

PHP:  echo "Hello, World!";
来源：http://dwr.xuanzx.com

JS:   console.log("Hello, World!");
来源：http://ekv.jinqigfzy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tzc.kuanghao11.cn

Java: System.out.println("Hello, World!");
来源：http://nia.fktsv.cn

Go:   fmt.Println("Hello, World!")
来源：http://txy.yfazqb.com

Ruby: puts "Hello, World!"
来源：http://sum.andypj.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://djh.jinqigfzy.top

[A02] 变量声明与赋值
来源：http://ijk.wangdashe.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://aft.kuanghao11.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gqx.guowangkeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://ssb.nwbrower.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://eee.bbcook.cn

Java: String name = "Alex"; int age = 20;
来源：http://pml.jinyuanbaomall.cn

Go:   name := "Alex"; age := 20
来源：http://cla.hfpthk.cn

Ruby: name = "Alex"; age = 20
来源：http://fhn.shanyushiyangtech.top

C#:   string name = "Alex"; int age = 20;
来源：http://hkf.jqgfzy.top

[A03] 常量定义
来源：http://oqh.yueranfly.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zff.yfazqb.com

PHP:  const PI = 3.14159;
来源：http://toh.chenjidiqi.icu


<!-- 参考信息 -->