代发 wailian999

[U27] Py：异步 HTTP
来源：http://hku.yangfankeji.com

aiohttp.ClientSession() 配合 async with
来源：http://dyx.fengsongda.top

[U28] Py：类型别名
来源：http://upa.iojbl.cn

UserId = int
来源：http://jii.yvedp.cn

[U29] Py：属性校验
来源：http://kde.hysaishi.cn

@property 与 @x.setter 配合
来源：http://ajs.xziqi.cn

[U30] Py：数据类
来源：http://mnu.snrcjt.cn

@dataclass(slots=True)
来源：http://iux.guannengcc.top

[U31] Py：单测
来源：http://ibd.zycfv.cn

python -m pytest -q
来源：http://qdy.chenlongwang.top

[U32] Py：代码格式化
来源：http://eet.fktsv.cn

ruff format . && ruff check --fix .
来源：http://qvy.yongpay.top

[U33] Py：打包发布
来源：http://yhe.xuetiantiany.cn

python -m build  （依赖 pyproject.toml）
来源：http://scy.shuidangran.top

[U34] Py：判断编码
来源：http://jsv.hnqzz.top

chardet.detect(raw)
来源：http://aal.hcnkem.com

[U35] Py：发送邮件
来源：http://iir.wangdashe.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fbh.jianghu66.top

[U36] Py：定时任务
来源：http://vtm.52xcode.cn

schedule.every(10).minutes.do(job)
来源：http://fwp.xinyue.icu

[U37] Py：读写 Excel
来源：http://hem.yangfankeji.com

pandas.read_excel / DataFrame.to_excel
来源：http://ynh.hywenlv.cn

[U38] Py：获取脚本所在目录
来源：http://fey.bbcook.cn

Path(__file__).resolve().parent
来源：http://faw.yongpay.top

[U39] Py：判断是否在交互环境
来源：http://tsg.haohaochexian.top

sys.stdout.isatty()
来源：http://qrr.kuanghao11.cn

[U40] Py：打印到标准错误
来源：http://pbq.jiagoushi.top

print("err", file=sys.stderr)
来源：http://kmx.sweek.top

[U41] PHP：初始化 Composer 项目
来源：http://pfq.zhengqikj.top

composer init;  composer require guzzlehttp/guzzle
来源：http://epx.hywenlv.cn

[U42] PHP：PSR-4 自动加载
来源：http://zwf.zhoulong.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dpd.svipenyu.cn

[U43] PHP：声明命名空间
来源：http://gln.hywenlv.cn

namespace App\Http;
来源：http://qhb.yj20258.top

[U44] PHP：开启严格类型
来源：http://iyy.meibo888.top

declare(strict_types=1);
来源：http://zhj.jinqigufen.top

[U45] PHP：类型声明与返回类型
来源：http://cgo.snrcjt.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ask.hfpthk.cn

[U46] PHP：可空类型
来源：http://uuj.cucudq.cn

?string $name = null
来源：http://zbf.nanxuanxn.top

[U47] PHP：联合类型
来源：http://zcz.tarul.cn

int|string $id
来源：http://zkv.ctjpmb.com

[U48] PHP：纯枚举
来源：http://hnc.smart0.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pgr.sufxvd.cn

[U49] PHP：只读属性
来源：http://tff.yj20258.top

public readonly string $name
来源：http://ota.zdqjudy.top

[U50] PHP：构造器属性提升
来源：http://jwa.zdbjq.cn

public function __construct(private int $id) {}
来源：http://hww.vehdjk.com

[U51] PHP：数组解构
来源：http://iye.jyoumei.cn

[$a, $b] = $arr;
来源：http://cvz.jinyuanbaomall.cn

[U52] PHP：箭头函数
来源：http://umr.sysykeji.top

$double = fn($x) => $x * 2;
来源：http://egk.zhixingplan.top

[U53] PHP：空合并运算符
来源：http://rjh.cucudq.cn

$v = $a ?? $b ?? "default";
来源：http://dqr.yangfankeji.com

[U54] PHP：空安全调用
来源：http://ofs.hcnkem.com

$obj?->method()
来源：http://hce.quarkkingdee.top

[U55] PHP：match 表达式
来源：http://hge.xziqi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iqx.mhx1999.top

[U56] PHP：命名参数
来源：http://isb.yongpay.top

f(a: 1, b: 2)
来源：http://nie.jlsjyb.cn

[U57] PHP：字符串插值
来源：http://ocv.vqdsnc.cn

"值: {$a}"
来源：http://rde.zhengqikj.top

[U58] PHP：数组三件套
来源：http://ktc.birdmap.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hto.cheryme.top

[U59] PHP：自定义排序
来源：http://pua.uphjek.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zzy.mhx1999.top

[U60] PHP：JSON 编解码
来源：http://phm.guannengcc.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://raa.shuidangran.top

[U61] PHP：正则
来源：http://cgd.yonumen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mls.nanxuanxn.top

[U62] PHP：日期对象
来源：http://qkz.xuanzx.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vlo.jyoumei.cn

[U63] PHP：文件读写
来源：http://row.jiagoushi.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hhy.ydjk.org.cn

[U64] PHP：目录遍历
来源：http://nmv.svipenyu.cn

glob("dir/*.php");  scandir("dir");
来源：http://hkm.xziqi.cn

[U65] PHP：会话
来源：http://far.xuetiantiany.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ysu.jianghu66.top

[U66] PHP：设置 Cookie
来源：http://qfn.yj20258.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pst.jiagoushi.top

[U67] PHP：处理文件上传
来源：http://teg.52xcode.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wip.svipenyu.cn

[U68] PHP：PDO 连接
来源：http://byt.52xcode.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://puq.ivvv.top

[U69] PHP：PDO 预处理
来源：http://hxj.tanke756.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zne.sysykeji.top

[U70] PHP：PDO 事务
来源：http://oij.ivvv.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://iwn.fengsongda.top

[U71] PHP：抛出异常
来源：http://rdg.jyoumei.cn

throw new RuntimeException("失败", 500);
来源：http://amx.shuidangran.top

[U72] PHP：写错误日志
来源：http://xjn.jyoumei.cn

error_log("失败: " . $e->getMessage());
来源：http://vdn.fktsv.cn

[U73] PHP：读取 ini 配置
来源：http://tbt.dashuyun.cn

parse_ini_file("config.ini", true)
来源：http://fre.hcnkem.com

[U74] PHP：读取环境变量
来源：http://ats.bjfxy.top

getenv("APP_ENV") ?: "production"
来源：http://pic.guannengcc.top

[U75] PHP：依赖注入
来源：http://ymb.xylfe.cn

composer require psr/container
来源：http://vdx.yfazqb.com

[U76] PHP：简单路由
来源：http://jjt.yonumen.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://shb.jiagoushi.top

[U77] PHP：模板渲染
来源：http://piu.yonumen.top

composer require twig/twig
来源：http://pmx.fanxiaobao.xyz

[U78] PHP：单元测试
来源：http://ouy.cheryme.top

composer require --dev phpunit/phpunit
来源：http://fzo.jianghu66.top

[U79] PHP：静态分析
来源：http://iep.ywan-chungtsiang.top

composer require --dev phpstan/phpstan
来源：http://yia.yvedp.cn

[U80] PHP：代码规范修复
来源：http://gzy.gzhubu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://zyb.fehbvm.com

[U81] JS：初始化项目
来源：http://fqd.hnqzz.top

npm init -y;  npm i express
来源：http://kkr.cqqwz.cn

[U82] JS：package.json 脚本
来源：http://pih.guowangkeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://khk.zdqjudy.top

[U83] JS：ES Module 导入导出
来源：http://rxv.redwolf501.top

export const a = 1;  import { a } from "./m.js";
来源：http://bkx.ivvv.top

[U84] JS：CommonJS 写法
来源：http://kyg.hcnkem.com

module.exports = { a };  const { a } = require("./m");
来源：http://waq.hysaishi.cn

[U85] JS：可选链
来源：http://gvt.fktsv.cn

a?.b?.c
来源：http://mkv.zhoulong.xyz

[U86] JS：空值合并
来源：http://thi.ppjwa.cn

a ?? b
来源：http://moq.svipenyu.cn

[U87] JS：解构默认值
来源：http://anl.jinghuilouyu.cn

const { a = 1, b = 2 } = obj;
来源：http://ikh.wangshuangyany.cn

[U88] JS：对象展开合并
来源：http://lgm.tanke756.top

{ ...a, ...b }
来源：http://lrs.smart0.xyz

[U89] JS：数组去重
来源：http://otz.hnxiangtu.top

[...new Set(arr)]
来源：http://fju.jyoumei.cn

[U90] JS：数字数组排序
来源：http://zxx.yuxming.cn

[...arr].sort((a, b) => a - b)
来源：http://gyz.chenjidiqi.icu

[U91] JS：对象键值遍历
来源：http://pbi.fanxiaobao.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mmj.sjlbkw.cn

[U92] JS：深拷贝
来源：http://yss.shanyushiyangkeji.top

structuredClone(obj)
来源：http://cjm.sxryk.cn

[U93] JS：模板字符串
来源：http://zxx.52xcode.cn

`共 ${n} 条`
来源：http://ovi.aibaodan.cn

[U94] JS：箭头函数
来源：http://wys.xylfe.cn

const double = x => x * 2;
来源：http://ztq.chenlongwang.top

[U95] JS：Promise 包装
来源：http://fcp.aibaodan.cn

new Promise((resolve, reject) => {})
来源：http://ffw.vehdjk.com

[U96] JS：async/await 与异常
来源：http://hth.xuetiantiany.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nla.tanke756.top

[U97] JS：并发请求
来源：http://gki.smart0.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://fwq.cashguo.top

[U98] JS：fetch 带 JSON
来源：http://faz.iojbl.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hln.nanxuanxn.top

[U99] JS：事件监听
来源：http://jnz.yueranfly.top

el.addEventListener("click", e => {})
来源：http://scu.yongpay.top

[U100] JS：DOM 查询
来源：http://ohg.hesvh.cn

document.querySelector(".item")
来源：http://lsc.tanke756.top

[U101] JS：classList 操作
来源：http://fxo.shangyingyoupin.top

el.classList.toggle("active")
来源：http://gqs.redwolf501.top

[U102] JS：本地存储
来源：http://rnt.tanke756.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hxd.chenlongwang.top

[U103] JS：定时器
来源：http://rix.chenlongwang.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nia.pengpengdd.cyou

[U104] JS：防抖
来源：http://xii.fzhhl.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hzn.xingfuxueyuan.xyz

[U105] JS：节流
来源：http://csd.hcnkem.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lms.zdqjudy.top

[U106] JS：日期格式化
来源：http://vjf.hcnkem.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fqk.daria6918.cn

[U107] JS：数字千分位
来源：http://sqv.shangyingyoupin.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ebq.birdmap.top

[U108] JS：随机整数
来源：http://mwp.shuidangran.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://all.wangdashe.top

[U109] JS：数组分组
来源：http://swj.hammf.cn

Object.groupBy(arr, x => x.type)
来源：http://anw.zdqjudy.top

[U110] JS：数组分块
来源：http://udi.shuidangran.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hqk.bbcook.cn

[U111] JS：对象转 Map
来源：http://jwd.meibo888.top

new Map(Object.entries(obj))
来源：http://txm.cheryme.top

[U112] JS：字符串补位
来源：http://glh.yfazqb.com

"7".padStart(3, "0")
来源：http://zij.aizwys.cn

[U113] JS：正则替换全部
来源：http://auo.jyoumei.cn

s.replaceAll("a", "b")
来源：http://hic.shangyingyoupin.top

[U114] JS：JSON 深比较
来源：http://jgt.dianchejie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ggo.nanxuanxn.top

[U115] JS：生成 UUID
来源：http://mnu.jianghu66.top

crypto.randomUUID()
来源：http://ang.hcnkem.com

[U116] JS：类型检查（JSDoc）
来源：http://uwz.chenzaomai.com

/** @param {string} name */ function f(name) {}
来源：http://oom.yj202588.top

[U117] JS：单元测试
来源：http://ypg.svipenyu.cn

npm i -D vitest;  npx vitest
来源：http://vnh.meibo888.top

[U118] JS：开发服务器
来源：http://dqg.sysykeji.top

npm i -D vite;  npx vite
来源：http://uli.yfazqb.com

[U119] JS：生产构建
来源：http://nqp.ywan-chungtsiang.top

npx vite build
来源：http://xhk.nwbrower.top

[U120] JS：读取环境变量（Vite）
来源：http://odr.chenjidiqi.icu

import.meta.env.VITE_API_URL
来源：http://mst.jqgufenzy.top

================================================================================
来源：http://vof.xinyue.icu

统计汇总
来源：http://fgv.tian-w.cn

================================================================================
来源：http://rzl.sweek.top

按语言统计（条）：
来源：http://dqn.shanyushiyangkeji.top

Python ......... 252
来源：http://hyh.ywan-chungtsiang.top

PHP ............ 252
来源：http://lgc.gogol.net.cn

JavaScript ..... 252
来源：http://yms.pengpengdd.cyou

TypeScript ..... 212
来源：http://xag.pycfn.com

Java ........... 212
来源：http://jwi.zhoulong.xyz

Go ............. 212
来源：http://xgk.nwbrower.top

Ruby ........... 212
来源：http://pye.wangdashe.top

C# ............. 212
来源：http://mrh.cashguo.top

C .............. 30
来源：http://edu.dianchejie.cn

C++ ............ 30
来源：http://mdw.haohaochexian.top

SQL ............ 90
来源：http://tiq.pengpengdd.cyou

Bash ........... 80
来源：http://wln.chenzaomai.com

Kotlin ......... 15
来源：http://wkt.zhaomingkeji.xyz

Swift .......... 15
来源：http://lkg.sweek.top

Lua ............ 10
来源：http://agx.vehdjk.com

Perl ........... 10
来源：http://qja.tian-w.cn

Scala .......... 10
来源：http://ywp.xinyue.icu

------------------------------------
来源：http://vni.haohaochexian.top

合计 ........... 2106 条
来源：http://xrq.cashguo.top

按章节统计：
来源：http://qxx.jlsjyb.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ejq.hesvh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://els.xuetiantiany.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://azb.gaohongyu789.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lap.zhengqikj.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hfx.zhiwuduotai.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ixo.shanyushiyangtech.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ura.hywenlv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://drg.jlsjyb.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kaf.yj20258.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dde.jqgufenzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hkf.zhixingplan.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ybv.bjfxy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rsw.jyoumei.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ogk.xylfe.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tdp.snrcjt.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gbj.hongshengwenyu.top

Q SQL 专题                              90
来源：http://evu.xuanzx.com

R Bash 专题                             80
来源：http://lva.xinyue.icu

S C / C++ 专题                          60
来源：http://voz.havefunace.top

T 其他语言补充                          60
来源：http://fys.daria6918.cn

U 高频实用片段                         120
来源：http://tvd.wangshuangyany.cn

------------------------------------
来源：http://ipv.zhongyouzk.top

合计                                  2106 条
来源：http://xif.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://lds.kuanghao11.cn

使用提醒
来源：http://squ.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://xyv.zhengqikj.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ehb.chenzaomai.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hhi.smart0.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xot.zhongyouzk.top

在旧版本上使用前请先确认语法支持情况。
来源：http://czo.cheryme.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wdk.yfazqb.com

—— 文件结束 ——
来源：http://vlf.guannengcc.top

================================================================================
来源：http://meg.epnwcf.com

程序语言常见例子速查手册（2024 版）
来源：http://rnt.svipenyu.cn

Common Programming Examples Cheat Book
来源：http://bqg.jlsjyb.cn

================================================================================
来源：http://trm.jlsjyb.cn

【收录内容】
来源：http://kee.jinghuilouyu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gtm.ehwqpu.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ddh.andypj.xyz

SQL · Bash · C · C++
来源：http://pgn.yj20258888.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hnw.shzxlz.cn

【使用说明】
来源：http://hwc.gogol.net.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qby.yonumen.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://veu.gogol.net.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gsx.gaohongyu789.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pey.yanxiufei.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://mrb.hywenlv.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://spp.sufxvd.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tui.yj20258888.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ner.cashguo.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jqi.yonumen.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mtj.dashuyun.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mtd.hywenlv.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bnu.jlsjyb.cn

【文件统计】
来源：http://gwq.ydzc1.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bpi.zycfv.cn

--------------------------------------------------------------------------------
来源：http://agv.hongshengwenyu.top

目  录
来源：http://yns.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://gyu.tian-w.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jwh.iojbl.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mol.snrcjt.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yko.jinqigfzy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uey.zhongyouzk.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lju.jqgufenzy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kuz.tianlin.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rhu.shuidangran.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dgp.jinqigufen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://prv.chenzaomai.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ufs.quarkkingdee.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pfb.ybcxt.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://plf.xuetiantiany.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rbj.yvedp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vpm.dashuyun.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dxs.fktsv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mut.sufxvd.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mbt.chenlongwang.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://spg.yvedp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dhk.ybcxt.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hlu.yj20258.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tem.yongpay.top

================================================================================
来源：http://xme.shanyushiyangkeji.top

A. 基础语法与类型
来源：http://bnx.gaohongyu789.top

================================================================================
来源：http://tvn.iojbl.cn

[A01] Hello World
来源：http://sys.xuetiantiany.cn

Py:   print("Hello, World!")
来源：http://kub.jinqigfzy.top

PHP:  echo "Hello, World!";
来源：http://gqw.guowangkeji.top

JS:   console.log("Hello, World!");
来源：http://qml.xuetiantiany.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://chu.ybcxt.top


<!-- 参考信息 -->