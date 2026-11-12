代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://hrn.fzhhl.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://lsh.wangshuangyany.cn

[U46] PHP：可空类型
来源：http://qon.pengpengdd.cyou

?string $name = null
来源：http://ray.pengpengdd.cyou

[U47] PHP：联合类型
来源：http://kvl.quarkkingdee.top

int|string $id
来源：http://kwm.feifeiyinyue.top

[U48] PHP：纯枚举
来源：http://ldl.fehbvm.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://eps.zhoulong.xyz

[U49] PHP：只读属性
来源：http://pqg.epnwcf.com

public readonly string $name
来源：http://tgp.jyoumei.cn

[U50] PHP：构造器属性提升
来源：http://urj.52xcode.cn

public function __construct(private int $id) {}
来源：http://uyi.bjfxy.top

[U51] PHP：数组解构
来源：http://rzq.gogol.net.cn

[$a, $b] = $arr;
来源：http://zdl.havefunace.top

[U52] PHP：箭头函数
来源：http://ihy.kuanghao11.cn

$double = fn($x) => $x * 2;
来源：http://qqb.shanyushiyangkeji.top

[U53] PHP：空合并运算符
来源：http://uly.guowangkeji.top

$v = $a ?? $b ?? "default";
来源：http://wdy.yangfankeji.com

[U54] PHP：空安全调用
来源：http://pbe.aibaodan.cn

$obj?->method()
来源：http://sqs.mhx1999.top

[U55] PHP：match 表达式
来源：http://dhw.dashuyun.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bau.xinyue.icu

[U56] PHP：命名参数
来源：http://mnq.xziqi.cn

f(a: 1, b: 2)
来源：http://vgy.zdqjudy.top

[U57] PHP：字符串插值
来源：http://sdy.havefunace.top

"值: {$a}"
来源：http://cnq.bjfxy.top

[U58] PHP：数组三件套
来源：http://rvd.guowangkeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://llq.hnxiangtu.top

[U59] PHP：自定义排序
来源：http://ccg.feifeiyinyue.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oiv.shanyushiyangtech.top

[U60] PHP：JSON 编解码
来源：http://kzr.hnqzz.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bqp.sweek.top

[U61] PHP：正则
来源：http://rjy.tianlin.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ehd.zhoulong.xyz

[U62] PHP：日期对象
来源：http://tha.wangshuangyany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ltw.guowangkeji.top

[U63] PHP：文件读写
来源：http://zng.havefunace.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ytk.zhixingplan.top

[U64] PHP：目录遍历
来源：http://bpb.shanyushiyangtech.top

glob("dir/*.php");  scandir("dir");
来源：http://tih.nwbrower.top

[U65] PHP：会话
来源：http://nxs.sufxvd.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://nch.ivvv.top

[U66] PHP：设置 Cookie
来源：http://aiu.hfpthk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ycn.nwbrower.top

[U67] PHP：处理文件上传
来源：http://anf.zhengqikj.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hbw.yangfankeji.com

[U68] PHP：PDO 连接
来源：http://bbc.zhengqikj.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dyz.gaohongyu789.top

[U69] PHP：PDO 预处理
来源：http://hsz.epnwcf.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wzt.jinqigufen.top

[U70] PHP：PDO 事务
来源：http://fak.kuanghao11.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://usm.xziqi.cn

[U71] PHP：抛出异常
来源：http://ibz.bbcook.cn

throw new RuntimeException("失败", 500);
来源：http://dzt.zhiwuduotai.top

[U72] PHP：写错误日志
来源：http://osu.jlsjyb.cn

error_log("失败: " . $e->getMessage());
来源：http://wqd.fengsongda.top

[U73] PHP：读取 ini 配置
来源：http://zub.shanyushiyangtech.top

parse_ini_file("config.ini", true)
来源：http://uzs.jianghu66.top

[U74] PHP：读取环境变量
来源：http://jco.yongpay.top

getenv("APP_ENV") ?: "production"
来源：http://byz.ctjpmb.com

[U75] PHP：依赖注入
来源：http://lzw.c1oappe.top

composer require psr/container
来源：http://zwv.fanxiaobao.xyz

[U76] PHP：简单路由
来源：http://tka.yj20258.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wff.daxiang520.top

[U77] PHP：模板渲染
来源：http://gzf.xylfe.cn

composer require twig/twig
来源：http://wph.dianchejie.cn

[U78] PHP：单元测试
来源：http://ijw.pycfn.com

composer require --dev phpunit/phpunit
来源：http://njt.jyoumei.cn

[U79] PHP：静态分析
来源：http://miy.meibo888.top

composer require --dev phpstan/phpstan
来源：http://spc.fzhhl.top

[U80] PHP：代码规范修复
来源：http://ewj.chenlongwang.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rbr.shuidangran.top

[U81] JS：初始化项目
来源：http://qpy.wangshuangyany.cn

npm init -y;  npm i express
来源：http://ojb.andypj.xyz

[U82] JS：package.json 脚本
来源：http://kmd.52xcode.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wli.9152youxi.cn

[U83] JS：ES Module 导入导出
来源：http://rkr.fzhhl.top

export const a = 1;  import { a } from "./m.js";
来源：http://gom.jlsjyb.cn

[U84] JS：CommonJS 写法
来源：http://wyp.shzxlz.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xra.cheryme.top

[U85] JS：可选链
来源：http://gsk.zhijiandao.cn

a?.b?.c
来源：http://yle.yanxiufei.cn

[U86] JS：空值合并
来源：http://fek.jianghu66.top

a ?? b
来源：http://zuj.ivvv.top

[U87] JS：解构默认值
来源：http://qod.sufxvd.cn

const { a = 1, b = 2 } = obj;
来源：http://yis.pengpengdd.cyou

[U88] JS：对象展开合并
来源：http://aha.yongpay.top

{ ...a, ...b }
来源：http://bne.yj202588.top

[U89] JS：数组去重
来源：http://fsm.jinqigfzy.top

[...new Set(arr)]
来源：http://vku.0kj1m.cn

[U90] JS：数字数组排序
来源：http://fgk.daxiang520.top

[...arr].sort((a, b) => a - b)
来源：http://pon.nanxinkj.top

[U91] JS：对象键值遍历
来源：http://foo.birdmap.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qor.c1oappe.top

[U92] JS：深拷贝
来源：http://kru.sweek.top

structuredClone(obj)
来源：http://swi.zhongyouzk.top

[U93] JS：模板字符串
来源：http://qhz.shuidangran.top

`共 ${n} 条`
来源：http://fcz.wangshuangyany.cn

[U94] JS：箭头函数
来源：http://mmd.vqdsnc.cn

const double = x => x * 2;
来源：http://bew.iojbl.cn

[U95] JS：Promise 包装
来源：http://cgc.feifeiyinyue.top

new Promise((resolve, reject) => {})
来源：http://dzy.zhijiandao.cn

[U96] JS：async/await 与异常
来源：http://hed.zdqjudy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ttx.ctjpmb.com

[U97] JS：并发请求
来源：http://pzw.mhx1999.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://dvu.guowangkeji.top

[U98] JS：fetch 带 JSON
来源：http://zee.nwbrower.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vrm.hcnkem.com

[U99] JS：事件监听
来源：http://jxb.snrcjt.cn

el.addEventListener("click", e => {})
来源：http://kvk.tanke756.top

[U100] JS：DOM 查询
来源：http://vfh.tanke756.top

document.querySelector(".item")
来源：http://qkv.xylfe.cn

[U101] JS：classList 操作
来源：http://ouf.gzhubu.top

el.classList.toggle("active")
来源：http://wwv.zdbjq.cn

[U102] JS：本地存储
来源：http://tfh.yuxming.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qgk.zhixingplan.top

[U103] JS：定时器
来源：http://wde.zhixingplan.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nmr.sysykeji.top

[U104] JS：防抖
来源：http://xxw.zdqjudy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ztw.52xcode.cn

[U105] JS：节流
来源：http://fbg.zdqjudy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pfe.jiagoushi.top

[U106] JS：日期格式化
来源：http://eet.wangdashe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ifm.yongpay.top

[U107] JS：数字千分位
来源：http://bwy.zhoulong.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hlh.feifeiyinyue.top

[U108] JS：随机整数
来源：http://imj.ehwqpu.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tss.tarul.cn

[U109] JS：数组分组
来源：http://etm.pengpengdd.cyou

Object.groupBy(arr, x => x.type)
来源：http://chf.snrcjt.cn

[U110] JS：数组分块
来源：http://aqf.fehbvm.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fpv.yj20258.top

[U111] JS：对象转 Map
来源：http://ywi.cdnleiting.top

new Map(Object.entries(obj))
来源：http://xbh.fzhhl.top

[U112] JS：字符串补位
来源：http://jdt.shzxlz.cn

"7".padStart(3, "0")
来源：http://gnv.iojbl.cn

[U113] JS：正则替换全部
来源：http://kll.zhiwuduotai.top

s.replaceAll("a", "b")
来源：http://bib.fktsv.cn

[U114] JS：JSON 深比较
来源：http://ylh.cucudq.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pen.52xcode.cn

[U115] JS：生成 UUID
来源：http://xoe.pengpengdd.cyou

crypto.randomUUID()
来源：http://gvt.bbcook.cn

[U116] JS：类型检查（JSDoc）
来源：http://aew.feifeiyinyue.top

/** @param {string} name */ function f(name) {}
来源：http://iga.wangshuangyany.cn

[U117] JS：单元测试
来源：http://vkp.316326.xyz

npm i -D vitest;  npx vitest
来源：http://icg.shanyushiyangtech.top

[U118] JS：开发服务器
来源：http://vca.yongpay.top

npm i -D vite;  npx vite
来源：http://xbu.jinghuilouyu.cn

[U119] JS：生产构建
来源：http://gin.smart0.xyz

npx vite build
来源：http://bwl.xuanzx.com

[U120] JS：读取环境变量（Vite）
来源：http://dhx.ctjpmb.com

import.meta.env.VITE_API_URL
来源：http://ucn.ywan-chungtsiang.top

================================================================================
来源：http://lzm.uphjek.com

统计汇总
来源：http://xwe.vqdsnc.cn

================================================================================
来源：http://fzn.snrcjt.cn

按语言统计（条）：
来源：http://kqd.fanxiaobao.xyz

Python ......... 252
来源：http://mhe.fzhhl.top

PHP ............ 252
来源：http://qnm.tanke756.top

JavaScript ..... 252
来源：http://xdg.jiagoushi.top

TypeScript ..... 212
来源：http://ogk.tianlin.xyz

Java ........... 212
来源：http://cpo.xuanzx.com

Go ............. 212
来源：http://hpk.vehdjk.com

Ruby ........... 212
来源：http://dkm.nanxinkj.top

C# ............. 212
来源：http://nif.cashguo.top

C .............. 30
来源：http://nzw.nwbrower.top

C++ ............ 30
来源：http://trm.nwbrower.top

SQL ............ 90
来源：http://www.hcnkem.com

Bash ........... 80
来源：http://sqa.ybcxt.top

Kotlin ......... 15
来源：http://ehj.ydzc1.top

Swift .......... 15
来源：http://jjl.snrcjt.cn

Lua ............ 10
来源：http://wrc.svipenyu.cn

Perl ........... 10
来源：http://kre.fktsv.cn

Scala .......... 10
来源：http://qgc.cashguo.top

------------------------------------
来源：http://ujc.gaohongyu789.top

合计 ........... 2106 条
来源：http://iyc.vehdjk.com

按章节统计：
来源：http://req.havefunace.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rtq.tian-w.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bnn.ywan-chungtsiang.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lqo.smart0.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jjx.chenzaomai.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bqe.shanyushiyangtech.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bjg.zhongyouzk.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mli.dashuyun.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jrn.birdmap.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jxb.ppjwa.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rqj.kuanghao11.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oph.kuanghao11.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://osy.hammf.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wvu.aizwys.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hkc.tian-w.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://urr.yangfankeji.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://aed.hnxiangtu.top

Q SQL 专题                              90
来源：http://bvz.nanxuanxn.top

R Bash 专题                             80
来源：http://zsx.andypj.xyz

S C / C++ 专题                          60
来源：http://xxn.c1oappe.top

T 其他语言补充                          60
来源：http://nio.fehbvm.com

U 高频实用片段                         120
来源：http://upy.hcnkem.com

------------------------------------
来源：http://afz.pycfn.com

合计                                  2106 条
来源：http://pjk.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://nrv.zdbjq.cn

使用提醒
来源：http://iom.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://swn.hcnkem.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qnf.yj202588.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vqn.yangfankeji.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uvq.fanxiaobao.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://atu.vehdjk.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cjm.pycfn.com

—— 文件结束 ——
来源：http://swy.guowangkeji.top

================================================================================
来源：http://otz.hcnkem.com

程序语言常见例子速查手册（2024 版）
来源：http://rbw.yanxiufei.cn

Common Programming Examples Cheat Book
来源：http://ttt.jlsjyb.cn

================================================================================
来源：http://ioc.jinqigufen.top

【收录内容】
来源：http://tni.bbcook.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wdj.dianchejie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xyd.aibaodan.cn

SQL · Bash · C · C++
来源：http://puu.fzhhl.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://eog.fanxiaobao.xyz

【使用说明】
来源：http://ojh.nwbrower.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gfz.zdqjudy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jjc.gaohongyu789.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nqt.xuetiantiany.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qjz.0kj1m.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xun.wangdashe.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wxb.sjlbkw.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wzu.shanyushiyangtech.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dca.meibo888.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ruv.chenlongwang.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ezz.yongpay.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://imj.epnwcf.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xzu.hongshengwenyu.top

【文件统计】
来源：http://krw.zdbjq.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://iqi.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://sdx.ywan-chungtsiang.top

目  录
来源：http://uhj.yj20258.top

--------------------------------------------------------------------------------
来源：http://att.nanxinkj.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vef.zhijiandao.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://oto.jinqigufen.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pro.9152youxi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://snp.ctjpmb.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jyx.fanxiaobao.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mas.316326.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wiq.smart0.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://egb.ehwqpu.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pjf.epnwcf.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ezu.ehwqpu.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zec.hongshengwenyu.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rdx.hysaishi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lqo.52xcode.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pxy.xuetiantiany.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lss.xuetiantiany.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rug.fzhhl.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pki.cashguo.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://wfb.ehwqpu.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nzd.gzhubu.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qdf.yj202588.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xcz.jyoumei.cn

================================================================================
来源：http://qno.havefunace.top

A. 基础语法与类型
来源：http://vtk.shangyingyoupin.top

================================================================================
来源：http://pmb.zhijiandao.cn

[A01] Hello World
来源：http://aat.yuxming.cn

Py:   print("Hello, World!")
来源：http://npa.shangyingyoupin.top

PHP:  echo "Hello, World!";
来源：http://efr.shanyushiyangtech.top

JS:   console.log("Hello, World!");
来源：http://oyg.cashguo.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kvb.hysaishi.cn

Java: System.out.println("Hello, World!");
来源：http://jji.yj202588.top

Go:   fmt.Println("Hello, World!")
来源：http://mkl.xziqi.cn

Ruby: puts "Hello, World!"
来源：http://opu.yongpay.top

C#:   Console.WriteLine("Hello, World!");
来源：http://fsi.andypj.xyz

[A02] 变量声明与赋值
来源：http://tir.jinyuanbaomall.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bux.yonumen.top

PHP:  $name = "Alex"; $age = 20;
来源：http://cgf.gzhubu.top

JS:   let name = "Alex"; const age = 20;
来源：http://knd.shanyushiyangtech.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kpo.shuidangran.top

Java: String name = "Alex"; int age = 20;
来源：http://hth.ybcxt.top

Go:   name := "Alex"; age := 20
来源：http://otu.shuidangran.top

Ruby: name = "Alex"; age = 20
来源：http://aer.jinqigufen.top

C#:   string name = "Alex"; int age = 20;
来源：http://mgq.gotoacloud.top

[A03] 常量定义
来源：http://irj.c1oappe.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://had.dashuyun.cn

PHP:  const PI = 3.14159;
来源：http://uvu.vehdjk.com

JS:   const PI = 3.14159;
来源：http://nrg.yuanzhike.top

TS:   const PI: number = 3.14159;
来源：http://emc.zhengqikj.top

Java: static final double PI = 3.14159;
来源：http://cna.fehbvm.com

Go:   const PI = 3.14159
来源：http://vet.dashuyun.cn

Ruby: PI = 3.14159
来源：http://kbi.shangyingyoupin.top

C#:   const double PI = 3.14159;
来源：http://kzb.bbcook.cn

[A04] 判断变量类型
来源：http://hqq.aibaodan.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cuz.yj20258.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vrn.shuidangran.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zdr.yuxming.cn

TS:   typeof x; x instanceof Date
来源：http://nad.yongpay.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xxn.52xcode.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ids.aizwys.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://jio.daxiang520.top

C#:   x.GetType().Name; x is int
来源：http://uwr.andypj.xyz

[A05] 整数除法与取模
来源：http://rcj.gzhubu.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lef.mhx1999.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://uth.gogol.net.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kge.pycfn.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zmv.pycfn.com


<!-- 参考信息 -->