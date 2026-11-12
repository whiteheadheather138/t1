代发 wailian999

[U25] Py：CSV 按字典读
来源：http://lfy.sufxvd.cn

csv.DictReader(f)
来源：http://oei.mhx1999.top

[U26] Py：并发下载
来源：http://jir.cashguo.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kdp.zhixingplan.top

[U27] Py：异步 HTTP
来源：http://biq.tanke756.top

aiohttp.ClientSession() 配合 async with
来源：http://frt.xylfe.cn

[U28] Py：类型别名
来源：http://jgx.zhengqikj.top

UserId = int
来源：http://ggy.ydzc1.top

[U29] Py：属性校验
来源：http://ash.birdmap.top

@property 与 @x.setter 配合
来源：http://hnx.haohaochexian.top

[U30] Py：数据类
来源：http://vty.cdnleiting.top

@dataclass(slots=True)
来源：http://fgi.gogol.net.cn

[U31] Py：单测
来源：http://tyt.kuanghao11.cn

python -m pytest -q
来源：http://glb.haohaochexian.top

[U32] Py：代码格式化
来源：http://ltx.sjlbkw.cn

ruff format . && ruff check --fix .
来源：http://wtj.zhijiandao.cn

[U33] Py：打包发布
来源：http://fdo.hywenlv.cn

python -m build  （依赖 pyproject.toml）
来源：http://ffk.svipenyu.cn

[U34] Py：判断编码
来源：http://zue.jinyuanbaomall.cn

chardet.detect(raw)
来源：http://yau.bjfxy.top

[U35] Py：发送邮件
来源：http://zhx.xingfuxueyuan.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gsc.fengsongda.top

[U36] Py：定时任务
来源：http://sfr.jinqigufen.top

schedule.every(10).minutes.do(job)
来源：http://tln.bbcook.cn

[U37] Py：读写 Excel
来源：http://iev.nanxuanxn.top

pandas.read_excel / DataFrame.to_excel
来源：http://vex.jyoumei.cn

[U38] Py：获取脚本所在目录
来源：http://bby.ppjwa.cn

Path(__file__).resolve().parent
来源：http://laf.jinqigufen.top

[U39] Py：判断是否在交互环境
来源：http://hpi.yj20258.top

sys.stdout.isatty()
来源：http://ctd.316326.xyz

[U40] Py：打印到标准错误
来源：http://yhb.snrcjt.cn

print("err", file=sys.stderr)
来源：http://fbe.snrcjt.cn

[U41] PHP：初始化 Composer 项目
来源：http://gni.gzhubu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://zit.shzxlz.cn

[U42] PHP：PSR-4 自动加载
来源：http://ezb.yangfankeji.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://aqq.zhiwuduotai.top

[U43] PHP：声明命名空间
来源：http://iui.yj20258888.top

namespace App\Http;
来源：http://onp.hfpthk.cn

[U44] PHP：开启严格类型
来源：http://rrk.ydzc1.top

declare(strict_types=1);
来源：http://fuh.aibaodan.cn

[U45] PHP：类型声明与返回类型
来源：http://vqm.yueranfly.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://eop.shangyingyoupin.top

[U46] PHP：可空类型
来源：http://knn.zdqjudy.top

?string $name = null
来源：http://sda.yj202588.top

[U47] PHP：联合类型
来源：http://uct.hywenlv.cn

int|string $id
来源：http://edw.jinqigfzy.top

[U48] PHP：纯枚举
来源：http://cse.tarul.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yon.yueranfly.top

[U49] PHP：只读属性
来源：http://wkg.guowangkeji.top

public readonly string $name
来源：http://evc.yuanzhike.top

[U50] PHP：构造器属性提升
来源：http://sww.nanxuanxn.top

public function __construct(private int $id) {}
来源：http://fcn.52xcode.cn

[U51] PHP：数组解构
来源：http://uij.yangfankeji.com

[$a, $b] = $arr;
来源：http://vux.shangyingyoupin.top

[U52] PHP：箭头函数
来源：http://hlt.zycfv.cn

$double = fn($x) => $x * 2;
来源：http://bgx.nanxinkj.top

[U53] PHP：空合并运算符
来源：http://vmd.yangfankeji.com

$v = $a ?? $b ?? "default";
来源：http://zqo.ydjk.org.cn

[U54] PHP：空安全调用
来源：http://awo.yanxiufei.cn

$obj?->method()
来源：http://rnq.yj20258888.top

[U55] PHP：match 表达式
来源：http://vpv.fktsv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bnl.yuanzhike.top

[U56] PHP：命名参数
来源：http://pgi.chenzaomai.com

f(a: 1, b: 2)
来源：http://iws.havefunace.top

[U57] PHP：字符串插值
来源：http://cpu.zhiwuduotai.top

"值: {$a}"
来源：http://cht.havefunace.top

[U58] PHP：数组三件套
来源：http://jch.svipenyu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tfi.jiagoushi.top

[U59] PHP：自定义排序
来源：http://esh.yj20258.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cvn.bbcook.cn

[U60] PHP：JSON 编解码
来源：http://zfl.tian-w.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nrc.ydjk.org.cn

[U61] PHP：正则
来源：http://urz.hnqzz.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bal.snrcjt.cn

[U62] PHP：日期对象
来源：http://rhv.yuanzhike.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lxp.jinghuilouyu.cn

[U63] PHP：文件读写
来源：http://pdf.xziqi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jwu.andypj.xyz

[U64] PHP：目录遍历
来源：http://xvm.haohaochexian.top

glob("dir/*.php");  scandir("dir");
来源：http://qry.zhengqikj.top

[U65] PHP：会话
来源：http://ipd.bjfxy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://uea.ivvv.top

[U66] PHP：设置 Cookie
来源：http://rhr.epnwcf.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cdy.tian-w.cn

[U67] PHP：处理文件上传
来源：http://tcg.andypj.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qgh.fehbvm.com

[U68] PHP：PDO 连接
来源：http://eag.fzhhl.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yrn.meibo888.top

[U69] PHP：PDO 预处理
来源：http://ysu.sysykeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lzr.ywan-chungtsiang.top

[U70] PHP：PDO 事务
来源：http://hpf.yuxming.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ftw.zhixingplan.top

[U71] PHP：抛出异常
来源：http://gft.fzhhl.top

throw new RuntimeException("失败", 500);
来源：http://zwm.quarkkingdee.top

[U72] PHP：写错误日志
来源：http://ynk.nanxuanxn.top

error_log("失败: " . $e->getMessage());
来源：http://znm.hywenlv.cn

[U73] PHP：读取 ini 配置
来源：http://xli.yj20258.top

parse_ini_file("config.ini", true)
来源：http://ylg.snrcjt.cn

[U74] PHP：读取环境变量
来源：http://nss.fanxiaobao.xyz

getenv("APP_ENV") ?: "production"
来源：http://adu.chenlongwang.top

[U75] PHP：依赖注入
来源：http://dyr.gaohongyu789.top

composer require psr/container
来源：http://tac.sysykeji.top

[U76] PHP：简单路由
来源：http://hzs.52xcode.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://flq.ywan-chungtsiang.top

[U77] PHP：模板渲染
来源：http://zia.xinyue.icu

composer require twig/twig
来源：http://rtr.kuanghao11.cn

[U78] PHP：单元测试
来源：http://tya.havefunace.top

composer require --dev phpunit/phpunit
来源：http://sfd.sweek.top

[U79] PHP：静态分析
来源：http://pob.mhx1999.top

composer require --dev phpstan/phpstan
来源：http://neu.jinghuilouyu.cn

[U80] PHP：代码规范修复
来源：http://tba.birdmap.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://thq.jianghu66.top

[U81] JS：初始化项目
来源：http://ijt.guannengcc.top

npm init -y;  npm i express
来源：http://pnv.feifeiyinyue.top

[U82] JS：package.json 脚本
来源：http://jst.shzxlz.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zth.vehdjk.com

[U83] JS：ES Module 导入导出
来源：http://ddt.zhijiandao.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mwh.dashuyun.cn

[U84] JS：CommonJS 写法
来源：http://viw.wangshuangyany.cn

module.exports = { a };  const { a } = require("./m");
来源：http://svp.cheryme.top

[U85] JS：可选链
来源：http://qne.guannengcc.top

a?.b?.c
来源：http://tsx.aibaodan.cn

[U86] JS：空值合并
来源：http://lhg.jlsjyb.cn

a ?? b
来源：http://vww.jinqigfzy.top

[U87] JS：解构默认值
来源：http://zcl.yj20258.top

const { a = 1, b = 2 } = obj;
来源：http://hjj.cdnleiting.top

[U88] JS：对象展开合并
来源：http://zqa.shuidangran.top

{ ...a, ...b }
来源：http://mog.sjlbkw.cn

[U89] JS：数组去重
来源：http://bfe.ivvv.top

[...new Set(arr)]
来源：http://dnq.gzhubu.top

[U90] JS：数字数组排序
来源：http://byq.hcnkem.com

[...arr].sort((a, b) => a - b)
来源：http://snf.hfpthk.cn

[U91] JS：对象键值遍历
来源：http://bmu.nanxinkj.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yxe.zhiwuduotai.top

[U92] JS：深拷贝
来源：http://ucr.smart0.xyz

structuredClone(obj)
来源：http://hxc.fanxiaobao.xyz

[U93] JS：模板字符串
来源：http://rwj.aibaodan.cn

`共 ${n} 条`
来源：http://vuc.daria6918.cn

[U94] JS：箭头函数
来源：http://yly.jinqigufen.top

const double = x => x * 2;
来源：http://izw.zhiwuduotai.top

[U95] JS：Promise 包装
来源：http://itv.zhongyouzk.top

new Promise((resolve, reject) => {})
来源：http://jjf.yvedp.cn

[U96] JS：async/await 与异常
来源：http://gyc.sufxvd.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rmk.316326.xyz

[U97] JS：并发请求
来源：http://sfq.birdmap.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://zpk.cucudq.cn

[U98] JS：fetch 带 JSON
来源：http://yji.yueranfly.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vwg.mhx1999.top

[U99] JS：事件监听
来源：http://ovh.uphjek.com

el.addEventListener("click", e => {})
来源：http://xpj.hfpthk.cn

[U100] JS：DOM 查询
来源：http://ilh.cashguo.top

document.querySelector(".item")
来源：http://nhr.hfpthk.cn

[U101] JS：classList 操作
来源：http://fcd.zhongyouzk.top

el.classList.toggle("active")
来源：http://pjs.aizwys.cn

[U102] JS：本地存储
来源：http://qwv.jqgufenzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://mhv.cdnleiting.top

[U103] JS：定时器
来源：http://nsj.c1oappe.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://iwd.tian-w.cn

[U104] JS：防抖
来源：http://yab.tanke756.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qvd.yj202588.top

[U105] JS：节流
来源：http://rfg.ehwqpu.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zeq.zhongyouzk.top

[U106] JS：日期格式化
来源：http://ohn.c1oappe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fev.sjlbkw.cn

[U107] JS：数字千分位
来源：http://tqq.wangdashe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cnp.dianchejie.cn

[U108] JS：随机整数
来源：http://fgi.fengsongda.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fcl.shangyingyoupin.top

[U109] JS：数组分组
来源：http://gjr.316326.xyz

Object.groupBy(arr, x => x.type)
来源：http://rhm.yonumen.top

[U110] JS：数组分块
来源：http://wmq.birdmap.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://obd.tanke756.top

[U111] JS：对象转 Map
来源：http://ckg.gogol.net.cn

new Map(Object.entries(obj))
来源：http://ehy.jinqigufen.top

[U112] JS：字符串补位
来源：http://fpo.dianchejie.cn

"7".padStart(3, "0")
来源：http://fgl.hysaishi.cn

[U113] JS：正则替换全部
来源：http://oxt.zhixingplan.top

s.replaceAll("a", "b")
来源：http://hsl.9152youxi.cn

[U114] JS：JSON 深比较
来源：http://qtz.shangyingyoupin.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://nbr.fengsongda.top

[U115] JS：生成 UUID
来源：http://lfu.zhongyouzk.top

crypto.randomUUID()
来源：http://noh.yj20258.top

[U116] JS：类型检查（JSDoc）
来源：http://zom.chenzaomai.com

/** @param {string} name */ function f(name) {}
来源：http://kih.xuanzx.com

[U117] JS：单元测试
来源：http://ext.cdnleiting.top

npm i -D vitest;  npx vitest
来源：http://tzi.daxiang520.top

[U118] JS：开发服务器
来源：http://fiq.yueranfly.top

npm i -D vite;  npx vite
来源：http://mhx.wangdashe.top

[U119] JS：生产构建
来源：http://hyd.shanyushiyangtech.top

npx vite build
来源：http://laj.zhaomingkeji.xyz

[U120] JS：读取环境变量（Vite）
来源：http://pyp.shanyushiyangkeji.top

import.meta.env.VITE_API_URL
来源：http://eky.ivvv.top

================================================================================
来源：http://wvn.tarul.cn

统计汇总
来源：http://hpy.9152youxi.cn

================================================================================
来源：http://ygp.snrcjt.cn

按语言统计（条）：
来源：http://eio.ehwqpu.com

Python ......... 252
来源：http://hai.daxiang520.top

PHP ............ 252
来源：http://tuz.shangyingyoupin.top

JavaScript ..... 252
来源：http://gxa.aizwys.cn

TypeScript ..... 212
来源：http://emf.xingfuxueyuan.xyz

Java ........... 212
来源：http://hrp.yuxming.cn

Go ............. 212
来源：http://pcb.yueranfly.top

Ruby ........... 212
来源：http://igp.zhixingplan.top

C# ............. 212
来源：http://kir.gogol.net.cn

C .............. 30
来源：http://jdv.tarul.cn

C++ ............ 30
来源：http://eie.fzhhl.top

SQL ............ 90
来源：http://gki.yongpay.top

Bash ........... 80
来源：http://htq.pycfn.com

Kotlin ......... 15
来源：http://ccs.vehdjk.com

Swift .......... 15
来源：http://tzi.nanxinkj.top

Lua ............ 10
来源：http://ngq.jqgufenzy.top

Perl ........... 10
来源：http://gtv.ydzc1.top

Scala .......... 10
来源：http://day.xinyue.icu

------------------------------------
来源：http://fqu.kuanghao11.cn

合计 ........... 2106 条
来源：http://fwm.jqgfzy.top

按章节统计：
来源：http://iuu.ydjk.org.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ozx.zhaomingkeji.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nbf.fehbvm.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wsv.hywenlv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://liq.jinqigufen.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://plq.sjlbkw.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gwj.havefunace.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lmd.zhaomingkeji.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vnk.nanxinkj.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wiz.jinghuilouyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yjk.xuetiantiany.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tpp.zhoulong.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nhh.hfpthk.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mld.feifeiyinyue.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kge.andypj.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mnk.tanke756.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cgt.epnwcf.com

Q SQL 专题                              90
来源：http://vyu.vehdjk.com

R Bash 专题                             80
来源：http://uhj.9152youxi.cn

S C / C++ 专题                          60
来源：http://rts.jqgfzy.top

T 其他语言补充                          60
来源：http://etu.cheryme.top

U 高频实用片段                         120
来源：http://doo.zhengqikj.top

------------------------------------
来源：http://gbt.yvedp.cn

合计                                  2106 条
来源：http://tut.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://rsk.xingfuxueyuan.xyz

使用提醒
来源：http://orq.havefunace.top

--------------------------------------------------------------------------------
来源：http://qsh.fktsv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vae.sweek.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hkx.birdmap.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nef.zhiwuduotai.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ubh.snrcjt.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://omf.ctjpmb.com

—— 文件结束 ——
来源：http://kbe.andypj.xyz

================================================================================
来源：http://ixk.yj202588.top

程序语言常见例子速查手册（2024 版）
来源：http://kwo.bbcook.cn

Common Programming Examples Cheat Book
来源：http://hbr.hongshengwenyu.top

================================================================================
来源：http://taj.shangyingyoupin.top

【收录内容】
来源：http://umr.ctjpmb.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://ymt.ppjwa.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://miv.smart0.xyz

SQL · Bash · C · C++
来源：http://dcr.svipenyu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kek.yfazqb.com

【使用说明】
来源：http://aqg.jqgfzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wor.0kj1m.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zug.jinyuanbaomall.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bax.ivvv.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xbx.zhongyouzk.top

Bash:  Shell         C:     C             C++:   C++
来源：http://itp.bbcook.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cxm.jinghuilouyu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://daa.tarul.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://coj.zdbjq.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hae.jinqigufen.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vfj.shuidangran.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eef.xuanzx.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wqn.yonumen.top

【文件统计】
来源：http://zlp.nwbrower.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kjo.andypj.xyz

--------------------------------------------------------------------------------
来源：http://osx.xylfe.cn

目  录
来源：http://ewx.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://jnv.xziqi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qmb.pengpengdd.cyou

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jnd.iojbl.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gui.fanxiaobao.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://owo.shzxlz.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ing.hnxiangtu.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nuy.redwolf501.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://moa.chenzaomai.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bhw.xylfe.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ins.iojbl.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mwl.ehwqpu.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xya.havefunace.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fru.fengsongda.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tpp.feifeiyinyue.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bxg.cdnleiting.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uhk.gogol.net.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hqr.zhiwuduotai.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tzk.shzxlz.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hgf.ydzc1.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lnt.shzxlz.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xbd.smart0.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zus.guowangkeji.top

================================================================================
来源：http://doe.hongshengwenyu.top

A. 基础语法与类型
来源：http://mks.zhaomingkeji.xyz

================================================================================
来源：http://mkr.gaohongyu789.top

[A01] Hello World
来源：http://tsa.kuanghao11.cn


<!-- 参考信息 -->