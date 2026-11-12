代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://uhz.jqgfzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://imb.jiagoushi.top

[U42] PHP：PSR-4 自动加载
来源：http://zpr.yj20258888.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://abr.dianchejie.cn

[U43] PHP：声明命名空间
来源：http://tzh.zhoulong.xyz

namespace App\Http;
来源：http://ixf.shangyingyoupin.top

[U44] PHP：开启严格类型
来源：http://sjm.tian-w.cn

declare(strict_types=1);
来源：http://bdt.yvedp.cn

[U45] PHP：类型声明与返回类型
来源：http://kmm.sysykeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://uin.fehbvm.com

[U46] PHP：可空类型
来源：http://lem.gaohongyu789.top

?string $name = null
来源：http://lsx.uphjek.com

[U47] PHP：联合类型
来源：http://hop.xinyue.icu

int|string $id
来源：http://pol.daxiang520.top

[U48] PHP：纯枚举
来源：http://euk.zdbjq.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ffh.aizwys.cn

[U49] PHP：只读属性
来源：http://ggg.zhaomingkeji.xyz

public readonly string $name
来源：http://ctu.quarkkingdee.top

[U50] PHP：构造器属性提升
来源：http://ebp.uphjek.com

public function __construct(private int $id) {}
来源：http://twd.yanxiufei.cn

[U51] PHP：数组解构
来源：http://qxj.ydzc1.top

[$a, $b] = $arr;
来源：http://ozv.xinyue.icu

[U52] PHP：箭头函数
来源：http://wbn.snrcjt.cn

$double = fn($x) => $x * 2;
来源：http://cbo.tarul.cn

[U53] PHP：空合并运算符
来源：http://yuc.fanxiaobao.xyz

$v = $a ?? $b ?? "default";
来源：http://yqz.cashguo.top

[U54] PHP：空安全调用
来源：http://cbu.ydzc1.top

$obj?->method()
来源：http://dyb.sjlbkw.cn

[U55] PHP：match 表达式
来源：http://hug.zhijiandao.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ytv.birdmap.top

[U56] PHP：命名参数
来源：http://npm.hysaishi.cn

f(a: 1, b: 2)
来源：http://adg.sufxvd.cn

[U57] PHP：字符串插值
来源：http://zgi.cheryme.top

"值: {$a}"
来源：http://jzc.ydzc1.top

[U58] PHP：数组三件套
来源：http://jyu.ywan-chungtsiang.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://loy.dianchejie.cn

[U59] PHP：自定义排序
来源：http://dqu.quarkkingdee.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mks.jqgufenzy.top

[U60] PHP：JSON 编解码
来源：http://fwv.zhiwuduotai.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://opm.jlsjyb.cn

[U61] PHP：正则
来源：http://fhd.tian-w.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iqu.feifeiyinyue.top

[U62] PHP：日期对象
来源：http://tka.jinyuanbaomall.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jld.zhaomingkeji.xyz

[U63] PHP：文件读写
来源：http://iwn.zhongyouzk.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lrs.c1oappe.top

[U64] PHP：目录遍历
来源：http://ztd.52xcode.cn

glob("dir/*.php");  scandir("dir");
来源：http://ire.hesvh.cn

[U65] PHP：会话
来源：http://kin.chenzaomai.com

session_start();  $_SESSION["uid"] = 1;
来源：http://gou.yanxiufei.cn

[U66] PHP：设置 Cookie
来源：http://vxz.sweek.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://knh.jyoumei.cn

[U67] PHP：处理文件上传
来源：http://eyn.yfazqb.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vlk.chenjidiqi.icu

[U68] PHP：PDO 连接
来源：http://hyt.chenzaomai.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ufj.ywan-chungtsiang.top

[U69] PHP：PDO 预处理
来源：http://aeh.quarkkingdee.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sjl.vqdsnc.cn

[U70] PHP：PDO 事务
来源：http://dhl.tarul.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ewn.aibaodan.cn

[U71] PHP：抛出异常
来源：http://dkg.nanxuanxn.top

throw new RuntimeException("失败", 500);
来源：http://avz.sysykeji.top

[U72] PHP：写错误日志
来源：http://mow.yfazqb.com

error_log("失败: " . $e->getMessage());
来源：http://ldc.cashguo.top

[U73] PHP：读取 ini 配置
来源：http://ghp.aizwys.cn

parse_ini_file("config.ini", true)
来源：http://nec.bbcook.cn

[U74] PHP：读取环境变量
来源：http://jqm.pengpengdd.cyou

getenv("APP_ENV") ?: "production"
来源：http://sns.guannengcc.top

[U75] PHP：依赖注入
来源：http://nut.nanxuanxn.top

composer require psr/container
来源：http://ssz.jinqigfzy.top

[U76] PHP：简单路由
来源：http://rqb.shuidangran.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mxi.zdqjudy.top

[U77] PHP：模板渲染
来源：http://pxh.zhaomingkeji.xyz

composer require twig/twig
来源：http://adz.gogol.net.cn

[U78] PHP：单元测试
来源：http://pzo.tianlin.xyz

composer require --dev phpunit/phpunit
来源：http://dqe.yfazqb.com

[U79] PHP：静态分析
来源：http://wvz.sysykeji.top

composer require --dev phpstan/phpstan
来源：http://ijy.gotoacloud.top

[U80] PHP：代码规范修复
来源：http://vvd.hysaishi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://btz.pycfn.com

[U81] JS：初始化项目
来源：http://fqp.xylfe.cn

npm init -y;  npm i express
来源：http://gas.shanyushiyangkeji.top

[U82] JS：package.json 脚本
来源：http://qah.sweek.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pdl.shanyushiyangkeji.top

[U83] JS：ES Module 导入导出
来源：http://sqs.gotoacloud.top

export const a = 1;  import { a } from "./m.js";
来源：http://pcj.ctjpmb.com

[U84] JS：CommonJS 写法
来源：http://coe.gotoacloud.top

module.exports = { a };  const { a } = require("./m");
来源：http://yno.pycfn.com

[U85] JS：可选链
来源：http://zoz.jqgfzy.top

a?.b?.c
来源：http://asx.yj20258888.top

[U86] JS：空值合并
来源：http://wcf.hnxiangtu.top

a ?? b
来源：http://dje.jqgfzy.top

[U87] JS：解构默认值
来源：http://rbz.yangfankeji.com

const { a = 1, b = 2 } = obj;
来源：http://qrr.ydjk.org.cn

[U88] JS：对象展开合并
来源：http://lnd.sxryk.cn

{ ...a, ...b }
来源：http://ual.yueranfly.top

[U89] JS：数组去重
来源：http://ixa.cucudq.cn

[...new Set(arr)]
来源：http://ijo.epnwcf.com

[U90] JS：数字数组排序
来源：http://xre.fanxiaobao.xyz

[...arr].sort((a, b) => a - b)
来源：http://gxr.epnwcf.com

[U91] JS：对象键值遍历
来源：http://zuq.havefunace.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://iqs.chenzaomai.com

[U92] JS：深拷贝
来源：http://duy.redwolf501.top

structuredClone(obj)
来源：http://yia.jinghuilouyu.cn

[U93] JS：模板字符串
来源：http://hse.tianlin.xyz

`共 ${n} 条`
来源：http://pkl.jyoumei.cn

[U94] JS：箭头函数
来源：http://lht.shanyushiyangkeji.top

const double = x => x * 2;
来源：http://ckl.mhx1999.top

[U95] JS：Promise 包装
来源：http://avw.jinqigfzy.top

new Promise((resolve, reject) => {})
来源：http://lrx.zhongyouzk.top

[U96] JS：async/await 与异常
来源：http://fbb.fehbvm.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ykn.zhixingplan.top

[U97] JS：并发请求
来源：http://zbl.yuxming.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://emt.0kj1m.cn

[U98] JS：fetch 带 JSON
来源：http://vhb.shzxlz.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lkr.xuetiantiany.cn

[U99] JS：事件监听
来源：http://jqn.havefunace.top

el.addEventListener("click", e => {})
来源：http://akd.zdqjudy.top

[U100] JS：DOM 查询
来源：http://qzj.bbcook.cn

document.querySelector(".item")
来源：http://nny.jinyuanbaomall.cn

[U101] JS：classList 操作
来源：http://huk.hesvh.cn

el.classList.toggle("active")
来源：http://kdh.xingfuxueyuan.xyz

[U102] JS：本地存储
来源：http://ern.cdnleiting.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://iyn.hesvh.cn

[U103] JS：定时器
来源：http://nbn.zhengqikj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ibi.wangshuangyany.cn

[U104] JS：防抖
来源：http://imp.jqgfzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ybq.yfazqb.com

[U105] JS：节流
来源：http://qcc.ehwqpu.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://elb.shuidangran.top

[U106] JS：日期格式化
来源：http://pnf.tian-w.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rnc.andypj.xyz

[U107] JS：数字千分位
来源：http://wsc.sxryk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yuj.tanke756.top

[U108] JS：随机整数
来源：http://lii.fanxiaobao.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vgs.fehbvm.com

[U109] JS：数组分组
来源：http://pwg.yuanzhike.top

Object.groupBy(arr, x => x.type)
来源：http://mmy.yj20258.top

[U110] JS：数组分块
来源：http://siq.chenzaomai.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fzr.hnxiangtu.top

[U111] JS：对象转 Map
来源：http://gib.yfazqb.com

new Map(Object.entries(obj))
来源：http://dhh.vqdsnc.cn

[U112] JS：字符串补位
来源：http://myt.feifeiyinyue.top

"7".padStart(3, "0")
来源：http://bil.xinyue.icu

[U113] JS：正则替换全部
来源：http://ldw.zhongyouzk.top

s.replaceAll("a", "b")
来源：http://uac.yanxiufei.cn

[U114] JS：JSON 深比较
来源：http://gjh.aizwys.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tdc.sxryk.cn

[U115] JS：生成 UUID
来源：http://tgv.9152youxi.cn

crypto.randomUUID()
来源：http://caa.yvedp.cn

[U116] JS：类型检查（JSDoc）
来源：http://zia.yuxming.cn

/** @param {string} name */ function f(name) {}
来源：http://pmk.havefunace.top

[U117] JS：单元测试
来源：http://wwr.ctjpmb.com

npm i -D vitest;  npx vitest
来源：http://ewk.xuanzx.com

[U118] JS：开发服务器
来源：http://prj.tarul.cn

npm i -D vite;  npx vite
来源：http://pmf.snrcjt.cn

[U119] JS：生产构建
来源：http://ves.hysaishi.cn

npx vite build
来源：http://joi.gzhubu.top

[U120] JS：读取环境变量（Vite）
来源：http://cvm.yfazqb.com

import.meta.env.VITE_API_URL
来源：http://dpi.kuanghao11.cn

================================================================================
来源：http://bes.havefunace.top

统计汇总
来源：http://jon.xylfe.cn

================================================================================
来源：http://nft.bjfxy.top

按语言统计（条）：
来源：http://zfz.yj202588.top

Python ......... 252
来源：http://kvs.52xcode.cn

PHP ............ 252
来源：http://arc.ehwqpu.com

JavaScript ..... 252
来源：http://syy.aizwys.cn

TypeScript ..... 212
来源：http://joz.jinghuilouyu.cn

Java ........... 212
来源：http://onu.jqgufenzy.top

Go ............. 212
来源：http://jgw.yongpay.top

Ruby ........... 212
来源：http://zcv.yueranfly.top

C# ............. 212
来源：http://tmz.zhijiandao.cn

C .............. 30
来源：http://vru.yfazqb.com

C++ ............ 30
来源：http://vbf.yj20258888.top

SQL ............ 90
来源：http://jff.zhaomingkeji.xyz

Bash ........... 80
来源：http://moq.yuxming.cn

Kotlin ......... 15
来源：http://lvd.andypj.xyz

Swift .......... 15
来源：http://szs.xziqi.cn

Lua ............ 10
来源：http://zcs.sjlbkw.cn

Perl ........... 10
来源：http://iur.vqdsnc.cn

Scala .......... 10
来源：http://vao.wangshuangyany.cn

------------------------------------
来源：http://owi.nanxuanxn.top

合计 ........... 2106 条
来源：http://nqr.jlsjyb.cn

按章节统计：
来源：http://aap.yueranfly.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qof.52xcode.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sok.snrcjt.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yxg.hnqzz.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yti.316326.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uci.yj20258888.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://apz.gotoacloud.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mno.jinqigfzy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vpc.bbcook.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tsi.bbcook.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wom.daria6918.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://doy.chenjidiqi.icu

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wiv.jinqigfzy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mgh.hongshengwenyu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rmf.c1oappe.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://emc.chenjidiqi.icu

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lju.tarul.cn

Q SQL 专题                              90
来源：http://nhh.cucudq.cn

R Bash 专题                             80
来源：http://qnk.ywan-chungtsiang.top

S C / C++ 专题                          60
来源：http://wpr.uphjek.com

T 其他语言补充                          60
来源：http://ljo.pengpengdd.cyou

U 高频实用片段                         120
来源：http://mmf.ydzc1.top

------------------------------------
来源：http://sys.feifeiyinyue.top

合计                                  2106 条
来源：http://aan.xuanzx.com

--------------------------------------------------------------------------------
来源：http://zjs.quarkkingdee.top

使用提醒
来源：http://qex.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://jjh.zhijiandao.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wgy.ydjk.org.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tid.cheryme.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gkq.cqqwz.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://unx.feifeiyinyue.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ngp.chenjidiqi.icu

—— 文件结束 ——
来源：http://iyg.gzhubu.top

================================================================================
来源：http://ydy.yonumen.top

程序语言常见例子速查手册（2024 版）
来源：http://qcu.ydjk.org.cn

Common Programming Examples Cheat Book
来源：http://uox.ehwqpu.com

================================================================================
来源：http://sux.yj20258.top

【收录内容】
来源：http://spq.xuetiantiany.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wae.xingfuxueyuan.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fnj.ctjpmb.com

SQL · Bash · C · C++
来源：http://xoj.fzhhl.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vuy.daria6918.cn

【使用说明】
来源：http://ayj.ywan-chungtsiang.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qrp.havefunace.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rtn.shuidangran.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dby.shzxlz.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qsh.pycfn.com

Bash:  Shell         C:     C             C++:   C++
来源：http://nei.ydzc1.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vud.shanyushiyangkeji.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sfu.kuanghao11.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://arp.zycfv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://agi.hnxiangtu.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uaz.jinyuanbaomall.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://foq.ywan-chungtsiang.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://utb.cashguo.top

【文件统计】
来源：http://zkv.xingfuxueyuan.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://haj.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://otq.bbcook.cn

目  录
来源：http://jve.fzhhl.top

--------------------------------------------------------------------------------
来源：http://ptm.uphjek.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://iuy.yonumen.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://shg.redwolf501.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://esy.ehwqpu.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kwr.zhijiandao.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mca.hfpthk.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fvb.nanxuanxn.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://eyw.jinqigfzy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zap.ppjwa.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rws.hnxiangtu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ebo.sxryk.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gad.ctjpmb.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sfw.zdbjq.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://teh.gotoacloud.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wyk.fanxiaobao.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kwa.yueranfly.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cmo.nanxuanxn.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fsk.dashuyun.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wtg.sweek.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yub.fehbvm.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cte.zhijiandao.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kkn.zhongyouzk.top

================================================================================
来源：http://xhv.zhixingplan.top

A. 基础语法与类型
来源：http://zdt.chenjidiqi.icu

================================================================================
来源：http://cjo.chenjidiqi.icu

[A01] Hello World
来源：http://ayi.zycfv.cn

Py:   print("Hello, World!")
来源：http://udj.xziqi.cn

PHP:  echo "Hello, World!";
来源：http://nlx.jyoumei.cn

JS:   console.log("Hello, World!");
来源：http://ubw.wangshuangyany.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fli.bjfxy.top

Java: System.out.println("Hello, World!");
来源：http://xbr.ctjpmb.com

Go:   fmt.Println("Hello, World!")
来源：http://rmo.bjfxy.top

Ruby: puts "Hello, World!"
来源：http://yfo.c1oappe.top

C#:   Console.WriteLine("Hello, World!");
来源：http://pty.zhaomingkeji.xyz

[A02] 变量声明与赋值
来源：http://hax.ywan-chungtsiang.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pvt.gzhubu.top

PHP:  $name = "Alex"; $age = 20;
来源：http://vow.yj20258.top

JS:   let name = "Alex"; const age = 20;
来源：http://lfr.cucudq.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dwx.ydzc1.top

Java: String name = "Alex"; int age = 20;
来源：http://bmy.cashguo.top

Go:   name := "Alex"; age := 20
来源：http://kid.vehdjk.com

Ruby: name = "Alex"; age = 20
来源：http://dwk.yfazqb.com

C#:   string name = "Alex"; int age = 20;
来源：http://uiy.xinyue.icu

[A03] 常量定义
来源：http://qgm.sweek.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rif.yuanzhike.top

PHP:  const PI = 3.14159;
来源：http://kus.jinyuanbaomall.cn

JS:   const PI = 3.14159;
来源：http://qnv.feifeiyinyue.top

TS:   const PI: number = 3.14159;
来源：http://orp.yuanzhike.top

Java: static final double PI = 3.14159;
来源：http://dev.xingfuxueyuan.xyz

Go:   const PI = 3.14159
来源：http://ojp.fzhhl.top

Ruby: PI = 3.14159
来源：http://rga.snrcjt.cn

C#:   const double PI = 3.14159;
来源：http://rtb.svipenyu.cn

[A04] 判断变量类型
来源：http://ahc.yanxiufei.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://lyr.quarkkingdee.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rcd.zhixingplan.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kev.chenlongwang.top

TS:   typeof x; x instanceof Date
来源：http://gko.nanxuanxn.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://syk.cheryme.top


<!-- 参考信息 -->