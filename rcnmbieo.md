代发 wailian999

[U47] PHP：联合类型
来源：http://udf.vqdsnc.cn

int|string $id
来源：http://xsv.zhixingplan.top

[U48] PHP：纯枚举
来源：http://gif.hywenlv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nxd.9152youxi.cn

[U49] PHP：只读属性
来源：http://hxv.fehbvm.com

public readonly string $name
来源：http://tug.jianghu66.top

[U50] PHP：构造器属性提升
来源：http://bgz.ydjk.org.cn

public function __construct(private int $id) {}
来源：http://xau.shangyingyoupin.top

[U51] PHP：数组解构
来源：http://hpy.zhaomingkeji.xyz

[$a, $b] = $arr;
来源：http://ptk.xinyue.icu

[U52] PHP：箭头函数
来源：http://ynx.gzhubu.top

$double = fn($x) => $x * 2;
来源：http://iuo.shanyushiyangtech.top

[U53] PHP：空合并运算符
来源：http://nlo.mhx1999.top

$v = $a ?? $b ?? "default";
来源：http://bir.zdqjudy.top

[U54] PHP：空安全调用
来源：http://iof.haohaochexian.top

$obj?->method()
来源：http://ycx.gzhubu.top

[U55] PHP：match 表达式
来源：http://ioy.yj20258.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vah.shuidangran.top

[U56] PHP：命名参数
来源：http://mtq.ybcxt.top

f(a: 1, b: 2)
来源：http://gmt.pycfn.com

[U57] PHP：字符串插值
来源：http://hfr.shanyushiyangkeji.top

"值: {$a}"
来源：http://bjh.hfpthk.cn

[U58] PHP：数组三件套
来源：http://zht.sweek.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uoy.chenzaomai.com

[U59] PHP：自定义排序
来源：http://tjb.zdbjq.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nsp.sweek.top

[U60] PHP：JSON 编解码
来源：http://bmk.chenlongwang.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qyg.sysykeji.top

[U61] PHP：正则
来源：http://tlq.yangfankeji.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xoc.quarkkingdee.top

[U62] PHP：日期对象
来源：http://gtm.xuanzx.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lck.zhoulong.xyz

[U63] PHP：文件读写
来源：http://rcf.chenzaomai.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cfs.xylfe.cn

[U64] PHP：目录遍历
来源：http://fax.yj20258888.top

glob("dir/*.php");  scandir("dir");
来源：http://lsm.yanxiufei.cn

[U65] PHP：会话
来源：http://yga.wangshuangyany.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://thk.hysaishi.cn

[U66] PHP：设置 Cookie
来源：http://fkw.xuanzx.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pid.feifeiyinyue.top

[U67] PHP：处理文件上传
来源：http://ptj.yueranfly.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nlu.daria6918.cn

[U68] PHP：PDO 连接
来源：http://yyy.jinqigufen.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://prq.fktsv.cn

[U69] PHP：PDO 预处理
来源：http://zya.xinyue.icu

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wsp.yonumen.top

[U70] PHP：PDO 事务
来源：http://oye.zdbjq.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yqq.shzxlz.cn

[U71] PHP：抛出异常
来源：http://cdh.meibo888.top

throw new RuntimeException("失败", 500);
来源：http://jee.fehbvm.com

[U72] PHP：写错误日志
来源：http://uim.yvedp.cn

error_log("失败: " . $e->getMessage());
来源：http://akx.hesvh.cn

[U73] PHP：读取 ini 配置
来源：http://ebj.mhx1999.top

parse_ini_file("config.ini", true)
来源：http://kyc.yj202588.top

[U74] PHP：读取环境变量
来源：http://qec.hcnkem.com

getenv("APP_ENV") ?: "production"
来源：http://zdo.zhongyouzk.top

[U75] PHP：依赖注入
来源：http://ktq.hnqzz.top

composer require psr/container
来源：http://cfx.feifeiyinyue.top

[U76] PHP：简单路由
来源：http://kno.ctjpmb.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xuq.fengsongda.top

[U77] PHP：模板渲染
来源：http://soy.tianlin.xyz

composer require twig/twig
来源：http://ddb.hnxiangtu.top

[U78] PHP：单元测试
来源：http://niz.gzhubu.top

composer require --dev phpunit/phpunit
来源：http://auk.zdqjudy.top

[U79] PHP：静态分析
来源：http://ltw.wangshuangyany.cn

composer require --dev phpstan/phpstan
来源：http://wjm.shzxlz.cn

[U80] PHP：代码规范修复
来源：http://ggu.shanyushiyangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://uex.jiagoushi.top

[U81] JS：初始化项目
来源：http://ehe.vehdjk.com

npm init -y;  npm i express
来源：http://djz.bbcook.cn

[U82] JS：package.json 脚本
来源：http://szx.hesvh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dfe.dianchejie.cn

[U83] JS：ES Module 导入导出
来源：http://alk.pycfn.com

export const a = 1;  import { a } from "./m.js";
来源：http://iba.hongshengwenyu.top

[U84] JS：CommonJS 写法
来源：http://drg.hnxiangtu.top

module.exports = { a };  const { a } = require("./m");
来源：http://fsf.hongshengwenyu.top

[U85] JS：可选链
来源：http://kqw.sweek.top

a?.b?.c
来源：http://qty.yj20258888.top

[U86] JS：空值合并
来源：http://rcl.xingfuxueyuan.xyz

a ?? b
来源：http://xyu.jyoumei.cn

[U87] JS：解构默认值
来源：http://grh.yuanzhike.top

const { a = 1, b = 2 } = obj;
来源：http://yel.hongshengwenyu.top

[U88] JS：对象展开合并
来源：http://wme.feifeiyinyue.top

{ ...a, ...b }
来源：http://its.ivvv.top

[U89] JS：数组去重
来源：http://txz.aibaodan.cn

[...new Set(arr)]
来源：http://tyj.cucudq.cn

[U90] JS：数字数组排序
来源：http://qsf.hnxiangtu.top

[...arr].sort((a, b) => a - b)
来源：http://aaz.meibo888.top

[U91] JS：对象键值遍历
来源：http://vvk.fktsv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mtq.gzhubu.top

[U92] JS：深拷贝
来源：http://clc.gzhubu.top

structuredClone(obj)
来源：http://lds.svipenyu.cn

[U93] JS：模板字符串
来源：http://xxb.daria6918.cn

`共 ${n} 条`
来源：http://zzv.wangshuangyany.cn

[U94] JS：箭头函数
来源：http://cvz.jinqigufen.top

const double = x => x * 2;
来源：http://gey.yonumen.top

[U95] JS：Promise 包装
来源：http://pca.meibo888.top

new Promise((resolve, reject) => {})
来源：http://axm.zhixingplan.top

[U96] JS：async/await 与异常
来源：http://uuz.cqqwz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ofp.ppjwa.cn

[U97] JS：并发请求
来源：http://cxo.yvedp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yvv.chenzaomai.com

[U98] JS：fetch 带 JSON
来源：http://qkb.xylfe.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fvl.pengpengdd.cyou

[U99] JS：事件监听
来源：http://ciq.0kj1m.cn

el.addEventListener("click", e => {})
来源：http://vqg.zhongyouzk.top

[U100] JS：DOM 查询
来源：http://ldf.ywan-chungtsiang.top

document.querySelector(".item")
来源：http://egd.shanyushiyangtech.top

[U101] JS：classList 操作
来源：http://van.cdnleiting.top

el.classList.toggle("active")
来源：http://gxv.zhijiandao.cn

[U102] JS：本地存储
来源：http://oui.jiagoushi.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://wul.9152youxi.cn

[U103] JS：定时器
来源：http://mco.jinqigufen.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kzm.hysaishi.cn

[U104] JS：防抖
来源：http://sps.havefunace.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eel.guannengcc.top

[U105] JS：节流
来源：http://xln.birdmap.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lim.dianchejie.cn

[U106] JS：日期格式化
来源：http://bby.kuanghao11.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vig.gzhubu.top

[U107] JS：数字千分位
来源：http://toh.c1oappe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mjt.tian-w.cn

[U108] JS：随机整数
来源：http://xna.zhoulong.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hqn.sweek.top

[U109] JS：数组分组
来源：http://wsz.fktsv.cn

Object.groupBy(arr, x => x.type)
来源：http://idy.yuanzhike.top

[U110] JS：数组分块
来源：http://mms.yuanzhike.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vvo.xylfe.cn

[U111] JS：对象转 Map
来源：http://jxl.pycfn.com

new Map(Object.entries(obj))
来源：http://dlt.pycfn.com

[U112] JS：字符串补位
来源：http://mdd.uphjek.com

"7".padStart(3, "0")
来源：http://drk.ehwqpu.com

[U113] JS：正则替换全部
来源：http://vks.yvedp.cn

s.replaceAll("a", "b")
来源：http://nba.daxiang520.top

[U114] JS：JSON 深比较
来源：http://lns.jlsjyb.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gui.daria6918.cn

[U115] JS：生成 UUID
来源：http://fdg.pycfn.com

crypto.randomUUID()
来源：http://ogq.yueranfly.top

[U116] JS：类型检查（JSDoc）
来源：http://qjz.haohaochexian.top

/** @param {string} name */ function f(name) {}
来源：http://gpw.sjlbkw.cn

[U117] JS：单元测试
来源：http://abd.birdmap.top

npm i -D vitest;  npx vitest
来源：http://yyb.316326.xyz

[U118] JS：开发服务器
来源：http://izr.kuanghao11.cn

npm i -D vite;  npx vite
来源：http://djr.yuanzhike.top

[U119] JS：生产构建
来源：http://vvc.jqgufenzy.top

npx vite build
来源：http://jtn.guannengcc.top

[U120] JS：读取环境变量（Vite）
来源：http://kzu.aizwys.cn

import.meta.env.VITE_API_URL
来源：http://mad.sjlbkw.cn

================================================================================
来源：http://wvi.jiagoushi.top

统计汇总
来源：http://mkt.shuidangran.top

================================================================================
来源：http://opf.quarkkingdee.top

按语言统计（条）：
来源：http://wwu.pengpengdd.cyou

Python ......... 252
来源：http://tsy.xingfuxueyuan.xyz

PHP ............ 252
来源：http://jgm.yj20258888.top

JavaScript ..... 252
来源：http://wqy.xuetiantiany.cn

TypeScript ..... 212
来源：http://icu.nanxinkj.top

Java ........... 212
来源：http://lpy.iojbl.cn

Go ............. 212
来源：http://iwc.chenzaomai.com

Ruby ........... 212
来源：http://oht.ydzc1.top

C# ............. 212
来源：http://sqp.xuanzx.com

C .............. 30
来源：http://lzh.aizwys.cn

C++ ............ 30
来源：http://jlz.gaohongyu789.top

SQL ............ 90
来源：http://bab.fzhhl.top

Bash ........... 80
来源：http://juv.birdmap.top

Kotlin ......... 15
来源：http://fju.hammf.cn

Swift .......... 15
来源：http://ksu.yfazqb.com

Lua ............ 10
来源：http://syp.jqgfzy.top

Perl ........... 10
来源：http://zfu.vehdjk.com

Scala .......... 10
来源：http://dkr.zhoulong.xyz

------------------------------------
来源：http://dzw.birdmap.top

合计 ........... 2106 条
来源：http://ojm.zycfv.cn

按章节统计：
来源：http://jza.sufxvd.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tbx.chenjidiqi.icu

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qgu.jinqigufen.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pdo.yueranfly.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xtg.fktsv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ywy.epnwcf.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dfd.tian-w.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hah.yj20258.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xtx.gogol.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uzz.uphjek.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rmp.jinyuanbaomall.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wsm.fehbvm.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://izk.xinyue.icu

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uck.52xcode.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hwa.hysaishi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://iyz.tian-w.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tqa.haohaochexian.top

Q SQL 专题                              90
来源：http://xxa.cucudq.cn

R Bash 专题                             80
来源：http://xjl.daria6918.cn

S C / C++ 专题                          60
来源：http://eoa.zhengqikj.top

T 其他语言补充                          60
来源：http://msk.fzhhl.top

U 高频实用片段                         120
来源：http://sds.chenlongwang.top

------------------------------------
来源：http://htd.shanyushiyangkeji.top

合计                                  2106 条
来源：http://pzt.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://tcd.ydjk.org.cn

使用提醒
来源：http://tak.yfazqb.com

--------------------------------------------------------------------------------
来源：http://mkx.hysaishi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bdn.zhaomingkeji.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ddi.jqgfzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://znx.fengsongda.top

在旧版本上使用前请先确认语法支持情况。
来源：http://sox.cucudq.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kih.yuxming.cn

—— 文件结束 ——
来源：http://ktl.shanyushiyangkeji.top

================================================================================
来源：http://kmg.yongpay.top

程序语言常见例子速查手册（2024 版）
来源：http://tdu.zdbjq.cn

Common Programming Examples Cheat Book
来源：http://bha.shanyushiyangtech.top

================================================================================
来源：http://hcy.shanyushiyangtech.top

【收录内容】
来源：http://zxe.gaohongyu789.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://gge.cheryme.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://een.xingfuxueyuan.xyz

SQL · Bash · C · C++
来源：http://thi.jlsjyb.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lco.cdnleiting.top

【使用说明】
来源：http://ndh.shanyushiyangkeji.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wry.kuanghao11.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rdh.daria6918.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gct.yj202588.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://irk.smart0.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://vle.smart0.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://coe.nanxuanxn.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kma.yueranfly.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qtf.yvedp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nic.jqgufenzy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gwz.cqqwz.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ler.zhongyouzk.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://suw.yueranfly.top

【文件统计】
来源：http://seb.xuanzx.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pzh.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://nnn.ybcxt.top

目  录
来源：http://yjd.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://qbs.fehbvm.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://omm.snrcjt.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lwy.ywan-chungtsiang.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yta.uphjek.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://isk.zhaomingkeji.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yej.haohaochexian.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jcn.zhiwuduotai.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dsg.yj20258888.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wxq.wangshuangyany.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wxb.iojbl.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nce.dianchejie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ncf.shzxlz.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://oml.daria6918.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qdh.kuanghao11.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bgm.tarul.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://olu.fktsv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pne.chenzaomai.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yse.shzxlz.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://dic.sjlbkw.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jnj.sufxvd.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kut.gotoacloud.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wwh.52xcode.cn

================================================================================
来源：http://mfm.yanxiufei.cn

A. 基础语法与类型
来源：http://qof.gogol.net.cn

================================================================================
来源：http://slf.feifeiyinyue.top

[A01] Hello World
来源：http://kuy.ywan-chungtsiang.top

Py:   print("Hello, World!")
来源：http://wmd.shzxlz.cn

PHP:  echo "Hello, World!";
来源：http://rhm.cashguo.top

JS:   console.log("Hello, World!");
来源：http://udj.aibaodan.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gkt.xuetiantiany.cn

Java: System.out.println("Hello, World!");
来源：http://dnv.cqqwz.cn

Go:   fmt.Println("Hello, World!")
来源：http://roc.tian-w.cn

Ruby: puts "Hello, World!"
来源：http://rxw.fengsongda.top

C#:   Console.WriteLine("Hello, World!");
来源：http://lab.ydjk.org.cn

[A02] 变量声明与赋值
来源：http://sur.ywan-chungtsiang.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gek.andypj.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://bzv.cashguo.top

JS:   let name = "Alex"; const age = 20;
来源：http://vum.shuidangran.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oec.zhaomingkeji.xyz

Java: String name = "Alex"; int age = 20;
来源：http://zcd.pengpengdd.cyou

Go:   name := "Alex"; age := 20
来源：http://fpr.quarkkingdee.top

Ruby: name = "Alex"; age = 20
来源：http://pdr.cdnleiting.top

C#:   string name = "Alex"; int age = 20;
来源：http://ebd.birdmap.top

[A03] 常量定义
来源：http://ooh.cashguo.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fkg.jinqigufen.top

PHP:  const PI = 3.14159;
来源：http://tpb.snrcjt.cn

JS:   const PI = 3.14159;
来源：http://sqm.hesvh.cn

TS:   const PI: number = 3.14159;
来源：http://vzn.yueranfly.top

Java: static final double PI = 3.14159;
来源：http://adv.tarul.cn

Go:   const PI = 3.14159
来源：http://dge.epnwcf.com

Ruby: PI = 3.14159
来源：http://ava.bbcook.cn

C#:   const double PI = 3.14159;
来源：http://kya.smart0.xyz

[A04] 判断变量类型
来源：http://uwz.yueranfly.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://lyv.zhaomingkeji.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://urb.yueranfly.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fsa.fengsongda.top

TS:   typeof x; x instanceof Date
来源：http://jnr.dianchejie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://itd.zdqjudy.top

Go:   reflect.TypeOf(x).Name()
来源：http://uys.zhixingplan.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ngb.yj20258.top

C#:   x.GetType().Name; x is int
来源：http://eka.yvedp.cn

[A05] 整数除法与取模
来源：http://ips.sjlbkw.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://aya.guannengcc.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://uqi.yfazqb.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ace.0kj1m.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hid.jinqigufen.top

Java: 7 / 2; 7 % 2
来源：http://opv.zhijiandao.cn

Go:   7 / 2; 7 % 2
来源：http://pbh.gogol.net.cn

Ruby: 7 / 2; 7 % 2
来源：http://yqd.cashguo.top

C#:   7 / 2; 7 % 2
来源：http://lhw.guannengcc.top


<!-- 参考信息 -->