代发 wailian999

[U35] Py：发送邮件
来源：http://edo.epnwcf.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yrz.chenlongwang.top

[U36] Py：定时任务
来源：http://ifm.epnwcf.com

schedule.every(10).minutes.do(job)
来源：http://dib.ivvv.top

[U37] Py：读写 Excel
来源：http://lrx.jinyuanbaomall.cn

pandas.read_excel / DataFrame.to_excel
来源：http://plo.pengpengdd.cyou

[U38] Py：获取脚本所在目录
来源：http://vwf.yj20258888.top

Path(__file__).resolve().parent
来源：http://oak.snrcjt.cn

[U39] Py：判断是否在交互环境
来源：http://taa.wangdashe.top

sys.stdout.isatty()
来源：http://yya.zhixingplan.top

[U40] Py：打印到标准错误
来源：http://ovg.cheryme.top

print("err", file=sys.stderr)
来源：http://zty.yvedp.cn

[U41] PHP：初始化 Composer 项目
来源：http://yrc.guowangkeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://yyv.mhx1999.top

[U42] PHP：PSR-4 自动加载
来源：http://ldc.wangshuangyany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://whu.gogol.net.cn

[U43] PHP：声明命名空间
来源：http://gzh.quarkkingdee.top

namespace App\Http;
来源：http://gkw.haohaochexian.top

[U44] PHP：开启严格类型
来源：http://wcl.aibaodan.cn

declare(strict_types=1);
来源：http://sir.tarul.cn

[U45] PHP：类型声明与返回类型
来源：http://egs.tanke756.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://wvk.xinyue.icu

[U46] PHP：可空类型
来源：http://num.nanxinkj.top

?string $name = null
来源：http://gtb.ctjpmb.com

[U47] PHP：联合类型
来源：http://vwf.sufxvd.cn

int|string $id
来源：http://wcx.redwolf501.top

[U48] PHP：纯枚举
来源：http://nug.yueranfly.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ijd.cucudq.cn

[U49] PHP：只读属性
来源：http://szb.yj20258.top

public readonly string $name
来源：http://mcr.pengpengdd.cyou

[U50] PHP：构造器属性提升
来源：http://zbr.9152youxi.cn

public function __construct(private int $id) {}
来源：http://pto.yj20258.top

[U51] PHP：数组解构
来源：http://txx.cucudq.cn

[$a, $b] = $arr;
来源：http://ekp.dashuyun.cn

[U52] PHP：箭头函数
来源：http://pfs.hesvh.cn

$double = fn($x) => $x * 2;
来源：http://ksy.yueranfly.top

[U53] PHP：空合并运算符
来源：http://kqs.andypj.xyz

$v = $a ?? $b ?? "default";
来源：http://vef.fengsongda.top

[U54] PHP：空安全调用
来源：http://iob.fzhhl.top

$obj?->method()
来源：http://bbd.hnqzz.top

[U55] PHP：match 表达式
来源：http://igw.xuanzx.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://obc.meibo888.top

[U56] PHP：命名参数
来源：http://umk.nwbrower.top

f(a: 1, b: 2)
来源：http://lcx.tianlin.xyz

[U57] PHP：字符串插值
来源：http://nko.shanyushiyangtech.top

"值: {$a}"
来源：http://ype.ivvv.top

[U58] PHP：数组三件套
来源：http://kfj.yanxiufei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hup.ppjwa.cn

[U59] PHP：自定义排序
来源：http://eko.zhoulong.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://czc.fehbvm.com

[U60] PHP：JSON 编解码
来源：http://jtd.aibaodan.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ris.zdbjq.cn

[U61] PHP：正则
来源：http://dzg.gaohongyu789.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wze.dianchejie.cn

[U62] PHP：日期对象
来源：http://ebx.kuanghao11.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://thc.meibo888.top

[U63] PHP：文件读写
来源：http://rjd.ehwqpu.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tlj.redwolf501.top

[U64] PHP：目录遍历
来源：http://hpn.sufxvd.cn

glob("dir/*.php");  scandir("dir");
来源：http://vng.yangfankeji.com

[U65] PHP：会话
来源：http://cag.tianlin.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://wen.yuanzhike.top

[U66] PHP：设置 Cookie
来源：http://yok.cheryme.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uky.yuanzhike.top

[U67] PHP：处理文件上传
来源：http://ezd.sxryk.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blr.yonumen.top

[U68] PHP：PDO 连接
来源：http://cvv.jinqigfzy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bmk.xinyue.icu

[U69] PHP：PDO 预处理
来源：http://yfz.jiagoushi.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zpq.shanyushiyangkeji.top

[U70] PHP：PDO 事务
来源：http://yyx.epnwcf.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wvn.hnxiangtu.top

[U71] PHP：抛出异常
来源：http://oeq.chenlongwang.top

throw new RuntimeException("失败", 500);
来源：http://plf.mhx1999.top

[U72] PHP：写错误日志
来源：http://tqv.jinyuanbaomall.cn

error_log("失败: " . $e->getMessage());
来源：http://ejo.zhongyouzk.top

[U73] PHP：读取 ini 配置
来源：http://cif.ydzc1.top

parse_ini_file("config.ini", true)
来源：http://qnw.smart0.xyz

[U74] PHP：读取环境变量
来源：http://dzr.yangfankeji.com

getenv("APP_ENV") ?: "production"
来源：http://hzh.wangshuangyany.cn

[U75] PHP：依赖注入
来源：http://hev.quarkkingdee.top

composer require psr/container
来源：http://vto.zhijiandao.cn

[U76] PHP：简单路由
来源：http://hzy.hcnkem.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jdt.vehdjk.com

[U77] PHP：模板渲染
来源：http://ppi.ehwqpu.com

composer require twig/twig
来源：http://jop.zhoulong.xyz

[U78] PHP：单元测试
来源：http://aiz.quarkkingdee.top

composer require --dev phpunit/phpunit
来源：http://qcw.chenjidiqi.icu

[U79] PHP：静态分析
来源：http://qav.jiagoushi.top

composer require --dev phpstan/phpstan
来源：http://lgq.xinyue.icu

[U80] PHP：代码规范修复
来源：http://ocp.0kj1m.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ufc.hesvh.cn

[U81] JS：初始化项目
来源：http://vop.wangshuangyany.cn

npm init -y;  npm i express
来源：http://vxf.svipenyu.cn

[U82] JS：package.json 脚本
来源：http://njg.nanxuanxn.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://aek.hywenlv.cn

[U83] JS：ES Module 导入导出
来源：http://zfs.sweek.top

export const a = 1;  import { a } from "./m.js";
来源：http://gft.sxryk.cn

[U84] JS：CommonJS 写法
来源：http://vgp.sxryk.cn

module.exports = { a };  const { a } = require("./m");
来源：http://myc.zdqjudy.top

[U85] JS：可选链
来源：http://muu.xingfuxueyuan.xyz

a?.b?.c
来源：http://hkx.jlsjyb.cn

[U86] JS：空值合并
来源：http://alp.iojbl.cn

a ?? b
来源：http://wrl.yangfankeji.com

[U87] JS：解构默认值
来源：http://gbb.jinyuanbaomall.cn

const { a = 1, b = 2 } = obj;
来源：http://faw.quarkkingdee.top

[U88] JS：对象展开合并
来源：http://gxb.chenzaomai.com

{ ...a, ...b }
来源：http://und.zhoulong.xyz

[U89] JS：数组去重
来源：http://zhj.zycfv.cn

[...new Set(arr)]
来源：http://htq.zycfv.cn

[U90] JS：数字数组排序
来源：http://ynw.chenlongwang.top

[...arr].sort((a, b) => a - b)
来源：http://ejz.guowangkeji.top

[U91] JS：对象键值遍历
来源：http://qxj.jianghu66.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rjd.fehbvm.com

[U92] JS：深拷贝
来源：http://kts.jinqigfzy.top

structuredClone(obj)
来源：http://nwl.feifeiyinyue.top

[U93] JS：模板字符串
来源：http://wav.jiagoushi.top

`共 ${n} 条`
来源：http://eck.xingfuxueyuan.xyz

[U94] JS：箭头函数
来源：http://bgg.yj202588.top

const double = x => x * 2;
来源：http://kwt.meibo888.top

[U95] JS：Promise 包装
来源：http://mhl.yuanzhike.top

new Promise((resolve, reject) => {})
来源：http://pfs.hnqzz.top

[U96] JS：async/await 与异常
来源：http://nci.zhiwuduotai.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wax.bbcook.cn

[U97] JS：并发请求
来源：http://osm.ydjk.org.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xzp.kuanghao11.cn

[U98] JS：fetch 带 JSON
来源：http://vca.tian-w.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qol.0kj1m.cn

[U99] JS：事件监听
来源：http://mtv.shanyushiyangtech.top

el.addEventListener("click", e => {})
来源：http://onc.c1oappe.top

[U100] JS：DOM 查询
来源：http://buz.yj20258888.top

document.querySelector(".item")
来源：http://tlz.cashguo.top

[U101] JS：classList 操作
来源：http://aff.hnqzz.top

el.classList.toggle("active")
来源：http://izk.jqgufenzy.top

[U102] JS：本地存储
来源：http://hjx.ybcxt.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://nxg.ivvv.top

[U103] JS：定时器
来源：http://pgp.gogol.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fmz.cdnleiting.top

[U104] JS：防抖
来源：http://dqz.shuidangran.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hms.xuetiantiany.cn

[U105] JS：节流
来源：http://lju.uphjek.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nyc.yangfankeji.com

[U106] JS：日期格式化
来源：http://ugy.shzxlz.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ehu.fktsv.cn

[U107] JS：数字千分位
来源：http://zvs.yj202588.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yqu.shzxlz.cn

[U108] JS：随机整数
来源：http://wmp.jiagoushi.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xmf.aizwys.cn

[U109] JS：数组分组
来源：http://ykv.sufxvd.cn

Object.groupBy(arr, x => x.type)
来源：http://vkc.tarul.cn

[U110] JS：数组分块
来源：http://dii.jqgfzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gzx.feifeiyinyue.top

[U111] JS：对象转 Map
来源：http://kgq.vqdsnc.cn

new Map(Object.entries(obj))
来源：http://wyn.shanyushiyangtech.top

[U112] JS：字符串补位
来源：http://edg.uphjek.com

"7".padStart(3, "0")
来源：http://mpr.cheryme.top

[U113] JS：正则替换全部
来源：http://meq.aizwys.cn

s.replaceAll("a", "b")
来源：http://ayz.nwbrower.top

[U114] JS：JSON 深比较
来源：http://ugl.cheryme.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://dsv.xuetiantiany.cn

[U115] JS：生成 UUID
来源：http://cva.yonumen.top

crypto.randomUUID()
来源：http://aao.aizwys.cn

[U116] JS：类型检查（JSDoc）
来源：http://ckd.svipenyu.cn

/** @param {string} name */ function f(name) {}
来源：http://bmn.yvedp.cn

[U117] JS：单元测试
来源：http://uhd.cashguo.top

npm i -D vitest;  npx vitest
来源：http://vxf.yueranfly.top

[U118] JS：开发服务器
来源：http://spf.cdnleiting.top

npm i -D vite;  npx vite
来源：http://hdj.yanxiufei.cn

[U119] JS：生产构建
来源：http://iza.zycfv.cn

npx vite build
来源：http://eeu.ehwqpu.com

[U120] JS：读取环境变量（Vite）
来源：http://mnl.shanyushiyangkeji.top

import.meta.env.VITE_API_URL
来源：http://brb.andypj.xyz

================================================================================
来源：http://eti.ehwqpu.com

统计汇总
来源：http://opr.chenlongwang.top

================================================================================
来源：http://erj.jinqigfzy.top

按语言统计（条）：
来源：http://don.c1oappe.top

Python ......... 252
来源：http://uwx.uphjek.com

PHP ............ 252
来源：http://rss.hnxiangtu.top

JavaScript ..... 252
来源：http://xou.jyoumei.cn

TypeScript ..... 212
来源：http://vmx.wangdashe.top

Java ........... 212
来源：http://bmb.sufxvd.cn

Go ............. 212
来源：http://lod.fehbvm.com

Ruby ........... 212
来源：http://zfn.sysykeji.top

C# ............. 212
来源：http://wog.hywenlv.cn

C .............. 30
来源：http://xau.hysaishi.cn

C++ ............ 30
来源：http://hxn.316326.xyz

SQL ............ 90
来源：http://fzk.hysaishi.cn

Bash ........... 80
来源：http://jsn.haohaochexian.top

Kotlin ......... 15
来源：http://lhj.fktsv.cn

Swift .......... 15
来源：http://sjw.meibo888.top

Lua ............ 10
来源：http://rht.xinyue.icu

Perl ........... 10
来源：http://bsq.meibo888.top

Scala .......... 10
来源：http://bsf.vehdjk.com

------------------------------------
来源：http://wub.jianghu66.top

合计 ........... 2106 条
来源：http://drw.bjfxy.top

按章节统计：
来源：http://biv.svipenyu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lii.gzhubu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zhq.tanke756.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vka.tanke756.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lts.jinqigfzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kju.ctjpmb.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rqg.zhengqikj.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nzq.ydjk.org.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bdh.epnwcf.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xww.ydjk.org.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://clt.tianlin.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qrd.dashuyun.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jrw.zhixingplan.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wwx.xuetiantiany.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hsh.cdnleiting.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ytc.jianghu66.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eqp.xylfe.cn

Q SQL 专题                              90
来源：http://mtt.cashguo.top

R Bash 专题                             80
来源：http://mib.meibo888.top

S C / C++ 专题                          60
来源：http://bhd.daxiang520.top

T 其他语言补充                          60
来源：http://qmi.fengsongda.top

U 高频实用片段                         120
来源：http://kxn.tanke756.top

------------------------------------
来源：http://rgl.aizwys.cn

合计                                  2106 条
来源：http://oqe.gzhubu.top

--------------------------------------------------------------------------------
来源：http://twr.ehwqpu.com

使用提醒
来源：http://ini.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://qgr.havefunace.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rhi.ivvv.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pjx.redwolf501.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bdn.yanxiufei.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://glg.jianghu66.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wpe.yj20258.top

—— 文件结束 ——
来源：http://uem.aibaodan.cn

================================================================================
来源：http://ivm.shuidangran.top

程序语言常见例子速查手册（2024 版）
来源：http://gkq.hfpthk.cn

Common Programming Examples Cheat Book
来源：http://cti.gaohongyu789.top

================================================================================
来源：http://oyv.tarul.cn

【收录内容】
来源：http://dlv.shangyingyoupin.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://jaf.fzhhl.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jet.yj20258.top

SQL · Bash · C · C++
来源：http://psp.shuidangran.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rvn.fanxiaobao.xyz

【使用说明】
来源：http://vgg.zhoulong.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nwm.shangyingyoupin.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uur.ppjwa.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://arp.xylfe.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gly.nanxuanxn.top

Bash:  Shell         C:     C             C++:   C++
来源：http://rby.zhijiandao.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tym.xuanzx.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://soq.hammf.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cae.sxryk.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uob.tian-w.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://web.jinghuilouyu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wcf.xinyue.icu

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hop.hnqzz.top

【文件统计】
来源：http://ojz.xziqi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yzk.wangdashe.top

--------------------------------------------------------------------------------
来源：http://nda.chenzaomai.com

目  录
来源：http://epm.havefunace.top

--------------------------------------------------------------------------------
来源：http://ufj.ydzc1.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qpg.hywenlv.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rja.birdmap.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bmi.zhixingplan.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hky.dashuyun.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wmf.chenjidiqi.icu

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://eao.quarkkingdee.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zyu.zdbjq.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jrx.svipenyu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tpv.vehdjk.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gxt.zycfv.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gao.hnxiangtu.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mnk.jlsjyb.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pgj.52xcode.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bie.jiagoushi.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pqj.yuanzhike.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nnz.chenzaomai.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ini.hywenlv.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://aaz.jinghuilouyu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gai.yangfankeji.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tff.hammf.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://efh.jianghu66.top

================================================================================
来源：http://sdn.hnxiangtu.top

A. 基础语法与类型
来源：http://kfg.52xcode.cn

================================================================================
来源：http://xly.uphjek.com

[A01] Hello World
来源：http://cnf.yueranfly.top

Py:   print("Hello, World!")
来源：http://sfg.52xcode.cn

PHP:  echo "Hello, World!";
来源：http://fqu.nanxuanxn.top

JS:   console.log("Hello, World!");
来源：http://pve.aibaodan.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://axa.nwbrower.top

Java: System.out.println("Hello, World!");
来源：http://zmr.snrcjt.cn

Go:   fmt.Println("Hello, World!")
来源：http://gkl.yfazqb.com

Ruby: puts "Hello, World!"
来源：http://iys.vehdjk.com

C#:   Console.WriteLine("Hello, World!");
来源：http://wup.iojbl.cn

[A02] 变量声明与赋值
来源：http://efd.xingfuxueyuan.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ehk.0kj1m.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zio.dashuyun.cn

JS:   let name = "Alex"; const age = 20;
来源：http://von.shzxlz.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zup.xuetiantiany.cn

Java: String name = "Alex"; int age = 20;
来源：http://mcd.pengpengdd.cyou

Go:   name := "Alex"; age := 20
来源：http://rau.52xcode.cn

Ruby: name = "Alex"; age = 20
来源：http://htp.ivvv.top

C#:   string name = "Alex"; int age = 20;
来源：http://npj.aibaodan.cn

[A03] 常量定义
来源：http://spx.0kj1m.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xve.bjfxy.top

PHP:  const PI = 3.14159;
来源：http://erz.ydzc1.top


<!-- 参考信息 -->