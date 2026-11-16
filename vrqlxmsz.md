代发 wailian999

[U47] PHP：联合类型
来源：http://crw.uphjek.com

int|string $id
来源：http://ipq.c1oappe.top

[U48] PHP：纯枚举
来源：http://dog.gaohongyu789.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dcy.yj20258888.top

[U49] PHP：只读属性
来源：http://jwk.xinyue.icu

public readonly string $name
来源：http://bfd.316326.xyz

[U50] PHP：构造器属性提升
来源：http://dmu.yanxiufei.cn

public function __construct(private int $id) {}
来源：http://mst.cheryme.top

[U51] PHP：数组解构
来源：http://ueq.sysykeji.top

[$a, $b] = $arr;
来源：http://bbx.sxryk.cn

[U52] PHP：箭头函数
来源：http://mva.guannengcc.top

$double = fn($x) => $x * 2;
来源：http://smc.shuidangran.top

[U53] PHP：空合并运算符
来源：http://rvs.feifeiyinyue.top

$v = $a ?? $b ?? "default";
来源：http://scr.jinyuanbaomall.cn

[U54] PHP：空安全调用
来源：http://nyp.jinghuilouyu.cn

$obj?->method()
来源：http://wqg.epnwcf.com

[U55] PHP：match 表达式
来源：http://jlq.pengpengdd.cyou

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xlp.fengsongda.top

[U56] PHP：命名参数
来源：http://qte.xziqi.cn

f(a: 1, b: 2)
来源：http://gyp.ivvv.top

[U57] PHP：字符串插值
来源：http://qcp.cucudq.cn

"值: {$a}"
来源：http://zou.zdqjudy.top

[U58] PHP：数组三件套
来源：http://xbj.wangdashe.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ueq.gzhubu.top

[U59] PHP：自定义排序
来源：http://kjo.cqqwz.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wua.ehwqpu.com

[U60] PHP：JSON 编解码
来源：http://wsg.yanxiufei.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://joe.havefunace.top

[U61] PHP：正则
来源：http://myl.yongpay.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lpg.hywenlv.cn

[U62] PHP：日期对象
来源：http://flv.haohaochexian.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wvk.zdbjq.cn

[U63] PHP：文件读写
来源：http://ccm.pengpengdd.cyou

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uib.jiagoushi.top

[U64] PHP：目录遍历
来源：http://psp.yj20258888.top

glob("dir/*.php");  scandir("dir");
来源：http://xul.cqqwz.cn

[U65] PHP：会话
来源：http://xey.c1oappe.top

session_start();  $_SESSION["uid"] = 1;
来源：http://fml.jinghuilouyu.cn

[U66] PHP：设置 Cookie
来源：http://zdx.jinqigfzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://koj.gotoacloud.top

[U67] PHP：处理文件上传
来源：http://btx.smart0.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gss.mhx1999.top

[U68] PHP：PDO 连接
来源：http://mwg.jlsjyb.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://btx.bbcook.cn

[U69] PHP：PDO 预处理
来源：http://kas.cheryme.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bby.ppjwa.cn

[U70] PHP：PDO 事务
来源：http://rpj.hammf.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xpy.andypj.xyz

[U71] PHP：抛出异常
来源：http://rsu.zhoulong.xyz

throw new RuntimeException("失败", 500);
来源：http://zbl.chenjidiqi.icu

[U72] PHP：写错误日志
来源：http://ujy.jinqigufen.top

error_log("失败: " . $e->getMessage());
来源：http://edh.wangshuangyany.cn

[U73] PHP：读取 ini 配置
来源：http://zub.cdnleiting.top

parse_ini_file("config.ini", true)
来源：http://grc.zhaomingkeji.xyz

[U74] PHP：读取环境变量
来源：http://yqr.pycfn.com

getenv("APP_ENV") ?: "production"
来源：http://hww.ctjpmb.com

[U75] PHP：依赖注入
来源：http://shk.sjlbkw.cn

composer require psr/container
来源：http://pck.shangyingyoupin.top

[U76] PHP：简单路由
来源：http://bvd.guannengcc.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pnu.sysykeji.top

[U77] PHP：模板渲染
来源：http://rba.yueranfly.top

composer require twig/twig
来源：http://jkh.havefunace.top

[U78] PHP：单元测试
来源：http://wht.shangyingyoupin.top

composer require --dev phpunit/phpunit
来源：http://tlh.pengpengdd.cyou

[U79] PHP：静态分析
来源：http://yad.andypj.xyz

composer require --dev phpstan/phpstan
来源：http://nbv.chenjidiqi.icu

[U80] PHP：代码规范修复
来源：http://yet.guowangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://nqd.jyoumei.cn

[U81] JS：初始化项目
来源：http://git.jinyuanbaomall.cn

npm init -y;  npm i express
来源：http://ivg.jyoumei.cn

[U82] JS：package.json 脚本
来源：http://ryx.yfazqb.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://twj.jianghu66.top

[U83] JS：ES Module 导入导出
来源：http://vop.ybcxt.top

export const a = 1;  import { a } from "./m.js";
来源：http://niq.bjfxy.top

[U84] JS：CommonJS 写法
来源：http://wke.jinqigfzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://uke.guowangkeji.top

[U85] JS：可选链
来源：http://oda.chenjidiqi.icu

a?.b?.c
来源：http://blf.hesvh.cn

[U86] JS：空值合并
来源：http://uaz.dashuyun.cn

a ?? b
来源：http://vwk.xuetiantiany.cn

[U87] JS：解构默认值
来源：http://vjp.sysykeji.top

const { a = 1, b = 2 } = obj;
来源：http://umv.nanxinkj.top

[U88] JS：对象展开合并
来源：http://rwm.vqdsnc.cn

{ ...a, ...b }
来源：http://onc.nwbrower.top

[U89] JS：数组去重
来源：http://ngu.fehbvm.com

[...new Set(arr)]
来源：http://mpb.zhixingplan.top

[U90] JS：数字数组排序
来源：http://adt.hongshengwenyu.top

[...arr].sort((a, b) => a - b)
来源：http://cck.hysaishi.cn

[U91] JS：对象键值遍历
来源：http://klk.snrcjt.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oks.jiagoushi.top

[U92] JS：深拷贝
来源：http://cyx.9152youxi.cn

structuredClone(obj)
来源：http://cqm.pycfn.com

[U93] JS：模板字符串
来源：http://wen.yj20258.top

`共 ${n} 条`
来源：http://aqa.cucudq.cn

[U94] JS：箭头函数
来源：http://rtj.ivvv.top

const double = x => x * 2;
来源：http://mxw.gaohongyu789.top

[U95] JS：Promise 包装
来源：http://grh.cdnleiting.top

new Promise((resolve, reject) => {})
来源：http://vjr.kuanghao11.cn

[U96] JS：async/await 与异常
来源：http://eij.yj20258888.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lxr.ivvv.top

[U97] JS：并发请求
来源：http://ddo.daxiang520.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://yeg.xuetiantiany.cn

[U98] JS：fetch 带 JSON
来源：http://avm.zhengqikj.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://whz.jqgfzy.top

[U99] JS：事件监听
来源：http://qdk.yueranfly.top

el.addEventListener("click", e => {})
来源：http://sfu.kuanghao11.cn

[U100] JS：DOM 查询
来源：http://gmp.hnxiangtu.top

document.querySelector(".item")
来源：http://xws.vehdjk.com

[U101] JS：classList 操作
来源：http://qgc.smart0.xyz

el.classList.toggle("active")
来源：http://ksu.zdbjq.cn

[U102] JS：本地存储
来源：http://byk.svipenyu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bge.yfazqb.com

[U103] JS：定时器
来源：http://izm.shanyushiyangkeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ckb.svipenyu.cn

[U104] JS：防抖
来源：http://jlx.aizwys.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nur.andypj.xyz

[U105] JS：节流
来源：http://jux.nwbrower.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://utq.pycfn.com

[U106] JS：日期格式化
来源：http://tuz.gogol.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://awo.zhijiandao.cn

[U107] JS：数字千分位
来源：http://gwp.yonumen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qbk.zhijiandao.cn

[U108] JS：随机整数
来源：http://xql.haohaochexian.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wjb.zhaomingkeji.xyz

[U109] JS：数组分组
来源：http://csr.ybcxt.top

Object.groupBy(arr, x => x.type)
来源：http://ify.zdbjq.cn

[U110] JS：数组分块
来源：http://qys.sysykeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://toi.ctjpmb.com

[U111] JS：对象转 Map
来源：http://igk.smart0.xyz

new Map(Object.entries(obj))
来源：http://iob.ybcxt.top

[U112] JS：字符串补位
来源：http://gil.meibo888.top

"7".padStart(3, "0")
来源：http://ixl.jqgufenzy.top

[U113] JS：正则替换全部
来源：http://ydy.ppjwa.cn

s.replaceAll("a", "b")
来源：http://jah.ivvv.top

[U114] JS：JSON 深比较
来源：http://czl.iojbl.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hrb.guannengcc.top

[U115] JS：生成 UUID
来源：http://zgp.cheryme.top

crypto.randomUUID()
来源：http://ciu.mhx1999.top

[U116] JS：类型检查（JSDoc）
来源：http://bqi.pycfn.com

/** @param {string} name */ function f(name) {}
来源：http://tcf.9152youxi.cn

[U117] JS：单元测试
来源：http://ebo.52xcode.cn

npm i -D vitest;  npx vitest
来源：http://lqq.jinqigfzy.top

[U118] JS：开发服务器
来源：http://rhp.yj202588.top

npm i -D vite;  npx vite
来源：http://nyf.cucudq.cn

[U119] JS：生产构建
来源：http://xxs.pengpengdd.cyou

npx vite build
来源：http://zyg.ehwqpu.com

[U120] JS：读取环境变量（Vite）
来源：http://kzf.shuidangran.top

import.meta.env.VITE_API_URL
来源：http://nii.tanke756.top

================================================================================
来源：http://krg.yangfankeji.com

统计汇总
来源：http://boa.hesvh.cn

================================================================================
来源：http://ufx.chenlongwang.top

按语言统计（条）：
来源：http://ncl.chenzaomai.com

Python ......... 252
来源：http://piu.bbcook.cn

PHP ............ 252
来源：http://rux.tian-w.cn

JavaScript ..... 252
来源：http://jhe.zhongyouzk.top

TypeScript ..... 212
来源：http://wzi.fengsongda.top

Java ........... 212
来源：http://lgu.vehdjk.com

Go ............. 212
来源：http://ita.sxryk.cn

Ruby ........... 212
来源：http://fyc.zhengqikj.top

C# ............. 212
来源：http://zrz.hysaishi.cn

C .............. 30
来源：http://vnv.zdqjudy.top

C++ ............ 30
来源：http://iqf.jqgfzy.top

SQL ............ 90
来源：http://prx.52xcode.cn

Bash ........... 80
来源：http://znv.guowangkeji.top

Kotlin ......... 15
来源：http://jbp.cashguo.top

Swift .......... 15
来源：http://xnt.316326.xyz

Lua ............ 10
来源：http://lhw.0kj1m.cn

Perl ........... 10
来源：http://pfk.jyoumei.cn

Scala .......... 10
来源：http://mxs.jiagoushi.top

------------------------------------
来源：http://scp.fzhhl.top

合计 ........... 2106 条
来源：http://yci.shuidangran.top

按章节统计：
来源：http://wnk.yj20258888.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nkh.shanyushiyangtech.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://auk.vehdjk.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qbe.zhaomingkeji.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dsk.jiagoushi.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ssx.hongshengwenyu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fxl.gotoacloud.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://exj.chenlongwang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://srk.yuanzhike.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zhz.daria6918.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jmg.fktsv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ngd.svipenyu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://euo.shanyushiyangkeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ndv.uphjek.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://znq.jlsjyb.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fim.sysykeji.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tbo.tianlin.xyz

Q SQL 专题                              90
来源：http://his.ydjk.org.cn

R Bash 专题                             80
来源：http://ddb.shanyushiyangtech.top

S C / C++ 专题                          60
来源：http://vxg.fktsv.cn

T 其他语言补充                          60
来源：http://jci.shangyingyoupin.top

U 高频实用片段                         120
来源：http://eqi.quarkkingdee.top

------------------------------------
来源：http://qxx.gotoacloud.top

合计                                  2106 条
来源：http://ccp.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://dfr.ywan-chungtsiang.top

使用提醒
来源：http://vfk.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://yze.meibo888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zgj.sysykeji.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gfv.hcnkem.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://irj.aizwys.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://rgp.nanxuanxn.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://opm.daxiang520.top

—— 文件结束 ——
来源：http://nim.cashguo.top

================================================================================
来源：http://uqx.sjlbkw.cn

程序语言常见例子速查手册（2024 版）
来源：http://hhq.gzhubu.top

Common Programming Examples Cheat Book
来源：http://uxa.yuxming.cn

================================================================================
来源：http://zta.sweek.top

【收录内容】
来源：http://xvh.aizwys.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pbc.fehbvm.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wxs.havefunace.top

SQL · Bash · C · C++
来源：http://ojx.bjfxy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://eed.hnqzz.top

【使用说明】
来源：http://oai.yvedp.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yuk.ydzc1.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kma.wangshuangyany.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xty.guowangkeji.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://red.chenzaomai.com

Bash:  Shell         C:     C             C++:   C++
来源：http://rry.xingfuxueyuan.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wml.ivvv.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ssq.yuanzhike.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kuu.xingfuxueyuan.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rvu.guowangkeji.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gmb.daria6918.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dbz.ppjwa.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gkp.daxiang520.top

【文件统计】
来源：http://chj.guowangkeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://czz.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://dkr.fzhhl.top

目  录
来源：http://xei.wangdashe.top

--------------------------------------------------------------------------------
来源：http://azk.sufxvd.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sqn.wangshuangyany.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wve.aibaodan.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nat.fanxiaobao.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fuf.gzhubu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://snt.pengpengdd.cyou

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uvg.fengsongda.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ufp.fktsv.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zrn.uphjek.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://frd.jianghu66.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://thq.zhoulong.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wxw.jiagoushi.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dxx.yj20258888.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nmb.zhixingplan.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wbx.jinqigfzy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://frt.chenjidiqi.icu

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yjq.pengpengdd.cyou

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nqs.xziqi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://aks.fehbvm.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qxu.xinyue.icu

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ntw.ehwqpu.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yqz.xinyue.icu

================================================================================
来源：http://tlh.jianghu66.top

A. 基础语法与类型
来源：http://ukm.xinyue.icu

================================================================================
来源：http://ian.jinqigufen.top

[A01] Hello World
来源：http://unm.zhengqikj.top

Py:   print("Hello, World!")
来源：http://yod.9152youxi.cn

PHP:  echo "Hello, World!";
来源：http://rjj.yangfankeji.com

JS:   console.log("Hello, World!");
来源：http://vtp.fengsongda.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ohg.zdqjudy.top

Java: System.out.println("Hello, World!");
来源：http://axu.ehwqpu.com

Go:   fmt.Println("Hello, World!")
来源：http://hno.sxryk.cn

Ruby: puts "Hello, World!"
来源：http://hzq.52xcode.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yod.zdqjudy.top

[A02] 变量声明与赋值
来源：http://qgr.0kj1m.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://isc.shanyushiyangkeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ixl.zhoulong.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://fcp.redwolf501.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nhc.chenlongwang.top

Java: String name = "Alex"; int age = 20;
来源：http://znm.birdmap.top

Go:   name := "Alex"; age := 20
来源：http://ekr.xylfe.cn

Ruby: name = "Alex"; age = 20
来源：http://hxx.tarul.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vwa.fengsongda.top

[A03] 常量定义
来源：http://xms.yvedp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fho.jinghuilouyu.cn

PHP:  const PI = 3.14159;
来源：http://vpz.uphjek.com

JS:   const PI = 3.14159;
来源：http://who.jqgufenzy.top

TS:   const PI: number = 3.14159;
来源：http://hhd.hysaishi.cn

Java: static final double PI = 3.14159;
来源：http://smt.sufxvd.cn

Go:   const PI = 3.14159
来源：http://vrt.52xcode.cn

Ruby: PI = 3.14159
来源：http://hqa.aibaodan.cn

C#:   const double PI = 3.14159;
来源：http://ghm.yvedp.cn

[A04] 判断变量类型
来源：http://fhg.mhx1999.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://yyj.zhixingplan.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qaw.andypj.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dbo.zhengqikj.top

TS:   typeof x; x instanceof Date
来源：http://ioc.yongpay.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zzg.chenzaomai.com

Go:   reflect.TypeOf(x).Name()
来源：http://amq.yongpay.top

Ruby: x.class; x.is_a?(Integer)
来源：http://alr.sxryk.cn

C#:   x.GetType().Name; x is int
来源：http://rrv.wangshuangyany.cn

[A05] 整数除法与取模
来源：http://qdq.birdmap.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ray.hongshengwenyu.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://uyw.gogol.net.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://myq.yfazqb.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fyy.haohaochexian.top

Java: 7 / 2; 7 % 2
来源：http://mly.hywenlv.cn

Go:   7 / 2; 7 % 2
来源：http://tos.yanxiufei.cn

Ruby: 7 / 2; 7 % 2
来源：http://ghu.zhongyouzk.top

C#:   7 / 2; 7 % 2
来源：http://oli.kuanghao11.cn


<!-- 参考信息 -->