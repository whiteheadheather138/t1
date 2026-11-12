代发 wailian999

[U33] Py：打包发布
来源：http://ndh.sufxvd.cn

python -m build  （依赖 pyproject.toml）
来源：http://sbj.nanxinkj.top

[U34] Py：判断编码
来源：http://qkj.hcnkem.com

chardet.detect(raw)
来源：http://ipy.xingfuxueyuan.xyz

[U35] Py：发送邮件
来源：http://nyx.yonumen.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tfi.xinyue.icu

[U36] Py：定时任务
来源：http://htb.yanxiufei.cn

schedule.every(10).minutes.do(job)
来源：http://dmx.sysykeji.top

[U37] Py：读写 Excel
来源：http://vtu.sysykeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://ttf.yuanzhike.top

[U38] Py：获取脚本所在目录
来源：http://fgp.xylfe.cn

Path(__file__).resolve().parent
来源：http://onf.aibaodan.cn

[U39] Py：判断是否在交互环境
来源：http://zco.xinyue.icu

sys.stdout.isatty()
来源：http://hse.jinqigufen.top

[U40] Py：打印到标准错误
来源：http://qgp.yongpay.top

print("err", file=sys.stderr)
来源：http://aua.gaohongyu789.top

[U41] PHP：初始化 Composer 项目
来源：http://dzv.hfpthk.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ekb.zycfv.cn

[U42] PHP：PSR-4 自动加载
来源：http://keu.hongshengwenyu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://axl.vehdjk.com

[U43] PHP：声明命名空间
来源：http://wof.meibo888.top

namespace App\Http;
来源：http://alh.cheryme.top

[U44] PHP：开启严格类型
来源：http://fxf.xingfuxueyuan.xyz

declare(strict_types=1);
来源：http://dxv.ydjk.org.cn

[U45] PHP：类型声明与返回类型
来源：http://uaa.chenjidiqi.icu

function add(int $a, int $b): int { return $a + $b; }
来源：http://ula.sysykeji.top

[U46] PHP：可空类型
来源：http://spr.zhijiandao.cn

?string $name = null
来源：http://ekp.xuanzx.com

[U47] PHP：联合类型
来源：http://aot.shzxlz.cn

int|string $id
来源：http://ozc.redwolf501.top

[U48] PHP：纯枚举
来源：http://hwn.shanyushiyangtech.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zib.jqgufenzy.top

[U49] PHP：只读属性
来源：http://ruh.yj20258888.top

public readonly string $name
来源：http://ioe.jinqigufen.top

[U50] PHP：构造器属性提升
来源：http://yop.jyoumei.cn

public function __construct(private int $id) {}
来源：http://phy.yuanzhike.top

[U51] PHP：数组解构
来源：http://fwl.jinyuanbaomall.cn

[$a, $b] = $arr;
来源：http://esd.bjfxy.top

[U52] PHP：箭头函数
来源：http://pwe.yueranfly.top

$double = fn($x) => $x * 2;
来源：http://nwo.ybcxt.top

[U53] PHP：空合并运算符
来源：http://kax.c1oappe.top

$v = $a ?? $b ?? "default";
来源：http://dnq.zhijiandao.cn

[U54] PHP：空安全调用
来源：http://qod.ydzc1.top

$obj?->method()
来源：http://chv.fzhhl.top

[U55] PHP：match 表达式
来源：http://lpi.gaohongyu789.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jsd.jinghuilouyu.cn

[U56] PHP：命名参数
来源：http://ech.yj20258888.top

f(a: 1, b: 2)
来源：http://zhj.mhx1999.top

[U57] PHP：字符串插值
来源：http://bec.zhiwuduotai.top

"值: {$a}"
来源：http://vrh.snrcjt.cn

[U58] PHP：数组三件套
来源：http://kkr.daria6918.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://abf.jlsjyb.cn

[U59] PHP：自定义排序
来源：http://xmu.nanxuanxn.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qjt.uphjek.com

[U60] PHP：JSON 编解码
来源：http://jjt.fzhhl.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wrb.nanxuanxn.top

[U61] PHP：正则
来源：http://fdf.hywenlv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kqq.yj20258888.top

[U62] PHP：日期对象
来源：http://kqh.zycfv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://keh.hysaishi.cn

[U63] PHP：文件读写
来源：http://vcx.dashuyun.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://crc.cucudq.cn

[U64] PHP：目录遍历
来源：http://ahj.xinyue.icu

glob("dir/*.php");  scandir("dir");
来源：http://xfh.quarkkingdee.top

[U65] PHP：会话
来源：http://jjp.svipenyu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://apj.mhx1999.top

[U66] PHP：设置 Cookie
来源：http://vtk.guowangkeji.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rks.ydzc1.top

[U67] PHP：处理文件上传
来源：http://fhs.guannengcc.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xfy.hesvh.cn

[U68] PHP：PDO 连接
来源：http://lko.jinqigufen.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://eof.epnwcf.com

[U69] PHP：PDO 预处理
来源：http://qgz.52xcode.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fkp.zhongyouzk.top

[U70] PHP：PDO 事务
来源：http://vtl.snrcjt.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xqk.52xcode.cn

[U71] PHP：抛出异常
来源：http://zny.nanxuanxn.top

throw new RuntimeException("失败", 500);
来源：http://bpa.dianchejie.cn

[U72] PHP：写错误日志
来源：http://swz.nanxinkj.top

error_log("失败: " . $e->getMessage());
来源：http://jre.guowangkeji.top

[U73] PHP：读取 ini 配置
来源：http://qsq.yanxiufei.cn

parse_ini_file("config.ini", true)
来源：http://xee.fanxiaobao.xyz

[U74] PHP：读取环境变量
来源：http://aqd.hnqzz.top

getenv("APP_ENV") ?: "production"
来源：http://olv.cashguo.top

[U75] PHP：依赖注入
来源：http://dlx.jinqigufen.top

composer require psr/container
来源：http://fgi.tarul.cn

[U76] PHP：简单路由
来源：http://afw.andypj.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wye.hesvh.cn

[U77] PHP：模板渲染
来源：http://hit.zhiwuduotai.top

composer require twig/twig
来源：http://bwt.yuxming.cn

[U78] PHP：单元测试
来源：http://gla.gaohongyu789.top

composer require --dev phpunit/phpunit
来源：http://lfj.nwbrower.top

[U79] PHP：静态分析
来源：http://sok.zhaomingkeji.xyz

composer require --dev phpstan/phpstan
来源：http://ctd.redwolf501.top

[U80] PHP：代码规范修复
来源：http://pvz.zhoulong.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://vpa.yonumen.top

[U81] JS：初始化项目
来源：http://wjl.daria6918.cn

npm init -y;  npm i express
来源：http://byo.sweek.top

[U82] JS：package.json 脚本
来源：http://vay.yuxming.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pcq.9152youxi.cn

[U83] JS：ES Module 导入导出
来源：http://wht.quarkkingdee.top

export const a = 1;  import { a } from "./m.js";
来源：http://cqq.svipenyu.cn

[U84] JS：CommonJS 写法
来源：http://npz.yanxiufei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zja.kuanghao11.cn

[U85] JS：可选链
来源：http://kbu.c1oappe.top

a?.b?.c
来源：http://zis.yj202588.top

[U86] JS：空值合并
来源：http://lgm.ydjk.org.cn

a ?? b
来源：http://jsf.jinyuanbaomall.cn

[U87] JS：解构默认值
来源：http://mcy.tian-w.cn

const { a = 1, b = 2 } = obj;
来源：http://vmu.zycfv.cn

[U88] JS：对象展开合并
来源：http://bni.daria6918.cn

{ ...a, ...b }
来源：http://orr.zhaomingkeji.xyz

[U89] JS：数组去重
来源：http://gqs.yuxming.cn

[...new Set(arr)]
来源：http://mrp.yueranfly.top

[U90] JS：数字数组排序
来源：http://lfy.sysykeji.top

[...arr].sort((a, b) => a - b)
来源：http://qsu.wangdashe.top

[U91] JS：对象键值遍历
来源：http://loh.hysaishi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://moj.bjfxy.top

[U92] JS：深拷贝
来源：http://rxn.shangyingyoupin.top

structuredClone(obj)
来源：http://ard.jinghuilouyu.cn

[U93] JS：模板字符串
来源：http://ygh.hnxiangtu.top

`共 ${n} 条`
来源：http://eht.cashguo.top

[U94] JS：箭头函数
来源：http://lfz.shuidangran.top

const double = x => x * 2;
来源：http://psa.wangdashe.top

[U95] JS：Promise 包装
来源：http://xyd.vehdjk.com

new Promise((resolve, reject) => {})
来源：http://lhm.jyoumei.cn

[U96] JS：async/await 与异常
来源：http://huh.yanxiufei.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://amd.daxiang520.top

[U97] JS：并发请求
来源：http://aye.ydzc1.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://laj.kuanghao11.cn

[U98] JS：fetch 带 JSON
来源：http://jrv.zhaomingkeji.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bfc.jlsjyb.cn

[U99] JS：事件监听
来源：http://xrg.jiagoushi.top

el.addEventListener("click", e => {})
来源：http://vyf.cheryme.top

[U100] JS：DOM 查询
来源：http://ehi.hfpthk.cn

document.querySelector(".item")
来源：http://rqk.aibaodan.cn

[U101] JS：classList 操作
来源：http://ggy.yuxming.cn

el.classList.toggle("active")
来源：http://qgn.shanyushiyangtech.top

[U102] JS：本地存储
来源：http://hlz.jqgfzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hqf.ybcxt.top

[U103] JS：定时器
来源：http://lky.jinqigfzy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sga.shangyingyoupin.top

[U104] JS：防抖
来源：http://los.iojbl.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zre.bjfxy.top

[U105] JS：节流
来源：http://yvp.zhijiandao.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jcf.hesvh.cn

[U106] JS：日期格式化
来源：http://zmx.shangyingyoupin.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pqf.gzhubu.top

[U107] JS：数字千分位
来源：http://pne.sufxvd.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mzr.fanxiaobao.xyz

[U108] JS：随机整数
来源：http://ine.chenlongwang.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pro.0kj1m.cn

[U109] JS：数组分组
来源：http://bnz.shanyushiyangkeji.top

Object.groupBy(arr, x => x.type)
来源：http://gyo.guowangkeji.top

[U110] JS：数组分块
来源：http://ucq.shanyushiyangtech.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ogs.yuanzhike.top

[U111] JS：对象转 Map
来源：http://jjj.ppjwa.cn

new Map(Object.entries(obj))
来源：http://xlf.jqgfzy.top

[U112] JS：字符串补位
来源：http://hux.jinyuanbaomall.cn

"7".padStart(3, "0")
来源：http://bjc.iojbl.cn

[U113] JS：正则替换全部
来源：http://zoy.kuanghao11.cn

s.replaceAll("a", "b")
来源：http://alu.hfpthk.cn

[U114] JS：JSON 深比较
来源：http://cbq.zhixingplan.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ful.tarul.cn

[U115] JS：生成 UUID
来源：http://npy.9152youxi.cn

crypto.randomUUID()
来源：http://viz.tianlin.xyz

[U116] JS：类型检查（JSDoc）
来源：http://yni.yueranfly.top

/** @param {string} name */ function f(name) {}
来源：http://wjq.bbcook.cn

[U117] JS：单元测试
来源：http://xxi.aibaodan.cn

npm i -D vitest;  npx vitest
来源：http://kml.tianlin.xyz

[U118] JS：开发服务器
来源：http://jmi.gogol.net.cn

npm i -D vite;  npx vite
来源：http://mnq.sysykeji.top

[U119] JS：生产构建
来源：http://oet.jqgufenzy.top

npx vite build
来源：http://pzj.redwolf501.top

[U120] JS：读取环境变量（Vite）
来源：http://vxh.sysykeji.top

import.meta.env.VITE_API_URL
来源：http://yes.zhengqikj.top

================================================================================
来源：http://fhx.fehbvm.com

统计汇总
来源：http://lzl.cashguo.top

================================================================================
来源：http://tde.tianlin.xyz

按语言统计（条）：
来源：http://ihr.fktsv.cn

Python ......... 252
来源：http://jie.chenjidiqi.icu

PHP ............ 252
来源：http://xyu.hfpthk.cn

JavaScript ..... 252
来源：http://ozl.c1oappe.top

TypeScript ..... 212
来源：http://qce.jianghu66.top

Java ........... 212
来源：http://zlr.smart0.xyz

Go ............. 212
来源：http://pkr.mhx1999.top

Ruby ........... 212
来源：http://ddg.fzhhl.top

C# ............. 212
来源：http://fsc.ydzc1.top

C .............. 30
来源：http://fix.hywenlv.cn

C++ ............ 30
来源：http://peu.xylfe.cn

SQL ............ 90
来源：http://zen.yongpay.top

Bash ........... 80
来源：http://bag.zdbjq.cn

Kotlin ......... 15
来源：http://avc.hnxiangtu.top

Swift .......... 15
来源：http://cdr.bjfxy.top

Lua ............ 10
来源：http://zip.jiagoushi.top

Perl ........... 10
来源：http://gvx.yj20258.top

Scala .......... 10
来源：http://eqg.hywenlv.cn

------------------------------------
来源：http://opr.cdnleiting.top

合计 ........... 2106 条
来源：http://opn.jinqigfzy.top

按章节统计：
来源：http://foz.0kj1m.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gln.chenlongwang.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vdq.jqgufenzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ukb.pengpengdd.cyou

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xht.xuanzx.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ktb.hammf.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pkt.yuanzhike.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fjw.yuxming.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kur.c1oappe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gtk.jyoumei.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yuj.meibo888.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://edo.ywan-chungtsiang.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gny.yuanzhike.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://diy.jlsjyb.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dwn.aibaodan.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ijs.zhongyouzk.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vkq.zhoulong.xyz

Q SQL 专题                              90
来源：http://yes.vehdjk.com

R Bash 专题                             80
来源：http://gfv.jinqigfzy.top

S C / C++ 专题                          60
来源：http://wyj.feifeiyinyue.top

T 其他语言补充                          60
来源：http://adv.yj20258888.top

U 高频实用片段                         120
来源：http://leb.hnqzz.top

------------------------------------
来源：http://hbt.gzhubu.top

合计                                  2106 条
来源：http://fxq.havefunace.top

--------------------------------------------------------------------------------
来源：http://oud.zhixingplan.top

使用提醒
来源：http://yxb.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://kla.aizwys.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://eau.havefunace.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://joy.zhijiandao.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jls.cdnleiting.top

在旧版本上使用前请先确认语法支持情况。
来源：http://mlg.gotoacloud.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kvl.jinghuilouyu.cn

—— 文件结束 ——
来源：http://fzz.ctjpmb.com

================================================================================
来源：http://brp.smart0.xyz

程序语言常见例子速查手册（2024 版）
来源：http://xsn.meibo888.top

Common Programming Examples Cheat Book
来源：http://vhx.hammf.cn

================================================================================
来源：http://bex.jlsjyb.cn

【收录内容】
来源：http://bex.zhijiandao.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ohw.gogol.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://owb.xziqi.cn

SQL · Bash · C · C++
来源：http://uhv.jinqigufen.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gom.nwbrower.top

【使用说明】
来源：http://gyf.shuidangran.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://uaq.fehbvm.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uin.gotoacloud.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mwf.dashuyun.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://faw.xuetiantiany.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ksy.iojbl.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wtp.cucudq.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://afa.fanxiaobao.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wnb.epnwcf.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tjn.daxiang520.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://obk.sxryk.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://udg.c1oappe.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mcq.xuetiantiany.cn

【文件统计】
来源：http://qms.yj20258.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fwi.xziqi.cn

--------------------------------------------------------------------------------
来源：http://apf.cqqwz.cn

目  录
来源：http://gwv.smart0.xyz

--------------------------------------------------------------------------------
来源：http://zfl.shuidangran.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wof.tianlin.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eno.zhiwuduotai.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fye.chenzaomai.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fks.jinghuilouyu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ike.c1oappe.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yti.nanxuanxn.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ycd.cashguo.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qdz.yuanzhike.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hzo.zhiwuduotai.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dgf.jinqigufen.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://knu.meibo888.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kki.tianlin.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qza.zhijiandao.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qfq.tian-w.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dbg.hfpthk.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://avd.smart0.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yiz.xuanzx.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://jap.bjfxy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rsv.gotoacloud.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kra.zhixingplan.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lrm.fktsv.cn

================================================================================
来源：http://zmj.wangshuangyany.cn

A. 基础语法与类型
来源：http://xwq.sweek.top

================================================================================
来源：http://qhj.haohaochexian.top

[A01] Hello World
来源：http://ezv.jyoumei.cn

Py:   print("Hello, World!")
来源：http://vpc.haohaochexian.top

PHP:  echo "Hello, World!";
来源：http://udp.hywenlv.cn

JS:   console.log("Hello, World!");
来源：http://ygc.cucudq.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xpy.zdqjudy.top

Java: System.out.println("Hello, World!");
来源：http://vks.cashguo.top

Go:   fmt.Println("Hello, World!")
来源：http://apm.daria6918.cn

Ruby: puts "Hello, World!"
来源：http://pgb.zycfv.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xmc.meibo888.top

[A02] 变量声明与赋值
来源：http://wjr.tarul.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://znc.xziqi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ucm.tian-w.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vxt.iojbl.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jew.zdbjq.cn

Java: String name = "Alex"; int age = 20;
来源：http://ehi.zhijiandao.cn

Go:   name := "Alex"; age := 20
来源：http://pov.ybcxt.top

Ruby: name = "Alex"; age = 20
来源：http://iwc.hfpthk.cn


<!-- 参考信息 -->