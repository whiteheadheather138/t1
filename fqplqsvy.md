代发 wailian999

[U43] PHP：声明命名空间
来源：http://mcd.xziqi.cn

namespace App\Http;
来源：http://vdo.yj20258888.top

[U44] PHP：开启严格类型
来源：http://pnv.tarul.cn

declare(strict_types=1);
来源：http://sfs.shzxlz.cn

[U45] PHP：类型声明与返回类型
来源：http://dqk.hongshengwenyu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://jkz.fengsongda.top

[U46] PHP：可空类型
来源：http://fjj.tianlin.xyz

?string $name = null
来源：http://bga.ppjwa.cn

[U47] PHP：联合类型
来源：http://izi.pycfn.com

int|string $id
来源：http://yax.chenlongwang.top

[U48] PHP：纯枚举
来源：http://ams.9152youxi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hdo.shanyushiyangkeji.top

[U49] PHP：只读属性
来源：http://olg.zhongyouzk.top

public readonly string $name
来源：http://wvj.sjlbkw.cn

[U50] PHP：构造器属性提升
来源：http://qdp.epnwcf.com

public function __construct(private int $id) {}
来源：http://vnp.daria6918.cn

[U51] PHP：数组解构
来源：http://txb.316326.xyz

[$a, $b] = $arr;
来源：http://xqp.cashguo.top

[U52] PHP：箭头函数
来源：http://rcn.ppjwa.cn

$double = fn($x) => $x * 2;
来源：http://lpv.yonumen.top

[U53] PHP：空合并运算符
来源：http://gzg.tianlin.xyz

$v = $a ?? $b ?? "default";
来源：http://lgz.fanxiaobao.xyz

[U54] PHP：空安全调用
来源：http://nja.shanyushiyangtech.top

$obj?->method()
来源：http://pte.jqgufenzy.top

[U55] PHP：match 表达式
来源：http://sfn.fengsongda.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://umv.zhiwuduotai.top

[U56] PHP：命名参数
来源：http://zzk.yangfankeji.com

f(a: 1, b: 2)
来源：http://cbz.aibaodan.cn

[U57] PHP：字符串插值
来源：http://peg.ydzc1.top

"值: {$a}"
来源：http://uwo.zhijiandao.cn

[U58] PHP：数组三件套
来源：http://als.yvedp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tyd.sjlbkw.cn

[U59] PHP：自定义排序
来源：http://eyy.yueranfly.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aia.ppjwa.cn

[U60] PHP：JSON 编解码
来源：http://yxs.fengsongda.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dtu.zhongyouzk.top

[U61] PHP：正则
来源：http://wkk.hammf.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dxb.andypj.xyz

[U62] PHP：日期对象
来源：http://ksf.zhiwuduotai.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yvg.kuanghao11.cn

[U63] PHP：文件读写
来源：http://vzq.dashuyun.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xuc.jinqigufen.top

[U64] PHP：目录遍历
来源：http://cyx.meibo888.top

glob("dir/*.php");  scandir("dir");
来源：http://pls.ywan-chungtsiang.top

[U65] PHP：会话
来源：http://emj.kuanghao11.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hps.jinqigufen.top

[U66] PHP：设置 Cookie
来源：http://yxu.fengsongda.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yes.xuanzx.com

[U67] PHP：处理文件上传
来源：http://ujv.vehdjk.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vre.jinyuanbaomall.cn

[U68] PHP：PDO 连接
来源：http://xzv.yj202588.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pgo.ppjwa.cn

[U69] PHP：PDO 预处理
来源：http://ydf.0kj1m.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://icf.fktsv.cn

[U70] PHP：PDO 事务
来源：http://oyw.sufxvd.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xji.vqdsnc.cn

[U71] PHP：抛出异常
来源：http://blz.cdnleiting.top

throw new RuntimeException("失败", 500);
来源：http://xfd.shuidangran.top

[U72] PHP：写错误日志
来源：http://tge.gogol.net.cn

error_log("失败: " . $e->getMessage());
来源：http://hbf.fanxiaobao.xyz

[U73] PHP：读取 ini 配置
来源：http://ake.daria6918.cn

parse_ini_file("config.ini", true)
来源：http://dsg.quarkkingdee.top

[U74] PHP：读取环境变量
来源：http://qal.shzxlz.cn

getenv("APP_ENV") ?: "production"
来源：http://gvn.aibaodan.cn

[U75] PHP：依赖注入
来源：http://hmt.xylfe.cn

composer require psr/container
来源：http://fnz.zhengqikj.top

[U76] PHP：简单路由
来源：http://gsb.redwolf501.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sga.yangfankeji.com

[U77] PHP：模板渲染
来源：http://jlm.redwolf501.top

composer require twig/twig
来源：http://ctb.yj20258888.top

[U78] PHP：单元测试
来源：http://gar.yuxming.cn

composer require --dev phpunit/phpunit
来源：http://lai.ivvv.top

[U79] PHP：静态分析
来源：http://ahz.hnqzz.top

composer require --dev phpstan/phpstan
来源：http://tse.ybcxt.top

[U80] PHP：代码规范修复
来源：http://wxh.zycfv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tny.hywenlv.cn

[U81] JS：初始化项目
来源：http://dnh.zhaomingkeji.xyz

npm init -y;  npm i express
来源：http://mrm.sxryk.cn

[U82] JS：package.json 脚本
来源：http://ulk.yuanzhike.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xmm.jqgufenzy.top

[U83] JS：ES Module 导入导出
来源：http://yhk.tianlin.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://kmw.guowangkeji.top

[U84] JS：CommonJS 写法
来源：http://taf.hammf.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cnl.chenlongwang.top

[U85] JS：可选链
来源：http://gml.wangshuangyany.cn

a?.b?.c
来源：http://drz.yvedp.cn

[U86] JS：空值合并
来源：http://zts.guowangkeji.top

a ?? b
来源：http://pqh.ivvv.top

[U87] JS：解构默认值
来源：http://xlk.wangshuangyany.cn

const { a = 1, b = 2 } = obj;
来源：http://ama.daria6918.cn

[U88] JS：对象展开合并
来源：http://esm.zycfv.cn

{ ...a, ...b }
来源：http://hmz.fengsongda.top

[U89] JS：数组去重
来源：http://jjf.jinqigfzy.top

[...new Set(arr)]
来源：http://fmh.sxryk.cn

[U90] JS：数字数组排序
来源：http://egt.zhengqikj.top

[...arr].sort((a, b) => a - b)
来源：http://ezf.quarkkingdee.top

[U91] JS：对象键值遍历
来源：http://glp.ehwqpu.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kmt.0kj1m.cn

[U92] JS：深拷贝
来源：http://hza.zhijiandao.cn

structuredClone(obj)
来源：http://fbj.daxiang520.top

[U93] JS：模板字符串
来源：http://nqk.sysykeji.top

`共 ${n} 条`
来源：http://dtb.ybcxt.top

[U94] JS：箭头函数
来源：http://wyj.xuanzx.com

const double = x => x * 2;
来源：http://dyz.uphjek.com

[U95] JS：Promise 包装
来源：http://ygv.jinyuanbaomall.cn

new Promise((resolve, reject) => {})
来源：http://zkh.shanyushiyangkeji.top

[U96] JS：async/await 与异常
来源：http://tzq.hnqzz.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bhe.xingfuxueyuan.xyz

[U97] JS：并发请求
来源：http://gae.jqgufenzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ahw.jianghu66.top

[U98] JS：fetch 带 JSON
来源：http://jjv.yj202588.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://udi.yj202588.top

[U99] JS：事件监听
来源：http://uaj.shuidangran.top

el.addEventListener("click", e => {})
来源：http://wrm.cqqwz.cn

[U100] JS：DOM 查询
来源：http://wum.vqdsnc.cn

document.querySelector(".item")
来源：http://mww.shanyushiyangkeji.top

[U101] JS：classList 操作
来源：http://taj.hfpthk.cn

el.classList.toggle("active")
来源：http://kql.yj202588.top

[U102] JS：本地存储
来源：http://jiy.jianghu66.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://cqt.wangdashe.top

[U103] JS：定时器
来源：http://qht.haohaochexian.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qqw.jiagoushi.top

[U104] JS：防抖
来源：http://wfx.xingfuxueyuan.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zbv.tian-w.cn

[U105] JS：节流
来源：http://huk.yj20258.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lqy.jiagoushi.top

[U106] JS：日期格式化
来源：http://vrl.hywenlv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rmm.zhijiandao.cn

[U107] JS：数字千分位
来源：http://eed.yueranfly.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uhq.hysaishi.cn

[U108] JS：随机整数
来源：http://zin.cqqwz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bkf.xinyue.icu

[U109] JS：数组分组
来源：http://uwo.yueranfly.top

Object.groupBy(arr, x => x.type)
来源：http://qxt.gotoacloud.top

[U110] JS：数组分块
来源：http://ggg.sufxvd.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sbk.nwbrower.top

[U111] JS：对象转 Map
来源：http://fib.ywan-chungtsiang.top

new Map(Object.entries(obj))
来源：http://zpx.ywan-chungtsiang.top

[U112] JS：字符串补位
来源：http://eyg.xuanzx.com

"7".padStart(3, "0")
来源：http://ord.dianchejie.cn

[U113] JS：正则替换全部
来源：http://ncr.daxiang520.top

s.replaceAll("a", "b")
来源：http://xps.vqdsnc.cn

[U114] JS：JSON 深比较
来源：http://maa.jqgfzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rcj.hnxiangtu.top

[U115] JS：生成 UUID
来源：http://ydn.yj202588.top

crypto.randomUUID()
来源：http://fif.jqgfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://biv.daria6918.cn

/** @param {string} name */ function f(name) {}
来源：http://iof.hcnkem.com

[U117] JS：单元测试
来源：http://rlr.jinqigfzy.top

npm i -D vitest;  npx vitest
来源：http://ock.chenlongwang.top

[U118] JS：开发服务器
来源：http://zua.nanxinkj.top

npm i -D vite;  npx vite
来源：http://qcb.shanyushiyangkeji.top

[U119] JS：生产构建
来源：http://jpa.yuxming.cn

npx vite build
来源：http://niy.ybcxt.top

[U120] JS：读取环境变量（Vite）
来源：http://hkm.ywan-chungtsiang.top

import.meta.env.VITE_API_URL
来源：http://lsy.guowangkeji.top

================================================================================
来源：http://arr.aibaodan.cn

统计汇总
来源：http://yud.chenlongwang.top

================================================================================
来源：http://gww.hnxiangtu.top

按语言统计（条）：
来源：http://ljt.zhijiandao.cn

Python ......... 252
来源：http://xvb.snrcjt.cn

PHP ............ 252
来源：http://whg.ywan-chungtsiang.top

JavaScript ..... 252
来源：http://drl.cashguo.top

TypeScript ..... 212
来源：http://ckj.sxryk.cn

Java ........... 212
来源：http://jqx.aibaodan.cn

Go ............. 212
来源：http://vig.dashuyun.cn

Ruby ........... 212
来源：http://ckm.hnqzz.top

C# ............. 212
来源：http://hsq.shanyushiyangtech.top

C .............. 30
来源：http://tlx.yvedp.cn

C++ ............ 30
来源：http://zyr.sweek.top

SQL ............ 90
来源：http://bty.ivvv.top

Bash ........... 80
来源：http://sjk.sxryk.cn

Kotlin ......... 15
来源：http://qpi.feifeiyinyue.top

Swift .......... 15
来源：http://fuw.jqgufenzy.top

Lua ............ 10
来源：http://sao.aibaodan.cn

Perl ........... 10
来源：http://mdn.fanxiaobao.xyz

Scala .......... 10
来源：http://dyl.xuanzx.com

------------------------------------
来源：http://wfs.sweek.top

合计 ........... 2106 条
来源：http://cxr.pycfn.com

按章节统计：
来源：http://juj.fktsv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sbr.dashuyun.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://eed.xylfe.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ace.yvedp.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rfz.yj20258888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gyn.nanxinkj.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fse.tarul.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uks.fktsv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qho.ywan-chungtsiang.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ogq.gotoacloud.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cat.wangshuangyany.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hzs.316326.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wtu.hnxiangtu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fsi.cheryme.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nkz.fktsv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mmc.wangdashe.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hfx.nanxuanxn.top

Q SQL 专题                              90
来源：http://qeo.yangfankeji.com

R Bash 专题                             80
来源：http://ysl.zhaomingkeji.xyz

S C / C++ 专题                          60
来源：http://ibw.xylfe.cn

T 其他语言补充                          60
来源：http://rwa.yuanzhike.top

U 高频实用片段                         120
来源：http://vgq.quarkkingdee.top

------------------------------------
来源：http://nfk.zhaomingkeji.xyz

合计                                  2106 条
来源：http://cnp.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://cmg.tarul.cn

使用提醒
来源：http://mym.yonumen.top

--------------------------------------------------------------------------------
来源：http://aos.xuanzx.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://slj.aizwys.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://iku.hcnkem.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://etk.sysykeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://yab.c1oappe.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bci.fehbvm.com

—— 文件结束 ——
来源：http://scv.xinyue.icu

================================================================================
来源：http://dbj.zhixingplan.top

程序语言常见例子速查手册（2024 版）
来源：http://jaf.jinqigfzy.top

Common Programming Examples Cheat Book
来源：http://iqa.c1oappe.top

================================================================================
来源：http://ddg.xinyue.icu

【收录内容】
来源：http://ved.daria6918.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rli.shzxlz.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nnb.chenjidiqi.icu

SQL · Bash · C · C++
来源：http://taa.shangyingyoupin.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ptq.redwolf501.top

【使用说明】
来源：http://luh.sweek.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dff.sysykeji.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wco.fengsongda.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xdx.gzhubu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://euq.jinyuanbaomall.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ssz.chenjidiqi.icu

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uih.kuanghao11.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zro.fktsv.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sno.dashuyun.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://myr.cheryme.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kcy.jinyuanbaomall.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wmv.quarkkingdee.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mam.zhengqikj.top

【文件统计】
来源：http://rum.jqgufenzy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qob.yuxming.cn

--------------------------------------------------------------------------------
来源：http://zxz.9152youxi.cn

目  录
来源：http://uic.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://yyi.shanyushiyangtech.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://abg.cashguo.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gsh.sxryk.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mlj.dashuyun.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://prx.sysykeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wej.shzxlz.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xld.shangyingyoupin.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lhp.sjlbkw.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://aqg.gzhubu.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ibe.gogol.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://udb.ivvv.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bbu.gaohongyu789.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wgl.chenlongwang.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lfc.zycfv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nep.zhaomingkeji.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hvb.zdbjq.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jpz.ydzc1.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ptn.dashuyun.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://etc.havefunace.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xup.gotoacloud.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dqp.yanxiufei.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tni.zdbjq.cn

================================================================================
来源：http://ege.yuanzhike.top

A. 基础语法与类型
来源：http://edj.meibo888.top

================================================================================
来源：http://dbo.yanxiufei.cn

[A01] Hello World
来源：http://cgj.chenzaomai.com

Py:   print("Hello, World!")
来源：http://fer.zhengqikj.top

PHP:  echo "Hello, World!";
来源：http://wmu.hammf.cn

JS:   console.log("Hello, World!");
来源：http://kit.daxiang520.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ipw.smart0.xyz

Java: System.out.println("Hello, World!");
来源：http://cfa.jiagoushi.top

Go:   fmt.Println("Hello, World!")
来源：http://zir.hesvh.cn

Ruby: puts "Hello, World!"
来源：http://jjx.wangdashe.top

C#:   Console.WriteLine("Hello, World!");
来源：http://hpf.haohaochexian.top

[A02] 变量声明与赋值
来源：http://fst.gaohongyu789.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yox.hysaishi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wpn.sysykeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://meo.hammf.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://omq.yj20258888.top

Java: String name = "Alex"; int age = 20;
来源：http://cmw.zhijiandao.cn

Go:   name := "Alex"; age := 20
来源：http://jio.vqdsnc.cn

Ruby: name = "Alex"; age = 20
来源：http://zge.fktsv.cn

C#:   string name = "Alex"; int age = 20;
来源：http://far.shuidangran.top

[A03] 常量定义
来源：http://rpv.jianghu66.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ccf.chenjidiqi.icu

PHP:  const PI = 3.14159;
来源：http://fsp.jinyuanbaomall.cn

JS:   const PI = 3.14159;
来源：http://mev.zhixingplan.top

TS:   const PI: number = 3.14159;
来源：http://cde.hnqzz.top

Java: static final double PI = 3.14159;
来源：http://hyh.nanxuanxn.top

Go:   const PI = 3.14159
来源：http://uhf.wangshuangyany.cn

Ruby: PI = 3.14159
来源：http://mvt.xuanzx.com

C#:   const double PI = 3.14159;
来源：http://tnl.meibo888.top

[A04] 判断变量类型
来源：http://wsq.ehwqpu.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://atd.zhiwuduotai.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pio.316326.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wyn.yuxming.cn

TS:   typeof x; x instanceof Date
来源：http://qxf.bjfxy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bht.fktsv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://gcj.andypj.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://nhu.ppjwa.cn

C#:   x.GetType().Name; x is int
来源：http://hvs.yfazqb.com

[A05] 整数除法与取模
来源：http://dsg.mhx1999.top


<!-- 参考信息 -->