代发 wailian999

[U31] Py：单测
来源：http://fjc.jqgufenzy.top

python -m pytest -q
来源：http://ure.redwolf501.top

[U32] Py：代码格式化
来源：http://vjh.feifeiyinyue.top

ruff format . && ruff check --fix .
来源：http://pum.hysaishi.cn

[U33] Py：打包发布
来源：http://xqq.xylfe.cn

python -m build  （依赖 pyproject.toml）
来源：http://daz.jyoumei.cn

[U34] Py：判断编码
来源：http://mld.ywan-chungtsiang.top

chardet.detect(raw)
来源：http://wsd.sufxvd.cn

[U35] Py：发送邮件
来源：http://shc.xylfe.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oik.xinyue.icu

[U36] Py：定时任务
来源：http://wpo.zdbjq.cn

schedule.every(10).minutes.do(job)
来源：http://kux.gogol.net.cn

[U37] Py：读写 Excel
来源：http://kch.yuanzhike.top

pandas.read_excel / DataFrame.to_excel
来源：http://uem.cdnleiting.top

[U38] Py：获取脚本所在目录
来源：http://lxc.gogol.net.cn

Path(__file__).resolve().parent
来源：http://lfd.jinqigufen.top

[U39] Py：判断是否在交互环境
来源：http://sfu.fehbvm.com

sys.stdout.isatty()
来源：http://nsm.hesvh.cn

[U40] Py：打印到标准错误
来源：http://sks.zdqjudy.top

print("err", file=sys.stderr)
来源：http://oah.gaohongyu789.top

[U41] PHP：初始化 Composer 项目
来源：http://vva.ivvv.top

composer init;  composer require guzzlehttp/guzzle
来源：http://jvd.cucudq.cn

[U42] PHP：PSR-4 自动加载
来源：http://uxh.cdnleiting.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tgh.tanke756.top

[U43] PHP：声明命名空间
来源：http://ecu.zhongyouzk.top

namespace App\Http;
来源：http://vur.tanke756.top

[U44] PHP：开启严格类型
来源：http://zeg.smart0.xyz

declare(strict_types=1);
来源：http://tht.bjfxy.top

[U45] PHP：类型声明与返回类型
来源：http://fzf.hesvh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vzd.vehdjk.com

[U46] PHP：可空类型
来源：http://qvh.cdnleiting.top

?string $name = null
来源：http://wvt.tanke756.top

[U47] PHP：联合类型
来源：http://mrb.chenjidiqi.icu

int|string $id
来源：http://vwu.jyoumei.cn

[U48] PHP：纯枚举
来源：http://lvi.hywenlv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cph.kuanghao11.cn

[U49] PHP：只读属性
来源：http://ffw.shanyushiyangkeji.top

public readonly string $name
来源：http://fcp.sysykeji.top

[U50] PHP：构造器属性提升
来源：http://ntn.jqgufenzy.top

public function __construct(private int $id) {}
来源：http://gyh.meibo888.top

[U51] PHP：数组解构
来源：http://gam.shangyingyoupin.top

[$a, $b] = $arr;
来源：http://wag.gaohongyu789.top

[U52] PHP：箭头函数
来源：http://gmt.dianchejie.cn

$double = fn($x) => $x * 2;
来源：http://gdo.zhaomingkeji.xyz

[U53] PHP：空合并运算符
来源：http://bcx.zdqjudy.top

$v = $a ?? $b ?? "default";
来源：http://tyi.jlsjyb.cn

[U54] PHP：空安全调用
来源：http://mml.redwolf501.top

$obj?->method()
来源：http://jcp.birdmap.top

[U55] PHP：match 表达式
来源：http://bwz.hnxiangtu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zjq.yonumen.top

[U56] PHP：命名参数
来源：http://qvh.yj20258.top

f(a: 1, b: 2)
来源：http://coa.cashguo.top

[U57] PHP：字符串插值
来源：http://amo.yueranfly.top

"值: {$a}"
来源：http://wdj.sufxvd.cn

[U58] PHP：数组三件套
来源：http://waq.0kj1m.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ikw.epnwcf.com

[U59] PHP：自定义排序
来源：http://mbh.daria6918.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bje.cheryme.top

[U60] PHP：JSON 编解码
来源：http://vtj.smart0.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pof.hesvh.cn

[U61] PHP：正则
来源：http://ewy.ehwqpu.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xff.xuetiantiany.cn

[U62] PHP：日期对象
来源：http://eax.fktsv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yir.dianchejie.cn

[U63] PHP：文件读写
来源：http://wlc.hammf.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mwl.tanke756.top

[U64] PHP：目录遍历
来源：http://bpx.redwolf501.top

glob("dir/*.php");  scandir("dir");
来源：http://gdu.yonumen.top

[U65] PHP：会话
来源：http://rrn.daria6918.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xzf.jinyuanbaomall.cn

[U66] PHP：设置 Cookie
来源：http://zhq.52xcode.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rgy.tarul.cn

[U67] PHP：处理文件上传
来源：http://qfx.hywenlv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://poy.chenlongwang.top

[U68] PHP：PDO 连接
来源：http://fvc.shanyushiyangtech.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ogr.zdbjq.cn

[U69] PHP：PDO 预处理
来源：http://ukx.yj20258.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://stn.shzxlz.cn

[U70] PHP：PDO 事务
来源：http://mpl.ydzc1.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vul.jinqigfzy.top

[U71] PHP：抛出异常
来源：http://cbg.sxryk.cn

throw new RuntimeException("失败", 500);
来源：http://ynb.yonumen.top

[U72] PHP：写错误日志
来源：http://vfc.fktsv.cn

error_log("失败: " . $e->getMessage());
来源：http://mvs.xuetiantiany.cn

[U73] PHP：读取 ini 配置
来源：http://brp.zhengqikj.top

parse_ini_file("config.ini", true)
来源：http://jky.shanyushiyangtech.top

[U74] PHP：读取环境变量
来源：http://hxm.cdnleiting.top

getenv("APP_ENV") ?: "production"
来源：http://uty.yj20258.top

[U75] PHP：依赖注入
来源：http://zqu.ctjpmb.com

composer require psr/container
来源：http://hge.yanxiufei.cn

[U76] PHP：简单路由
来源：http://uar.fktsv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zjm.hywenlv.cn

[U77] PHP：模板渲染
来源：http://wdn.jlsjyb.cn

composer require twig/twig
来源：http://lvz.fktsv.cn

[U78] PHP：单元测试
来源：http://ppu.vqdsnc.cn

composer require --dev phpunit/phpunit
来源：http://ilx.jinyuanbaomall.cn

[U79] PHP：静态分析
来源：http://agn.jinghuilouyu.cn

composer require --dev phpstan/phpstan
来源：http://rdx.shuidangran.top

[U80] PHP：代码规范修复
来源：http://cls.sjlbkw.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vac.yj202588.top

[U81] JS：初始化项目
来源：http://fer.9152youxi.cn

npm init -y;  npm i express
来源：http://xqc.yuanzhike.top

[U82] JS：package.json 脚本
来源：http://qju.yvedp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ark.shangyingyoupin.top

[U83] JS：ES Module 导入导出
来源：http://hwu.hcnkem.com

export const a = 1;  import { a } from "./m.js";
来源：http://vrt.shuidangran.top

[U84] JS：CommonJS 写法
来源：http://viy.zhongyouzk.top

module.exports = { a };  const { a } = require("./m");
来源：http://myn.pycfn.com

[U85] JS：可选链
来源：http://tpf.nwbrower.top

a?.b?.c
来源：http://ucb.zhongyouzk.top

[U86] JS：空值合并
来源：http://opx.daria6918.cn

a ?? b
来源：http://hdt.ywan-chungtsiang.top

[U87] JS：解构默认值
来源：http://qcl.snrcjt.cn

const { a = 1, b = 2 } = obj;
来源：http://csd.yj20258888.top

[U88] JS：对象展开合并
来源：http://azq.mhx1999.top

{ ...a, ...b }
来源：http://zsy.dashuyun.cn

[U89] JS：数组去重
来源：http://gup.jinyuanbaomall.cn

[...new Set(arr)]
来源：http://gjq.sufxvd.cn

[U90] JS：数字数组排序
来源：http://cdr.nanxinkj.top

[...arr].sort((a, b) => a - b)
来源：http://did.vehdjk.com

[U91] JS：对象键值遍历
来源：http://frw.sxryk.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kra.52xcode.cn

[U92] JS：深拷贝
来源：http://gxu.gzhubu.top

structuredClone(obj)
来源：http://cqk.hesvh.cn

[U93] JS：模板字符串
来源：http://jqf.fktsv.cn

`共 ${n} 条`
来源：http://fpk.xinyue.icu

[U94] JS：箭头函数
来源：http://nez.sweek.top

const double = x => x * 2;
来源：http://khc.ydjk.org.cn

[U95] JS：Promise 包装
来源：http://fug.dashuyun.cn

new Promise((resolve, reject) => {})
来源：http://nib.hysaishi.cn

[U96] JS：async/await 与异常
来源：http://ynh.hnqzz.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zls.hammf.cn

[U97] JS：并发请求
来源：http://bha.sufxvd.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lsi.dianchejie.cn

[U98] JS：fetch 带 JSON
来源：http://ysz.snrcjt.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vko.gotoacloud.top

[U99] JS：事件监听
来源：http://pck.vqdsnc.cn

el.addEventListener("click", e => {})
来源：http://eql.aibaodan.cn

[U100] JS：DOM 查询
来源：http://shs.sjlbkw.cn

document.querySelector(".item")
来源：http://vod.ehwqpu.com

[U101] JS：classList 操作
来源：http://rlh.jiagoushi.top

el.classList.toggle("active")
来源：http://zkm.pengpengdd.cyou

[U102] JS：本地存储
来源：http://cfa.epnwcf.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://hgq.cdnleiting.top

[U103] JS：定时器
来源：http://xyl.ybcxt.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rwi.tian-w.cn

[U104] JS：防抖
来源：http://lik.sxryk.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rvm.jiagoushi.top

[U105] JS：节流
来源：http://kbb.yj202588.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vwo.jinqigfzy.top

[U106] JS：日期格式化
来源：http://djg.pycfn.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://upz.chenjidiqi.icu

[U107] JS：数字千分位
来源：http://kou.feifeiyinyue.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rwm.smart0.xyz

[U108] JS：随机整数
来源：http://lqx.pengpengdd.cyou

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ajn.hnxiangtu.top

[U109] JS：数组分组
来源：http://sys.fehbvm.com

Object.groupBy(arr, x => x.type)
来源：http://vmx.cdnleiting.top

[U110] JS：数组分块
来源：http://xst.cdnleiting.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://acp.havefunace.top

[U111] JS：对象转 Map
来源：http://mfb.zhixingplan.top

new Map(Object.entries(obj))
来源：http://wvr.yangfankeji.com

[U112] JS：字符串补位
来源：http://wvr.wangshuangyany.cn

"7".padStart(3, "0")
来源：http://shf.haohaochexian.top

[U113] JS：正则替换全部
来源：http://osi.ydzc1.top

s.replaceAll("a", "b")
来源：http://opt.zhoulong.xyz

[U114] JS：JSON 深比较
来源：http://xhl.fktsv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wwe.xinyue.icu

[U115] JS：生成 UUID
来源：http://gyu.sjlbkw.cn

crypto.randomUUID()
来源：http://zom.ehwqpu.com

[U116] JS：类型检查（JSDoc）
来源：http://oin.c1oappe.top

/** @param {string} name */ function f(name) {}
来源：http://rbd.haohaochexian.top

[U117] JS：单元测试
来源：http://dqo.zdbjq.cn

npm i -D vitest;  npx vitest
来源：http://ltn.0kj1m.cn

[U118] JS：开发服务器
来源：http://owf.zhoulong.xyz

npm i -D vite;  npx vite
来源：http://xly.guannengcc.top

[U119] JS：生产构建
来源：http://phq.shanyushiyangtech.top

npx vite build
来源：http://eva.jinqigfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://hoi.daria6918.cn

import.meta.env.VITE_API_URL
来源：http://nyr.pengpengdd.cyou

================================================================================
来源：http://vnv.nwbrower.top

统计汇总
来源：http://bjl.havefunace.top

================================================================================
来源：http://frk.xylfe.cn

按语言统计（条）：
来源：http://sqb.pengpengdd.cyou

Python ......... 252
来源：http://wdc.yfazqb.com

PHP ............ 252
来源：http://xqu.shuidangran.top

JavaScript ..... 252
来源：http://byg.gogol.net.cn

TypeScript ..... 212
来源：http://vpt.redwolf501.top

Java ........... 212
来源：http://agi.fktsv.cn

Go ............. 212
来源：http://fyh.guowangkeji.top

Ruby ........... 212
来源：http://irx.aizwys.cn

C# ............. 212
来源：http://bnp.bbcook.cn

C .............. 30
来源：http://dle.chenzaomai.com

C++ ............ 30
来源：http://aip.feifeiyinyue.top

SQL ............ 90
来源：http://cni.52xcode.cn

Bash ........... 80
来源：http://fpx.cdnleiting.top

Kotlin ......... 15
来源：http://gqt.haohaochexian.top

Swift .......... 15
来源：http://zfn.ywan-chungtsiang.top

Lua ............ 10
来源：http://rwm.hesvh.cn

Perl ........... 10
来源：http://wff.iojbl.cn

Scala .......... 10
来源：http://tit.jqgfzy.top

------------------------------------
来源：http://jck.tianlin.xyz

合计 ........... 2106 条
来源：http://ytz.ehwqpu.com

按章节统计：
来源：http://wna.zhijiandao.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ine.zhoulong.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mzp.tarul.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lpx.xingfuxueyuan.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://oxs.havefunace.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tcg.hesvh.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fzv.zdbjq.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ezm.ehwqpu.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mkp.yvedp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jnx.hongshengwenyu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ajz.jqgfzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://voz.zdqjudy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bxp.cucudq.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jvi.hfpthk.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wdu.hammf.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dvt.zhongyouzk.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://haa.daxiang520.top

Q SQL 专题                              90
来源：http://pxv.hammf.cn

R Bash 专题                             80
来源：http://zlg.yfazqb.com

S C / C++ 专题                          60
来源：http://ysk.ywan-chungtsiang.top

T 其他语言补充                          60
来源：http://vwa.yfazqb.com

U 高频实用片段                         120
来源：http://xcw.hesvh.cn

------------------------------------
来源：http://gtp.zhongyouzk.top

合计                                  2106 条
来源：http://mhb.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://rux.zhoulong.xyz

使用提醒
来源：http://fdw.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://wux.xinyue.icu

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kvc.bbcook.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://shn.dashuyun.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://oqq.jlsjyb.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dun.dashuyun.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bva.nanxuanxn.top

—— 文件结束 ——
来源：http://nlf.0kj1m.cn

================================================================================
来源：http://mme.ivvv.top

程序语言常见例子速查手册（2024 版）
来源：http://mjy.pycfn.com

Common Programming Examples Cheat Book
来源：http://xws.ppjwa.cn

================================================================================
来源：http://zno.kuanghao11.cn

【收录内容】
来源：http://dyr.chenjidiqi.icu

覆盖 12 种语言 / 语法与常见 API：
来源：http://iil.shzxlz.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://oec.ywan-chungtsiang.top

SQL · Bash · C · C++
来源：http://qma.zhixingplan.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uyu.havefunace.top

【使用说明】
来源：http://fil.zdqjudy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://iba.hammf.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://icd.guannengcc.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bnp.ehwqpu.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zhf.xinyue.icu

Bash:  Shell         C:     C             C++:   C++
来源：http://vsm.epnwcf.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zvi.hfpthk.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vma.tian-w.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hoq.zhiwuduotai.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://sfn.haohaochexian.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://alj.tianlin.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dxa.fehbvm.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tyb.fktsv.cn

【文件统计】
来源：http://eyw.tanke756.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://uhk.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://hht.ybcxt.top

目  录
来源：http://uyy.yj202588.top

--------------------------------------------------------------------------------
来源：http://fxd.jqgufenzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://soc.nanxinkj.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://piv.cqqwz.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dgx.ydzc1.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://drm.fzhhl.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://riv.epnwcf.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cbn.shanyushiyangkeji.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ier.cqqwz.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jlp.snrcjt.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://uxc.xylfe.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jrl.jinqigufen.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vbe.yuanzhike.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pyq.guannengcc.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fxo.tianlin.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://stg.sufxvd.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://slt.wangdashe.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jql.xuanzx.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zng.tian-w.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://dcy.chenjidiqi.icu

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cvy.yfazqb.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tfv.zhongyouzk.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dvf.tianlin.xyz

================================================================================
来源：http://cjd.yvedp.cn

A. 基础语法与类型
来源：http://gvz.zhongyouzk.top

================================================================================
来源：http://gtl.sysykeji.top

[A01] Hello World
来源：http://dns.ppjwa.cn

Py:   print("Hello, World!")
来源：http://qia.bbcook.cn

PHP:  echo "Hello, World!";
来源：http://vfj.yj20258.top

JS:   console.log("Hello, World!");
来源：http://btu.guannengcc.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vbl.sysykeji.top

Java: System.out.println("Hello, World!");
来源：http://etm.hcnkem.com

Go:   fmt.Println("Hello, World!")
来源：http://rim.guowangkeji.top

Ruby: puts "Hello, World!"
来源：http://fef.yvedp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nep.hnxiangtu.top

[A02] 变量声明与赋值
来源：http://zvb.wangdashe.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vkm.andypj.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://aiq.ctjpmb.com

JS:   let name = "Alex"; const age = 20;
来源：http://dsj.fanxiaobao.xyz


<!-- 参考信息 -->