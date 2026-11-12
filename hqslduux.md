代发 wailian999

[U35] Py：发送邮件
来源：http://ebw.yuxming.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oji.birdmap.top

[U36] Py：定时任务
来源：http://xzr.zdbjq.cn

schedule.every(10).minutes.do(job)
来源：http://gao.ppjwa.cn

[U37] Py：读写 Excel
来源：http://iuw.cdnleiting.top

pandas.read_excel / DataFrame.to_excel
来源：http://zno.sjlbkw.cn

[U38] Py：获取脚本所在目录
来源：http://ejh.yvedp.cn

Path(__file__).resolve().parent
来源：http://olf.jinqigufen.top

[U39] Py：判断是否在交互环境
来源：http://hok.haohaochexian.top

sys.stdout.isatty()
来源：http://sqz.yvedp.cn

[U40] Py：打印到标准错误
来源：http://ngw.hfpthk.cn

print("err", file=sys.stderr)
来源：http://eji.fengsongda.top

[U41] PHP：初始化 Composer 项目
来源：http://bio.xuanzx.com

composer init;  composer require guzzlehttp/guzzle
来源：http://gka.gogol.net.cn

[U42] PHP：PSR-4 自动加载
来源：http://ovq.fengsongda.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cpc.cdnleiting.top

[U43] PHP：声明命名空间
来源：http://wfl.shuidangran.top

namespace App\Http;
来源：http://ypc.zycfv.cn

[U44] PHP：开启严格类型
来源：http://kht.yfazqb.com

declare(strict_types=1);
来源：http://tcy.shangyingyoupin.top

[U45] PHP：类型声明与返回类型
来源：http://xtu.ehwqpu.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://pzs.jqgfzy.top

[U46] PHP：可空类型
来源：http://xir.jiagoushi.top

?string $name = null
来源：http://acc.hysaishi.cn

[U47] PHP：联合类型
来源：http://nsp.vehdjk.com

int|string $id
来源：http://ool.cqqwz.cn

[U48] PHP：纯枚举
来源：http://rvf.gogol.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jbg.zhiwuduotai.top

[U49] PHP：只读属性
来源：http://ffl.chenlongwang.top

public readonly string $name
来源：http://ern.haohaochexian.top

[U50] PHP：构造器属性提升
来源：http://kwz.gogol.net.cn

public function __construct(private int $id) {}
来源：http://obc.xinyue.icu

[U51] PHP：数组解构
来源：http://dny.hfpthk.cn

[$a, $b] = $arr;
来源：http://sql.ehwqpu.com

[U52] PHP：箭头函数
来源：http://llz.yuxming.cn

$double = fn($x) => $x * 2;
来源：http://crv.zdbjq.cn

[U53] PHP：空合并运算符
来源：http://cav.shangyingyoupin.top

$v = $a ?? $b ?? "default";
来源：http://dyw.zdqjudy.top

[U54] PHP：空安全调用
来源：http://ieh.yuanzhike.top

$obj?->method()
来源：http://clh.vqdsnc.cn

[U55] PHP：match 表达式
来源：http://evr.ywan-chungtsiang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wus.yueranfly.top

[U56] PHP：命名参数
来源：http://kfg.jqgufenzy.top

f(a: 1, b: 2)
来源：http://tsr.sufxvd.cn

[U57] PHP：字符串插值
来源：http://tzj.havefunace.top

"值: {$a}"
来源：http://jxw.zhixingplan.top

[U58] PHP：数组三件套
来源：http://nhn.yueranfly.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dnv.zhengqikj.top

[U59] PHP：自定义排序
来源：http://zvt.yuxming.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rul.cheryme.top

[U60] PHP：JSON 编解码
来源：http://nby.jinghuilouyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jjb.yvedp.cn

[U61] PHP：正则
来源：http://jyr.zhengqikj.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://omj.0kj1m.cn

[U62] PHP：日期对象
来源：http://bny.chenjidiqi.icu

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xfw.yvedp.cn

[U63] PHP：文件读写
来源：http://oud.birdmap.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uub.cdnleiting.top

[U64] PHP：目录遍历
来源：http://smw.jqgfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://gfs.snrcjt.cn

[U65] PHP：会话
来源：http://gia.hcnkem.com

session_start();  $_SESSION["uid"] = 1;
来源：http://oio.hfpthk.cn

[U66] PHP：设置 Cookie
来源：http://zwk.ybcxt.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://spd.xingfuxueyuan.xyz

[U67] PHP：处理文件上传
来源：http://emi.aizwys.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://quf.pycfn.com

[U68] PHP：PDO 连接
来源：http://xjx.andypj.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://btr.jqgfzy.top

[U69] PHP：PDO 预处理
来源：http://hsy.mhx1999.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hem.jinqigfzy.top

[U70] PHP：PDO 事务
来源：http://vno.jianghu66.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qlw.cqqwz.cn

[U71] PHP：抛出异常
来源：http://zcv.nanxinkj.top

throw new RuntimeException("失败", 500);
来源：http://pzr.cucudq.cn

[U72] PHP：写错误日志
来源：http://mmi.gzhubu.top

error_log("失败: " . $e->getMessage());
来源：http://gnj.yonumen.top

[U73] PHP：读取 ini 配置
来源：http://yum.gotoacloud.top

parse_ini_file("config.ini", true)
来源：http://yob.gzhubu.top

[U74] PHP：读取环境变量
来源：http://nyl.ybcxt.top

getenv("APP_ENV") ?: "production"
来源：http://mkr.hongshengwenyu.top

[U75] PHP：依赖注入
来源：http://joo.tarul.cn

composer require psr/container
来源：http://jzd.nwbrower.top

[U76] PHP：简单路由
来源：http://uqx.hnxiangtu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hvi.xuanzx.com

[U77] PHP：模板渲染
来源：http://sew.yonumen.top

composer require twig/twig
来源：http://rtu.bjfxy.top

[U78] PHP：单元测试
来源：http://qcp.ehwqpu.com

composer require --dev phpunit/phpunit
来源：http://ttq.quarkkingdee.top

[U79] PHP：静态分析
来源：http://stt.fzhhl.top

composer require --dev phpstan/phpstan
来源：http://gfw.yangfankeji.com

[U80] PHP：代码规范修复
来源：http://lkr.vqdsnc.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kku.hnxiangtu.top

[U81] JS：初始化项目
来源：http://mts.bjfxy.top

npm init -y;  npm i express
来源：http://cjh.pycfn.com

[U82] JS：package.json 脚本
来源：http://skh.svipenyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qcr.jinyuanbaomall.cn

[U83] JS：ES Module 导入导出
来源：http://zyk.cheryme.top

export const a = 1;  import { a } from "./m.js";
来源：http://wim.pycfn.com

[U84] JS：CommonJS 写法
来源：http://yof.cucudq.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vra.bbcook.cn

[U85] JS：可选链
来源：http://cst.iojbl.cn

a?.b?.c
来源：http://uzz.tarul.cn

[U86] JS：空值合并
来源：http://jqn.hysaishi.cn

a ?? b
来源：http://vsg.yj20258.top

[U87] JS：解构默认值
来源：http://lqn.chenlongwang.top

const { a = 1, b = 2 } = obj;
来源：http://vqq.gogol.net.cn

[U88] JS：对象展开合并
来源：http://ued.zhengqikj.top

{ ...a, ...b }
来源：http://tkg.cqqwz.cn

[U89] JS：数组去重
来源：http://mxf.yuanzhike.top

[...new Set(arr)]
来源：http://cfw.yuxming.cn

[U90] JS：数字数组排序
来源：http://yie.fengsongda.top

[...arr].sort((a, b) => a - b)
来源：http://pus.aizwys.cn

[U91] JS：对象键值遍历
来源：http://npi.9152youxi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cwy.cdnleiting.top

[U92] JS：深拷贝
来源：http://evl.jyoumei.cn

structuredClone(obj)
来源：http://wqw.hongshengwenyu.top

[U93] JS：模板字符串
来源：http://yhu.chenjidiqi.icu

`共 ${n} 条`
来源：http://gfh.dianchejie.cn

[U94] JS：箭头函数
来源：http://pls.haohaochexian.top

const double = x => x * 2;
来源：http://xof.guannengcc.top

[U95] JS：Promise 包装
来源：http://qpi.yangfankeji.com

new Promise((resolve, reject) => {})
来源：http://pgc.svipenyu.cn

[U96] JS：async/await 与异常
来源：http://svy.yj202588.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cwp.hnxiangtu.top

[U97] JS：并发请求
来源：http://whg.ctjpmb.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://ueu.iojbl.cn

[U98] JS：fetch 带 JSON
来源：http://nvy.fengsongda.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://aan.fktsv.cn

[U99] JS：事件监听
来源：http://yqt.kuanghao11.cn

el.addEventListener("click", e => {})
来源：http://fff.zhijiandao.cn

[U100] JS：DOM 查询
来源：http://nrz.xylfe.cn

document.querySelector(".item")
来源：http://wwi.zycfv.cn

[U101] JS：classList 操作
来源：http://xtd.ydzc1.top

el.classList.toggle("active")
来源：http://xrz.nanxuanxn.top

[U102] JS：本地存储
来源：http://ihw.ydzc1.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://znb.yvedp.cn

[U103] JS：定时器
来源：http://qlr.zdbjq.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mqi.nwbrower.top

[U104] JS：防抖
来源：http://mdu.ydjk.org.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sxs.cqqwz.cn

[U105] JS：节流
来源：http://uvk.epnwcf.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rbs.vqdsnc.cn

[U106] JS：日期格式化
来源：http://ixz.jinyuanbaomall.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://alj.hfpthk.cn

[U107] JS：数字千分位
来源：http://kid.pycfn.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xom.hcnkem.com

[U108] JS：随机整数
来源：http://hbs.wangdashe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ajs.chenlongwang.top

[U109] JS：数组分组
来源：http://nir.nwbrower.top

Object.groupBy(arr, x => x.type)
来源：http://tov.ppjwa.cn

[U110] JS：数组分块
来源：http://gmr.zycfv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://eoi.tian-w.cn

[U111] JS：对象转 Map
来源：http://lqr.cheryme.top

new Map(Object.entries(obj))
来源：http://mer.zhiwuduotai.top

[U112] JS：字符串补位
来源：http://pnr.bjfxy.top

"7".padStart(3, "0")
来源：http://cfe.ybcxt.top

[U113] JS：正则替换全部
来源：http://lvy.meibo888.top

s.replaceAll("a", "b")
来源：http://aax.yfazqb.com

[U114] JS：JSON 深比较
来源：http://lzi.shanyushiyangtech.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://nod.cheryme.top

[U115] JS：生成 UUID
来源：http://zgl.ctjpmb.com

crypto.randomUUID()
来源：http://bvj.redwolf501.top

[U116] JS：类型检查（JSDoc）
来源：http://lvh.xuanzx.com

/** @param {string} name */ function f(name) {}
来源：http://hdx.yj202588.top

[U117] JS：单元测试
来源：http://nup.sxryk.cn

npm i -D vitest;  npx vitest
来源：http://pns.svipenyu.cn

[U118] JS：开发服务器
来源：http://scy.ehwqpu.com

npm i -D vite;  npx vite
来源：http://uvo.yanxiufei.cn

[U119] JS：生产构建
来源：http://cok.hnxiangtu.top

npx vite build
来源：http://wud.yueranfly.top

[U120] JS：读取环境变量（Vite）
来源：http://bvs.fehbvm.com

import.meta.env.VITE_API_URL
来源：http://zse.fanxiaobao.xyz

================================================================================
来源：http://nuh.ybcxt.top

统计汇总
来源：http://twb.ybcxt.top

================================================================================
来源：http://mmc.dianchejie.cn

按语言统计（条）：
来源：http://tpf.aibaodan.cn

Python ......... 252
来源：http://wdw.jinqigfzy.top

PHP ............ 252
来源：http://ruy.hongshengwenyu.top

JavaScript ..... 252
来源：http://pfm.gogol.net.cn

TypeScript ..... 212
来源：http://iia.gaohongyu789.top

Java ........... 212
来源：http://ebk.ybcxt.top

Go ............. 212
来源：http://ieh.gogol.net.cn

Ruby ........... 212
来源：http://tqd.yonumen.top

C# ............. 212
来源：http://czt.chenjidiqi.icu

C .............. 30
来源：http://xos.zhijiandao.cn

C++ ............ 30
来源：http://cga.birdmap.top

SQL ............ 90
来源：http://iad.ydzc1.top

Bash ........... 80
来源：http://lqc.hfpthk.cn

Kotlin ......... 15
来源：http://kkf.cashguo.top

Swift .......... 15
来源：http://imj.shanyushiyangtech.top

Lua ............ 10
来源：http://bpn.haohaochexian.top

Perl ........... 10
来源：http://wmw.shangyingyoupin.top

Scala .......... 10
来源：http://ile.yanxiufei.cn

------------------------------------
来源：http://ybj.yanxiufei.cn

合计 ........... 2106 条
来源：http://bie.dashuyun.cn

按章节统计：
来源：http://emr.zdbjq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://usb.ehwqpu.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tnx.pengpengdd.cyou

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xak.jinqigufen.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yyk.jianghu66.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rrx.quarkkingdee.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tss.yj202588.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xix.yangfankeji.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rhz.tarul.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rlj.aibaodan.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://idw.bjfxy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nzu.jinqigufen.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gvv.dianchejie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sxw.gaohongyu789.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xdk.fzhhl.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jyo.yueranfly.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tjo.redwolf501.top

Q SQL 专题                              90
来源：http://yya.shangyingyoupin.top

R Bash 专题                             80
来源：http://gyh.hnqzz.top

S C / C++ 专题                          60
来源：http://dke.aibaodan.cn

T 其他语言补充                          60
来源：http://foz.svipenyu.cn

U 高频实用片段                         120
来源：http://ofo.zycfv.cn

------------------------------------
来源：http://xga.ivvv.top

合计                                  2106 条
来源：http://vgc.fzhhl.top

--------------------------------------------------------------------------------
来源：http://twp.jinghuilouyu.cn

使用提醒
来源：http://nsi.nwbrower.top

--------------------------------------------------------------------------------
来源：http://ccs.iojbl.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://naa.hesvh.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wgz.zhiwuduotai.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bdf.yvedp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dkg.xuanzx.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://aak.sysykeji.top

—— 文件结束 ——
来源：http://dtc.fanxiaobao.xyz

================================================================================
来源：http://zga.fanxiaobao.xyz

程序语言常见例子速查手册（2024 版）
来源：http://mfx.ywan-chungtsiang.top

Common Programming Examples Cheat Book
来源：http://qqb.meibo888.top

================================================================================
来源：http://mxp.andypj.xyz

【收录内容】
来源：http://osa.yfazqb.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://tjm.fehbvm.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://uhl.hammf.cn

SQL · Bash · C · C++
来源：http://rjv.jiagoushi.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ohk.gzhubu.top

【使用说明】
来源：http://zqt.hysaishi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cmq.jinghuilouyu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kje.chenjidiqi.icu

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tpu.yueranfly.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nvw.316326.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://fgq.nanxinkj.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ebw.52xcode.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mnf.fanxiaobao.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ley.wangshuangyany.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kjj.zycfv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zkn.birdmap.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://peb.jyoumei.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gea.ybcxt.top

【文件统计】
来源：http://rlx.wangdashe.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tsn.gaohongyu789.top

--------------------------------------------------------------------------------
来源：http://gtf.guowangkeji.top

目  录
来源：http://try.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://tpd.bjfxy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lzi.mhx1999.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zbi.zhiwuduotai.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ykj.hesvh.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://iek.9152youxi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://aqw.pengpengdd.cyou

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://slr.hnqzz.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wti.zhengqikj.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nbo.shanyushiyangtech.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://len.daxiang520.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lwc.shanyushiyangkeji.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wmt.jinghuilouyu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xpx.0kj1m.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kjv.bjfxy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://izb.nanxinkj.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yvx.nanxinkj.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ihq.quarkkingdee.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mrp.zycfv.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vgq.yuxming.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://joj.ywan-chungtsiang.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rai.jqgfzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ziz.hywenlv.cn

================================================================================
来源：http://lmt.yuxming.cn

A. 基础语法与类型
来源：http://vhp.nwbrower.top

================================================================================
来源：http://qpt.ywan-chungtsiang.top

[A01] Hello World
来源：http://vrl.meibo888.top

Py:   print("Hello, World!")
来源：http://zou.xingfuxueyuan.xyz

PHP:  echo "Hello, World!";
来源：http://vyo.uphjek.com

JS:   console.log("Hello, World!");
来源：http://fuq.zhongyouzk.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xrv.9152youxi.cn

Java: System.out.println("Hello, World!");
来源：http://lfq.nanxinkj.top

Go:   fmt.Println("Hello, World!")
来源：http://cfq.sjlbkw.cn

Ruby: puts "Hello, World!"
来源：http://ozw.jianghu66.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ekc.316326.xyz

[A02] 变量声明与赋值
来源：http://huf.sufxvd.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dds.shuidangran.top

PHP:  $name = "Alex"; $age = 20;
来源：http://puu.guannengcc.top

JS:   let name = "Alex"; const age = 20;
来源：http://cqu.dashuyun.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ypr.nanxinkj.top

Java: String name = "Alex"; int age = 20;
来源：http://lff.kuanghao11.cn

Go:   name := "Alex"; age := 20
来源：http://exj.ydzc1.top

Ruby: name = "Alex"; age = 20
来源：http://yqa.aizwys.cn

C#:   string name = "Alex"; int age = 20;
来源：http://qcb.jiagoushi.top

[A03] 常量定义
来源：http://yaz.dashuyun.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://urn.xuanzx.com

PHP:  const PI = 3.14159;
来源：http://vve.guowangkeji.top


<!-- 参考信息 -->