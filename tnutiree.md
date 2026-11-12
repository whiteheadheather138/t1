代发 wailian999

[U49] PHP：只读属性
来源：http://myh.sjlbkw.cn

public readonly string $name
来源：http://pja.haohaochexian.top

[U50] PHP：构造器属性提升
来源：http://naw.hesvh.cn

public function __construct(private int $id) {}
来源：http://shu.ybcxt.top

[U51] PHP：数组解构
来源：http://uyu.jyoumei.cn

[$a, $b] = $arr;
来源：http://dhp.jqgfzy.top

[U52] PHP：箭头函数
来源：http://cux.yj202588.top

$double = fn($x) => $x * 2;
来源：http://vvy.tian-w.cn

[U53] PHP：空合并运算符
来源：http://eth.nanxuanxn.top

$v = $a ?? $b ?? "default";
来源：http://ydz.epnwcf.com

[U54] PHP：空安全调用
来源：http://xzv.hfpthk.cn

$obj?->method()
来源：http://rpc.zycfv.cn

[U55] PHP：match 表达式
来源：http://jai.jqgfzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nmj.yueranfly.top

[U56] PHP：命名参数
来源：http://euo.hcnkem.com

f(a: 1, b: 2)
来源：http://aqd.hnqzz.top

[U57] PHP：字符串插值
来源：http://seb.nanxuanxn.top

"值: {$a}"
来源：http://dit.fktsv.cn

[U58] PHP：数组三件套
来源：http://cfb.daxiang520.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ims.hesvh.cn

[U59] PHP：自定义排序
来源：http://kta.sufxvd.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ghh.zhoulong.xyz

[U60] PHP：JSON 编解码
来源：http://wqh.dianchejie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fca.zhiwuduotai.top

[U61] PHP：正则
来源：http://oft.hcnkem.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vyj.tianlin.xyz

[U62] PHP：日期对象
来源：http://yib.jqgfzy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mrk.hcnkem.com

[U63] PHP：文件读写
来源：http://psv.sufxvd.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hql.pycfn.com

[U64] PHP：目录遍历
来源：http://qfk.ppjwa.cn

glob("dir/*.php");  scandir("dir");
来源：http://hqp.sjlbkw.cn

[U65] PHP：会话
来源：http://cmy.chenlongwang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wya.nwbrower.top

[U66] PHP：设置 Cookie
来源：http://qwv.pengpengdd.cyou

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uje.fehbvm.com

[U67] PHP：处理文件上传
来源：http://cgp.yuanzhike.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mjc.havefunace.top

[U68] PHP：PDO 连接
来源：http://mrv.jinqigfzy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wtg.sweek.top

[U69] PHP：PDO 预处理
来源：http://xud.fktsv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dea.gaohongyu789.top

[U70] PHP：PDO 事务
来源：http://zkq.hnqzz.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ipu.jyoumei.cn

[U71] PHP：抛出异常
来源：http://nsf.cqqwz.cn

throw new RuntimeException("失败", 500);
来源：http://syy.sufxvd.cn

[U72] PHP：写错误日志
来源：http://sos.yuanzhike.top

error_log("失败: " . $e->getMessage());
来源：http://reu.guannengcc.top

[U73] PHP：读取 ini 配置
来源：http://wwu.ivvv.top

parse_ini_file("config.ini", true)
来源：http://dwv.jlsjyb.cn

[U74] PHP：读取环境变量
来源：http://esk.epnwcf.com

getenv("APP_ENV") ?: "production"
来源：http://uzz.sxryk.cn

[U75] PHP：依赖注入
来源：http://czu.shuidangran.top

composer require psr/container
来源：http://afl.tianlin.xyz

[U76] PHP：简单路由
来源：http://ufn.ybcxt.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://auy.aizwys.cn

[U77] PHP：模板渲染
来源：http://wim.redwolf501.top

composer require twig/twig
来源：http://aom.shangyingyoupin.top

[U78] PHP：单元测试
来源：http://eqk.fehbvm.com

composer require --dev phpunit/phpunit
来源：http://hrl.jinqigfzy.top

[U79] PHP：静态分析
来源：http://cpg.yj20258888.top

composer require --dev phpstan/phpstan
来源：http://tzj.bbcook.cn

[U80] PHP：代码规范修复
来源：http://muk.yuxming.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nqr.jqgfzy.top

[U81] JS：初始化项目
来源：http://rtf.zhixingplan.top

npm init -y;  npm i express
来源：http://rnn.hywenlv.cn

[U82] JS：package.json 脚本
来源：http://kbi.ywan-chungtsiang.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hiq.hongshengwenyu.top

[U83] JS：ES Module 导入导出
来源：http://emu.hfpthk.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tom.jianghu66.top

[U84] JS：CommonJS 写法
来源：http://gau.jiagoushi.top

module.exports = { a };  const { a } = require("./m");
来源：http://rqa.sxryk.cn

[U85] JS：可选链
来源：http://ttq.cdnleiting.top

a?.b?.c
来源：http://xib.shangyingyoupin.top

[U86] JS：空值合并
来源：http://dtg.zhongyouzk.top

a ?? b
来源：http://zlq.yueranfly.top

[U87] JS：解构默认值
来源：http://dva.chenzaomai.com

const { a = 1, b = 2 } = obj;
来源：http://hgu.jiagoushi.top

[U88] JS：对象展开合并
来源：http://ent.cdnleiting.top

{ ...a, ...b }
来源：http://vwm.zhongyouzk.top

[U89] JS：数组去重
来源：http://dib.iojbl.cn

[...new Set(arr)]
来源：http://sqb.nanxinkj.top

[U90] JS：数字数组排序
来源：http://ivb.cheryme.top

[...arr].sort((a, b) => a - b)
来源：http://lqe.yonumen.top

[U91] JS：对象键值遍历
来源：http://gwe.svipenyu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yvo.zdqjudy.top

[U92] JS：深拷贝
来源：http://qan.sjlbkw.cn

structuredClone(obj)
来源：http://mkj.pengpengdd.cyou

[U93] JS：模板字符串
来源：http://prn.haohaochexian.top

`共 ${n} 条`
来源：http://oob.aizwys.cn

[U94] JS：箭头函数
来源：http://tcl.sxryk.cn

const double = x => x * 2;
来源：http://joy.gotoacloud.top

[U95] JS：Promise 包装
来源：http://iaw.sxryk.cn

new Promise((resolve, reject) => {})
来源：http://qnt.dianchejie.cn

[U96] JS：async/await 与异常
来源：http://wja.yuxming.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://khr.ehwqpu.com

[U97] JS：并发请求
来源：http://bqz.chenzaomai.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://pca.c1oappe.top

[U98] JS：fetch 带 JSON
来源：http://xab.wangshuangyany.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://efy.shanyushiyangkeji.top

[U99] JS：事件监听
来源：http://kgz.ppjwa.cn

el.addEventListener("click", e => {})
来源：http://cym.shanyushiyangtech.top

[U100] JS：DOM 查询
来源：http://igr.gzhubu.top

document.querySelector(".item")
来源：http://dvo.gzhubu.top

[U101] JS：classList 操作
来源：http://cmt.jlsjyb.cn

el.classList.toggle("active")
来源：http://ukt.daxiang520.top

[U102] JS：本地存储
来源：http://zuq.fzhhl.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xgj.9152youxi.cn

[U103] JS：定时器
来源：http://edd.zhaomingkeji.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yhg.yj20258.top

[U104] JS：防抖
来源：http://yyv.cdnleiting.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pkz.epnwcf.com

[U105] JS：节流
来源：http://vgg.sysykeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pvz.ehwqpu.com

[U106] JS：日期格式化
来源：http://jmv.zhoulong.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dcz.xuanzx.com

[U107] JS：数字千分位
来源：http://llx.yuanzhike.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ktr.jqgfzy.top

[U108] JS：随机整数
来源：http://oqw.hesvh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://krw.tarul.cn

[U109] JS：数组分组
来源：http://obc.9152youxi.cn

Object.groupBy(arr, x => x.type)
来源：http://mdu.gotoacloud.top

[U110] JS：数组分块
来源：http://rhe.yanxiufei.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vbi.zhongyouzk.top

[U111] JS：对象转 Map
来源：http://srl.jlsjyb.cn

new Map(Object.entries(obj))
来源：http://qvz.redwolf501.top

[U112] JS：字符串补位
来源：http://kug.zhiwuduotai.top

"7".padStart(3, "0")
来源：http://mzs.shuidangran.top

[U113] JS：正则替换全部
来源：http://mgo.guannengcc.top

s.replaceAll("a", "b")
来源：http://xjq.zhiwuduotai.top

[U114] JS：JSON 深比较
来源：http://mtj.andypj.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://xiw.yj20258.top

[U115] JS：生成 UUID
来源：http://wai.aizwys.cn

crypto.randomUUID()
来源：http://ztp.ehwqpu.com

[U116] JS：类型检查（JSDoc）
来源：http://oul.yj20258888.top

/** @param {string} name */ function f(name) {}
来源：http://zlj.vehdjk.com

[U117] JS：单元测试
来源：http://zoz.zhijiandao.cn

npm i -D vitest;  npx vitest
来源：http://pqg.zhongyouzk.top

[U118] JS：开发服务器
来源：http://tii.ydjk.org.cn

npm i -D vite;  npx vite
来源：http://qcr.316326.xyz

[U119] JS：生产构建
来源：http://tfa.yuanzhike.top

npx vite build
来源：http://eza.smart0.xyz

[U120] JS：读取环境变量（Vite）
来源：http://zyn.ywan-chungtsiang.top

import.meta.env.VITE_API_URL
来源：http://csd.shzxlz.cn

================================================================================
来源：http://dqd.shzxlz.cn

统计汇总
来源：http://quj.tian-w.cn

================================================================================
来源：http://vqf.zhijiandao.cn

按语言统计（条）：
来源：http://ylf.daria6918.cn

Python ......... 252
来源：http://iba.jqgfzy.top

PHP ............ 252
来源：http://lsb.guowangkeji.top

JavaScript ..... 252
来源：http://qyw.yonumen.top

TypeScript ..... 212
来源：http://ots.c1oappe.top

Java ........... 212
来源：http://gii.zhijiandao.cn

Go ............. 212
来源：http://jfv.jianghu66.top

Ruby ........... 212
来源：http://vqu.ctjpmb.com

C# ............. 212
来源：http://vrw.dianchejie.cn

C .............. 30
来源：http://ymg.gaohongyu789.top

C++ ............ 30
来源：http://mtm.quarkkingdee.top

SQL ............ 90
来源：http://jxw.jianghu66.top

Bash ........... 80
来源：http://mge.wangshuangyany.cn

Kotlin ......... 15
来源：http://xve.jqgufenzy.top

Swift .......... 15
来源：http://xmy.yongpay.top

Lua ............ 10
来源：http://xqh.yueranfly.top

Perl ........... 10
来源：http://xxx.xingfuxueyuan.xyz

Scala .......... 10
来源：http://rkb.bjfxy.top

------------------------------------
来源：http://hwb.jyoumei.cn

合计 ........... 2106 条
来源：http://hdm.tarul.cn

按章节统计：
来源：http://rnm.fengsongda.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://snz.zhoulong.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nim.wangshuangyany.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://csm.ivvv.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://flf.zhengqikj.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://was.316326.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vnr.hnqzz.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lwi.epnwcf.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dzp.jlsjyb.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mwj.wangdashe.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tcz.pycfn.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oky.xylfe.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uqo.shzxlz.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qfy.yangfankeji.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wnt.ydzc1.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rxo.fanxiaobao.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ouo.shanyushiyangtech.top

Q SQL 专题                              90
来源：http://jlg.shanyushiyangtech.top

R Bash 专题                             80
来源：http://kwo.yongpay.top

S C / C++ 专题                          60
来源：http://eak.ctjpmb.com

T 其他语言补充                          60
来源：http://tza.jqgufenzy.top

U 高频实用片段                         120
来源：http://wgc.snrcjt.cn

------------------------------------
来源：http://ytw.gogol.net.cn

合计                                  2106 条
来源：http://kwm.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://gyd.smart0.xyz

使用提醒
来源：http://wae.tarul.cn

--------------------------------------------------------------------------------
来源：http://dzk.dianchejie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zlc.zycfv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://uvk.zycfv.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://unq.9152youxi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://kcl.zycfv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cfy.xinyue.icu

—— 文件结束 ——
来源：http://mck.jinqigufen.top

================================================================================
来源：http://ncl.yangfankeji.com

程序语言常见例子速查手册（2024 版）
来源：http://sns.wangdashe.top

Common Programming Examples Cheat Book
来源：http://hhh.hfpthk.cn

================================================================================
来源：http://qdo.ctjpmb.com

【收录内容】
来源：http://fjq.0kj1m.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vjo.jlsjyb.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rvf.jqgufenzy.top

SQL · Bash · C · C++
来源：http://qio.fengsongda.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gbi.bbcook.cn

【使用说明】
来源：http://fnk.kuanghao11.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mzh.jianghu66.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uoc.jinyuanbaomall.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tck.cheryme.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yuq.fanxiaobao.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://cim.316326.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cea.yongpay.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xxw.jinghuilouyu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ivx.andypj.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://get.dashuyun.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://soh.ydzc1.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xgz.cashguo.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qmj.zhongyouzk.top

【文件统计】
来源：http://yqf.zhiwuduotai.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tdm.hnqzz.top

--------------------------------------------------------------------------------
来源：http://uyp.cqqwz.cn

目  录
来源：http://qbi.cheryme.top

--------------------------------------------------------------------------------
来源：http://wza.jianghu66.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bzv.fanxiaobao.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ulk.chenzaomai.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fiq.zdqjudy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://isq.daria6918.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yof.jiagoushi.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mze.shzxlz.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jtq.ivvv.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ieq.xuetiantiany.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yrc.zycfv.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wvp.smart0.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ciq.daxiang520.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wze.hywenlv.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ahg.epnwcf.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://omt.jiagoushi.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ptj.jqgfzy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://urj.nanxuanxn.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rwt.52xcode.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tjl.tarul.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://emp.sweek.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tnn.aizwys.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://doh.zhaomingkeji.xyz

================================================================================
来源：http://hze.bjfxy.top

A. 基础语法与类型
来源：http://hvi.daxiang520.top

================================================================================
来源：http://olg.redwolf501.top

[A01] Hello World
来源：http://zlc.jinyuanbaomall.cn

Py:   print("Hello, World!")
来源：http://liu.wangshuangyany.cn

PHP:  echo "Hello, World!";
来源：http://dyi.zhongyouzk.top

JS:   console.log("Hello, World!");
来源：http://oqt.nanxuanxn.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gfn.hcnkem.com

Java: System.out.println("Hello, World!");
来源：http://lbq.hfpthk.cn

Go:   fmt.Println("Hello, World!")
来源：http://ynv.epnwcf.com

Ruby: puts "Hello, World!"
来源：http://oou.jianghu66.top

C#:   Console.WriteLine("Hello, World!");
来源：http://hom.cheryme.top

[A02] 变量声明与赋值
来源：http://hpq.nanxuanxn.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mfh.zhaomingkeji.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://cyn.fanxiaobao.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://rgo.svipenyu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bfb.dashuyun.cn

Java: String name = "Alex"; int age = 20;
来源：http://lso.cqqwz.cn

Go:   name := "Alex"; age := 20
来源：http://ggl.mhx1999.top

Ruby: name = "Alex"; age = 20
来源：http://gyp.fengsongda.top

C#:   string name = "Alex"; int age = 20;
来源：http://qac.fzhhl.top

[A03] 常量定义
来源：http://bpu.gzhubu.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kny.vqdsnc.cn

PHP:  const PI = 3.14159;
来源：http://jat.zycfv.cn

JS:   const PI = 3.14159;
来源：http://jko.meibo888.top

TS:   const PI: number = 3.14159;
来源：http://har.yfazqb.com

Java: static final double PI = 3.14159;
来源：http://cri.yj20258.top

Go:   const PI = 3.14159
来源：http://yda.ydzc1.top

Ruby: PI = 3.14159
来源：http://fdq.cdnleiting.top

C#:   const double PI = 3.14159;
来源：http://uar.fanxiaobao.xyz

[A04] 判断变量类型
来源：http://lnz.shuidangran.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://mrh.dashuyun.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mzb.jqgufenzy.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://opc.andypj.xyz

TS:   typeof x; x instanceof Date
来源：http://pxr.fzhhl.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pcx.wangdashe.top

Go:   reflect.TypeOf(x).Name()
来源：http://ptx.jyoumei.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hwq.epnwcf.com

C#:   x.GetType().Name; x is int
来源：http://tpt.xziqi.cn

[A05] 整数除法与取模
来源：http://ezm.yuanzhike.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bch.gaohongyu789.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://nju.fehbvm.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nlp.hnxiangtu.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rbj.yj20258.top

Java: 7 / 2; 7 % 2
来源：http://krk.tian-w.cn

Go:   7 / 2; 7 % 2
来源：http://zxo.zhijiandao.cn

Ruby: 7 / 2; 7 % 2
来源：http://dmt.zycfv.cn

C#:   7 / 2; 7 % 2
来源：http://arr.xinyue.icu

[A06] 字符串转数字
来源：http://pcm.snrcjt.cn

Py:   int("42"); float("3.14")
来源：http://cmy.ywan-chungtsiang.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://npb.xylfe.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nrg.xingfuxueyuan.xyz


<!-- 参考信息 -->