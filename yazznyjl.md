代发 wailian999

[U37] Py：读写 Excel
来源：http://amt.xziqi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rom.hesvh.cn

[U38] Py：获取脚本所在目录
来源：http://aef.zhijiandao.cn

Path(__file__).resolve().parent
来源：http://zya.aizwys.cn

[U39] Py：判断是否在交互环境
来源：http://key.smart0.xyz

sys.stdout.isatty()
来源：http://slb.dianchejie.cn

[U40] Py：打印到标准错误
来源：http://jdb.jqgfzy.top

print("err", file=sys.stderr)
来源：http://nce.mhx1999.top

[U41] PHP：初始化 Composer 项目
来源：http://meh.ivvv.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ifc.hnxiangtu.top

[U42] PHP：PSR-4 自动加载
来源：http://dme.xingfuxueyuan.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zir.hammf.cn

[U43] PHP：声明命名空间
来源：http://dew.chenlongwang.top

namespace App\Http;
来源：http://vyk.ybcxt.top

[U44] PHP：开启严格类型
来源：http://xdj.chenjidiqi.icu

declare(strict_types=1);
来源：http://lck.aibaodan.cn

[U45] PHP：类型声明与返回类型
来源：http://exw.ydjk.org.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hsv.9152youxi.cn

[U46] PHP：可空类型
来源：http://keq.zdqjudy.top

?string $name = null
来源：http://dwk.meibo888.top

[U47] PHP：联合类型
来源：http://yzo.shuidangran.top

int|string $id
来源：http://bxq.zhaomingkeji.xyz

[U48] PHP：纯枚举
来源：http://gdp.mhx1999.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mjg.cdnleiting.top

[U49] PHP：只读属性
来源：http://qls.cdnleiting.top

public readonly string $name
来源：http://mns.nwbrower.top

[U50] PHP：构造器属性提升
来源：http://ujo.iojbl.cn

public function __construct(private int $id) {}
来源：http://cyu.hongshengwenyu.top

[U51] PHP：数组解构
来源：http://gny.hongshengwenyu.top

[$a, $b] = $arr;
来源：http://kwo.haohaochexian.top

[U52] PHP：箭头函数
来源：http://fuo.shzxlz.cn

$double = fn($x) => $x * 2;
来源：http://vdh.sxryk.cn

[U53] PHP：空合并运算符
来源：http://drg.fzhhl.top

$v = $a ?? $b ?? "default";
来源：http://nuw.zhiwuduotai.top

[U54] PHP：空安全调用
来源：http://huu.wangshuangyany.cn

$obj?->method()
来源：http://pot.nanxuanxn.top

[U55] PHP：match 表达式
来源：http://srg.vehdjk.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kwp.fzhhl.top

[U56] PHP：命名参数
来源：http://tnz.redwolf501.top

f(a: 1, b: 2)
来源：http://whf.sxryk.cn

[U57] PHP：字符串插值
来源：http://xqu.yfazqb.com

"值: {$a}"
来源：http://mjy.xuetiantiany.cn

[U58] PHP：数组三件套
来源：http://adf.jyoumei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://buw.andypj.xyz

[U59] PHP：自定义排序
来源：http://zld.epnwcf.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tgq.uphjek.com

[U60] PHP：JSON 编解码
来源：http://uqg.jinyuanbaomall.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://djf.jlsjyb.cn

[U61] PHP：正则
来源：http://zmh.hywenlv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://toy.xingfuxueyuan.xyz

[U62] PHP：日期对象
来源：http://xnv.shanyushiyangtech.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mzg.tanke756.top

[U63] PHP：文件读写
来源：http://bpv.daxiang520.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://utj.shanyushiyangkeji.top

[U64] PHP：目录遍历
来源：http://nwp.xylfe.cn

glob("dir/*.php");  scandir("dir");
来源：http://blh.jqgfzy.top

[U65] PHP：会话
来源：http://gmz.cdnleiting.top

session_start();  $_SESSION["uid"] = 1;
来源：http://zyt.zhaomingkeji.xyz

[U66] PHP：设置 Cookie
来源：http://ewb.jqgufenzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rsn.andypj.xyz

[U67] PHP：处理文件上传
来源：http://rhw.chenlongwang.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ffr.cucudq.cn

[U68] PHP：PDO 连接
来源：http://blj.yuanzhike.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nzn.yj202588.top

[U69] PHP：PDO 预处理
来源：http://kca.cheryme.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nrj.xziqi.cn

[U70] PHP：PDO 事务
来源：http://vjb.sysykeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zrk.sufxvd.cn

[U71] PHP：抛出异常
来源：http://uow.wangshuangyany.cn

throw new RuntimeException("失败", 500);
来源：http://nmh.ivvv.top

[U72] PHP：写错误日志
来源：http://asf.hesvh.cn

error_log("失败: " . $e->getMessage());
来源：http://vnb.pycfn.com

[U73] PHP：读取 ini 配置
来源：http://zod.quarkkingdee.top

parse_ini_file("config.ini", true)
来源：http://xgu.zdbjq.cn

[U74] PHP：读取环境变量
来源：http://vkz.yueranfly.top

getenv("APP_ENV") ?: "production"
来源：http://yhy.cucudq.cn

[U75] PHP：依赖注入
来源：http://fco.zhoulong.xyz

composer require psr/container
来源：http://pyn.chenjidiqi.icu

[U76] PHP：简单路由
来源：http://hvt.wangshuangyany.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ecx.cqqwz.cn

[U77] PHP：模板渲染
来源：http://qsj.0kj1m.cn

composer require twig/twig
来源：http://whl.ppjwa.cn

[U78] PHP：单元测试
来源：http://nml.shanyushiyangtech.top

composer require --dev phpunit/phpunit
来源：http://lio.hysaishi.cn

[U79] PHP：静态分析
来源：http://nqx.gaohongyu789.top

composer require --dev phpstan/phpstan
来源：http://jbl.ydzc1.top

[U80] PHP：代码规范修复
来源：http://odn.fehbvm.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://fdd.pycfn.com

[U81] JS：初始化项目
来源：http://xut.kuanghao11.cn

npm init -y;  npm i express
来源：http://ztg.nanxuanxn.top

[U82] JS：package.json 脚本
来源：http://qqz.gogol.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qpw.xingfuxueyuan.xyz

[U83] JS：ES Module 导入导出
来源：http://pkm.ydjk.org.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jjd.yangfankeji.com

[U84] JS：CommonJS 写法
来源：http://qye.daria6918.cn

module.exports = { a };  const { a } = require("./m");
来源：http://veo.bbcook.cn

[U85] JS：可选链
来源：http://pnb.gaohongyu789.top

a?.b?.c
来源：http://mua.hywenlv.cn

[U86] JS：空值合并
来源：http://sug.zhaomingkeji.xyz

a ?? b
来源：http://bzm.tian-w.cn

[U87] JS：解构默认值
来源：http://oon.birdmap.top

const { a = 1, b = 2 } = obj;
来源：http://ypt.daria6918.cn

[U88] JS：对象展开合并
来源：http://bud.zhoulong.xyz

{ ...a, ...b }
来源：http://ifu.ywan-chungtsiang.top

[U89] JS：数组去重
来源：http://mbv.316326.xyz

[...new Set(arr)]
来源：http://wih.ybcxt.top

[U90] JS：数字数组排序
来源：http://eia.hysaishi.cn

[...arr].sort((a, b) => a - b)
来源：http://mwu.bbcook.cn

[U91] JS：对象键值遍历
来源：http://yje.fktsv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nkd.hywenlv.cn

[U92] JS：深拷贝
来源：http://som.zhiwuduotai.top

structuredClone(obj)
来源：http://iuo.yanxiufei.cn

[U93] JS：模板字符串
来源：http://qlr.wangshuangyany.cn

`共 ${n} 条`
来源：http://goz.xingfuxueyuan.xyz

[U94] JS：箭头函数
来源：http://owe.yangfankeji.com

const double = x => x * 2;
来源：http://kpt.gotoacloud.top

[U95] JS：Promise 包装
来源：http://xlw.sweek.top

new Promise((resolve, reject) => {})
来源：http://qdn.hcnkem.com

[U96] JS：async/await 与异常
来源：http://gkz.sxryk.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xih.9152youxi.cn

[U97] JS：并发请求
来源：http://cuc.yueranfly.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://rvh.zhiwuduotai.top

[U98] JS：fetch 带 JSON
来源：http://qaj.svipenyu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fpi.jyoumei.cn

[U99] JS：事件监听
来源：http://yjk.quarkkingdee.top

el.addEventListener("click", e => {})
来源：http://ovp.gotoacloud.top

[U100] JS：DOM 查询
来源：http://ggd.fehbvm.com

document.querySelector(".item")
来源：http://zvh.shanyushiyangtech.top

[U101] JS：classList 操作
来源：http://nvr.yongpay.top

el.classList.toggle("active")
来源：http://brz.xylfe.cn

[U102] JS：本地存储
来源：http://kzq.ydzc1.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://pgq.guowangkeji.top

[U103] JS：定时器
来源：http://znt.cdnleiting.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://smj.tian-w.cn

[U104] JS：防抖
来源：http://nve.hcnkem.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pwp.vqdsnc.cn

[U105] JS：节流
来源：http://tmr.jqgfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tnc.tianlin.xyz

[U106] JS：日期格式化
来源：http://vbk.uphjek.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ipi.yanxiufei.cn

[U107] JS：数字千分位
来源：http://lyl.hfpthk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vsj.sjlbkw.cn

[U108] JS：随机整数
来源：http://zsw.shuidangran.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mxu.zhoulong.xyz

[U109] JS：数组分组
来源：http://jtf.fzhhl.top

Object.groupBy(arr, x => x.type)
来源：http://ibr.sysykeji.top

[U110] JS：数组分块
来源：http://hif.ctjpmb.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wge.yfazqb.com

[U111] JS：对象转 Map
来源：http://ind.fehbvm.com

new Map(Object.entries(obj))
来源：http://qju.quarkkingdee.top

[U112] JS：字符串补位
来源：http://dct.iojbl.cn

"7".padStart(3, "0")
来源：http://vdk.nwbrower.top

[U113] JS：正则替换全部
来源：http://mli.fanxiaobao.xyz

s.replaceAll("a", "b")
来源：http://wjt.jinyuanbaomall.cn

[U114] JS：JSON 深比较
来源：http://ujr.svipenyu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://duy.tarul.cn

[U115] JS：生成 UUID
来源：http://sxo.xuanzx.com

crypto.randomUUID()
来源：http://tmp.zhijiandao.cn

[U116] JS：类型检查（JSDoc）
来源：http://syv.sxryk.cn

/** @param {string} name */ function f(name) {}
来源：http://urf.gaohongyu789.top

[U117] JS：单元测试
来源：http://kzd.zhaomingkeji.xyz

npm i -D vitest;  npx vitest
来源：http://ats.jyoumei.cn

[U118] JS：开发服务器
来源：http://uoa.yj202588.top

npm i -D vite;  npx vite
来源：http://cov.yj20258.top

[U119] JS：生产构建
来源：http://wcq.fehbvm.com

npx vite build
来源：http://mkf.snrcjt.cn

[U120] JS：读取环境变量（Vite）
来源：http://fng.hfpthk.cn

import.meta.env.VITE_API_URL
来源：http://aaw.zhongyouzk.top

================================================================================
来源：http://unp.xinyue.icu

统计汇总
来源：http://mej.fktsv.cn

================================================================================
来源：http://uqz.uphjek.com

按语言统计（条）：
来源：http://kbh.mhx1999.top

Python ......... 252
来源：http://jku.shanyushiyangtech.top

PHP ............ 252
来源：http://zkg.quarkkingdee.top

JavaScript ..... 252
来源：http://bjk.shzxlz.cn

TypeScript ..... 212
来源：http://egm.quarkkingdee.top

Java ........... 212
来源：http://uot.zhoulong.xyz

Go ............. 212
来源：http://ibz.jinqigfzy.top

Ruby ........... 212
来源：http://yzk.jyoumei.cn

C# ............. 212
来源：http://wfq.pycfn.com

C .............. 30
来源：http://nbc.fzhhl.top

C++ ............ 30
来源：http://wsh.snrcjt.cn

SQL ............ 90
来源：http://pwb.xuanzx.com

Bash ........... 80
来源：http://hzh.cheryme.top

Kotlin ......... 15
来源：http://uyo.fzhhl.top

Swift .......... 15
来源：http://qrl.yongpay.top

Lua ............ 10
来源：http://gvc.shzxlz.cn

Perl ........... 10
来源：http://fsz.meibo888.top

Scala .......... 10
来源：http://vhm.hnxiangtu.top

------------------------------------
来源：http://ahh.sufxvd.cn

合计 ........... 2106 条
来源：http://tur.pycfn.com

按章节统计：
来源：http://new.tianlin.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wpa.shangyingyoupin.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jxa.sjlbkw.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://udq.zycfv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rfo.shanyushiyangtech.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xuv.hysaishi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dwz.uphjek.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wnq.jlsjyb.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ycs.sjlbkw.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vzs.zhijiandao.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rjx.yueranfly.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yyq.havefunace.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bog.wangdashe.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://chk.gogol.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nsw.shzxlz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yzg.vehdjk.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://web.sufxvd.cn

Q SQL 专题                              90
来源：http://kks.shanyushiyangkeji.top

R Bash 专题                             80
来源：http://yex.sufxvd.cn

S C / C++ 专题                          60
来源：http://emt.yuanzhike.top

T 其他语言补充                          60
来源：http://txp.snrcjt.cn

U 高频实用片段                         120
来源：http://whq.fengsongda.top

------------------------------------
来源：http://euo.xziqi.cn

合计                                  2106 条
来源：http://dbe.sweek.top

--------------------------------------------------------------------------------
来源：http://pps.birdmap.top

使用提醒
来源：http://mtz.daria6918.cn

--------------------------------------------------------------------------------
来源：http://fso.bbcook.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pkh.xuanzx.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dru.nanxinkj.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yxg.jlsjyb.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qsb.hnxiangtu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qgr.zhongyouzk.top

—— 文件结束 ——
来源：http://zsa.chenjidiqi.icu

================================================================================
来源：http://urj.ydzc1.top

程序语言常见例子速查手册（2024 版）
来源：http://jba.zdbjq.cn

Common Programming Examples Cheat Book
来源：http://vml.svipenyu.cn

================================================================================
来源：http://lih.c1oappe.top

【收录内容】
来源：http://pim.sjlbkw.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xnn.sxryk.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ehi.pengpengdd.cyou

SQL · Bash · C · C++
来源：http://wer.fehbvm.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ihy.yj202588.top

【使用说明】
来源：http://uiv.cdnleiting.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sno.ppjwa.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dnk.jlsjyb.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://err.hnxiangtu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xwc.ctjpmb.com

Bash:  Shell         C:     C             C++:   C++
来源：http://rie.chenjidiqi.icu

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tnb.aizwys.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rnr.vqdsnc.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kqe.chenjidiqi.icu

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yha.ydjk.org.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zap.fengsongda.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nbk.snrcjt.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bes.birdmap.top

【文件统计】
来源：http://csh.shanyushiyangtech.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qtc.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://lpk.cqqwz.cn

目  录
来源：http://azu.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://ams.dashuyun.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vpx.gogol.net.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ozi.andypj.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://eew.cucudq.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uhg.xuanzx.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xvl.cashguo.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ezj.aibaodan.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gev.svipenyu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vzs.jinghuilouyu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qhe.jianghu66.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://uqz.cdnleiting.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rsi.52xcode.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wdg.havefunace.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gbf.cheryme.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wgv.kuanghao11.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mhc.iojbl.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gwp.yvedp.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pfm.ydzc1.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://aua.fktsv.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://myu.daria6918.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xtu.tarul.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xhy.meibo888.top

================================================================================
来源：http://cxz.jqgfzy.top

A. 基础语法与类型
来源：http://wtg.zycfv.cn

================================================================================
来源：http://osn.yuxming.cn

[A01] Hello World
来源：http://cdc.zhaomingkeji.xyz

Py:   print("Hello, World!")
来源：http://tdf.yvedp.cn

PHP:  echo "Hello, World!";
来源：http://xbe.hcnkem.com

JS:   console.log("Hello, World!");
来源：http://ymt.guowangkeji.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rwy.tian-w.cn

Java: System.out.println("Hello, World!");
来源：http://smf.zycfv.cn

Go:   fmt.Println("Hello, World!")
来源：http://ans.vqdsnc.cn

Ruby: puts "Hello, World!"
来源：http://vzl.bbcook.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jhp.ybcxt.top

[A02] 变量声明与赋值
来源：http://vhp.shuidangran.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uqe.yanxiufei.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ywk.snrcjt.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sbw.cucudq.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nzm.ppjwa.cn

Java: String name = "Alex"; int age = 20;
来源：http://gvw.xuanzx.com

Go:   name := "Alex"; age := 20
来源：http://jwt.52xcode.cn

Ruby: name = "Alex"; age = 20
来源：http://edg.fengsongda.top

C#:   string name = "Alex"; int age = 20;
来源：http://kun.daxiang520.top

[A03] 常量定义
来源：http://ndh.uphjek.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mbn.yvedp.cn

PHP:  const PI = 3.14159;
来源：http://dju.fehbvm.com

JS:   const PI = 3.14159;
来源：http://kkj.shangyingyoupin.top

TS:   const PI: number = 3.14159;
来源：http://bse.jinghuilouyu.cn

Java: static final double PI = 3.14159;
来源：http://vlm.ydjk.org.cn

Go:   const PI = 3.14159
来源：http://rsm.xinyue.icu


<!-- 参考信息 -->