代发 wailian999

[U47] PHP：联合类型
来源：http://xst.tanke756.top

int|string $id
来源：http://ygj.ybcxt.top

[U48] PHP：纯枚举
来源：http://aku.zhengqikj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://esu.gaohongyu789.top

[U49] PHP：只读属性
来源：http://isz.shanyushiyangkeji.top

public readonly string $name
来源：http://xwl.pycfn.com

[U50] PHP：构造器属性提升
来源：http://fga.iojbl.cn

public function __construct(private int $id) {}
来源：http://eaz.nanxuanxn.top

[U51] PHP：数组解构
来源：http://ygq.hnqzz.top

[$a, $b] = $arr;
来源：http://njd.ivvv.top

[U52] PHP：箭头函数
来源：http://jqu.shzxlz.cn

$double = fn($x) => $x * 2;
来源：http://oan.ybcxt.top

[U53] PHP：空合并运算符
来源：http://orv.chenlongwang.top

$v = $a ?? $b ?? "default";
来源：http://cet.yuxming.cn

[U54] PHP：空安全调用
来源：http://yzs.52xcode.cn

$obj?->method()
来源：http://ert.epnwcf.com

[U55] PHP：match 表达式
来源：http://ezq.iojbl.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vvu.meibo888.top

[U56] PHP：命名参数
来源：http://txs.iojbl.cn

f(a: 1, b: 2)
来源：http://jri.nanxinkj.top

[U57] PHP：字符串插值
来源：http://dfj.cdnleiting.top

"值: {$a}"
来源：http://yrh.yj202588.top

[U58] PHP：数组三件套
来源：http://yql.cqqwz.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rjh.yfazqb.com

[U59] PHP：自定义排序
来源：http://uax.vqdsnc.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ltb.tian-w.cn

[U60] PHP：JSON 编解码
来源：http://opi.sufxvd.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tyy.jiagoushi.top

[U61] PHP：正则
来源：http://hfj.sweek.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kgz.fehbvm.com

[U62] PHP：日期对象
来源：http://sed.iojbl.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qzp.0kj1m.cn

[U63] PHP：文件读写
来源：http://kzk.ydjk.org.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fda.jinghuilouyu.cn

[U64] PHP：目录遍历
来源：http://gfu.guannengcc.top

glob("dir/*.php");  scandir("dir");
来源：http://ygi.cucudq.cn

[U65] PHP：会话
来源：http://eke.zdbjq.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cbp.zhixingplan.top

[U66] PHP：设置 Cookie
来源：http://bhl.chenlongwang.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mfg.yongpay.top

[U67] PHP：处理文件上传
来源：http://ssp.yfazqb.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zuz.xuetiantiany.cn

[U68] PHP：PDO 连接
来源：http://izj.dashuyun.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mwk.xinyue.icu

[U69] PHP：PDO 预处理
来源：http://imq.sxryk.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ovu.yvedp.cn

[U70] PHP：PDO 事务
来源：http://vct.cheryme.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://thz.wangdashe.top

[U71] PHP：抛出异常
来源：http://ouh.daria6918.cn

throw new RuntimeException("失败", 500);
来源：http://pru.sxryk.cn

[U72] PHP：写错误日志
来源：http://rpf.jinyuanbaomall.cn

error_log("失败: " . $e->getMessage());
来源：http://tti.zhengqikj.top

[U73] PHP：读取 ini 配置
来源：http://kdl.kuanghao11.cn

parse_ini_file("config.ini", true)
来源：http://odl.pycfn.com

[U74] PHP：读取环境变量
来源：http://apk.gaohongyu789.top

getenv("APP_ENV") ?: "production"
来源：http://ahd.tarul.cn

[U75] PHP：依赖注入
来源：http://zvs.pycfn.com

composer require psr/container
来源：http://xch.yuxming.cn

[U76] PHP：简单路由
来源：http://idx.xuetiantiany.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cht.yangfankeji.com

[U77] PHP：模板渲染
来源：http://rtu.smart0.xyz

composer require twig/twig
来源：http://eqk.epnwcf.com

[U78] PHP：单元测试
来源：http://bhe.zhengqikj.top

composer require --dev phpunit/phpunit
来源：http://fey.fanxiaobao.xyz

[U79] PHP：静态分析
来源：http://xxn.gotoacloud.top

composer require --dev phpstan/phpstan
来源：http://cmz.yj202588.top

[U80] PHP：代码规范修复
来源：http://azh.ppjwa.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://aeg.zdbjq.cn

[U81] JS：初始化项目
来源：http://xzl.epnwcf.com

npm init -y;  npm i express
来源：http://njz.sysykeji.top

[U82] JS：package.json 脚本
来源：http://wmk.gzhubu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gfv.chenzaomai.com

[U83] JS：ES Module 导入导出
来源：http://cay.wangdashe.top

export const a = 1;  import { a } from "./m.js";
来源：http://fam.jianghu66.top

[U84] JS：CommonJS 写法
来源：http://sla.jqgufenzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://qvf.ydjk.org.cn

[U85] JS：可选链
来源：http://dab.xuetiantiany.cn

a?.b?.c
来源：http://bid.mhx1999.top

[U86] JS：空值合并
来源：http://cug.zhongyouzk.top

a ?? b
来源：http://uhp.hnqzz.top

[U87] JS：解构默认值
来源：http://zom.aizwys.cn

const { a = 1, b = 2 } = obj;
来源：http://uiu.sxryk.cn

[U88] JS：对象展开合并
来源：http://wee.ppjwa.cn

{ ...a, ...b }
来源：http://fzd.yj20258.top

[U89] JS：数组去重
来源：http://dkt.pengpengdd.cyou

[...new Set(arr)]
来源：http://ikz.yj202588.top

[U90] JS：数字数组排序
来源：http://ali.zhixingplan.top

[...arr].sort((a, b) => a - b)
来源：http://jpy.xziqi.cn

[U91] JS：对象键值遍历
来源：http://thr.jianghu66.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://iqy.fanxiaobao.xyz

[U92] JS：深拷贝
来源：http://jbj.pengpengdd.cyou

structuredClone(obj)
来源：http://gsl.sysykeji.top

[U93] JS：模板字符串
来源：http://rfb.jlsjyb.cn

`共 ${n} 条`
来源：http://cok.cucudq.cn

[U94] JS：箭头函数
来源：http://pts.daria6918.cn

const double = x => x * 2;
来源：http://wrx.hnxiangtu.top

[U95] JS：Promise 包装
来源：http://mbe.fehbvm.com

new Promise((resolve, reject) => {})
来源：http://dpg.andypj.xyz

[U96] JS：async/await 与异常
来源：http://hat.feifeiyinyue.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tow.hfpthk.cn

[U97] JS：并发请求
来源：http://mxc.sufxvd.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mwy.ctjpmb.com

[U98] JS：fetch 带 JSON
来源：http://zgg.sweek.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://njy.jlsjyb.cn

[U99] JS：事件监听
来源：http://aml.yj20258888.top

el.addEventListener("click", e => {})
来源：http://fnu.ivvv.top

[U100] JS：DOM 查询
来源：http://roo.cdnleiting.top

document.querySelector(".item")
来源：http://xdt.yueranfly.top

[U101] JS：classList 操作
来源：http://hwz.yonumen.top

el.classList.toggle("active")
来源：http://txg.fzhhl.top

[U102] JS：本地存储
来源：http://fcl.tian-w.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sme.redwolf501.top

[U103] JS：定时器
来源：http://cmh.quarkkingdee.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pjf.zhiwuduotai.top

[U104] JS：防抖
来源：http://wpg.haohaochexian.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://scg.yvedp.cn

[U105] JS：节流
来源：http://sex.gogol.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lpq.kuanghao11.cn

[U106] JS：日期格式化
来源：http://tpr.cashguo.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dko.aizwys.cn

[U107] JS：数字千分位
来源：http://xbu.yonumen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://shg.aibaodan.cn

[U108] JS：随机整数
来源：http://kne.zhoulong.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qsu.ywan-chungtsiang.top

[U109] JS：数组分组
来源：http://cyj.xylfe.cn

Object.groupBy(arr, x => x.type)
来源：http://ffj.sjlbkw.cn

[U110] JS：数组分块
来源：http://vwe.jinyuanbaomall.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qod.zhixingplan.top

[U111] JS：对象转 Map
来源：http://cph.xingfuxueyuan.xyz

new Map(Object.entries(obj))
来源：http://yjr.ydzc1.top

[U112] JS：字符串补位
来源：http://zoa.nwbrower.top

"7".padStart(3, "0")
来源：http://iib.yueranfly.top

[U113] JS：正则替换全部
来源：http://rtq.zdbjq.cn

s.replaceAll("a", "b")
来源：http://jli.fzhhl.top

[U114] JS：JSON 深比较
来源：http://jwq.yfazqb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://tjy.smart0.xyz

[U115] JS：生成 UUID
来源：http://zvs.gotoacloud.top

crypto.randomUUID()
来源：http://jjp.gogol.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://fth.hfpthk.cn

/** @param {string} name */ function f(name) {}
来源：http://kcm.ywan-chungtsiang.top

[U117] JS：单元测试
来源：http://jxn.shanyushiyangtech.top

npm i -D vitest;  npx vitest
来源：http://anf.fzhhl.top

[U118] JS：开发服务器
来源：http://ydt.fanxiaobao.xyz

npm i -D vite;  npx vite
来源：http://lno.zycfv.cn

[U119] JS：生产构建
来源：http://idl.zdbjq.cn

npx vite build
来源：http://xpq.hfpthk.cn

[U120] JS：读取环境变量（Vite）
来源：http://ccc.fehbvm.com

import.meta.env.VITE_API_URL
来源：http://obn.guannengcc.top

================================================================================
来源：http://gux.jinqigfzy.top

统计汇总
来源：http://eno.hcnkem.com

================================================================================
来源：http://mjx.c1oappe.top

按语言统计（条）：
来源：http://aly.pengpengdd.cyou

Python ......... 252
来源：http://kfh.zhixingplan.top

PHP ............ 252
来源：http://dbl.wangdashe.top

JavaScript ..... 252
来源：http://joz.316326.xyz

TypeScript ..... 212
来源：http://cod.ydjk.org.cn

Java ........... 212
来源：http://pdo.kuanghao11.cn

Go ............. 212
来源：http://rep.daxiang520.top

Ruby ........... 212
来源：http://xrl.daria6918.cn

C# ............. 212
来源：http://qvu.tarul.cn

C .............. 30
来源：http://edl.jinyuanbaomall.cn

C++ ............ 30
来源：http://bvc.bbcook.cn

SQL ............ 90
来源：http://gfo.fanxiaobao.xyz

Bash ........... 80
来源：http://wcb.shuidangran.top

Kotlin ......... 15
来源：http://qxe.xuanzx.com

Swift .......... 15
来源：http://tdy.andypj.xyz

Lua ............ 10
来源：http://bwe.redwolf501.top

Perl ........... 10
来源：http://huz.sweek.top

Scala .......... 10
来源：http://qnr.zdqjudy.top

------------------------------------
来源：http://rrq.cashguo.top

合计 ........... 2106 条
来源：http://rdq.zhiwuduotai.top

按章节统计：
来源：http://xxe.jianghu66.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ldq.zdqjudy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://btl.nwbrower.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fky.yangfankeji.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tlw.jlsjyb.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rtu.zdqjudy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xgd.316326.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mzn.nanxinkj.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://iji.xylfe.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jlz.haohaochexian.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bwd.dianchejie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oel.cashguo.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mir.epnwcf.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lgs.xinyue.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bdw.shuidangran.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lke.shuidangran.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fgo.yangfankeji.com

Q SQL 专题                              90
来源：http://irm.svipenyu.cn

R Bash 专题                             80
来源：http://acx.sxryk.cn

S C / C++ 专题                          60
来源：http://cqz.ivvv.top

T 其他语言补充                          60
来源：http://vfm.ppjwa.cn

U 高频实用片段                         120
来源：http://bjq.epnwcf.com

------------------------------------
来源：http://lez.jqgfzy.top

合计                                  2106 条
来源：http://mli.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://tpm.hesvh.cn

使用提醒
来源：http://egk.yangfankeji.com

--------------------------------------------------------------------------------
来源：http://tlx.xylfe.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qux.fengsongda.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zhl.zhaomingkeji.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gkx.tian-w.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://shu.gotoacloud.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xuy.xylfe.cn

—— 文件结束 ——
来源：http://eth.ppjwa.cn

================================================================================
来源：http://rls.jiagoushi.top

程序语言常见例子速查手册（2024 版）
来源：http://lag.xuetiantiany.cn

Common Programming Examples Cheat Book
来源：http://uhs.yvedp.cn

================================================================================
来源：http://tls.xinyue.icu

【收录内容】
来源：http://jej.hcnkem.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://trs.tarul.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://utl.jqgfzy.top

SQL · Bash · C · C++
来源：http://gsp.xziqi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://svu.chenzaomai.com

【使用说明】
来源：http://nle.jinqigfzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vap.feifeiyinyue.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://skk.jqgufenzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nmm.jiagoushi.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kid.yuanzhike.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ory.hfpthk.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xlt.uphjek.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hnv.xuanzx.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jpt.smart0.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lxh.chenzaomai.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ldu.tarul.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zxv.jiagoushi.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ikb.zhoulong.xyz

【文件统计】
来源：http://rqn.guannengcc.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yqw.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://qgw.chenzaomai.com

目  录
来源：http://oje.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://iyz.zhongyouzk.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lnb.ivvv.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bub.jiagoushi.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nxv.zdqjudy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hgd.fzhhl.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vok.shanyushiyangtech.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://obu.yfazqb.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fdv.shangyingyoupin.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lhz.zdqjudy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bjq.ctjpmb.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dlq.zhixingplan.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dek.gaohongyu789.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dxe.gaohongyu789.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gff.yfazqb.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xiq.hongshengwenyu.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ely.sxryk.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mvr.iojbl.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jbz.birdmap.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://hju.jinqigufen.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xmw.zhaomingkeji.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uka.shangyingyoupin.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kgq.hammf.cn

================================================================================
来源：http://mdv.sxryk.cn

A. 基础语法与类型
来源：http://ktk.gaohongyu789.top

================================================================================
来源：http://euo.ydzc1.top

[A01] Hello World
来源：http://hrs.hesvh.cn

Py:   print("Hello, World!")
来源：http://usx.yj20258888.top

PHP:  echo "Hello, World!";
来源：http://vzz.birdmap.top

JS:   console.log("Hello, World!");
来源：http://uji.zdqjudy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dgg.quarkkingdee.top

Java: System.out.println("Hello, World!");
来源：http://egm.epnwcf.com

Go:   fmt.Println("Hello, World!")
来源：http://dax.feifeiyinyue.top

Ruby: puts "Hello, World!"
来源：http://nvp.ehwqpu.com

C#:   Console.WriteLine("Hello, World!");
来源：http://rgo.nanxinkj.top

[A02] 变量声明与赋值
来源：http://xrd.aizwys.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xof.ywan-chungtsiang.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ier.vehdjk.com

JS:   let name = "Alex"; const age = 20;
来源：http://ble.vehdjk.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://syn.shzxlz.cn

Java: String name = "Alex"; int age = 20;
来源：http://eow.ywan-chungtsiang.top

Go:   name := "Alex"; age := 20
来源：http://ryr.hywenlv.cn

Ruby: name = "Alex"; age = 20
来源：http://inz.guowangkeji.top

C#:   string name = "Alex"; int age = 20;
来源：http://tld.xylfe.cn

[A03] 常量定义
来源：http://cca.xuetiantiany.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kts.hfpthk.cn

PHP:  const PI = 3.14159;
来源：http://wpi.daria6918.cn

JS:   const PI = 3.14159;
来源：http://yuy.tian-w.cn

TS:   const PI: number = 3.14159;
来源：http://ule.ydjk.org.cn

Java: static final double PI = 3.14159;
来源：http://iug.mhx1999.top

Go:   const PI = 3.14159
来源：http://vkz.dashuyun.cn

Ruby: PI = 3.14159
来源：http://huz.xuetiantiany.cn

C#:   const double PI = 3.14159;
来源：http://kxz.uphjek.com

[A04] 判断变量类型
来源：http://ajy.52xcode.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://kje.sxryk.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hwr.0kj1m.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://koh.zhaomingkeji.xyz

TS:   typeof x; x instanceof Date
来源：http://roi.fktsv.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fbt.shanyushiyangkeji.top

Go:   reflect.TypeOf(x).Name()
来源：http://dwf.yvedp.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://zwp.wangshuangyany.cn

C#:   x.GetType().Name; x is int
来源：http://jhb.vqdsnc.cn

[A05] 整数除法与取模
来源：http://sdn.sufxvd.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ogu.epnwcf.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://tap.ehwqpu.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rsi.svipenyu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gfc.hesvh.cn

Java: 7 / 2; 7 % 2
来源：http://lge.zhixingplan.top

Go:   7 / 2; 7 % 2
来源：http://dbl.tian-w.cn

Ruby: 7 / 2; 7 % 2
来源：http://gzn.tarul.cn

C#:   7 / 2; 7 % 2
来源：http://uer.yanxiufei.cn


<!-- 参考信息 -->