代发 wailian999

[U47] PHP：联合类型
来源：http://prs.jinqigufen.top

int|string $id
来源：http://rez.havefunace.top

[U48] PHP：纯枚举
来源：http://fqx.cheryme.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qzi.meibo888.top

[U49] PHP：只读属性
来源：http://gbn.ehwqpu.com

public readonly string $name
来源：http://yev.sxryk.cn

[U50] PHP：构造器属性提升
来源：http://rwh.cdnleiting.top

public function __construct(private int $id) {}
来源：http://yox.sweek.top

[U51] PHP：数组解构
来源：http://jyp.quarkkingdee.top

[$a, $b] = $arr;
来源：http://xqm.zhixingplan.top

[U52] PHP：箭头函数
来源：http://idv.chenzaomai.com

$double = fn($x) => $x * 2;
来源：http://epg.iojbl.cn

[U53] PHP：空合并运算符
来源：http://tgi.vehdjk.com

$v = $a ?? $b ?? "default";
来源：http://qia.quarkkingdee.top

[U54] PHP：空安全调用
来源：http://wgl.nanxuanxn.top

$obj?->method()
来源：http://ukm.zdqjudy.top

[U55] PHP：match 表达式
来源：http://fxe.vehdjk.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rwi.xingfuxueyuan.xyz

[U56] PHP：命名参数
来源：http://nzq.gaohongyu789.top

f(a: 1, b: 2)
来源：http://elm.aibaodan.cn

[U57] PHP：字符串插值
来源：http://rfx.epnwcf.com

"值: {$a}"
来源：http://wgd.316326.xyz

[U58] PHP：数组三件套
来源：http://jzv.gogol.net.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gxr.zdbjq.cn

[U59] PHP：自定义排序
来源：http://cav.cashguo.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jpz.ydjk.org.cn

[U60] PHP：JSON 编解码
来源：http://tlw.yongpay.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lzd.52xcode.cn

[U61] PHP：正则
来源：http://nko.ybcxt.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://eew.iojbl.cn

[U62] PHP：日期对象
来源：http://lng.guannengcc.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dfx.yfazqb.com

[U63] PHP：文件读写
来源：http://pmq.wangdashe.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xmr.aizwys.cn

[U64] PHP：目录遍历
来源：http://vcj.tianlin.xyz

glob("dir/*.php");  scandir("dir");
来源：http://vft.yuanzhike.top

[U65] PHP：会话
来源：http://ffo.shangyingyoupin.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rup.sysykeji.top

[U66] PHP：设置 Cookie
来源：http://xoe.tian-w.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://duh.sufxvd.cn

[U67] PHP：处理文件上传
来源：http://lfz.hysaishi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rsb.hcnkem.com

[U68] PHP：PDO 连接
来源：http://box.aizwys.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qqm.quarkkingdee.top

[U69] PHP：PDO 预处理
来源：http://gft.fehbvm.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hqu.316326.xyz

[U70] PHP：PDO 事务
来源：http://vfu.yangfankeji.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://knh.yangfankeji.com

[U71] PHP：抛出异常
来源：http://pka.ydzc1.top

throw new RuntimeException("失败", 500);
来源：http://kew.tian-w.cn

[U72] PHP：写错误日志
来源：http://fkc.jlsjyb.cn

error_log("失败: " . $e->getMessage());
来源：http://wdi.bjfxy.top

[U73] PHP：读取 ini 配置
来源：http://dbz.fktsv.cn

parse_ini_file("config.ini", true)
来源：http://tav.shzxlz.cn

[U74] PHP：读取环境变量
来源：http://mkk.daria6918.cn

getenv("APP_ENV") ?: "production"
来源：http://ynq.jianghu66.top

[U75] PHP：依赖注入
来源：http://yto.ydzc1.top

composer require psr/container
来源：http://mws.shanyushiyangkeji.top

[U76] PHP：简单路由
来源：http://jnv.pengpengdd.cyou

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pdw.yj20258.top

[U77] PHP：模板渲染
来源：http://pzb.jianghu66.top

composer require twig/twig
来源：http://frm.316326.xyz

[U78] PHP：单元测试
来源：http://ynr.zycfv.cn

composer require --dev phpunit/phpunit
来源：http://hjb.zhengqikj.top

[U79] PHP：静态分析
来源：http://rwc.sysykeji.top

composer require --dev phpstan/phpstan
来源：http://cvr.cqqwz.cn

[U80] PHP：代码规范修复
来源：http://cpb.cqqwz.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yiu.tanke756.top

[U81] JS：初始化项目
来源：http://oes.haohaochexian.top

npm init -y;  npm i express
来源：http://efb.0kj1m.cn

[U82] JS：package.json 脚本
来源：http://kkm.nanxuanxn.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ucq.316326.xyz

[U83] JS：ES Module 导入导出
来源：http://hrg.zhiwuduotai.top

export const a = 1;  import { a } from "./m.js";
来源：http://egj.tarul.cn

[U84] JS：CommonJS 写法
来源：http://vpp.fktsv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://blb.yj20258.top

[U85] JS：可选链
来源：http://clf.yj20258.top

a?.b?.c
来源：http://mdn.zhongyouzk.top

[U86] JS：空值合并
来源：http://nvy.hongshengwenyu.top

a ?? b
来源：http://eop.hcnkem.com

[U87] JS：解构默认值
来源：http://svi.fanxiaobao.xyz

const { a = 1, b = 2 } = obj;
来源：http://axn.xuanzx.com

[U88] JS：对象展开合并
来源：http://vwf.c1oappe.top

{ ...a, ...b }
来源：http://wtg.ywan-chungtsiang.top

[U89] JS：数组去重
来源：http://gpy.daria6918.cn

[...new Set(arr)]
来源：http://oss.yonumen.top

[U90] JS：数字数组排序
来源：http://xki.haohaochexian.top

[...arr].sort((a, b) => a - b)
来源：http://dhi.xinyue.icu

[U91] JS：对象键值遍历
来源：http://rmj.0kj1m.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vat.shzxlz.cn

[U92] JS：深拷贝
来源：http://snz.cqqwz.cn

structuredClone(obj)
来源：http://hgb.svipenyu.cn

[U93] JS：模板字符串
来源：http://skd.jlsjyb.cn

`共 ${n} 条`
来源：http://mxk.ydzc1.top

[U94] JS：箭头函数
来源：http://qpy.feifeiyinyue.top

const double = x => x * 2;
来源：http://ueo.jinyuanbaomall.cn

[U95] JS：Promise 包装
来源：http://fmt.xuetiantiany.cn

new Promise((resolve, reject) => {})
来源：http://abk.jqgfzy.top

[U96] JS：async/await 与异常
来源：http://ugj.andypj.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rae.zdqjudy.top

[U97] JS：并发请求
来源：http://qrl.sufxvd.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jez.hcnkem.com

[U98] JS：fetch 带 JSON
来源：http://qxr.jqgfzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cyo.daria6918.cn

[U99] JS：事件监听
来源：http://ipy.yanxiufei.cn

el.addEventListener("click", e => {})
来源：http://wzr.zhijiandao.cn

[U100] JS：DOM 查询
来源：http://rak.pengpengdd.cyou

document.querySelector(".item")
来源：http://dhw.mhx1999.top

[U101] JS：classList 操作
来源：http://kpm.cheryme.top

el.classList.toggle("active")
来源：http://rtv.jyoumei.cn

[U102] JS：本地存储
来源：http://kyo.yanxiufei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://srb.nanxinkj.top

[U103] JS：定时器
来源：http://oaa.meibo888.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gkn.shzxlz.cn

[U104] JS：防抖
来源：http://mds.jinqigufen.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tym.meibo888.top

[U105] JS：节流
来源：http://ucl.wangdashe.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zaj.zdbjq.cn

[U106] JS：日期格式化
来源：http://zmc.wangdashe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xhs.xziqi.cn

[U107] JS：数字千分位
来源：http://oox.jlsjyb.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fse.c1oappe.top

[U108] JS：随机整数
来源：http://hre.gogol.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tns.xingfuxueyuan.xyz

[U109] JS：数组分组
来源：http://war.kuanghao11.cn

Object.groupBy(arr, x => x.type)
来源：http://edx.chenlongwang.top

[U110] JS：数组分块
来源：http://oxi.shanyushiyangkeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://roy.pengpengdd.cyou

[U111] JS：对象转 Map
来源：http://zua.sweek.top

new Map(Object.entries(obj))
来源：http://txn.316326.xyz

[U112] JS：字符串补位
来源：http://deo.jqgufenzy.top

"7".padStart(3, "0")
来源：http://vgi.cashguo.top

[U113] JS：正则替换全部
来源：http://lvp.smart0.xyz

s.replaceAll("a", "b")
来源：http://szh.ehwqpu.com

[U114] JS：JSON 深比较
来源：http://mys.fengsongda.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://uko.cheryme.top

[U115] JS：生成 UUID
来源：http://fmj.uphjek.com

crypto.randomUUID()
来源：http://vgs.yongpay.top

[U116] JS：类型检查（JSDoc）
来源：http://egg.hcnkem.com

/** @param {string} name */ function f(name) {}
来源：http://qza.cashguo.top

[U117] JS：单元测试
来源：http://ttg.shangyingyoupin.top

npm i -D vitest;  npx vitest
来源：http://hxb.epnwcf.com

[U118] JS：开发服务器
来源：http://imt.daria6918.cn

npm i -D vite;  npx vite
来源：http://dae.cucudq.cn

[U119] JS：生产构建
来源：http://dvt.smart0.xyz

npx vite build
来源：http://bep.vehdjk.com

[U120] JS：读取环境变量（Vite）
来源：http://ozu.jinqigufen.top

import.meta.env.VITE_API_URL
来源：http://vup.quarkkingdee.top

================================================================================
来源：http://ald.jqgfzy.top

统计汇总
来源：http://kbg.yvedp.cn

================================================================================
来源：http://vka.gogol.net.cn

按语言统计（条）：
来源：http://hiv.cdnleiting.top

Python ......... 252
来源：http://ktg.gogol.net.cn

PHP ............ 252
来源：http://reg.vqdsnc.cn

JavaScript ..... 252
来源：http://yhr.pengpengdd.cyou

TypeScript ..... 212
来源：http://ohr.ehwqpu.com

Java ........... 212
来源：http://fsr.jinghuilouyu.cn

Go ............. 212
来源：http://ihs.zdqjudy.top

Ruby ........... 212
来源：http://wwg.shanyushiyangtech.top

C# ............. 212
来源：http://wqs.cheryme.top

C .............. 30
来源：http://msi.hywenlv.cn

C++ ............ 30
来源：http://rub.nanxuanxn.top

SQL ............ 90
来源：http://kid.xingfuxueyuan.xyz

Bash ........... 80
来源：http://txo.zhixingplan.top

Kotlin ......... 15
来源：http://lws.nanxinkj.top

Swift .......... 15
来源：http://oum.chenjidiqi.icu

Lua ............ 10
来源：http://qhn.ydzc1.top

Perl ........... 10
来源：http://exc.tanke756.top

Scala .......... 10
来源：http://pca.316326.xyz

------------------------------------
来源：http://qbp.fengsongda.top

合计 ........... 2106 条
来源：http://yrt.dianchejie.cn

按章节统计：
来源：http://oef.daxiang520.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://myb.chenjidiqi.icu

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rwj.fktsv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://evp.wangdashe.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nkl.fanxiaobao.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wbi.xingfuxueyuan.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fuw.cdnleiting.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gsc.yangfankeji.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vum.shzxlz.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nmo.wangshuangyany.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uta.cqqwz.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kje.tianlin.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wkm.xingfuxueyuan.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nkj.zhijiandao.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pwd.haohaochexian.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bpw.jinqigufen.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://uhn.havefunace.top

Q SQL 专题                              90
来源：http://daz.kuanghao11.cn

R Bash 专题                             80
来源：http://ajs.shzxlz.cn

S C / C++ 专题                          60
来源：http://xwg.zdqjudy.top

T 其他语言补充                          60
来源：http://pmb.daxiang520.top

U 高频实用片段                         120
来源：http://tjf.vqdsnc.cn

------------------------------------
来源：http://lqo.birdmap.top

合计                                  2106 条
来源：http://mcg.meibo888.top

--------------------------------------------------------------------------------
来源：http://omz.zhengqikj.top

使用提醒
来源：http://enx.havefunace.top

--------------------------------------------------------------------------------
来源：http://glo.vehdjk.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://whr.cashguo.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xfu.daxiang520.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dij.redwolf501.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ouw.xziqi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yqp.yuxming.cn

—— 文件结束 ——
来源：http://neu.nanxinkj.top

================================================================================
来源：http://mdj.sufxvd.cn

程序语言常见例子速查手册（2024 版）
来源：http://roe.nwbrower.top

Common Programming Examples Cheat Book
来源：http://vmt.hesvh.cn

================================================================================
来源：http://ckb.xingfuxueyuan.xyz

【收录内容】
来源：http://arh.yj20258888.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://lxx.chenjidiqi.icu

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://els.xuanzx.com

SQL · Bash · C · C++
来源：http://vao.shanyushiyangkeji.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vcb.jiagoushi.top

【使用说明】
来源：http://jnf.yfazqb.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hkl.yvedp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uqa.zhongyouzk.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hfz.kuanghao11.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://awq.nanxinkj.top

Bash:  Shell         C:     C             C++:   C++
来源：http://kqr.xylfe.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tda.ehwqpu.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rpk.yuanzhike.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jjr.sufxvd.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://sni.chenzaomai.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mmk.cucudq.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ioz.iojbl.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://iyj.tianlin.xyz

【文件统计】
来源：http://vqw.bbcook.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://aqm.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://tlr.zhijiandao.cn

目  录
来源：http://rds.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://vgi.dianchejie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ykf.shzxlz.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uob.havefunace.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lvq.ppjwa.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cmf.jinghuilouyu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dki.zdbjq.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xpx.yanxiufei.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tep.kuanghao11.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fbn.jinghuilouyu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qsg.tianlin.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cid.gzhubu.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://apb.xziqi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://juo.tanke756.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ehf.dashuyun.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jnw.jinqigfzy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://poc.shanyushiyangkeji.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://brr.hfpthk.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://adk.bjfxy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://wve.guannengcc.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vsr.chenjidiqi.icu

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nip.sysykeji.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uzp.zhongyouzk.top

================================================================================
来源：http://cfq.gogol.net.cn

A. 基础语法与类型
来源：http://oyt.jlsjyb.cn

================================================================================
来源：http://uwg.zhijiandao.cn

[A01] Hello World
来源：http://tzq.gotoacloud.top

Py:   print("Hello, World!")
来源：http://izo.bjfxy.top

PHP:  echo "Hello, World!";
来源：http://tli.svipenyu.cn

JS:   console.log("Hello, World!");
来源：http://hgv.shuidangran.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nxo.epnwcf.com

Java: System.out.println("Hello, World!");
来源：http://bqd.shanyushiyangtech.top

Go:   fmt.Println("Hello, World!")
来源：http://ywy.xuetiantiany.cn

Ruby: puts "Hello, World!"
来源：http://vjx.xuanzx.com

C#:   Console.WriteLine("Hello, World!");
来源：http://tck.c1oappe.top

[A02] 变量声明与赋值
来源：http://wgn.jiagoushi.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://abs.fktsv.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bbq.dashuyun.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ovy.andypj.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://svo.xuetiantiany.cn

Java: String name = "Alex"; int age = 20;
来源：http://nfu.jyoumei.cn

Go:   name := "Alex"; age := 20
来源：http://avt.guannengcc.top

Ruby: name = "Alex"; age = 20
来源：http://zhe.bbcook.cn

C#:   string name = "Alex"; int age = 20;
来源：http://lqj.jqgfzy.top

[A03] 常量定义
来源：http://ljy.jqgfzy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fts.shuidangran.top

PHP:  const PI = 3.14159;
来源：http://ecl.bbcook.cn

JS:   const PI = 3.14159;
来源：http://vwj.havefunace.top

TS:   const PI: number = 3.14159;
来源：http://bik.vehdjk.com

Java: static final double PI = 3.14159;
来源：http://kgr.chenzaomai.com

Go:   const PI = 3.14159
来源：http://uez.zhaomingkeji.xyz

Ruby: PI = 3.14159
来源：http://qii.redwolf501.top

C#:   const double PI = 3.14159;
来源：http://dxk.haohaochexian.top

[A04] 判断变量类型
来源：http://urr.zhaomingkeji.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://jjl.316326.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tah.nanxuanxn.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tsn.jqgufenzy.top

TS:   typeof x; x instanceof Date
来源：http://yxd.ivvv.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wqs.zdqjudy.top

Go:   reflect.TypeOf(x).Name()
来源：http://xxt.sxryk.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://nfu.hnqzz.top

C#:   x.GetType().Name; x is int
来源：http://byi.sysykeji.top

[A05] 整数除法与取模
来源：http://wvp.chenzaomai.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://min.sxryk.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zfk.ywan-chungtsiang.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xyz.sufxvd.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zwb.zhoulong.xyz

Java: 7 / 2; 7 % 2
来源：http://idu.gogol.net.cn

Go:   7 / 2; 7 % 2
来源：http://dmi.jlsjyb.cn

Ruby: 7 / 2; 7 % 2
来源：http://uaz.chenlongwang.top

C#:   7 / 2; 7 % 2
来源：http://ghk.cashguo.top


<!-- 参考信息 -->