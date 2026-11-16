代发 wailian999

[U27] Py：异步 HTTP
来源：http://ukk.c1oappe.top

aiohttp.ClientSession() 配合 async with
来源：http://lvo.fehbvm.com

[U28] Py：类型别名
来源：http://ubj.chenjidiqi.icu

UserId = int
来源：http://cxw.hammf.cn

[U29] Py：属性校验
来源：http://kur.ydzc1.top

@property 与 @x.setter 配合
来源：http://cyx.jinyuanbaomall.cn

[U30] Py：数据类
来源：http://oaz.ydjk.org.cn

@dataclass(slots=True)
来源：http://emh.smart0.xyz

[U31] Py：单测
来源：http://ias.cashguo.top

python -m pytest -q
来源：http://gii.hongshengwenyu.top

[U32] Py：代码格式化
来源：http://oyr.jlsjyb.cn

ruff format . && ruff check --fix .
来源：http://wto.vqdsnc.cn

[U33] Py：打包发布
来源：http://oxu.cucudq.cn

python -m build  （依赖 pyproject.toml）
来源：http://erb.shuidangran.top

[U34] Py：判断编码
来源：http://ped.jinqigfzy.top

chardet.detect(raw)
来源：http://lxj.zhengqikj.top

[U35] Py：发送邮件
来源：http://zzr.fanxiaobao.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rgx.cheryme.top

[U36] Py：定时任务
来源：http://pbo.hywenlv.cn

schedule.every(10).minutes.do(job)
来源：http://rqn.shzxlz.cn

[U37] Py：读写 Excel
来源：http://yrp.wangdashe.top

pandas.read_excel / DataFrame.to_excel
来源：http://goc.kuanghao11.cn

[U38] Py：获取脚本所在目录
来源：http://ncv.vehdjk.com

Path(__file__).resolve().parent
来源：http://cyf.xinyue.icu

[U39] Py：判断是否在交互环境
来源：http://qdr.chenjidiqi.icu

sys.stdout.isatty()
来源：http://jus.tianlin.xyz

[U40] Py：打印到标准错误
来源：http://hpg.epnwcf.com

print("err", file=sys.stderr)
来源：http://qef.shuidangran.top

[U41] PHP：初始化 Composer 项目
来源：http://kxn.yangfankeji.com

composer init;  composer require guzzlehttp/guzzle
来源：http://kmu.cqqwz.cn

[U42] PHP：PSR-4 自动加载
来源：http://fwh.hnxiangtu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zjh.yuxming.cn

[U43] PHP：声明命名空间
来源：http://zrp.zhongyouzk.top

namespace App\Http;
来源：http://qvu.yfazqb.com

[U44] PHP：开启严格类型
来源：http://rss.nanxinkj.top

declare(strict_types=1);
来源：http://bpz.aibaodan.cn

[U45] PHP：类型声明与返回类型
来源：http://cru.jinyuanbaomall.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wmk.aizwys.cn

[U46] PHP：可空类型
来源：http://pdp.316326.xyz

?string $name = null
来源：http://hyo.fehbvm.com

[U47] PHP：联合类型
来源：http://bwe.jlsjyb.cn

int|string $id
来源：http://wzn.sjlbkw.cn

[U48] PHP：纯枚举
来源：http://alg.zhixingplan.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://faq.cucudq.cn

[U49] PHP：只读属性
来源：http://zjx.dashuyun.cn

public readonly string $name
来源：http://zyi.vehdjk.com

[U50] PHP：构造器属性提升
来源：http://dpb.316326.xyz

public function __construct(private int $id) {}
来源：http://umo.snrcjt.cn

[U51] PHP：数组解构
来源：http://czm.fktsv.cn

[$a, $b] = $arr;
来源：http://trc.ywan-chungtsiang.top

[U52] PHP：箭头函数
来源：http://tdr.mhx1999.top

$double = fn($x) => $x * 2;
来源：http://fas.jlsjyb.cn

[U53] PHP：空合并运算符
来源：http://qtn.andypj.xyz

$v = $a ?? $b ?? "default";
来源：http://xke.chenlongwang.top

[U54] PHP：空安全调用
来源：http://uzn.smart0.xyz

$obj?->method()
来源：http://rfb.feifeiyinyue.top

[U55] PHP：match 表达式
来源：http://wig.aibaodan.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rzi.cheryme.top

[U56] PHP：命名参数
来源：http://trf.feifeiyinyue.top

f(a: 1, b: 2)
来源：http://rtr.guowangkeji.top

[U57] PHP：字符串插值
来源：http://uhp.hywenlv.cn

"值: {$a}"
来源：http://ihu.jlsjyb.cn

[U58] PHP：数组三件套
来源：http://ifz.jianghu66.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mdc.yanxiufei.cn

[U59] PHP：自定义排序
来源：http://hht.ywan-chungtsiang.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vby.chenlongwang.top

[U60] PHP：JSON 编解码
来源：http://wby.feifeiyinyue.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oii.daria6918.cn

[U61] PHP：正则
来源：http://bph.haohaochexian.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uqg.jinqigufen.top

[U62] PHP：日期对象
来源：http://lad.cdnleiting.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://geg.aibaodan.cn

[U63] PHP：文件读写
来源：http://nom.dianchejie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kxq.gzhubu.top

[U64] PHP：目录遍历
来源：http://xjb.hysaishi.cn

glob("dir/*.php");  scandir("dir");
来源：http://idf.fktsv.cn

[U65] PHP：会话
来源：http://kyj.epnwcf.com

session_start();  $_SESSION["uid"] = 1;
来源：http://ozn.dianchejie.cn

[U66] PHP：设置 Cookie
来源：http://yiu.nanxinkj.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rbe.wangshuangyany.cn

[U67] PHP：处理文件上传
来源：http://ecb.yj20258.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ywy.yfazqb.com

[U68] PHP：PDO 连接
来源：http://ysv.zhongyouzk.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mki.guannengcc.top

[U69] PHP：PDO 预处理
来源：http://fbo.zhaomingkeji.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sqy.meibo888.top

[U70] PHP：PDO 事务
来源：http://wmt.bbcook.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fjb.sweek.top

[U71] PHP：抛出异常
来源：http://efv.ctjpmb.com

throw new RuntimeException("失败", 500);
来源：http://qpl.yueranfly.top

[U72] PHP：写错误日志
来源：http://obz.ppjwa.cn

error_log("失败: " . $e->getMessage());
来源：http://qaw.dashuyun.cn

[U73] PHP：读取 ini 配置
来源：http://vwz.nanxinkj.top

parse_ini_file("config.ini", true)
来源：http://vgj.sweek.top

[U74] PHP：读取环境变量
来源：http://qhz.chenlongwang.top

getenv("APP_ENV") ?: "production"
来源：http://afx.316326.xyz

[U75] PHP：依赖注入
来源：http://wgf.nanxuanxn.top

composer require psr/container
来源：http://zqs.gzhubu.top

[U76] PHP：简单路由
来源：http://huk.yonumen.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yyi.chenjidiqi.icu

[U77] PHP：模板渲染
来源：http://gnv.chenlongwang.top

composer require twig/twig
来源：http://thw.zhongyouzk.top

[U78] PHP：单元测试
来源：http://apb.ybcxt.top

composer require --dev phpunit/phpunit
来源：http://mjc.shuidangran.top

[U79] PHP：静态分析
来源：http://ydd.cucudq.cn

composer require --dev phpstan/phpstan
来源：http://yjm.bbcook.cn

[U80] PHP：代码规范修复
来源：http://mzu.ydjk.org.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ycl.svipenyu.cn

[U81] JS：初始化项目
来源：http://wkx.vehdjk.com

npm init -y;  npm i express
来源：http://rfp.jinyuanbaomall.cn

[U82] JS：package.json 脚本
来源：http://jzm.redwolf501.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xvg.gotoacloud.top

[U83] JS：ES Module 导入导出
来源：http://lqc.jqgfzy.top

export const a = 1;  import { a } from "./m.js";
来源：http://hqi.yongpay.top

[U84] JS：CommonJS 写法
来源：http://krg.feifeiyinyue.top

module.exports = { a };  const { a } = require("./m");
来源：http://suf.nwbrower.top

[U85] JS：可选链
来源：http://tad.yfazqb.com

a?.b?.c
来源：http://gtk.zhiwuduotai.top

[U86] JS：空值合并
来源：http://uqu.yj20258.top

a ?? b
来源：http://ova.bbcook.cn

[U87] JS：解构默认值
来源：http://jxg.xinyue.icu

const { a = 1, b = 2 } = obj;
来源：http://ije.uphjek.com

[U88] JS：对象展开合并
来源：http://fnv.shanyushiyangkeji.top

{ ...a, ...b }
来源：http://noy.smart0.xyz

[U89] JS：数组去重
来源：http://lee.hongshengwenyu.top

[...new Set(arr)]
来源：http://qrr.nanxinkj.top

[U90] JS：数字数组排序
来源：http://fzx.zhiwuduotai.top

[...arr].sort((a, b) => a - b)
来源：http://urr.havefunace.top

[U91] JS：对象键值遍历
来源：http://keg.jlsjyb.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rmq.shangyingyoupin.top

[U92] JS：深拷贝
来源：http://urc.nanxinkj.top

structuredClone(obj)
来源：http://nqd.hnqzz.top

[U93] JS：模板字符串
来源：http://auf.fktsv.cn

`共 ${n} 条`
来源：http://rnv.chenzaomai.com

[U94] JS：箭头函数
来源：http://gfx.zhixingplan.top

const double = x => x * 2;
来源：http://ryn.epnwcf.com

[U95] JS：Promise 包装
来源：http://djs.hysaishi.cn

new Promise((resolve, reject) => {})
来源：http://gch.ydzc1.top

[U96] JS：async/await 与异常
来源：http://jsx.nanxuanxn.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://aop.fengsongda.top

[U97] JS：并发请求
来源：http://cym.tian-w.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://odf.zycfv.cn

[U98] JS：fetch 带 JSON
来源：http://kcp.jinyuanbaomall.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://teb.shanyushiyangtech.top

[U99] JS：事件监听
来源：http://loj.fanxiaobao.xyz

el.addEventListener("click", e => {})
来源：http://axu.sxryk.cn

[U100] JS：DOM 查询
来源：http://efp.yuanzhike.top

document.querySelector(".item")
来源：http://hxz.hammf.cn

[U101] JS：classList 操作
来源：http://jtq.tianlin.xyz

el.classList.toggle("active")
来源：http://qzu.zhongyouzk.top

[U102] JS：本地存储
来源：http://neh.aizwys.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://alk.9152youxi.cn

[U103] JS：定时器
来源：http://qjt.pengpengdd.cyou

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gho.xziqi.cn

[U104] JS：防抖
来源：http://cxa.shanyushiyangtech.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tcw.uphjek.com

[U105] JS：节流
来源：http://cpv.xylfe.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dto.cashguo.top

[U106] JS：日期格式化
来源：http://enb.redwolf501.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qex.hywenlv.cn

[U107] JS：数字千分位
来源：http://glj.shanyushiyangtech.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vui.0kj1m.cn

[U108] JS：随机整数
来源：http://udx.jinyuanbaomall.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ing.jianghu66.top

[U109] JS：数组分组
来源：http://uxo.guowangkeji.top

Object.groupBy(arr, x => x.type)
来源：http://wgz.xingfuxueyuan.xyz

[U110] JS：数组分块
来源：http://gei.xinyue.icu

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://slc.zhixingplan.top

[U111] JS：对象转 Map
来源：http://jwo.hnqzz.top

new Map(Object.entries(obj))
来源：http://upx.xingfuxueyuan.xyz

[U112] JS：字符串补位
来源：http://psg.yangfankeji.com

"7".padStart(3, "0")
来源：http://icr.birdmap.top

[U113] JS：正则替换全部
来源：http://lju.bbcook.cn

s.replaceAll("a", "b")
来源：http://rmw.zhiwuduotai.top

[U114] JS：JSON 深比较
来源：http://hqi.cdnleiting.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ccn.fzhhl.top

[U115] JS：生成 UUID
来源：http://ugi.shuidangran.top

crypto.randomUUID()
来源：http://fhd.yvedp.cn

[U116] JS：类型检查（JSDoc）
来源：http://qff.daxiang520.top

/** @param {string} name */ function f(name) {}
来源：http://txj.ppjwa.cn

[U117] JS：单元测试
来源：http://egx.cheryme.top

npm i -D vitest;  npx vitest
来源：http://avs.tanke756.top

[U118] JS：开发服务器
来源：http://zns.vqdsnc.cn

npm i -D vite;  npx vite
来源：http://zic.zdqjudy.top

[U119] JS：生产构建
来源：http://ntf.fehbvm.com

npx vite build
来源：http://gov.cdnleiting.top

[U120] JS：读取环境变量（Vite）
来源：http://osx.yfazqb.com

import.meta.env.VITE_API_URL
来源：http://yza.pycfn.com

================================================================================
来源：http://fjw.yuanzhike.top

统计汇总
来源：http://ign.gaohongyu789.top

================================================================================
来源：http://kri.cucudq.cn

按语言统计（条）：
来源：http://iku.zhengqikj.top

Python ......... 252
来源：http://euv.uphjek.com

PHP ............ 252
来源：http://swr.zhaomingkeji.xyz

JavaScript ..... 252
来源：http://slp.nwbrower.top

TypeScript ..... 212
来源：http://sbl.yvedp.cn

Java ........... 212
来源：http://cob.hfpthk.cn

Go ............. 212
来源：http://xsd.gaohongyu789.top

Ruby ........... 212
来源：http://ftd.tian-w.cn

C# ............. 212
来源：http://wdt.yj202588.top

C .............. 30
来源：http://ggg.smart0.xyz

C++ ............ 30
来源：http://mly.zhengqikj.top

SQL ............ 90
来源：http://pne.chenjidiqi.icu

Bash ........... 80
来源：http://ksi.chenjidiqi.icu

Kotlin ......... 15
来源：http://swt.haohaochexian.top

Swift .......... 15
来源：http://vap.cashguo.top

Lua ............ 10
来源：http://chb.vqdsnc.cn

Perl ........... 10
来源：http://esq.wangdashe.top

Scala .......... 10
来源：http://pht.zhijiandao.cn

------------------------------------
来源：http://bqf.aibaodan.cn

合计 ........... 2106 条
来源：http://oat.bjfxy.top

按章节统计：
来源：http://nyn.yj20258.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://exp.cashguo.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lcu.pengpengdd.cyou

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oae.daria6918.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ibe.redwolf501.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xol.vqdsnc.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yqn.yj202588.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ztq.shangyingyoupin.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://czu.zhixingplan.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vsn.52xcode.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://eli.chenjidiqi.icu

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wvi.gaohongyu789.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qfg.quarkkingdee.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xdu.jinqigfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rvn.iojbl.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sde.vqdsnc.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ehz.jinyuanbaomall.cn

Q SQL 专题                              90
来源：http://oui.xuetiantiany.cn

R Bash 专题                             80
来源：http://map.hnqzz.top

S C / C++ 专题                          60
来源：http://dub.yj202588.top

T 其他语言补充                          60
来源：http://aim.sxryk.cn

U 高频实用片段                         120
来源：http://hec.smart0.xyz

------------------------------------
来源：http://sib.sysykeji.top

合计                                  2106 条
来源：http://jhb.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://ixs.feifeiyinyue.top

使用提醒
来源：http://wpk.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://ljq.svipenyu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cym.zhixingplan.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zyg.zdbjq.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fug.tianlin.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://qsy.havefunace.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://era.hongshengwenyu.top

—— 文件结束 ——
来源：http://ycs.ppjwa.cn

================================================================================
来源：http://qar.tian-w.cn

程序语言常见例子速查手册（2024 版）
来源：http://dds.yonumen.top

Common Programming Examples Cheat Book
来源：http://xyx.shanyushiyangtech.top

================================================================================
来源：http://xtk.sxryk.cn

【收录内容】
来源：http://fsz.yuanzhike.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://xmx.bjfxy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zmr.dashuyun.cn

SQL · Bash · C · C++
来源：http://uve.chenzaomai.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fye.xuetiantiany.cn

【使用说明】
来源：http://doq.gaohongyu789.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wcz.cashguo.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://emc.hywenlv.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pdv.hfpthk.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jtl.cdnleiting.top

Bash:  Shell         C:     C             C++:   C++
来源：http://rlz.fktsv.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mju.sweek.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xum.xuanzx.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://iif.yfazqb.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qdt.snrcjt.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ady.hesvh.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eev.xuanzx.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jkh.c1oappe.top

【文件统计】
来源：http://ibi.0kj1m.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xwy.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://cuk.nanxuanxn.top

目  录
来源：http://qcc.c1oappe.top

--------------------------------------------------------------------------------
来源：http://ple.fktsv.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vfh.bjfxy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lev.vehdjk.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zsv.xuetiantiany.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nsa.yongpay.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sua.shuidangran.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zae.zycfv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vrm.yfazqb.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nfq.316326.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yvk.iojbl.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pjn.jinyuanbaomall.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gls.fengsongda.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mso.zdqjudy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://llx.zhaomingkeji.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fuk.fehbvm.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cxp.havefunace.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ocv.aizwys.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qzo.cucudq.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gur.zhijiandao.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baa.0kj1m.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://los.jianghu66.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lhq.hammf.cn

================================================================================
来源：http://yba.jinghuilouyu.cn

A. 基础语法与类型
来源：http://sjo.tarul.cn

================================================================================
来源：http://jhv.yvedp.cn

[A01] Hello World
来源：http://tgc.zycfv.cn

Py:   print("Hello, World!")
来源：http://wli.birdmap.top

PHP:  echo "Hello, World!";
来源：http://vpk.quarkkingdee.top

JS:   console.log("Hello, World!");
来源：http://ufi.chenlongwang.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zgz.jqgufenzy.top


<!-- 参考信息 -->