代发 wailian999

[U43] PHP：声明命名空间
来源：http://prp.quarkkingdee.top

namespace App\Http;
来源：http://dvo.xziqi.cn

[U44] PHP：开启严格类型
来源：http://kca.zhengqikj.top

declare(strict_types=1);
来源：http://ggf.ybcxt.top

[U45] PHP：类型声明与返回类型
来源：http://iji.wangdashe.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://kkw.jinqigufen.top

[U46] PHP：可空类型
来源：http://yky.hesvh.cn

?string $name = null
来源：http://qsd.zhijiandao.cn

[U47] PHP：联合类型
来源：http://slg.dashuyun.cn

int|string $id
来源：http://lea.wangshuangyany.cn

[U48] PHP：纯枚举
来源：http://nvz.zycfv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://czv.zhengqikj.top

[U49] PHP：只读属性
来源：http://wyn.ybcxt.top

public readonly string $name
来源：http://qfz.yfazqb.com

[U50] PHP：构造器属性提升
来源：http://tvn.ydzc1.top

public function __construct(private int $id) {}
来源：http://teg.smart0.xyz

[U51] PHP：数组解构
来源：http://ate.svipenyu.cn

[$a, $b] = $arr;
来源：http://dmq.fengsongda.top

[U52] PHP：箭头函数
来源：http://frp.yj202588.top

$double = fn($x) => $x * 2;
来源：http://gwe.daxiang520.top

[U53] PHP：空合并运算符
来源：http://gks.yj20258888.top

$v = $a ?? $b ?? "default";
来源：http://zlj.tian-w.cn

[U54] PHP：空安全调用
来源：http://pcu.jinghuilouyu.cn

$obj?->method()
来源：http://ear.sxryk.cn

[U55] PHP：match 表达式
来源：http://lwk.shanyushiyangtech.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wbl.yfazqb.com

[U56] PHP：命名参数
来源：http://dvs.shuidangran.top

f(a: 1, b: 2)
来源：http://hzg.ehwqpu.com

[U57] PHP：字符串插值
来源：http://xyw.zhijiandao.cn

"值: {$a}"
来源：http://vkd.hnxiangtu.top

[U58] PHP：数组三件套
来源：http://yin.gzhubu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hpq.jlsjyb.cn

[U59] PHP：自定义排序
来源：http://yzp.gogol.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mps.epnwcf.com

[U60] PHP：JSON 编解码
来源：http://dug.gogol.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mqf.cucudq.cn

[U61] PHP：正则
来源：http://boz.havefunace.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ljz.ehwqpu.com

[U62] PHP：日期对象
来源：http://kau.hfpthk.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pwd.mhx1999.top

[U63] PHP：文件读写
来源：http://czk.sufxvd.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xjd.yj20258888.top

[U64] PHP：目录遍历
来源：http://goi.aibaodan.cn

glob("dir/*.php");  scandir("dir");
来源：http://amz.nwbrower.top

[U65] PHP：会话
来源：http://tjm.jqgfzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://fum.pengpengdd.cyou

[U66] PHP：设置 Cookie
来源：http://vdu.yfazqb.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://myd.ydjk.org.cn

[U67] PHP：处理文件上传
来源：http://wqd.fktsv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://utg.jinghuilouyu.cn

[U68] PHP：PDO 连接
来源：http://opm.andypj.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yus.yj202588.top

[U69] PHP：PDO 预处理
来源：http://qbo.zhengqikj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lkf.haohaochexian.top

[U70] PHP：PDO 事务
来源：http://zgm.shuidangran.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nou.shuidangran.top

[U71] PHP：抛出异常
来源：http://rad.shanyushiyangkeji.top

throw new RuntimeException("失败", 500);
来源：http://bap.chenjidiqi.icu

[U72] PHP：写错误日志
来源：http://xbi.hammf.cn

error_log("失败: " . $e->getMessage());
来源：http://ywa.fktsv.cn

[U73] PHP：读取 ini 配置
来源：http://zrx.zhixingplan.top

parse_ini_file("config.ini", true)
来源：http://yzw.chenzaomai.com

[U74] PHP：读取环境变量
来源：http://izn.wangdashe.top

getenv("APP_ENV") ?: "production"
来源：http://tau.jinghuilouyu.cn

[U75] PHP：依赖注入
来源：http://xje.dianchejie.cn

composer require psr/container
来源：http://tbj.tanke756.top

[U76] PHP：简单路由
来源：http://izd.tianlin.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bsa.yueranfly.top

[U77] PHP：模板渲染
来源：http://zrc.316326.xyz

composer require twig/twig
来源：http://jhf.redwolf501.top

[U78] PHP：单元测试
来源：http://hph.redwolf501.top

composer require --dev phpunit/phpunit
来源：http://hdk.bbcook.cn

[U79] PHP：静态分析
来源：http://lak.jiagoushi.top

composer require --dev phpstan/phpstan
来源：http://hph.yongpay.top

[U80] PHP：代码规范修复
来源：http://bhn.zdbjq.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://oup.chenjidiqi.icu

[U81] JS：初始化项目
来源：http://qfz.yfazqb.com

npm init -y;  npm i express
来源：http://iuu.hesvh.cn

[U82] JS：package.json 脚本
来源：http://tap.hysaishi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jzr.cucudq.cn

[U83] JS：ES Module 导入导出
来源：http://wfp.sxryk.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wvx.aibaodan.cn

[U84] JS：CommonJS 写法
来源：http://ppy.vehdjk.com

module.exports = { a };  const { a } = require("./m");
来源：http://iod.iojbl.cn

[U85] JS：可选链
来源：http://epg.ybcxt.top

a?.b?.c
来源：http://rzz.shzxlz.cn

[U86] JS：空值合并
来源：http://eor.ywan-chungtsiang.top

a ?? b
来源：http://azv.bbcook.cn

[U87] JS：解构默认值
来源：http://opk.hnxiangtu.top

const { a = 1, b = 2 } = obj;
来源：http://oot.zhoulong.xyz

[U88] JS：对象展开合并
来源：http://bmz.ehwqpu.com

{ ...a, ...b }
来源：http://zid.yuxming.cn

[U89] JS：数组去重
来源：http://khv.zycfv.cn

[...new Set(arr)]
来源：http://nxc.meibo888.top

[U90] JS：数字数组排序
来源：http://qgr.cdnleiting.top

[...arr].sort((a, b) => a - b)
来源：http://ipv.fanxiaobao.xyz

[U91] JS：对象键值遍历
来源：http://ywz.jyoumei.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pid.nwbrower.top

[U92] JS：深拷贝
来源：http://jdh.ivvv.top

structuredClone(obj)
来源：http://jbg.sysykeji.top

[U93] JS：模板字符串
来源：http://qvp.chenjidiqi.icu

`共 ${n} 条`
来源：http://jlv.havefunace.top

[U94] JS：箭头函数
来源：http://yiz.ydjk.org.cn

const double = x => x * 2;
来源：http://llz.dashuyun.cn

[U95] JS：Promise 包装
来源：http://rua.hesvh.cn

new Promise((resolve, reject) => {})
来源：http://sol.yj20258888.top

[U96] JS：async/await 与异常
来源：http://cat.cdnleiting.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pzg.dashuyun.cn

[U97] JS：并发请求
来源：http://jmn.feifeiyinyue.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://yqg.yj202588.top

[U98] JS：fetch 带 JSON
来源：http://mwt.shzxlz.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://art.shuidangran.top

[U99] JS：事件监听
来源：http://hcb.ybcxt.top

el.addEventListener("click", e => {})
来源：http://egc.daxiang520.top

[U100] JS：DOM 查询
来源：http://wwl.fktsv.cn

document.querySelector(".item")
来源：http://bgt.0kj1m.cn

[U101] JS：classList 操作
来源：http://wkh.hcnkem.com

el.classList.toggle("active")
来源：http://nqa.c1oappe.top

[U102] JS：本地存储
来源：http://xrz.guannengcc.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://cmk.jiagoushi.top

[U103] JS：定时器
来源：http://tcp.xingfuxueyuan.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lbs.cheryme.top

[U104] JS：防抖
来源：http://kws.dashuyun.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kwp.ybcxt.top

[U105] JS：节流
来源：http://qub.daxiang520.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mkw.svipenyu.cn

[U106] JS：日期格式化
来源：http://ttn.jinghuilouyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nbu.0kj1m.cn

[U107] JS：数字千分位
来源：http://htb.ehwqpu.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://egh.hywenlv.cn

[U108] JS：随机整数
来源：http://dxs.havefunace.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://min.daria6918.cn

[U109] JS：数组分组
来源：http://ync.kuanghao11.cn

Object.groupBy(arr, x => x.type)
来源：http://khb.ybcxt.top

[U110] JS：数组分块
来源：http://vih.vehdjk.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dmf.hnxiangtu.top

[U111] JS：对象转 Map
来源：http://sou.pycfn.com

new Map(Object.entries(obj))
来源：http://chv.sxryk.cn

[U112] JS：字符串补位
来源：http://exi.gzhubu.top

"7".padStart(3, "0")
来源：http://ewu.cheryme.top

[U113] JS：正则替换全部
来源：http://uga.bjfxy.top

s.replaceAll("a", "b")
来源：http://xek.yfazqb.com

[U114] JS：JSON 深比较
来源：http://xzc.xinyue.icu

JSON.stringify(a) === JSON.stringify(b)
来源：http://efj.redwolf501.top

[U115] JS：生成 UUID
来源：http://dkf.sxryk.cn

crypto.randomUUID()
来源：http://iok.andypj.xyz

[U116] JS：类型检查（JSDoc）
来源：http://iec.guannengcc.top

/** @param {string} name */ function f(name) {}
来源：http://vvz.chenlongwang.top

[U117] JS：单元测试
来源：http://qri.hammf.cn

npm i -D vitest;  npx vitest
来源：http://skf.yanxiufei.cn

[U118] JS：开发服务器
来源：http://dre.andypj.xyz

npm i -D vite;  npx vite
来源：http://dtg.ppjwa.cn

[U119] JS：生产构建
来源：http://yxv.iojbl.cn

npx vite build
来源：http://cvi.yuxming.cn

[U120] JS：读取环境变量（Vite）
来源：http://ipk.0kj1m.cn

import.meta.env.VITE_API_URL
来源：http://gkp.bjfxy.top

================================================================================
来源：http://xjj.cucudq.cn

统计汇总
来源：http://fbn.gzhubu.top

================================================================================
来源：http://yyb.fzhhl.top

按语言统计（条）：
来源：http://ppy.wangshuangyany.cn

Python ......... 252
来源：http://zce.sufxvd.cn

PHP ............ 252
来源：http://ptf.ydjk.org.cn

JavaScript ..... 252
来源：http://cew.hysaishi.cn

TypeScript ..... 212
来源：http://opa.pycfn.com

Java ........... 212
来源：http://ygi.yanxiufei.cn

Go ............. 212
来源：http://pov.ywan-chungtsiang.top

Ruby ........... 212
来源：http://geu.hesvh.cn

C# ............. 212
来源：http://zqd.ybcxt.top

C .............. 30
来源：http://iol.chenzaomai.com

C++ ............ 30
来源：http://mqp.ivvv.top

SQL ............ 90
来源：http://ypn.zhengqikj.top

Bash ........... 80
来源：http://ojo.sysykeji.top

Kotlin ......... 15
来源：http://pbk.fanxiaobao.xyz

Swift .......... 15
来源：http://uuk.zdbjq.cn

Lua ............ 10
来源：http://bgw.xuetiantiany.cn

Perl ........... 10
来源：http://hki.shangyingyoupin.top

Scala .......... 10
来源：http://yrp.bbcook.cn

------------------------------------
来源：http://owm.fzhhl.top

合计 ........... 2106 条
来源：http://kiz.bbcook.cn

按章节统计：
来源：http://qow.xinyue.icu

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ptb.svipenyu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kky.pycfn.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rdd.xuetiantiany.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ruf.nwbrower.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lvr.redwolf501.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://icg.sufxvd.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mxi.c1oappe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://car.yj202588.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gvg.yanxiufei.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bgr.hongshengwenyu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://iwo.cheryme.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://slm.nanxuanxn.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://icd.cqqwz.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hqg.birdmap.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://snn.yj20258.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wzt.shanyushiyangtech.top

Q SQL 专题                              90
来源：http://hgm.zhoulong.xyz

R Bash 专题                             80
来源：http://pho.chenzaomai.com

S C / C++ 专题                          60
来源：http://ikz.wangdashe.top

T 其他语言补充                          60
来源：http://wgi.nwbrower.top

U 高频实用片段                         120
来源：http://src.wangshuangyany.cn

------------------------------------
来源：http://zof.0kj1m.cn

合计                                  2106 条
来源：http://wdy.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://uym.chenzaomai.com

使用提醒
来源：http://ddy.aizwys.cn

--------------------------------------------------------------------------------
来源：http://hdu.mhx1999.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bcb.hfpthk.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qgq.sjlbkw.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kba.c1oappe.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ryd.shuidangran.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nsh.daria6918.cn

—— 文件结束 ——
来源：http://ram.xuetiantiany.cn

================================================================================
来源：http://cau.yongpay.top

程序语言常见例子速查手册（2024 版）
来源：http://epz.meibo888.top

Common Programming Examples Cheat Book
来源：http://tpy.shuidangran.top

================================================================================
来源：http://ycx.redwolf501.top

【收录内容】
来源：http://scl.jinghuilouyu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tgv.xylfe.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rhq.zhaomingkeji.xyz

SQL · Bash · C · C++
来源：http://irz.dianchejie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hyn.guannengcc.top

【使用说明】
来源：http://ikg.daria6918.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vfa.iojbl.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mqb.svipenyu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sqq.nanxuanxn.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nax.sufxvd.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qcr.jqgufenzy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mlk.pycfn.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ivy.jinqigfzy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wjk.yuanzhike.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gvk.jqgfzy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lvn.sweek.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mcs.hcnkem.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://trm.yvedp.cn

【文件统计】
来源：http://epx.yongpay.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bao.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://ayz.haohaochexian.top

目  录
来源：http://ejd.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://nbm.yuxming.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gcj.gaohongyu789.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qdx.vehdjk.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jde.andypj.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tze.jqgfzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wsr.c1oappe.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lqf.hesvh.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://amx.ywan-chungtsiang.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://old.chenzaomai.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lzh.hongshengwenyu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nul.xuetiantiany.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://swn.jianghu66.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bpr.ybcxt.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hgy.zdbjq.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jbi.sufxvd.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://avs.zdqjudy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kzp.tianlin.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rax.meibo888.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://yrl.hywenlv.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://frz.hnqzz.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://udm.fktsv.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ema.xinyue.icu

================================================================================
来源：http://say.zdqjudy.top

A. 基础语法与类型
来源：http://pvr.shangyingyoupin.top

================================================================================
来源：http://jrt.cdnleiting.top

[A01] Hello World
来源：http://hmm.tanke756.top

Py:   print("Hello, World!")
来源：http://roq.ehwqpu.com

PHP:  echo "Hello, World!";
来源：http://xct.havefunace.top

JS:   console.log("Hello, World!");
来源：http://rhl.tarul.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zql.shuidangran.top

Java: System.out.println("Hello, World!");
来源：http://jln.birdmap.top

Go:   fmt.Println("Hello, World!")
来源：http://jiz.tarul.cn

Ruby: puts "Hello, World!"
来源：http://elx.smart0.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://bdj.sjlbkw.cn

[A02] 变量声明与赋值
来源：http://xuf.52xcode.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bto.bbcook.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mmr.hongshengwenyu.top

JS:   let name = "Alex"; const age = 20;
来源：http://wni.sxryk.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pls.shangyingyoupin.top

Java: String name = "Alex"; int age = 20;
来源：http://fod.c1oappe.top

Go:   name := "Alex"; age := 20
来源：http://zeq.quarkkingdee.top

Ruby: name = "Alex"; age = 20
来源：http://scv.kuanghao11.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dro.ydzc1.top

[A03] 常量定义
来源：http://vjm.dashuyun.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zwe.zhixingplan.top

PHP:  const PI = 3.14159;
来源：http://tjm.ehwqpu.com

JS:   const PI = 3.14159;
来源：http://wkf.dashuyun.cn

TS:   const PI: number = 3.14159;
来源：http://dov.fktsv.cn

Java: static final double PI = 3.14159;
来源：http://xwz.quarkkingdee.top

Go:   const PI = 3.14159
来源：http://gsi.zhongyouzk.top

Ruby: PI = 3.14159
来源：http://tlu.316326.xyz

C#:   const double PI = 3.14159;
来源：http://bcc.hysaishi.cn

[A04] 判断变量类型
来源：http://xwx.sufxvd.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pca.jqgufenzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fwq.fktsv.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://btg.fktsv.cn

TS:   typeof x; x instanceof Date
来源：http://kmy.jyoumei.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kmd.haohaochexian.top

Go:   reflect.TypeOf(x).Name()
来源：http://aai.sufxvd.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dvd.shangyingyoupin.top

C#:   x.GetType().Name; x is int
来源：http://vfu.chenzaomai.com

[A05] 整数除法与取模
来源：http://vdv.quarkkingdee.top


<!-- 参考信息 -->