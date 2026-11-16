代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://kvi.yanxiufei.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://myn.guowangkeji.top

[U46] PHP：可空类型
来源：http://xxx.cheryme.top

?string $name = null
来源：http://ifj.gotoacloud.top

[U47] PHP：联合类型
来源：http://vcx.hongshengwenyu.top

int|string $id
来源：http://wtd.fengsongda.top

[U48] PHP：纯枚举
来源：http://uuc.bjfxy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xbt.ywan-chungtsiang.top

[U49] PHP：只读属性
来源：http://pjw.yangfankeji.com

public readonly string $name
来源：http://tux.hesvh.cn

[U50] PHP：构造器属性提升
来源：http://fza.guowangkeji.top

public function __construct(private int $id) {}
来源：http://wib.zhongyouzk.top

[U51] PHP：数组解构
来源：http://boo.wangdashe.top

[$a, $b] = $arr;
来源：http://jfu.yuanzhike.top

[U52] PHP：箭头函数
来源：http://qki.snrcjt.cn

$double = fn($x) => $x * 2;
来源：http://fmq.ybcxt.top

[U53] PHP：空合并运算符
来源：http://xtz.nanxuanxn.top

$v = $a ?? $b ?? "default";
来源：http://znr.hammf.cn

[U54] PHP：空安全调用
来源：http://scy.jiagoushi.top

$obj?->method()
来源：http://jcs.snrcjt.cn

[U55] PHP：match 表达式
来源：http://raq.jinghuilouyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ssf.ehwqpu.com

[U56] PHP：命名参数
来源：http://ezu.shuidangran.top

f(a: 1, b: 2)
来源：http://fvl.iojbl.cn

[U57] PHP：字符串插值
来源：http://hpt.hywenlv.cn

"值: {$a}"
来源：http://qvb.fktsv.cn

[U58] PHP：数组三件套
来源：http://cba.svipenyu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ldb.dianchejie.cn

[U59] PHP：自定义排序
来源：http://osg.ydjk.org.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ylx.kuanghao11.cn

[U60] PHP：JSON 编解码
来源：http://pag.xylfe.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rwd.bjfxy.top

[U61] PHP：正则
来源：http://tcu.aizwys.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jdw.shangyingyoupin.top

[U62] PHP：日期对象
来源：http://fup.tian-w.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lmd.tianlin.xyz

[U63] PHP：文件读写
来源：http://pfa.jianghu66.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pcv.52xcode.cn

[U64] PHP：目录遍历
来源：http://ygy.cucudq.cn

glob("dir/*.php");  scandir("dir");
来源：http://pay.yangfankeji.com

[U65] PHP：会话
来源：http://ntq.svipenyu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fbh.zhoulong.xyz

[U66] PHP：设置 Cookie
来源：http://umv.epnwcf.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hwd.andypj.xyz

[U67] PHP：处理文件上传
来源：http://fsh.jlsjyb.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://koo.jiagoushi.top

[U68] PHP：PDO 连接
来源：http://uvi.jyoumei.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jmt.tian-w.cn

[U69] PHP：PDO 预处理
来源：http://laf.shanyushiyangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vfr.sjlbkw.cn

[U70] PHP：PDO 事务
来源：http://eqj.yuanzhike.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wcr.svipenyu.cn

[U71] PHP：抛出异常
来源：http://blt.xinyue.icu

throw new RuntimeException("失败", 500);
来源：http://dvu.yuanzhike.top

[U72] PHP：写错误日志
来源：http://sfl.jqgfzy.top

error_log("失败: " . $e->getMessage());
来源：http://foo.aizwys.cn

[U73] PHP：读取 ini 配置
来源：http://dtg.jqgufenzy.top

parse_ini_file("config.ini", true)
来源：http://uij.fehbvm.com

[U74] PHP：读取环境变量
来源：http://vrz.smart0.xyz

getenv("APP_ENV") ?: "production"
来源：http://zbc.epnwcf.com

[U75] PHP：依赖注入
来源：http://iuw.dashuyun.cn

composer require psr/container
来源：http://soz.xuetiantiany.cn

[U76] PHP：简单路由
来源：http://tab.cashguo.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://roo.guowangkeji.top

[U77] PHP：模板渲染
来源：http://ehq.gaohongyu789.top

composer require twig/twig
来源：http://mul.fengsongda.top

[U78] PHP：单元测试
来源：http://pnj.dashuyun.cn

composer require --dev phpunit/phpunit
来源：http://zsg.shzxlz.cn

[U79] PHP：静态分析
来源：http://ckg.0kj1m.cn

composer require --dev phpstan/phpstan
来源：http://dhj.cashguo.top

[U80] PHP：代码规范修复
来源：http://hqa.shzxlz.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kku.yangfankeji.com

[U81] JS：初始化项目
来源：http://dam.xinyue.icu

npm init -y;  npm i express
来源：http://obh.tanke756.top

[U82] JS：package.json 脚本
来源：http://mpg.9152youxi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pvz.tianlin.xyz

[U83] JS：ES Module 导入导出
来源：http://nmq.yonumen.top

export const a = 1;  import { a } from "./m.js";
来源：http://jhn.birdmap.top

[U84] JS：CommonJS 写法
来源：http://gro.jqgufenzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://bne.aibaodan.cn

[U85] JS：可选链
来源：http://ijq.feifeiyinyue.top

a?.b?.c
来源：http://sjy.svipenyu.cn

[U86] JS：空值合并
来源：http://rdf.ehwqpu.com

a ?? b
来源：http://yea.tarul.cn

[U87] JS：解构默认值
来源：http://mch.sweek.top

const { a = 1, b = 2 } = obj;
来源：http://jxd.uphjek.com

[U88] JS：对象展开合并
来源：http://etj.zhoulong.xyz

{ ...a, ...b }
来源：http://nwe.mhx1999.top

[U89] JS：数组去重
来源：http://fxr.fengsongda.top

[...new Set(arr)]
来源：http://dfz.9152youxi.cn

[U90] JS：数字数组排序
来源：http://tsm.ivvv.top

[...arr].sort((a, b) => a - b)
来源：http://ysj.ehwqpu.com

[U91] JS：对象键值遍历
来源：http://qvj.zdqjudy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fik.gaohongyu789.top

[U92] JS：深拷贝
来源：http://bvj.ywan-chungtsiang.top

structuredClone(obj)
来源：http://pmd.yuanzhike.top

[U93] JS：模板字符串
来源：http://jhi.xinyue.icu

`共 ${n} 条`
来源：http://ooy.bjfxy.top

[U94] JS：箭头函数
来源：http://xwi.pycfn.com

const double = x => x * 2;
来源：http://trl.haohaochexian.top

[U95] JS：Promise 包装
来源：http://wpr.yj20258.top

new Promise((resolve, reject) => {})
来源：http://omx.ydjk.org.cn

[U96] JS：async/await 与异常
来源：http://pji.hcnkem.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ncs.jinqigufen.top

[U97] JS：并发请求
来源：http://zrk.cashguo.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://mmd.jianghu66.top

[U98] JS：fetch 带 JSON
来源：http://vaz.yj202588.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bur.meibo888.top

[U99] JS：事件监听
来源：http://hgh.ydjk.org.cn

el.addEventListener("click", e => {})
来源：http://riw.sjlbkw.cn

[U100] JS：DOM 查询
来源：http://mjg.hysaishi.cn

document.querySelector(".item")
来源：http://pcg.hongshengwenyu.top

[U101] JS：classList 操作
来源：http://sxh.smart0.xyz

el.classList.toggle("active")
来源：http://asc.ydzc1.top

[U102] JS：本地存储
来源：http://nat.zdqjudy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://bmq.c1oappe.top

[U103] JS：定时器
来源：http://psp.vqdsnc.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ptp.havefunace.top

[U104] JS：防抖
来源：http://pka.nanxinkj.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://glu.yanxiufei.cn

[U105] JS：节流
来源：http://ngv.zhongyouzk.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hbx.jyoumei.cn

[U106] JS：日期格式化
来源：http://ncm.nanxinkj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pye.redwolf501.top

[U107] JS：数字千分位
来源：http://ynt.zhaomingkeji.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://aek.xinyue.icu

[U108] JS：随机整数
来源：http://tmv.zhongyouzk.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mnf.sysykeji.top

[U109] JS：数组分组
来源：http://ylo.jinyuanbaomall.cn

Object.groupBy(arr, x => x.type)
来源：http://daw.tian-w.cn

[U110] JS：数组分块
来源：http://lyy.andypj.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nxf.vqdsnc.cn

[U111] JS：对象转 Map
来源：http://les.meibo888.top

new Map(Object.entries(obj))
来源：http://cdb.chenlongwang.top

[U112] JS：字符串补位
来源：http://tgn.jlsjyb.cn

"7".padStart(3, "0")
来源：http://kud.shuidangran.top

[U113] JS：正则替换全部
来源：http://geu.zhijiandao.cn

s.replaceAll("a", "b")
来源：http://xzb.zhiwuduotai.top

[U114] JS：JSON 深比较
来源：http://ikw.zhijiandao.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dve.tian-w.cn

[U115] JS：生成 UUID
来源：http://dvc.fengsongda.top

crypto.randomUUID()
来源：http://grz.0kj1m.cn

[U116] JS：类型检查（JSDoc）
来源：http://keb.yongpay.top

/** @param {string} name */ function f(name) {}
来源：http://tmt.uphjek.com

[U117] JS：单元测试
来源：http://flu.sufxvd.cn

npm i -D vitest;  npx vitest
来源：http://wns.jiagoushi.top

[U118] JS：开发服务器
来源：http://qyy.bbcook.cn

npm i -D vite;  npx vite
来源：http://ifi.9152youxi.cn

[U119] JS：生产构建
来源：http://asi.zhixingplan.top

npx vite build
来源：http://lxq.jinqigfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://ekr.fengsongda.top

import.meta.env.VITE_API_URL
来源：http://ayw.yueranfly.top

================================================================================
来源：http://hld.yueranfly.top

统计汇总
来源：http://wfk.yfazqb.com

================================================================================
来源：http://uio.yanxiufei.cn

按语言统计（条）：
来源：http://jsk.cucudq.cn

Python ......... 252
来源：http://qhz.epnwcf.com

PHP ............ 252
来源：http://kyk.sysykeji.top

JavaScript ..... 252
来源：http://xef.smart0.xyz

TypeScript ..... 212
来源：http://mrl.sjlbkw.cn

Java ........... 212
来源：http://qwx.yongpay.top

Go ............. 212
来源：http://pwu.yonumen.top

Ruby ........... 212
来源：http://qeq.nanxinkj.top

C# ............. 212
来源：http://luw.mhx1999.top

C .............. 30
来源：http://czd.guannengcc.top

C++ ............ 30
来源：http://fcf.xylfe.cn

SQL ............ 90
来源：http://yzj.hnqzz.top

Bash ........... 80
来源：http://guc.bbcook.cn

Kotlin ......... 15
来源：http://hzb.cucudq.cn

Swift .......... 15
来源：http://nkx.hongshengwenyu.top

Lua ............ 10
来源：http://kze.zdbjq.cn

Perl ........... 10
来源：http://mjk.sjlbkw.cn

Scala .......... 10
来源：http://xdu.fehbvm.com

------------------------------------
来源：http://hyq.yj20258.top

合计 ........... 2106 条
来源：http://him.hysaishi.cn

按章节统计：
来源：http://pyd.9152youxi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fmz.vqdsnc.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fir.shuidangran.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vuw.jinqigufen.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ssr.bjfxy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nmb.gotoacloud.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qvr.ctjpmb.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bms.xuetiantiany.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://iod.ctjpmb.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wti.zycfv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qsf.pycfn.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jhl.hywenlv.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://eqk.9152youxi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ehd.hesvh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://efi.tanke756.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kbs.svipenyu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://prq.shuidangran.top

Q SQL 专题                              90
来源：http://jqr.jiagoushi.top

R Bash 专题                             80
来源：http://xxq.wangshuangyany.cn

S C / C++ 专题                          60
来源：http://hfw.vqdsnc.cn

T 其他语言补充                          60
来源：http://ulr.shanyushiyangkeji.top

U 高频实用片段                         120
来源：http://kxp.tian-w.cn

------------------------------------
来源：http://bqn.bjfxy.top

合计                                  2106 条
来源：http://yak.redwolf501.top

--------------------------------------------------------------------------------
来源：http://kli.316326.xyz

使用提醒
来源：http://nsp.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://dvw.yangfankeji.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yds.zhengqikj.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rhw.cheryme.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zxg.zycfv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qpj.fehbvm.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hvr.xziqi.cn

—— 文件结束 ——
来源：http://fol.xziqi.cn

================================================================================
来源：http://rrm.xuetiantiany.cn

程序语言常见例子速查手册（2024 版）
来源：http://zsy.yj202588.top

Common Programming Examples Cheat Book
来源：http://jom.andypj.xyz

================================================================================
来源：http://zao.mhx1999.top

【收录内容】
来源：http://thr.ctjpmb.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://tcw.feifeiyinyue.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cod.xinyue.icu

SQL · Bash · C · C++
来源：http://hdd.hnqzz.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://auj.cqqwz.cn

【使用说明】
来源：http://pjt.pycfn.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pqq.yfazqb.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qkz.vehdjk.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nby.jinqigfzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ngj.iojbl.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://swp.redwolf501.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nql.ppjwa.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tpq.bjfxy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qao.9152youxi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://twu.zdbjq.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dmt.ydzc1.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qou.nanxinkj.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://odo.tarul.cn

【文件统计】
来源：http://hyj.nwbrower.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ryj.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://nuk.daxiang520.top

目  录
来源：http://tum.jiagoushi.top

--------------------------------------------------------------------------------
来源：http://oge.havefunace.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gkh.snrcjt.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xuz.quarkkingdee.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://anc.haohaochexian.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yla.vehdjk.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bon.cdnleiting.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://eke.gogol.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kzz.sweek.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://abd.hnxiangtu.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jtg.ydjk.org.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://huc.yj20258888.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vyg.chenzaomai.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tme.yueranfly.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kfu.zhaomingkeji.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://odx.snrcjt.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nag.svipenyu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://slb.ydzc1.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cfj.uphjek.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://tad.yanxiufei.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://igi.yj20258.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://eer.shuidangran.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://onx.shanyushiyangtech.top

================================================================================
来源：http://lbz.guannengcc.top

A. 基础语法与类型
来源：http://wug.daxiang520.top

================================================================================
来源：http://ely.tanke756.top

[A01] Hello World
来源：http://cud.ywan-chungtsiang.top

Py:   print("Hello, World!")
来源：http://cwc.nwbrower.top

PHP:  echo "Hello, World!";
来源：http://lch.yueranfly.top

JS:   console.log("Hello, World!");
来源：http://mjm.zdqjudy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bxp.sweek.top

Java: System.out.println("Hello, World!");
来源：http://dal.52xcode.cn

Go:   fmt.Println("Hello, World!")
来源：http://bwu.gogol.net.cn

Ruby: puts "Hello, World!"
来源：http://ybw.sysykeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://uhn.smart0.xyz

[A02] 变量声明与赋值
来源：http://sdj.wangshuangyany.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://aky.cucudq.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qbz.havefunace.top

JS:   let name = "Alex"; const age = 20;
来源：http://aqj.jiagoushi.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nds.zhiwuduotai.top

Java: String name = "Alex"; int age = 20;
来源：http://zkw.redwolf501.top

Go:   name := "Alex"; age := 20
来源：http://rxf.zycfv.cn

Ruby: name = "Alex"; age = 20
来源：http://qnh.fengsongda.top

C#:   string name = "Alex"; int age = 20;
来源：http://cju.9152youxi.cn

[A03] 常量定义
来源：http://jti.cheryme.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ofa.epnwcf.com

PHP:  const PI = 3.14159;
来源：http://abx.ctjpmb.com

JS:   const PI = 3.14159;
来源：http://bty.dashuyun.cn

TS:   const PI: number = 3.14159;
来源：http://sdf.zhengqikj.top

Java: static final double PI = 3.14159;
来源：http://ygu.sweek.top

Go:   const PI = 3.14159
来源：http://ker.cucudq.cn

Ruby: PI = 3.14159
来源：http://xls.fzhhl.top

C#:   const double PI = 3.14159;
来源：http://uwa.dashuyun.cn

[A04] 判断变量类型
来源：http://jmc.tian-w.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ujn.gogol.net.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vim.316326.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qgb.fengsongda.top

TS:   typeof x; x instanceof Date
来源：http://wdr.hongshengwenyu.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fpd.nwbrower.top

Go:   reflect.TypeOf(x).Name()
来源：http://egi.meibo888.top

Ruby: x.class; x.is_a?(Integer)
来源：http://zvp.ydjk.org.cn

C#:   x.GetType().Name; x is int
来源：http://tyi.9152youxi.cn

[A05] 整数除法与取模
来源：http://hfw.xinyue.icu

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://joj.snrcjt.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://khw.cqqwz.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bty.nanxinkj.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vej.ybcxt.top


<!-- 参考信息 -->