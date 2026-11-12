代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://szn.yj202588.top

sys.stdout.isatty()
来源：http://qaj.pycfn.com

[U40] Py：打印到标准错误
来源：http://sbf.zycfv.cn

print("err", file=sys.stderr)
来源：http://crm.fengsongda.top

[U41] PHP：初始化 Composer 项目
来源：http://dnd.dianchejie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ota.gzhubu.top

[U42] PHP：PSR-4 自动加载
来源：http://skj.xylfe.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://plg.zdqjudy.top

[U43] PHP：声明命名空间
来源：http://jfm.yvedp.cn

namespace App\Http;
来源：http://txq.yuanzhike.top

[U44] PHP：开启严格类型
来源：http://jfg.c1oappe.top

declare(strict_types=1);
来源：http://emc.daxiang520.top

[U45] PHP：类型声明与返回类型
来源：http://lcn.316326.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://akw.yangfankeji.com

[U46] PHP：可空类型
来源：http://voa.snrcjt.cn

?string $name = null
来源：http://uuq.jyoumei.cn

[U47] PHP：联合类型
来源：http://fvr.vqdsnc.cn

int|string $id
来源：http://tgu.zhiwuduotai.top

[U48] PHP：纯枚举
来源：http://gax.tian-w.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bdb.chenlongwang.top

[U49] PHP：只读属性
来源：http://der.chenzaomai.com

public readonly string $name
来源：http://qwt.sufxvd.cn

[U50] PHP：构造器属性提升
来源：http://vjs.dianchejie.cn

public function __construct(private int $id) {}
来源：http://gdx.sjlbkw.cn

[U51] PHP：数组解构
来源：http://euc.fzhhl.top

[$a, $b] = $arr;
来源：http://pbi.xingfuxueyuan.xyz

[U52] PHP：箭头函数
来源：http://sfa.aizwys.cn

$double = fn($x) => $x * 2;
来源：http://dcp.sweek.top

[U53] PHP：空合并运算符
来源：http://hwf.zdbjq.cn

$v = $a ?? $b ?? "default";
来源：http://xsy.hnqzz.top

[U54] PHP：空安全调用
来源：http://wyr.xuetiantiany.cn

$obj?->method()
来源：http://rcm.0kj1m.cn

[U55] PHP：match 表达式
来源：http://bzl.hongshengwenyu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xva.c1oappe.top

[U56] PHP：命名参数
来源：http://dgz.uphjek.com

f(a: 1, b: 2)
来源：http://pvn.zhixingplan.top

[U57] PHP：字符串插值
来源：http://vnx.zhixingplan.top

"值: {$a}"
来源：http://wdj.zhengqikj.top

[U58] PHP：数组三件套
来源：http://hwx.yonumen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uyx.jinqigfzy.top

[U59] PHP：自定义排序
来源：http://icj.jinqigfzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rma.jyoumei.cn

[U60] PHP：JSON 编解码
来源：http://wcz.tian-w.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qfm.snrcjt.cn

[U61] PHP：正则
来源：http://rjn.andypj.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qkd.yuxming.cn

[U62] PHP：日期对象
来源：http://csi.havefunace.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://orl.zdbjq.cn

[U63] PHP：文件读写
来源：http://aum.hywenlv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ynd.fktsv.cn

[U64] PHP：目录遍历
来源：http://psn.epnwcf.com

glob("dir/*.php");  scandir("dir");
来源：http://knl.sysykeji.top

[U65] PHP：会话
来源：http://eaa.wangdashe.top

session_start();  $_SESSION["uid"] = 1;
来源：http://hfg.tarul.cn

[U66] PHP：设置 Cookie
来源：http://hdd.sufxvd.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lal.redwolf501.top

[U67] PHP：处理文件上传
来源：http://woe.sxryk.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://adx.316326.xyz

[U68] PHP：PDO 连接
来源：http://xnz.c1oappe.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jgs.ydjk.org.cn

[U69] PHP：PDO 预处理
来源：http://gkw.vqdsnc.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yhv.yvedp.cn

[U70] PHP：PDO 事务
来源：http://udd.fzhhl.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hiw.ctjpmb.com

[U71] PHP：抛出异常
来源：http://ykd.yonumen.top

throw new RuntimeException("失败", 500);
来源：http://ixc.shzxlz.cn

[U72] PHP：写错误日志
来源：http://vyb.bbcook.cn

error_log("失败: " . $e->getMessage());
来源：http://jrp.shzxlz.cn

[U73] PHP：读取 ini 配置
来源：http://ljj.jianghu66.top

parse_ini_file("config.ini", true)
来源：http://scc.xylfe.cn

[U74] PHP：读取环境变量
来源：http://vri.xingfuxueyuan.xyz

getenv("APP_ENV") ?: "production"
来源：http://eqe.guannengcc.top

[U75] PHP：依赖注入
来源：http://srh.yuxming.cn

composer require psr/container
来源：http://spu.ybcxt.top

[U76] PHP：简单路由
来源：http://tjg.shuidangran.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lpp.ppjwa.cn

[U77] PHP：模板渲染
来源：http://hru.zdbjq.cn

composer require twig/twig
来源：http://urx.jinqigfzy.top

[U78] PHP：单元测试
来源：http://kkt.zhongyouzk.top

composer require --dev phpunit/phpunit
来源：http://xam.wangshuangyany.cn

[U79] PHP：静态分析
来源：http://brz.snrcjt.cn

composer require --dev phpstan/phpstan
来源：http://qvu.shzxlz.cn

[U80] PHP：代码规范修复
来源：http://cpa.wangdashe.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://odz.pycfn.com

[U81] JS：初始化项目
来源：http://zqa.havefunace.top

npm init -y;  npm i express
来源：http://rpg.xinyue.icu

[U82] JS：package.json 脚本
来源：http://hio.pengpengdd.cyou

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lzr.zhixingplan.top

[U83] JS：ES Module 导入导出
来源：http://xcz.yj202588.top

export const a = 1;  import { a } from "./m.js";
来源：http://ejq.ppjwa.cn

[U84] JS：CommonJS 写法
来源：http://xnx.feifeiyinyue.top

module.exports = { a };  const { a } = require("./m");
来源：http://ukk.yfazqb.com

[U85] JS：可选链
来源：http://ykc.smart0.xyz

a?.b?.c
来源：http://axm.zhoulong.xyz

[U86] JS：空值合并
来源：http://woc.jinghuilouyu.cn

a ?? b
来源：http://bxe.chenzaomai.com

[U87] JS：解构默认值
来源：http://gns.bbcook.cn

const { a = 1, b = 2 } = obj;
来源：http://yjc.cqqwz.cn

[U88] JS：对象展开合并
来源：http://lcb.bjfxy.top

{ ...a, ...b }
来源：http://hoa.andypj.xyz

[U89] JS：数组去重
来源：http://pcd.hesvh.cn

[...new Set(arr)]
来源：http://dqn.nwbrower.top

[U90] JS：数字数组排序
来源：http://oxu.ybcxt.top

[...arr].sort((a, b) => a - b)
来源：http://upt.jqgufenzy.top

[U91] JS：对象键值遍历
来源：http://bpr.zhaomingkeji.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rgx.cqqwz.cn

[U92] JS：深拷贝
来源：http://lmn.ybcxt.top

structuredClone(obj)
来源：http://mtk.shzxlz.cn

[U93] JS：模板字符串
来源：http://tvz.fzhhl.top

`共 ${n} 条`
来源：http://hwv.jiagoushi.top

[U94] JS：箭头函数
来源：http://sep.fktsv.cn

const double = x => x * 2;
来源：http://xjx.yvedp.cn

[U95] JS：Promise 包装
来源：http://jmq.quarkkingdee.top

new Promise((resolve, reject) => {})
来源：http://zfy.vqdsnc.cn

[U96] JS：async/await 与异常
来源：http://izq.hnqzz.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zeb.shuidangran.top

[U97] JS：并发请求
来源：http://ggr.gaohongyu789.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://saw.yvedp.cn

[U98] JS：fetch 带 JSON
来源：http://xuq.fzhhl.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ery.nanxuanxn.top

[U99] JS：事件监听
来源：http://yct.yuxming.cn

el.addEventListener("click", e => {})
来源：http://ldv.sufxvd.cn

[U100] JS：DOM 查询
来源：http://cfw.zhoulong.xyz

document.querySelector(".item")
来源：http://gbf.jqgfzy.top

[U101] JS：classList 操作
来源：http://ivw.hywenlv.cn

el.classList.toggle("active")
来源：http://edh.zhixingplan.top

[U102] JS：本地存储
来源：http://ruq.meibo888.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://nsi.ydjk.org.cn

[U103] JS：定时器
来源：http://ooz.cqqwz.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vsz.yvedp.cn

[U104] JS：防抖
来源：http://dba.cashguo.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zqz.9152youxi.cn

[U105] JS：节流
来源：http://usq.tianlin.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fvy.wangdashe.top

[U106] JS：日期格式化
来源：http://hjx.sjlbkw.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dcs.yuanzhike.top

[U107] JS：数字千分位
来源：http://ixk.feifeiyinyue.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jdk.jqgufenzy.top

[U108] JS：随机整数
来源：http://gsb.ppjwa.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ios.ehwqpu.com

[U109] JS：数组分组
来源：http://kii.ydjk.org.cn

Object.groupBy(arr, x => x.type)
来源：http://kmw.yongpay.top

[U110] JS：数组分块
来源：http://ubo.daria6918.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gng.cucudq.cn

[U111] JS：对象转 Map
来源：http://tva.chenjidiqi.icu

new Map(Object.entries(obj))
来源：http://jmf.jinqigufen.top

[U112] JS：字符串补位
来源：http://ckk.hnxiangtu.top

"7".padStart(3, "0")
来源：http://mtv.sufxvd.cn

[U113] JS：正则替换全部
来源：http://wta.xziqi.cn

s.replaceAll("a", "b")
来源：http://vop.shangyingyoupin.top

[U114] JS：JSON 深比较
来源：http://yjm.xuetiantiany.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://acm.cucudq.cn

[U115] JS：生成 UUID
来源：http://jcy.yj20258888.top

crypto.randomUUID()
来源：http://bmi.nanxuanxn.top

[U116] JS：类型检查（JSDoc）
来源：http://jai.jqgufenzy.top

/** @param {string} name */ function f(name) {}
来源：http://pqu.yongpay.top

[U117] JS：单元测试
来源：http://dap.yueranfly.top

npm i -D vitest;  npx vitest
来源：http://ryn.meibo888.top

[U118] JS：开发服务器
来源：http://zxt.ydzc1.top

npm i -D vite;  npx vite
来源：http://yig.dianchejie.cn

[U119] JS：生产构建
来源：http://jpz.bjfxy.top

npx vite build
来源：http://ipu.zhoulong.xyz

[U120] JS：读取环境变量（Vite）
来源：http://ukb.gaohongyu789.top

import.meta.env.VITE_API_URL
来源：http://kcy.jinqigfzy.top

================================================================================
来源：http://pat.epnwcf.com

统计汇总
来源：http://jax.ctjpmb.com

================================================================================
来源：http://szb.yanxiufei.cn

按语言统计（条）：
来源：http://fkn.zhixingplan.top

Python ......... 252
来源：http://cou.pycfn.com

PHP ............ 252
来源：http://nhr.jinqigfzy.top

JavaScript ..... 252
来源：http://squ.mhx1999.top

TypeScript ..... 212
来源：http://gvh.mhx1999.top

Java ........... 212
来源：http://efh.hysaishi.cn

Go ............. 212
来源：http://wvk.xylfe.cn

Ruby ........... 212
来源：http://evx.uphjek.com

C# ............. 212
来源：http://vgf.daria6918.cn

C .............. 30
来源：http://pzc.zdqjudy.top

C++ ............ 30
来源：http://pur.gzhubu.top

SQL ............ 90
来源：http://whj.yfazqb.com

Bash ........... 80
来源：http://rvy.shzxlz.cn

Kotlin ......... 15
来源：http://xen.ehwqpu.com

Swift .......... 15
来源：http://vdt.yangfankeji.com

Lua ............ 10
来源：http://lmk.yj202588.top

Perl ........... 10
来源：http://qaw.yanxiufei.cn

Scala .......... 10
来源：http://nod.tarul.cn

------------------------------------
来源：http://rlr.chenjidiqi.icu

合计 ........... 2106 条
来源：http://axc.ydjk.org.cn

按章节统计：
来源：http://cph.xuetiantiany.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gzr.ivvv.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nad.sjlbkw.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://imo.dashuyun.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zyw.iojbl.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lwc.shanyushiyangkeji.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://odz.mhx1999.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lyi.uphjek.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wee.jlsjyb.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qpa.ybcxt.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ydk.fanxiaobao.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://agu.tarul.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ybp.gotoacloud.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yru.jqgfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lpj.tianlin.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://iih.quarkkingdee.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ruv.wangdashe.top

Q SQL 专题                              90
来源：http://mbi.cashguo.top

R Bash 专题                             80
来源：http://ana.ydjk.org.cn

S C / C++ 专题                          60
来源：http://kkw.jinqigfzy.top

T 其他语言补充                          60
来源：http://dnr.zdqjudy.top

U 高频实用片段                         120
来源：http://igb.daria6918.cn

------------------------------------
来源：http://hxx.yongpay.top

合计                                  2106 条
来源：http://ome.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://nav.wangdashe.top

使用提醒
来源：http://fzi.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://ult.hammf.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wfv.hywenlv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jko.dianchejie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tci.zhijiandao.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zlz.guowangkeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gvv.yangfankeji.com

—— 文件结束 ——
来源：http://rro.svipenyu.cn

================================================================================
来源：http://iaz.hammf.cn

程序语言常见例子速查手册（2024 版）
来源：http://gbl.hysaishi.cn

Common Programming Examples Cheat Book
来源：http://dex.jinqigfzy.top

================================================================================
来源：http://ohs.iojbl.cn

【收录内容】
来源：http://wek.ctjpmb.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://lah.yongpay.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wpl.yueranfly.top

SQL · Bash · C · C++
来源：http://bcw.shangyingyoupin.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mxr.cheryme.top

【使用说明】
来源：http://wxy.fengsongda.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ifr.nwbrower.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rzm.tianlin.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mbh.hammf.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://amt.zhongyouzk.top

Bash:  Shell         C:     C             C++:   C++
来源：http://cqg.zhijiandao.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vdn.jlsjyb.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pkv.tarul.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pgx.zdbjq.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rut.9152youxi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://grz.haohaochexian.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://exp.xuanzx.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wrv.aibaodan.cn

【文件统计】
来源：http://kql.guannengcc.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ewr.birdmap.top

--------------------------------------------------------------------------------
来源：http://dao.feifeiyinyue.top

目  录
来源：http://sdd.shuidangran.top

--------------------------------------------------------------------------------
来源：http://fqu.gzhubu.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://min.cheryme.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://egv.yueranfly.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kuw.ydjk.org.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wyb.guowangkeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fii.gogol.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hzt.shangyingyoupin.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bni.xinyue.icu

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ogz.yfazqb.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vew.yj20258888.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jjl.dashuyun.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tup.hongshengwenyu.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dfv.meibo888.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yzx.epnwcf.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ler.ivvv.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uvt.nanxuanxn.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vtx.zhaomingkeji.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pqw.ywan-chungtsiang.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://slt.ydjk.org.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wiv.svipenyu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uff.fktsv.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qus.yfazqb.com

================================================================================
来源：http://hcz.jinghuilouyu.cn

A. 基础语法与类型
来源：http://sgw.sufxvd.cn

================================================================================
来源：http://xsi.hnqzz.top

[A01] Hello World
来源：http://bnw.cdnleiting.top

Py:   print("Hello, World!")
来源：http://jnp.hnxiangtu.top

PHP:  echo "Hello, World!";
来源：http://ogn.fehbvm.com

JS:   console.log("Hello, World!");
来源：http://exz.pengpengdd.cyou

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wnc.hywenlv.cn

Java: System.out.println("Hello, World!");
来源：http://ves.ydjk.org.cn

Go:   fmt.Println("Hello, World!")
来源：http://qts.hcnkem.com

Ruby: puts "Hello, World!"
来源：http://idb.tianlin.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://vyp.guowangkeji.top

[A02] 变量声明与赋值
来源：http://rnf.hnxiangtu.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://oir.xuanzx.com

PHP:  $name = "Alex"; $age = 20;
来源：http://pna.yuanzhike.top

JS:   let name = "Alex"; const age = 20;
来源：http://avh.ywan-chungtsiang.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vwm.feifeiyinyue.top

Java: String name = "Alex"; int age = 20;
来源：http://vsp.tian-w.cn

Go:   name := "Alex"; age := 20
来源：http://fqw.jianghu66.top

Ruby: name = "Alex"; age = 20
来源：http://iel.xuanzx.com

C#:   string name = "Alex"; int age = 20;
来源：http://gyo.yonumen.top

[A03] 常量定义
来源：http://tuw.hnxiangtu.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://itx.sufxvd.cn

PHP:  const PI = 3.14159;
来源：http://xcp.tian-w.cn

JS:   const PI = 3.14159;
来源：http://dck.fzhhl.top

TS:   const PI: number = 3.14159;
来源：http://rvm.yuxming.cn

Java: static final double PI = 3.14159;
来源：http://czf.nanxinkj.top

Go:   const PI = 3.14159
来源：http://dfo.yuanzhike.top

Ruby: PI = 3.14159
来源：http://fvp.shangyingyoupin.top

C#:   const double PI = 3.14159;
来源：http://ynp.jiagoushi.top

[A04] 判断变量类型
来源：http://pcy.aizwys.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tbf.daxiang520.top


<!-- 参考信息 -->