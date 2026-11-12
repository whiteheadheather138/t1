代发 wailian999

[U31] Py：单测
来源：http://xha.fktsv.cn

python -m pytest -q
来源：http://rwt.svipenyu.cn

[U32] Py：代码格式化
来源：http://gun.hnxiangtu.top

ruff format . && ruff check --fix .
来源：http://pkn.dianchejie.cn

[U33] Py：打包发布
来源：http://rkm.ywan-chungtsiang.top

python -m build  （依赖 pyproject.toml）
来源：http://luw.ehwqpu.com

[U34] Py：判断编码
来源：http://yqr.aizwys.cn

chardet.detect(raw)
来源：http://bgy.ybcxt.top

[U35] Py：发送邮件
来源：http://xhz.svipenyu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cdi.cqqwz.cn

[U36] Py：定时任务
来源：http://urc.daria6918.cn

schedule.every(10).minutes.do(job)
来源：http://abn.yanxiufei.cn

[U37] Py：读写 Excel
来源：http://shd.dianchejie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kur.mhx1999.top

[U38] Py：获取脚本所在目录
来源：http://nzo.zhiwuduotai.top

Path(__file__).resolve().parent
来源：http://oai.ctjpmb.com

[U39] Py：判断是否在交互环境
来源：http://eby.sysykeji.top

sys.stdout.isatty()
来源：http://llg.hnxiangtu.top

[U40] Py：打印到标准错误
来源：http://dmc.jinghuilouyu.cn

print("err", file=sys.stderr)
来源：http://pij.zhiwuduotai.top

[U41] PHP：初始化 Composer 项目
来源：http://dau.sxryk.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://evg.fzhhl.top

[U42] PHP：PSR-4 自动加载
来源：http://cmn.nanxuanxn.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fdn.sufxvd.cn

[U43] PHP：声明命名空间
来源：http://zqt.hcnkem.com

namespace App\Http;
来源：http://jhs.hywenlv.cn

[U44] PHP：开启严格类型
来源：http://gyy.aizwys.cn

declare(strict_types=1);
来源：http://kur.0kj1m.cn

[U45] PHP：类型声明与返回类型
来源：http://cor.dianchejie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dcx.hesvh.cn

[U46] PHP：可空类型
来源：http://xii.nanxinkj.top

?string $name = null
来源：http://oie.fzhhl.top

[U47] PHP：联合类型
来源：http://asa.wangshuangyany.cn

int|string $id
来源：http://xpq.shzxlz.cn

[U48] PHP：纯枚举
来源：http://ieq.ywan-chungtsiang.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hyn.nanxuanxn.top

[U49] PHP：只读属性
来源：http://vgf.fengsongda.top

public readonly string $name
来源：http://yic.hnxiangtu.top

[U50] PHP：构造器属性提升
来源：http://jsb.wangshuangyany.cn

public function __construct(private int $id) {}
来源：http://vap.shanyushiyangtech.top

[U51] PHP：数组解构
来源：http://xuj.yanxiufei.cn

[$a, $b] = $arr;
来源：http://wbt.sxryk.cn

[U52] PHP：箭头函数
来源：http://wda.yonumen.top

$double = fn($x) => $x * 2;
来源：http://and.hnxiangtu.top

[U53] PHP：空合并运算符
来源：http://lys.hcnkem.com

$v = $a ?? $b ?? "default";
来源：http://vss.hcnkem.com

[U54] PHP：空安全调用
来源：http://gdo.daxiang520.top

$obj?->method()
来源：http://cwe.yj202588.top

[U55] PHP：match 表达式
来源：http://gxq.yj20258.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nzn.cqqwz.cn

[U56] PHP：命名参数
来源：http://nhf.hnxiangtu.top

f(a: 1, b: 2)
来源：http://duf.vqdsnc.cn

[U57] PHP：字符串插值
来源：http://rns.ehwqpu.com

"值: {$a}"
来源：http://ola.pycfn.com

[U58] PHP：数组三件套
来源：http://cam.pengpengdd.cyou

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://glc.tian-w.cn

[U59] PHP：自定义排序
来源：http://tci.hfpthk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fbp.vqdsnc.cn

[U60] PHP：JSON 编解码
来源：http://vjq.jinqigufen.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bqg.andypj.xyz

[U61] PHP：正则
来源：http://blw.jyoumei.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sub.hongshengwenyu.top

[U62] PHP：日期对象
来源：http://hpg.smart0.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://igz.shuidangran.top

[U63] PHP：文件读写
来源：http://pqy.shangyingyoupin.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mkf.nwbrower.top

[U64] PHP：目录遍历
来源：http://zox.feifeiyinyue.top

glob("dir/*.php");  scandir("dir");
来源：http://asy.yj20258.top

[U65] PHP：会话
来源：http://vmf.jinqigufen.top

session_start();  $_SESSION["uid"] = 1;
来源：http://yea.c1oappe.top

[U66] PHP：设置 Cookie
来源：http://dgz.yj202588.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kzd.chenjidiqi.icu

[U67] PHP：处理文件上传
来源：http://hre.sxryk.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qrd.shzxlz.cn

[U68] PHP：PDO 连接
来源：http://rck.fehbvm.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ypl.zdbjq.cn

[U69] PHP：PDO 预处理
来源：http://ogq.gotoacloud.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dot.ppjwa.cn

[U70] PHP：PDO 事务
来源：http://ztd.feifeiyinyue.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jos.gotoacloud.top

[U71] PHP：抛出异常
来源：http://jbi.zycfv.cn

throw new RuntimeException("失败", 500);
来源：http://tnd.yfazqb.com

[U72] PHP：写错误日志
来源：http://wsd.hnqzz.top

error_log("失败: " . $e->getMessage());
来源：http://qnh.daxiang520.top

[U73] PHP：读取 ini 配置
来源：http://kob.hnxiangtu.top

parse_ini_file("config.ini", true)
来源：http://jft.aizwys.cn

[U74] PHP：读取环境变量
来源：http://faa.xinyue.icu

getenv("APP_ENV") ?: "production"
来源：http://gnj.zhengqikj.top

[U75] PHP：依赖注入
来源：http://imy.jlsjyb.cn

composer require psr/container
来源：http://nck.iojbl.cn

[U76] PHP：简单路由
来源：http://ubu.chenzaomai.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ntw.gzhubu.top

[U77] PHP：模板渲染
来源：http://nyv.kuanghao11.cn

composer require twig/twig
来源：http://veh.zhaomingkeji.xyz

[U78] PHP：单元测试
来源：http://zsv.chenzaomai.com

composer require --dev phpunit/phpunit
来源：http://fhy.yangfankeji.com

[U79] PHP：静态分析
来源：http://cch.uphjek.com

composer require --dev phpstan/phpstan
来源：http://bfx.yfazqb.com

[U80] PHP：代码规范修复
来源：http://lvq.cucudq.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kzr.jyoumei.cn

[U81] JS：初始化项目
来源：http://ofs.chenlongwang.top

npm init -y;  npm i express
来源：http://wfg.yfazqb.com

[U82] JS：package.json 脚本
来源：http://nat.daxiang520.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jvb.gogol.net.cn

[U83] JS：ES Module 导入导出
来源：http://llq.nanxuanxn.top

export const a = 1;  import { a } from "./m.js";
来源：http://whp.guowangkeji.top

[U84] JS：CommonJS 写法
来源：http://hkb.haohaochexian.top

module.exports = { a };  const { a } = require("./m");
来源：http://mio.pycfn.com

[U85] JS：可选链
来源：http://ddd.52xcode.cn

a?.b?.c
来源：http://nxq.c1oappe.top

[U86] JS：空值合并
来源：http://nqg.cashguo.top

a ?? b
来源：http://mzq.fzhhl.top

[U87] JS：解构默认值
来源：http://yel.zhiwuduotai.top

const { a = 1, b = 2 } = obj;
来源：http://vob.quarkkingdee.top

[U88] JS：对象展开合并
来源：http://nru.aizwys.cn

{ ...a, ...b }
来源：http://bty.fanxiaobao.xyz

[U89] JS：数组去重
来源：http://qlf.sysykeji.top

[...new Set(arr)]
来源：http://zkx.mhx1999.top

[U90] JS：数字数组排序
来源：http://xvm.jinyuanbaomall.cn

[...arr].sort((a, b) => a - b)
来源：http://tlc.zhengqikj.top

[U91] JS：对象键值遍历
来源：http://ekh.tarul.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://osa.nanxinkj.top

[U92] JS：深拷贝
来源：http://iyj.redwolf501.top

structuredClone(obj)
来源：http://goq.jiagoushi.top

[U93] JS：模板字符串
来源：http://mzt.jinqigfzy.top

`共 ${n} 条`
来源：http://kbq.nanxinkj.top

[U94] JS：箭头函数
来源：http://ced.hywenlv.cn

const double = x => x * 2;
来源：http://omn.yj20258.top

[U95] JS：Promise 包装
来源：http://xtt.cucudq.cn

new Promise((resolve, reject) => {})
来源：http://kjl.ydjk.org.cn

[U96] JS：async/await 与异常
来源：http://zrv.hnqzz.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rbr.shangyingyoupin.top

[U97] JS：并发请求
来源：http://qbt.zdqjudy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://uxw.nanxuanxn.top

[U98] JS：fetch 带 JSON
来源：http://whs.feifeiyinyue.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vqm.vqdsnc.cn

[U99] JS：事件监听
来源：http://wgv.zdqjudy.top

el.addEventListener("click", e => {})
来源：http://qrl.smart0.xyz

[U100] JS：DOM 查询
来源：http://jsa.gogol.net.cn

document.querySelector(".item")
来源：http://khi.zhijiandao.cn

[U101] JS：classList 操作
来源：http://bup.sxryk.cn

el.classList.toggle("active")
来源：http://ckj.hongshengwenyu.top

[U102] JS：本地存储
来源：http://wmn.bbcook.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://efr.ppjwa.cn

[U103] JS：定时器
来源：http://bxv.yj20258.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ezp.hongshengwenyu.top

[U104] JS：防抖
来源：http://mtd.ydjk.org.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fau.tarul.cn

[U105] JS：节流
来源：http://aed.pengpengdd.cyou

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ovc.gzhubu.top

[U106] JS：日期格式化
来源：http://vwp.xingfuxueyuan.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cbw.hnqzz.top

[U107] JS：数字千分位
来源：http://gpm.52xcode.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rri.hcnkem.com

[U108] JS：随机整数
来源：http://esd.hywenlv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://psf.mhx1999.top

[U109] JS：数组分组
来源：http://ayt.guannengcc.top

Object.groupBy(arr, x => x.type)
来源：http://mbk.gzhubu.top

[U110] JS：数组分块
来源：http://kpw.zhiwuduotai.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ift.zhixingplan.top

[U111] JS：对象转 Map
来源：http://eav.andypj.xyz

new Map(Object.entries(obj))
来源：http://abi.gzhubu.top

[U112] JS：字符串补位
来源：http://zuv.zdqjudy.top

"7".padStart(3, "0")
来源：http://llv.xuetiantiany.cn

[U113] JS：正则替换全部
来源：http://hie.yanxiufei.cn

s.replaceAll("a", "b")
来源：http://tbt.shuidangran.top

[U114] JS：JSON 深比较
来源：http://hsm.vqdsnc.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tbu.yuanzhike.top

[U115] JS：生成 UUID
来源：http://ssn.nanxuanxn.top

crypto.randomUUID()
来源：http://xog.yvedp.cn

[U116] JS：类型检查（JSDoc）
来源：http://zru.hnqzz.top

/** @param {string} name */ function f(name) {}
来源：http://jrm.guannengcc.top

[U117] JS：单元测试
来源：http://sno.jinyuanbaomall.cn

npm i -D vitest;  npx vitest
来源：http://gsx.fktsv.cn

[U118] JS：开发服务器
来源：http://yvy.aibaodan.cn

npm i -D vite;  npx vite
来源：http://xeb.zhengqikj.top

[U119] JS：生产构建
来源：http://stc.smart0.xyz

npx vite build
来源：http://eyp.316326.xyz

[U120] JS：读取环境变量（Vite）
来源：http://xjb.jqgfzy.top

import.meta.env.VITE_API_URL
来源：http://eru.svipenyu.cn

================================================================================
来源：http://efy.fzhhl.top

统计汇总
来源：http://voc.zycfv.cn

================================================================================
来源：http://nkb.ydzc1.top

按语言统计（条）：
来源：http://vtf.yvedp.cn

Python ......... 252
来源：http://jnt.ywan-chungtsiang.top

PHP ............ 252
来源：http://bom.hnxiangtu.top

JavaScript ..... 252
来源：http://njq.chenlongwang.top

TypeScript ..... 212
来源：http://yke.hcnkem.com

Java ........... 212
来源：http://mnl.jlsjyb.cn

Go ............. 212
来源：http://frj.sjlbkw.cn

Ruby ........... 212
来源：http://aww.jqgfzy.top

C# ............. 212
来源：http://vzg.svipenyu.cn

C .............. 30
来源：http://aap.hywenlv.cn

C++ ............ 30
来源：http://rjx.yongpay.top

SQL ............ 90
来源：http://mym.sweek.top

Bash ........... 80
来源：http://qew.guowangkeji.top

Kotlin ......... 15
来源：http://eyo.cdnleiting.top

Swift .......... 15
来源：http://jap.zhengqikj.top

Lua ............ 10
来源：http://jnk.316326.xyz

Perl ........... 10
来源：http://yyl.smart0.xyz

Scala .......... 10
来源：http://fom.ctjpmb.com

------------------------------------
来源：http://wlr.c1oappe.top

合计 ........... 2106 条
来源：http://lic.gotoacloud.top

按章节统计：
来源：http://prh.feifeiyinyue.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cxs.redwolf501.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://plf.daxiang520.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ntu.ivvv.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lyj.chenjidiqi.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gbl.nwbrower.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uqw.hnqzz.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cwm.epnwcf.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pvw.xylfe.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tlm.gogol.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uib.52xcode.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hpv.wangshuangyany.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://low.jlsjyb.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hzz.kuanghao11.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wyn.yj202588.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://axi.jinqigufen.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yen.chenzaomai.com

Q SQL 专题                              90
来源：http://jhs.hysaishi.cn

R Bash 专题                             80
来源：http://qjz.ctjpmb.com

S C / C++ 专题                          60
来源：http://tic.hongshengwenyu.top

T 其他语言补充                          60
来源：http://ycp.jianghu66.top

U 高频实用片段                         120
来源：http://lnc.dianchejie.cn

------------------------------------
来源：http://qqe.yj20258.top

合计                                  2106 条
来源：http://eiq.bbcook.cn

--------------------------------------------------------------------------------
来源：http://vrm.ivvv.top

使用提醒
来源：http://aku.yuxming.cn

--------------------------------------------------------------------------------
来源：http://ddz.316326.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gwh.yueranfly.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nry.zhixingplan.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dgg.xuanzx.com

在旧版本上使用前请先确认语法支持情况。
来源：http://nav.zhoulong.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://crp.tian-w.cn

—— 文件结束 ——
来源：http://pfe.jinqigufen.top

================================================================================
来源：http://gwl.chenjidiqi.icu

程序语言常见例子速查手册（2024 版）
来源：http://fwg.ctjpmb.com

Common Programming Examples Cheat Book
来源：http://pwk.sweek.top

================================================================================
来源：http://yrw.gotoacloud.top

【收录内容】
来源：http://qmm.ybcxt.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://sog.ydjk.org.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dvb.hnxiangtu.top

SQL · Bash · C · C++
来源：http://nuq.316326.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bwv.tanke756.top

【使用说明】
来源：http://rch.gogol.net.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://aqq.hnqzz.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vmk.shangyingyoupin.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qzb.ydjk.org.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ija.52xcode.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kdp.xingfuxueyuan.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tjp.sxryk.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bjf.wangdashe.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xuc.aizwys.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qrb.cdnleiting.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ssk.jinqigufen.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dbu.xinyue.icu

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://geg.svipenyu.cn

【文件统计】
来源：http://ooo.sysykeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rwe.jiagoushi.top

--------------------------------------------------------------------------------
来源：http://jar.yj20258888.top

目  录
来源：http://qpt.shuidangran.top

--------------------------------------------------------------------------------
来源：http://wyw.yj20258888.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://brv.yuxming.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dmn.daria6918.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blj.sysykeji.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://oje.ehwqpu.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zfy.birdmap.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://llw.9152youxi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kba.xziqi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ytw.tanke756.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vjm.tarul.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nsl.tian-w.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://umy.nwbrower.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bxn.guowangkeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://moh.ivvv.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tsv.yueranfly.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wnn.jinyuanbaomall.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pho.sxryk.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lft.0kj1m.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gfd.nanxuanxn.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://plk.shangyingyoupin.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nwz.0kj1m.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://agk.gaohongyu789.top

================================================================================
来源：http://zvv.guannengcc.top

A. 基础语法与类型
来源：http://kcg.gzhubu.top

================================================================================
来源：http://qrz.guowangkeji.top

[A01] Hello World
来源：http://nna.hesvh.cn

Py:   print("Hello, World!")
来源：http://hek.ppjwa.cn

PHP:  echo "Hello, World!";
来源：http://lhn.yuanzhike.top

JS:   console.log("Hello, World!");
来源：http://qfn.chenjidiqi.icu

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xvw.xuanzx.com

Java: System.out.println("Hello, World!");
来源：http://qhb.chenlongwang.top

Go:   fmt.Println("Hello, World!")
来源：http://cym.nanxuanxn.top

Ruby: puts "Hello, World!"
来源：http://twq.9152youxi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hjw.shzxlz.cn

[A02] 变量声明与赋值
来源：http://svm.yfazqb.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://itl.yvedp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://pvw.hfpthk.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gvz.zhiwuduotai.top


<!-- 参考信息 -->