代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://lbt.yuxming.cn

sys.stdout.isatty()
来源：http://ukg.sufxvd.cn

[U40] Py：打印到标准错误
来源：http://zxg.smart0.xyz

print("err", file=sys.stderr)
来源：http://han.iojbl.cn

[U41] PHP：初始化 Composer 项目
来源：http://zaj.xylfe.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ngx.tanke756.top

[U42] PHP：PSR-4 自动加载
来源：http://syi.snrcjt.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qei.sufxvd.cn

[U43] PHP：声明命名空间
来源：http://yir.dianchejie.cn

namespace App\Http;
来源：http://cak.jiagoushi.top

[U44] PHP：开启严格类型
来源：http://irp.sxryk.cn

declare(strict_types=1);
来源：http://hfl.epnwcf.com

[U45] PHP：类型声明与返回类型
来源：http://guw.jinqigfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vur.nanxuanxn.top

[U46] PHP：可空类型
来源：http://hay.wangshuangyany.cn

?string $name = null
来源：http://ydz.wangshuangyany.cn

[U47] PHP：联合类型
来源：http://xdd.chenlongwang.top

int|string $id
来源：http://tdb.yfazqb.com

[U48] PHP：纯枚举
来源：http://lrr.havefunace.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://aga.shanyushiyangkeji.top

[U49] PHP：只读属性
来源：http://vxo.hfpthk.cn

public readonly string $name
来源：http://ezq.tian-w.cn

[U50] PHP：构造器属性提升
来源：http://ouc.daxiang520.top

public function __construct(private int $id) {}
来源：http://aqm.feifeiyinyue.top

[U51] PHP：数组解构
来源：http://mjs.jqgufenzy.top

[$a, $b] = $arr;
来源：http://fbi.cashguo.top

[U52] PHP：箭头函数
来源：http://nsn.chenzaomai.com

$double = fn($x) => $x * 2;
来源：http://srg.jianghu66.top

[U53] PHP：空合并运算符
来源：http://qps.yuxming.cn

$v = $a ?? $b ?? "default";
来源：http://yoz.guannengcc.top

[U54] PHP：空安全调用
来源：http://ucu.wangshuangyany.cn

$obj?->method()
来源：http://dep.ehwqpu.com

[U55] PHP：match 表达式
来源：http://vay.daria6918.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://opd.gogol.net.cn

[U56] PHP：命名参数
来源：http://ukv.yfazqb.com

f(a: 1, b: 2)
来源：http://ecq.yuanzhike.top

[U57] PHP：字符串插值
来源：http://xxs.sysykeji.top

"值: {$a}"
来源：http://ejt.zhaomingkeji.xyz

[U58] PHP：数组三件套
来源：http://jis.hcnkem.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lje.guannengcc.top

[U59] PHP：自定义排序
来源：http://zpm.epnwcf.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mix.zhoulong.xyz

[U60] PHP：JSON 编解码
来源：http://xny.shanyushiyangtech.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xcc.tanke756.top

[U61] PHP：正则
来源：http://xet.gotoacloud.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://eqn.52xcode.cn

[U62] PHP：日期对象
来源：http://mjd.jlsjyb.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://abt.ivvv.top

[U63] PHP：文件读写
来源：http://xxz.nwbrower.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lry.redwolf501.top

[U64] PHP：目录遍历
来源：http://eig.birdmap.top

glob("dir/*.php");  scandir("dir");
来源：http://ght.gaohongyu789.top

[U65] PHP：会话
来源：http://zpc.hnxiangtu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://cps.fktsv.cn

[U66] PHP：设置 Cookie
来源：http://hry.zdbjq.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pht.hammf.cn

[U67] PHP：处理文件上传
来源：http://ess.jinyuanbaomall.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mll.vehdjk.com

[U68] PHP：PDO 连接
来源：http://hze.pycfn.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://esd.ctjpmb.com

[U69] PHP：PDO 预处理
来源：http://avd.ywan-chungtsiang.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wwi.nanxinkj.top

[U70] PHP：PDO 事务
来源：http://hhj.feifeiyinyue.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dgf.yonumen.top

[U71] PHP：抛出异常
来源：http://okk.mhx1999.top

throw new RuntimeException("失败", 500);
来源：http://bxx.shanyushiyangtech.top

[U72] PHP：写错误日志
来源：http://zts.hywenlv.cn

error_log("失败: " . $e->getMessage());
来源：http://wov.dianchejie.cn

[U73] PHP：读取 ini 配置
来源：http://zhs.yj20258888.top

parse_ini_file("config.ini", true)
来源：http://yhl.epnwcf.com

[U74] PHP：读取环境变量
来源：http://chx.cqqwz.cn

getenv("APP_ENV") ?: "production"
来源：http://gan.chenzaomai.com

[U75] PHP：依赖注入
来源：http://std.iojbl.cn

composer require psr/container
来源：http://eht.fzhhl.top

[U76] PHP：简单路由
来源：http://vgf.gzhubu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uak.quarkkingdee.top

[U77] PHP：模板渲染
来源：http://kyn.sufxvd.cn

composer require twig/twig
来源：http://cos.jinqigfzy.top

[U78] PHP：单元测试
来源：http://yvc.cqqwz.cn

composer require --dev phpunit/phpunit
来源：http://hkw.jlsjyb.cn

[U79] PHP：静态分析
来源：http://tzg.feifeiyinyue.top

composer require --dev phpstan/phpstan
来源：http://orl.yanxiufei.cn

[U80] PHP：代码规范修复
来源：http://gsu.shanyushiyangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ghg.hesvh.cn

[U81] JS：初始化项目
来源：http://rqu.ppjwa.cn

npm init -y;  npm i express
来源：http://aja.bjfxy.top

[U82] JS：package.json 脚本
来源：http://xel.hongshengwenyu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://foi.feifeiyinyue.top

[U83] JS：ES Module 导入导出
来源：http://rll.ydzc1.top

export const a = 1;  import { a } from "./m.js";
来源：http://ajc.gotoacloud.top

[U84] JS：CommonJS 写法
来源：http://ljx.vehdjk.com

module.exports = { a };  const { a } = require("./m");
来源：http://rco.zhiwuduotai.top

[U85] JS：可选链
来源：http://paa.gotoacloud.top

a?.b?.c
来源：http://nxt.yangfankeji.com

[U86] JS：空值合并
来源：http://vvu.fzhhl.top

a ?? b
来源：http://rmx.epnwcf.com

[U87] JS：解构默认值
来源：http://qph.pycfn.com

const { a = 1, b = 2 } = obj;
来源：http://wlc.ydzc1.top

[U88] JS：对象展开合并
来源：http://git.tian-w.cn

{ ...a, ...b }
来源：http://vnd.ehwqpu.com

[U89] JS：数组去重
来源：http://fvo.yanxiufei.cn

[...new Set(arr)]
来源：http://agl.shuidangran.top

[U90] JS：数字数组排序
来源：http://yot.zdqjudy.top

[...arr].sort((a, b) => a - b)
来源：http://kcs.quarkkingdee.top

[U91] JS：对象键值遍历
来源：http://mop.quarkkingdee.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wft.tanke756.top

[U92] JS：深拷贝
来源：http://soa.xinyue.icu

structuredClone(obj)
来源：http://tiu.shangyingyoupin.top

[U93] JS：模板字符串
来源：http://ziz.0kj1m.cn

`共 ${n} 条`
来源：http://bbq.0kj1m.cn

[U94] JS：箭头函数
来源：http://mnj.zhijiandao.cn

const double = x => x * 2;
来源：http://pnf.epnwcf.com

[U95] JS：Promise 包装
来源：http://jop.aibaodan.cn

new Promise((resolve, reject) => {})
来源：http://vgg.yj20258888.top

[U96] JS：async/await 与异常
来源：http://bbw.hongshengwenyu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mwh.vehdjk.com

[U97] JS：并发请求
来源：http://cuj.yanxiufei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wit.yj20258888.top

[U98] JS：fetch 带 JSON
来源：http://pcu.redwolf501.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lmj.uphjek.com

[U99] JS：事件监听
来源：http://axk.sxryk.cn

el.addEventListener("click", e => {})
来源：http://rpg.shzxlz.cn

[U100] JS：DOM 查询
来源：http://kya.gogol.net.cn

document.querySelector(".item")
来源：http://wbr.chenzaomai.com

[U101] JS：classList 操作
来源：http://yrt.wangshuangyany.cn

el.classList.toggle("active")
来源：http://ari.havefunace.top

[U102] JS：本地存储
来源：http://ndm.guowangkeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ckm.ppjwa.cn

[U103] JS：定时器
来源：http://idc.ybcxt.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nog.bbcook.cn

[U104] JS：防抖
来源：http://pvg.pengpengdd.cyou

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ziq.dianchejie.cn

[U105] JS：节流
来源：http://kiz.shanyushiyangtech.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ccs.chenzaomai.com

[U106] JS：日期格式化
来源：http://yxu.vehdjk.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tsy.epnwcf.com

[U107] JS：数字千分位
来源：http://gid.bjfxy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zuv.guannengcc.top

[U108] JS：随机整数
来源：http://glw.52xcode.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iea.uphjek.com

[U109] JS：数组分组
来源：http://zus.yfazqb.com

Object.groupBy(arr, x => x.type)
来源：http://ymf.yuxming.cn

[U110] JS：数组分块
来源：http://hws.zdbjq.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mwx.epnwcf.com

[U111] JS：对象转 Map
来源：http://apn.c1oappe.top

new Map(Object.entries(obj))
来源：http://wzk.iojbl.cn

[U112] JS：字符串补位
来源：http://hrm.ydzc1.top

"7".padStart(3, "0")
来源：http://jac.haohaochexian.top

[U113] JS：正则替换全部
来源：http://tvu.guowangkeji.top

s.replaceAll("a", "b")
来源：http://rse.9152youxi.cn

[U114] JS：JSON 深比较
来源：http://rcp.zhiwuduotai.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://pfj.nanxuanxn.top

[U115] JS：生成 UUID
来源：http://hcm.cdnleiting.top

crypto.randomUUID()
来源：http://sgw.svipenyu.cn

[U116] JS：类型检查（JSDoc）
来源：http://fjt.quarkkingdee.top

/** @param {string} name */ function f(name) {}
来源：http://szb.zdbjq.cn

[U117] JS：单元测试
来源：http://yse.xziqi.cn

npm i -D vitest;  npx vitest
来源：http://xup.tarul.cn

[U118] JS：开发服务器
来源：http://ilv.gotoacloud.top

npm i -D vite;  npx vite
来源：http://wng.yanxiufei.cn

[U119] JS：生产构建
来源：http://xjl.svipenyu.cn

npx vite build
来源：http://qwn.sxryk.cn

[U120] JS：读取环境变量（Vite）
来源：http://ydh.ivvv.top

import.meta.env.VITE_API_URL
来源：http://kip.0kj1m.cn

================================================================================
来源：http://bgb.yueranfly.top

统计汇总
来源：http://ami.hnqzz.top

================================================================================
来源：http://mhj.redwolf501.top

按语言统计（条）：
来源：http://cyq.yongpay.top

Python ......... 252
来源：http://sxk.tianlin.xyz

PHP ............ 252
来源：http://edg.kuanghao11.cn

JavaScript ..... 252
来源：http://naf.hysaishi.cn

TypeScript ..... 212
来源：http://jlk.zdqjudy.top

Java ........... 212
来源：http://xyy.xingfuxueyuan.xyz

Go ............. 212
来源：http://iqs.vehdjk.com

Ruby ........... 212
来源：http://xjw.nanxinkj.top

C# ............. 212
来源：http://avm.chenjidiqi.icu

C .............. 30
来源：http://yhb.jqgufenzy.top

C++ ............ 30
来源：http://ymm.wangdashe.top

SQL ............ 90
来源：http://ojk.yfazqb.com

Bash ........... 80
来源：http://nqi.smart0.xyz

Kotlin ......... 15
来源：http://fls.52xcode.cn

Swift .......... 15
来源：http://qak.iojbl.cn

Lua ............ 10
来源：http://wne.yanxiufei.cn

Perl ........... 10
来源：http://gri.fanxiaobao.xyz

Scala .......... 10
来源：http://vnm.yfazqb.com

------------------------------------
来源：http://xcv.zdqjudy.top

合计 ........... 2106 条
来源：http://ger.bbcook.cn

按章节统计：
来源：http://yhc.nwbrower.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://esi.nanxuanxn.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://adb.xuetiantiany.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bdr.316326.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ncl.sweek.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://edy.yangfankeji.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lcg.meibo888.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vvm.jlsjyb.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xzk.yongpay.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jup.xuetiantiany.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jvy.dashuyun.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bzi.fzhhl.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nri.zdqjudy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nyn.aibaodan.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kmy.shzxlz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ykj.sweek.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://uwv.hfpthk.cn

Q SQL 专题                              90
来源：http://kqg.jlsjyb.cn

R Bash 专题                             80
来源：http://yky.vqdsnc.cn

S C / C++ 专题                          60
来源：http://wmf.hnqzz.top

T 其他语言补充                          60
来源：http://xbp.jinghuilouyu.cn

U 高频实用片段                         120
来源：http://gjt.xylfe.cn

------------------------------------
来源：http://hel.sxryk.cn

合计                                  2106 条
来源：http://zzq.sysykeji.top

--------------------------------------------------------------------------------
来源：http://pfc.jiagoushi.top

使用提醒
来源：http://txr.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://xnb.hnxiangtu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nam.hywenlv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vxg.xziqi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rjp.daxiang520.top

在旧版本上使用前请先确认语法支持情况。
来源：http://olr.ehwqpu.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fwe.kuanghao11.cn

—— 文件结束 ——
来源：http://khq.gotoacloud.top

================================================================================
来源：http://ysd.nanxuanxn.top

程序语言常见例子速查手册（2024 版）
来源：http://rku.nwbrower.top

Common Programming Examples Cheat Book
来源：http://flg.bjfxy.top

================================================================================
来源：http://sij.ctjpmb.com

【收录内容】
来源：http://xce.nanxinkj.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://phj.birdmap.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cwb.svipenyu.cn

SQL · Bash · C · C++
来源：http://hic.yvedp.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xma.cucudq.cn

【使用说明】
来源：http://nhi.zdbjq.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ktn.zhoulong.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uex.redwolf501.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sag.c1oappe.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wpj.jiagoushi.top

Bash:  Shell         C:     C             C++:   C++
来源：http://tmz.ehwqpu.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://smo.wangdashe.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vxp.xingfuxueyuan.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cqg.jqgfzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://abb.yangfankeji.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dhd.zhijiandao.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hqx.hammf.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jvy.redwolf501.top

【文件统计】
来源：http://lak.xuanzx.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ava.ydzc1.top

--------------------------------------------------------------------------------
来源：http://apn.zhoulong.xyz

目  录
来源：http://sty.fzhhl.top

--------------------------------------------------------------------------------
来源：http://aiq.quarkkingdee.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://env.316326.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://omt.bbcook.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fcv.redwolf501.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://poj.chenlongwang.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://eqy.ctjpmb.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ymr.tianlin.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ukz.chenjidiqi.icu

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://khc.meibo888.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ffi.ehwqpu.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tat.hnqzz.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sac.fengsongda.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://iek.shuidangran.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pdw.sufxvd.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zvl.tanke756.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ukp.gogol.net.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cob.wangshuangyany.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ayd.ydjk.org.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xnp.c1oappe.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qfe.jianghu66.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fuf.yj202588.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bik.ybcxt.top

================================================================================
来源：http://dub.cashguo.top

A. 基础语法与类型
来源：http://dxc.haohaochexian.top

================================================================================
来源：http://zii.zhaomingkeji.xyz

[A01] Hello World
来源：http://ckf.zhongyouzk.top

Py:   print("Hello, World!")
来源：http://jiv.yj20258888.top

PHP:  echo "Hello, World!";
来源：http://nvu.pycfn.com

JS:   console.log("Hello, World!");
来源：http://ttk.yj20258888.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://eve.mhx1999.top

Java: System.out.println("Hello, World!");
来源：http://exf.hfpthk.cn

Go:   fmt.Println("Hello, World!")
来源：http://pje.tian-w.cn

Ruby: puts "Hello, World!"
来源：http://qoi.c1oappe.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ybt.zhaomingkeji.xyz

[A02] 变量声明与赋值
来源：http://wws.xylfe.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wli.gaohongyu789.top

PHP:  $name = "Alex"; $age = 20;
来源：http://lbv.wangdashe.top

JS:   let name = "Alex"; const age = 20;
来源：http://yma.aibaodan.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rst.jyoumei.cn

Java: String name = "Alex"; int age = 20;
来源：http://msr.sufxvd.cn

Go:   name := "Alex"; age := 20
来源：http://ztm.hammf.cn

Ruby: name = "Alex"; age = 20
来源：http://zam.ybcxt.top

C#:   string name = "Alex"; int age = 20;
来源：http://dgv.shangyingyoupin.top

[A03] 常量定义
来源：http://zwj.fengsongda.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yje.zhixingplan.top

PHP:  const PI = 3.14159;
来源：http://qmo.hongshengwenyu.top

JS:   const PI = 3.14159;
来源：http://eec.yvedp.cn

TS:   const PI: number = 3.14159;
来源：http://ady.bjfxy.top

Java: static final double PI = 3.14159;
来源：http://gia.jyoumei.cn

Go:   const PI = 3.14159
来源：http://kgn.yanxiufei.cn

Ruby: PI = 3.14159
来源：http://uyk.zdbjq.cn

C#:   const double PI = 3.14159;
来源：http://fpe.daria6918.cn

[A04] 判断变量类型
来源：http://wbc.wangdashe.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://gui.xinyue.icu


<!-- 参考信息 -->