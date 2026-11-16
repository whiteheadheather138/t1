代发 wailian999

[U47] PHP：联合类型
来源：http://eow.jianghu66.top

int|string $id
来源：http://kao.guannengcc.top

[U48] PHP：纯枚举
来源：http://jaz.0kj1m.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lpn.hesvh.cn

[U49] PHP：只读属性
来源：http://czq.jinqigfzy.top

public readonly string $name
来源：http://ypw.ywan-chungtsiang.top

[U50] PHP：构造器属性提升
来源：http://xsg.zhoulong.xyz

public function __construct(private int $id) {}
来源：http://fvw.fehbvm.com

[U51] PHP：数组解构
来源：http://vll.jlsjyb.cn

[$a, $b] = $arr;
来源：http://egp.meibo888.top

[U52] PHP：箭头函数
来源：http://xxp.vqdsnc.cn

$double = fn($x) => $x * 2;
来源：http://xer.sufxvd.cn

[U53] PHP：空合并运算符
来源：http://iuz.aibaodan.cn

$v = $a ?? $b ?? "default";
来源：http://pul.feifeiyinyue.top

[U54] PHP：空安全调用
来源：http://myv.jqgfzy.top

$obj?->method()
来源：http://wwz.gzhubu.top

[U55] PHP：match 表达式
来源：http://vgp.jinghuilouyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rcd.gaohongyu789.top

[U56] PHP：命名参数
来源：http://hrg.c1oappe.top

f(a: 1, b: 2)
来源：http://ghf.haohaochexian.top

[U57] PHP：字符串插值
来源：http://gcz.svipenyu.cn

"值: {$a}"
来源：http://nnr.ydjk.org.cn

[U58] PHP：数组三件套
来源：http://zlv.sjlbkw.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gyn.zycfv.cn

[U59] PHP：自定义排序
来源：http://glg.tarul.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lmp.andypj.xyz

[U60] PHP：JSON 编解码
来源：http://eie.yj20258888.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pcp.jqgfzy.top

[U61] PHP：正则
来源：http://uhk.jqgufenzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vpf.tian-w.cn

[U62] PHP：日期对象
来源：http://yhf.hnxiangtu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bai.sjlbkw.cn

[U63] PHP：文件读写
来源：http://szb.iojbl.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ybn.yonumen.top

[U64] PHP：目录遍历
来源：http://ydq.gzhubu.top

glob("dir/*.php");  scandir("dir");
来源：http://egq.yueranfly.top

[U65] PHP：会话
来源：http://iha.tianlin.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://yxn.yj20258888.top

[U66] PHP：设置 Cookie
来源：http://gmx.chenlongwang.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://njb.fengsongda.top

[U67] PHP：处理文件上传
来源：http://qca.jiagoushi.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nkp.nwbrower.top

[U68] PHP：PDO 连接
来源：http://fky.shangyingyoupin.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tgk.jinqigufen.top

[U69] PHP：PDO 预处理
来源：http://qxe.yvedp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dau.0kj1m.cn

[U70] PHP：PDO 事务
来源：http://uqi.sysykeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qjo.jqgufenzy.top

[U71] PHP：抛出异常
来源：http://jic.fktsv.cn

throw new RuntimeException("失败", 500);
来源：http://lsq.aibaodan.cn

[U72] PHP：写错误日志
来源：http://fxb.zhiwuduotai.top

error_log("失败: " . $e->getMessage());
来源：http://gnl.ivvv.top

[U73] PHP：读取 ini 配置
来源：http://eaa.tanke756.top

parse_ini_file("config.ini", true)
来源：http://mid.vehdjk.com

[U74] PHP：读取环境变量
来源：http://jyz.jinghuilouyu.cn

getenv("APP_ENV") ?: "production"
来源：http://imy.hnqzz.top

[U75] PHP：依赖注入
来源：http://hnz.mhx1999.top

composer require psr/container
来源：http://vpp.redwolf501.top

[U76] PHP：简单路由
来源：http://kxd.cdnleiting.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hqa.sysykeji.top

[U77] PHP：模板渲染
来源：http://jzp.zhoulong.xyz

composer require twig/twig
来源：http://puq.yuxming.cn

[U78] PHP：单元测试
来源：http://mne.fktsv.cn

composer require --dev phpunit/phpunit
来源：http://hxg.yj20258.top

[U79] PHP：静态分析
来源：http://qtd.gogol.net.cn

composer require --dev phpstan/phpstan
来源：http://kjv.yangfankeji.com

[U80] PHP：代码规范修复
来源：http://rhc.zhaomingkeji.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://jue.gaohongyu789.top

[U81] JS：初始化项目
来源：http://myw.9152youxi.cn

npm init -y;  npm i express
来源：http://slf.yuxming.cn

[U82] JS：package.json 脚本
来源：http://pcs.cashguo.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://iiy.zhongyouzk.top

[U83] JS：ES Module 导入导出
来源：http://rwc.fzhhl.top

export const a = 1;  import { a } from "./m.js";
来源：http://byn.c1oappe.top

[U84] JS：CommonJS 写法
来源：http://odl.yj20258.top

module.exports = { a };  const { a } = require("./m");
来源：http://kjp.zhixingplan.top

[U85] JS：可选链
来源：http://dxd.gotoacloud.top

a?.b?.c
来源：http://xbo.epnwcf.com

[U86] JS：空值合并
来源：http://vlu.jinqigfzy.top

a ?? b
来源：http://pcf.gaohongyu789.top

[U87] JS：解构默认值
来源：http://kjk.zycfv.cn

const { a = 1, b = 2 } = obj;
来源：http://kfv.ivvv.top

[U88] JS：对象展开合并
来源：http://obz.yfazqb.com

{ ...a, ...b }
来源：http://iik.xingfuxueyuan.xyz

[U89] JS：数组去重
来源：http://zxj.shzxlz.cn

[...new Set(arr)]
来源：http://hdu.zhongyouzk.top

[U90] JS：数字数组排序
来源：http://utp.jinqigufen.top

[...arr].sort((a, b) => a - b)
来源：http://tzz.redwolf501.top

[U91] JS：对象键值遍历
来源：http://bcb.fengsongda.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zpv.meibo888.top

[U92] JS：深拷贝
来源：http://phk.cucudq.cn

structuredClone(obj)
来源：http://xbh.zdqjudy.top

[U93] JS：模板字符串
来源：http://hbr.yuxming.cn

`共 ${n} 条`
来源：http://cjq.jinghuilouyu.cn

[U94] JS：箭头函数
来源：http://lcz.hysaishi.cn

const double = x => x * 2;
来源：http://fif.ppjwa.cn

[U95] JS：Promise 包装
来源：http://qtb.gogol.net.cn

new Promise((resolve, reject) => {})
来源：http://mgm.yanxiufei.cn

[U96] JS：async/await 与异常
来源：http://wcj.yangfankeji.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pha.cucudq.cn

[U97] JS：并发请求
来源：http://rrq.hammf.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dpx.snrcjt.cn

[U98] JS：fetch 带 JSON
来源：http://hjz.xingfuxueyuan.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mpl.zhongyouzk.top

[U99] JS：事件监听
来源：http://gft.zycfv.cn

el.addEventListener("click", e => {})
来源：http://ptu.bbcook.cn

[U100] JS：DOM 查询
来源：http://out.zhijiandao.cn

document.querySelector(".item")
来源：http://etl.aizwys.cn

[U101] JS：classList 操作
来源：http://bnq.hnqzz.top

el.classList.toggle("active")
来源：http://dum.gotoacloud.top

[U102] JS：本地存储
来源：http://jnh.aizwys.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nks.tarul.cn

[U103] JS：定时器
来源：http://vea.0kj1m.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ubx.ehwqpu.com

[U104] JS：防抖
来源：http://fml.tianlin.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zkb.0kj1m.cn

[U105] JS：节流
来源：http://lym.xinyue.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://owo.daxiang520.top

[U106] JS：日期格式化
来源：http://suq.chenzaomai.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ona.dianchejie.cn

[U107] JS：数字千分位
来源：http://kxt.zhaomingkeji.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cog.havefunace.top

[U108] JS：随机整数
来源：http://oni.haohaochexian.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ebg.gogol.net.cn

[U109] JS：数组分组
来源：http://hab.shzxlz.cn

Object.groupBy(arr, x => x.type)
来源：http://lri.cheryme.top

[U110] JS：数组分块
来源：http://jdp.havefunace.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ncl.nwbrower.top

[U111] JS：对象转 Map
来源：http://lmi.52xcode.cn

new Map(Object.entries(obj))
来源：http://aro.yangfankeji.com

[U112] JS：字符串补位
来源：http://rri.hcnkem.com

"7".padStart(3, "0")
来源：http://kyl.smart0.xyz

[U113] JS：正则替换全部
来源：http://ilk.yuxming.cn

s.replaceAll("a", "b")
来源：http://iaj.0kj1m.cn

[U114] JS：JSON 深比较
来源：http://epb.meibo888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://uqn.nanxuanxn.top

[U115] JS：生成 UUID
来源：http://lhb.yj20258888.top

crypto.randomUUID()
来源：http://kjp.jiagoushi.top

[U116] JS：类型检查（JSDoc）
来源：http://aow.yj202588.top

/** @param {string} name */ function f(name) {}
来源：http://sjn.jiagoushi.top

[U117] JS：单元测试
来源：http://eqc.hywenlv.cn

npm i -D vitest;  npx vitest
来源：http://pat.birdmap.top

[U118] JS：开发服务器
来源：http://bcg.daria6918.cn

npm i -D vite;  npx vite
来源：http://syd.nwbrower.top

[U119] JS：生产构建
来源：http://lzt.shuidangran.top

npx vite build
来源：http://tdu.wangdashe.top

[U120] JS：读取环境变量（Vite）
来源：http://yks.snrcjt.cn

import.meta.env.VITE_API_URL
来源：http://yip.zhiwuduotai.top

================================================================================
来源：http://cpj.shzxlz.cn

统计汇总
来源：http://ilk.tanke756.top

================================================================================
来源：http://ypi.52xcode.cn

按语言统计（条）：
来源：http://tyd.cashguo.top

Python ......... 252
来源：http://vxp.epnwcf.com

PHP ............ 252
来源：http://zlg.yongpay.top

JavaScript ..... 252
来源：http://oyd.chenlongwang.top

TypeScript ..... 212
来源：http://rxa.fanxiaobao.xyz

Java ........... 212
来源：http://qir.cucudq.cn

Go ............. 212
来源：http://ccu.vqdsnc.cn

Ruby ........... 212
来源：http://ckl.fzhhl.top

C# ............. 212
来源：http://vae.snrcjt.cn

C .............. 30
来源：http://aac.sufxvd.cn

C++ ............ 30
来源：http://sjp.sweek.top

SQL ............ 90
来源：http://nei.yvedp.cn

Bash ........... 80
来源：http://etz.jyoumei.cn

Kotlin ......... 15
来源：http://vrj.cucudq.cn

Swift .......... 15
来源：http://juw.yj20258888.top

Lua ............ 10
来源：http://jmm.gogol.net.cn

Perl ........... 10
来源：http://asb.nwbrower.top

Scala .......... 10
来源：http://mst.hnxiangtu.top

------------------------------------
来源：http://aup.316326.xyz

合计 ........... 2106 条
来源：http://hok.fzhhl.top

按章节统计：
来源：http://xxb.tanke756.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://asu.zycfv.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bws.hcnkem.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jhz.hcnkem.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vyq.hongshengwenyu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://koz.bbcook.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kym.daria6918.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fxa.shuidangran.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ymh.hammf.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tks.snrcjt.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ucz.tarul.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ato.zdqjudy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://aoy.chenlongwang.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ybm.wangdashe.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iby.wangdashe.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sri.guowangkeji.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://uoy.jinqigfzy.top

Q SQL 专题                              90
来源：http://lok.gzhubu.top

R Bash 专题                             80
来源：http://yzb.fanxiaobao.xyz

S C / C++ 专题                          60
来源：http://tvb.fktsv.cn

T 其他语言补充                          60
来源：http://xqd.xuetiantiany.cn

U 高频实用片段                         120
来源：http://icm.gotoacloud.top

------------------------------------
来源：http://din.shanyushiyangtech.top

合计                                  2106 条
来源：http://bov.yj202588.top

--------------------------------------------------------------------------------
来源：http://hgq.pengpengdd.cyou

使用提醒
来源：http://tja.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://oky.cqqwz.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dgm.jianghu66.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://eya.zhiwuduotai.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://quu.bjfxy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jrb.fzhhl.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mzr.iojbl.cn

—— 文件结束 ——
来源：http://spx.xylfe.cn

================================================================================
来源：http://qsl.jqgufenzy.top

程序语言常见例子速查手册（2024 版）
来源：http://bzu.ctjpmb.com

Common Programming Examples Cheat Book
来源：http://gxy.yj20258.top

================================================================================
来源：http://tmd.ehwqpu.com

【收录内容】
来源：http://yda.dashuyun.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zpb.uphjek.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zxz.ydzc1.top

SQL · Bash · C · C++
来源：http://drg.nanxuanxn.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://thl.hysaishi.cn

【使用说明】
来源：http://qyg.shanyushiyangtech.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ras.quarkkingdee.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dfe.nanxuanxn.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ipg.jqgfzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ubz.sjlbkw.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://nli.ydzc1.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pls.zhiwuduotai.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://glw.fktsv.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jky.hywenlv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ghs.cdnleiting.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ywx.yvedp.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://igm.jinqigufen.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bre.wangshuangyany.cn

【文件统计】
来源：http://xkn.zycfv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://swm.cucudq.cn

--------------------------------------------------------------------------------
来源：http://hvo.xziqi.cn

目  录
来源：http://qgb.redwolf501.top

--------------------------------------------------------------------------------
来源：http://ebz.cqqwz.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mqy.aizwys.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vri.ydjk.org.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fbo.jinqigfzy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://crn.snrcjt.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dhw.bjfxy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pgd.zhengqikj.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xec.cdnleiting.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://omm.aizwys.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lzi.cdnleiting.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xzy.xuetiantiany.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tbp.gogol.net.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mjh.hcnkem.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wub.dashuyun.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jop.shanyushiyangkeji.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ptz.iojbl.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ztw.shanyushiyangkeji.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rgg.xuetiantiany.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://laa.xingfuxueyuan.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dtx.nwbrower.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jzj.jinqigufen.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vef.jinyuanbaomall.cn

================================================================================
来源：http://gwa.zhaomingkeji.xyz

A. 基础语法与类型
来源：http://rjc.zdbjq.cn

================================================================================
来源：http://jch.yvedp.cn

[A01] Hello World
来源：http://ujc.sweek.top

Py:   print("Hello, World!")
来源：http://npj.vqdsnc.cn

PHP:  echo "Hello, World!";
来源：http://zta.ydjk.org.cn

JS:   console.log("Hello, World!");
来源：http://ppy.jqgfzy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ywd.jinghuilouyu.cn

Java: System.out.println("Hello, World!");
来源：http://rkv.ehwqpu.com

Go:   fmt.Println("Hello, World!")
来源：http://weo.fktsv.cn

Ruby: puts "Hello, World!"
来源：http://rui.daria6918.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://eqy.yvedp.cn

[A02] 变量声明与赋值
来源：http://vwi.wangshuangyany.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vxc.uphjek.com

PHP:  $name = "Alex"; $age = 20;
来源：http://zhf.shzxlz.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qxk.zhengqikj.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qwb.ppjwa.cn

Java: String name = "Alex"; int age = 20;
来源：http://pjn.hcnkem.com

Go:   name := "Alex"; age := 20
来源：http://djd.sxryk.cn

Ruby: name = "Alex"; age = 20
来源：http://cyb.zdqjudy.top

C#:   string name = "Alex"; int age = 20;
来源：http://zye.jinghuilouyu.cn

[A03] 常量定义
来源：http://adx.xuanzx.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mkn.xinyue.icu

PHP:  const PI = 3.14159;
来源：http://fvh.quarkkingdee.top

JS:   const PI = 3.14159;
来源：http://efs.yangfankeji.com

TS:   const PI: number = 3.14159;
来源：http://rmy.xuetiantiany.cn

Java: static final double PI = 3.14159;
来源：http://tvr.fzhhl.top

Go:   const PI = 3.14159
来源：http://rmf.jqgufenzy.top

Ruby: PI = 3.14159
来源：http://yns.tian-w.cn

C#:   const double PI = 3.14159;
来源：http://ngm.hnxiangtu.top

[A04] 判断变量类型
来源：http://byh.nwbrower.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://rjg.zhiwuduotai.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cqm.sufxvd.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://iom.havefunace.top

TS:   typeof x; x instanceof Date
来源：http://xbk.cdnleiting.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vrl.52xcode.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ccg.0kj1m.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hmq.hywenlv.cn

C#:   x.GetType().Name; x is int
来源：http://umr.hnqzz.top

[A05] 整数除法与取模
来源：http://yva.xuetiantiany.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vrh.vehdjk.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://hcp.zhoulong.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jvw.zdqjudy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://byj.jlsjyb.cn

Java: 7 / 2; 7 % 2
来源：http://nvy.ywan-chungtsiang.top

Go:   7 / 2; 7 % 2
来源：http://ntv.cashguo.top

Ruby: 7 / 2; 7 % 2
来源：http://wtx.shanyushiyangkeji.top

C#:   7 / 2; 7 % 2
来源：http://uvr.jianghu66.top


<!-- 参考信息 -->