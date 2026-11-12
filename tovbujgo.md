代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://iev.iojbl.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jtt.shanyushiyangkeji.top

[U42] PHP：PSR-4 自动加载
来源：http://dah.dashuyun.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gip.birdmap.top

[U43] PHP：声明命名空间
来源：http://mjz.snrcjt.cn

namespace App\Http;
来源：http://blm.dashuyun.cn

[U44] PHP：开启严格类型
来源：http://kov.iojbl.cn

declare(strict_types=1);
来源：http://xbt.jiagoushi.top

[U45] PHP：类型声明与返回类型
来源：http://wjn.chenzaomai.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://oju.jinqigfzy.top

[U46] PHP：可空类型
来源：http://rwc.gzhubu.top

?string $name = null
来源：http://xhm.316326.xyz

[U47] PHP：联合类型
来源：http://yqe.zdqjudy.top

int|string $id
来源：http://cax.shanyushiyangtech.top

[U48] PHP：纯枚举
来源：http://fdf.bbcook.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lae.andypj.xyz

[U49] PHP：只读属性
来源：http://tht.jinyuanbaomall.cn

public readonly string $name
来源：http://znm.andypj.xyz

[U50] PHP：构造器属性提升
来源：http://gkv.jiagoushi.top

public function __construct(private int $id) {}
来源：http://cac.jyoumei.cn

[U51] PHP：数组解构
来源：http://sxn.pycfn.com

[$a, $b] = $arr;
来源：http://sqn.jinyuanbaomall.cn

[U52] PHP：箭头函数
来源：http://oen.xylfe.cn

$double = fn($x) => $x * 2;
来源：http://jwu.zdbjq.cn

[U53] PHP：空合并运算符
来源：http://vdx.pycfn.com

$v = $a ?? $b ?? "default";
来源：http://wyy.bbcook.cn

[U54] PHP：空安全调用
来源：http://tbw.zhiwuduotai.top

$obj?->method()
来源：http://ork.vqdsnc.cn

[U55] PHP：match 表达式
来源：http://upg.shuidangran.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lkb.zhixingplan.top

[U56] PHP：命名参数
来源：http://uqq.ydjk.org.cn

f(a: 1, b: 2)
来源：http://qmx.yuanzhike.top

[U57] PHP：字符串插值
来源：http://inr.fzhhl.top

"值: {$a}"
来源：http://vqn.yj20258.top

[U58] PHP：数组三件套
来源：http://rix.ehwqpu.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://scm.9152youxi.cn

[U59] PHP：自定义排序
来源：http://cit.gogol.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ykh.jinqigufen.top

[U60] PHP：JSON 编解码
来源：http://huk.yanxiufei.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gcr.ppjwa.cn

[U61] PHP：正则
来源：http://ukk.gaohongyu789.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xop.ydzc1.top

[U62] PHP：日期对象
来源：http://bfe.iojbl.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gdp.jyoumei.cn

[U63] PHP：文件读写
来源：http://nqh.tianlin.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xga.sxryk.cn

[U64] PHP：目录遍历
来源：http://sem.hesvh.cn

glob("dir/*.php");  scandir("dir");
来源：http://vfa.yueranfly.top

[U65] PHP：会话
来源：http://kss.guowangkeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ptq.zhoulong.xyz

[U66] PHP：设置 Cookie
来源：http://cvw.316326.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dwt.nwbrower.top

[U67] PHP：处理文件上传
来源：http://qqv.smart0.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vxg.xinyue.icu

[U68] PHP：PDO 连接
来源：http://ssh.yj20258.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hdc.wangshuangyany.cn

[U69] PHP：PDO 预处理
来源：http://gtf.svipenyu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rdu.smart0.xyz

[U70] PHP：PDO 事务
来源：http://fqn.zhijiandao.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ojg.yueranfly.top

[U71] PHP：抛出异常
来源：http://iyj.jiagoushi.top

throw new RuntimeException("失败", 500);
来源：http://xji.dianchejie.cn

[U72] PHP：写错误日志
来源：http://ict.jinqigfzy.top

error_log("失败: " . $e->getMessage());
来源：http://qrh.zhiwuduotai.top

[U73] PHP：读取 ini 配置
来源：http://wxy.havefunace.top

parse_ini_file("config.ini", true)
来源：http://sns.hysaishi.cn

[U74] PHP：读取环境变量
来源：http://ryu.shzxlz.cn

getenv("APP_ENV") ?: "production"
来源：http://ztt.tanke756.top

[U75] PHP：依赖注入
来源：http://rfk.vqdsnc.cn

composer require psr/container
来源：http://khb.birdmap.top

[U76] PHP：简单路由
来源：http://cxi.zhijiandao.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://scn.ivvv.top

[U77] PHP：模板渲染
来源：http://gyc.yj20258888.top

composer require twig/twig
来源：http://plc.0kj1m.cn

[U78] PHP：单元测试
来源：http://wub.meibo888.top

composer require --dev phpunit/phpunit
来源：http://rof.nanxuanxn.top

[U79] PHP：静态分析
来源：http://cfa.tianlin.xyz

composer require --dev phpstan/phpstan
来源：http://ial.shangyingyoupin.top

[U80] PHP：代码规范修复
来源：http://otb.nanxuanxn.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://yoh.yongpay.top

[U81] JS：初始化项目
来源：http://ejo.jinqigufen.top

npm init -y;  npm i express
来源：http://rrn.xuetiantiany.cn

[U82] JS：package.json 脚本
来源：http://wbg.cashguo.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fmy.jinqigufen.top

[U83] JS：ES Module 导入导出
来源：http://esg.ppjwa.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vxw.aibaodan.cn

[U84] JS：CommonJS 写法
来源：http://cse.fanxiaobao.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://asm.jlsjyb.cn

[U85] JS：可选链
来源：http://csp.ehwqpu.com

a?.b?.c
来源：http://szs.tanke756.top

[U86] JS：空值合并
来源：http://akz.hcnkem.com

a ?? b
来源：http://ose.xingfuxueyuan.xyz

[U87] JS：解构默认值
来源：http://flf.jianghu66.top

const { a = 1, b = 2 } = obj;
来源：http://yag.hammf.cn

[U88] JS：对象展开合并
来源：http://tly.daria6918.cn

{ ...a, ...b }
来源：http://fvj.fehbvm.com

[U89] JS：数组去重
来源：http://mta.yj20258888.top

[...new Set(arr)]
来源：http://tsa.xuanzx.com

[U90] JS：数字数组排序
来源：http://aab.yueranfly.top

[...arr].sort((a, b) => a - b)
来源：http://txm.havefunace.top

[U91] JS：对象键值遍历
来源：http://pgf.dashuyun.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://noo.zhixingplan.top

[U92] JS：深拷贝
来源：http://dyu.jinghuilouyu.cn

structuredClone(obj)
来源：http://rmi.xuetiantiany.cn

[U93] JS：模板字符串
来源：http://nfd.shanyushiyangtech.top

`共 ${n} 条`
来源：http://din.xinyue.icu

[U94] JS：箭头函数
来源：http://xzh.yuanzhike.top

const double = x => x * 2;
来源：http://iuu.guannengcc.top

[U95] JS：Promise 包装
来源：http://qpa.sweek.top

new Promise((resolve, reject) => {})
来源：http://msn.yj202588.top

[U96] JS：async/await 与异常
来源：http://shw.hysaishi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ywe.jqgufenzy.top

[U97] JS：并发请求
来源：http://wdm.fktsv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wjm.chenjidiqi.icu

[U98] JS：fetch 带 JSON
来源：http://lxy.0kj1m.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wlv.pengpengdd.cyou

[U99] JS：事件监听
来源：http://kam.bjfxy.top

el.addEventListener("click", e => {})
来源：http://zib.ydzc1.top

[U100] JS：DOM 查询
来源：http://jfq.haohaochexian.top

document.querySelector(".item")
来源：http://joy.dianchejie.cn

[U101] JS：classList 操作
来源：http://fqz.0kj1m.cn

el.classList.toggle("active")
来源：http://gyg.yongpay.top

[U102] JS：本地存储
来源：http://nib.gogol.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lrf.sjlbkw.cn

[U103] JS：定时器
来源：http://mns.dashuyun.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mzd.tarul.cn

[U104] JS：防抖
来源：http://kxx.c1oappe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jib.tarul.cn

[U105] JS：节流
来源：http://gsz.9152youxi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mvb.jlsjyb.cn

[U106] JS：日期格式化
来源：http://dej.guowangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jsc.haohaochexian.top

[U107] JS：数字千分位
来源：http://pyf.hnqzz.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vqc.shzxlz.cn

[U108] JS：随机整数
来源：http://gzl.sxryk.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jcf.fktsv.cn

[U109] JS：数组分组
来源：http://byz.nanxinkj.top

Object.groupBy(arr, x => x.type)
来源：http://hgx.haohaochexian.top

[U110] JS：数组分块
来源：http://qpo.vqdsnc.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uoo.wangdashe.top

[U111] JS：对象转 Map
来源：http://mty.ctjpmb.com

new Map(Object.entries(obj))
来源：http://anu.meibo888.top

[U112] JS：字符串补位
来源：http://hvh.yfazqb.com

"7".padStart(3, "0")
来源：http://acp.aibaodan.cn

[U113] JS：正则替换全部
来源：http://qxu.tarul.cn

s.replaceAll("a", "b")
来源：http://jdk.zdqjudy.top

[U114] JS：JSON 深比较
来源：http://bgs.daxiang520.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://zcx.fanxiaobao.xyz

[U115] JS：生成 UUID
来源：http://sfc.cashguo.top

crypto.randomUUID()
来源：http://bhn.dianchejie.cn

[U116] JS：类型检查（JSDoc）
来源：http://dun.chenlongwang.top

/** @param {string} name */ function f(name) {}
来源：http://naq.hnqzz.top

[U117] JS：单元测试
来源：http://wmp.chenzaomai.com

npm i -D vitest;  npx vitest
来源：http://yrr.ywan-chungtsiang.top

[U118] JS：开发服务器
来源：http://dmf.mhx1999.top

npm i -D vite;  npx vite
来源：http://nlr.0kj1m.cn

[U119] JS：生产构建
来源：http://azs.cheryme.top

npx vite build
来源：http://jzr.tianlin.xyz

[U120] JS：读取环境变量（Vite）
来源：http://wyc.haohaochexian.top

import.meta.env.VITE_API_URL
来源：http://ram.uphjek.com

================================================================================
来源：http://xgn.zhaomingkeji.xyz

统计汇总
来源：http://llj.ydzc1.top

================================================================================
来源：http://xli.xylfe.cn

按语言统计（条）：
来源：http://wzq.9152youxi.cn

Python ......... 252
来源：http://otg.jlsjyb.cn

PHP ............ 252
来源：http://eqd.yongpay.top

JavaScript ..... 252
来源：http://nzz.hfpthk.cn

TypeScript ..... 212
来源：http://jvn.yueranfly.top

Java ........... 212
来源：http://jmd.yongpay.top

Go ............. 212
来源：http://ohv.xuanzx.com

Ruby ........... 212
来源：http://uqv.xingfuxueyuan.xyz

C# ............. 212
来源：http://bsw.yonumen.top

C .............. 30
来源：http://erd.dianchejie.cn

C++ ............ 30
来源：http://wrw.xingfuxueyuan.xyz

SQL ............ 90
来源：http://yho.chenlongwang.top

Bash ........... 80
来源：http://sme.hcnkem.com

Kotlin ......... 15
来源：http://jgn.zdbjq.cn

Swift .......... 15
来源：http://dnc.xziqi.cn

Lua ............ 10
来源：http://aeg.snrcjt.cn

Perl ........... 10
来源：http://uie.jinqigfzy.top

Scala .......... 10
来源：http://cvi.shangyingyoupin.top

------------------------------------
来源：http://zgy.xinyue.icu

合计 ........... 2106 条
来源：http://yeq.shanyushiyangkeji.top

按章节统计：
来源：http://xjy.zhijiandao.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gov.cucudq.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wae.jiagoushi.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mck.meibo888.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yok.52xcode.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hna.yuanzhike.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xrd.hesvh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://djt.redwolf501.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://iir.pycfn.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ppc.zdqjudy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wxg.hysaishi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cwu.guowangkeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tgl.fktsv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hbi.tian-w.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://adv.xuanzx.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fsr.jinqigufen.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://doq.sjlbkw.cn

Q SQL 专题                              90
来源：http://nlc.shzxlz.cn

R Bash 专题                             80
来源：http://flv.fengsongda.top

S C / C++ 专题                          60
来源：http://mbx.gotoacloud.top

T 其他语言补充                          60
来源：http://rvs.ehwqpu.com

U 高频实用片段                         120
来源：http://lyk.ywan-chungtsiang.top

------------------------------------
来源：http://ypu.zycfv.cn

合计                                  2106 条
来源：http://zup.cucudq.cn

--------------------------------------------------------------------------------
来源：http://apq.shuidangran.top

使用提醒
来源：http://zqr.hcnkem.com

--------------------------------------------------------------------------------
来源：http://kht.yj20258888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kfm.shzxlz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ekq.zhixingplan.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hmj.pengpengdd.cyou

在旧版本上使用前请先确认语法支持情况。
来源：http://brm.jinqigfzy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tog.tanke756.top

—— 文件结束 ——
来源：http://wyw.uphjek.com

================================================================================
来源：http://txf.yfazqb.com

程序语言常见例子速查手册（2024 版）
来源：http://mzd.yvedp.cn

Common Programming Examples Cheat Book
来源：http://hsl.xuanzx.com

================================================================================
来源：http://dww.jqgfzy.top

【收录内容】
来源：http://xhn.svipenyu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://oow.meibo888.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fwe.svipenyu.cn

SQL · Bash · C · C++
来源：http://ctm.yj20258.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://djb.yonumen.top

【使用说明】
来源：http://ywp.hammf.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://brl.hysaishi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lee.jqgufenzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ppo.wangdashe.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yis.cqqwz.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://iet.vehdjk.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cca.sxryk.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bfk.hnqzz.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://upj.guowangkeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yoh.nanxinkj.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nbi.bjfxy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nyx.yuxming.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uxf.yongpay.top

【文件统计】
来源：http://rtc.gotoacloud.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vtn.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://lwv.aibaodan.cn

目  录
来源：http://jqx.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://sxp.jlsjyb.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wod.dashuyun.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mid.chenjidiqi.icu

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fin.xziqi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uwk.hnxiangtu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://buq.xylfe.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vgr.jinqigufen.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rxz.ydzc1.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bjk.jinyuanbaomall.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://agq.redwolf501.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ujc.jlsjyb.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xrq.guannengcc.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fxc.yonumen.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://aph.wangdashe.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xgk.ctjpmb.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://igx.sweek.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nbf.tianlin.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dyc.chenlongwang.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://yui.xuetiantiany.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cpi.sjlbkw.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nmy.tianlin.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://psu.nwbrower.top

================================================================================
来源：http://ogi.ppjwa.cn

A. 基础语法与类型
来源：http://yia.nwbrower.top

================================================================================
来源：http://knr.316326.xyz

[A01] Hello World
来源：http://hyh.jianghu66.top

Py:   print("Hello, World!")
来源：http://jvr.vehdjk.com

PHP:  echo "Hello, World!";
来源：http://cru.uphjek.com

JS:   console.log("Hello, World!");
来源：http://fls.shangyingyoupin.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gpj.ppjwa.cn

Java: System.out.println("Hello, World!");
来源：http://kwz.fzhhl.top

Go:   fmt.Println("Hello, World!")
来源：http://ibq.ydjk.org.cn

Ruby: puts "Hello, World!"
来源：http://bkw.mhx1999.top

C#:   Console.WriteLine("Hello, World!");
来源：http://dzi.gogol.net.cn

[A02] 变量声明与赋值
来源：http://chm.iojbl.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bbe.ehwqpu.com

PHP:  $name = "Alex"; $age = 20;
来源：http://jku.ctjpmb.com

JS:   let name = "Alex"; const age = 20;
来源：http://qzy.gogol.net.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ozw.fanxiaobao.xyz

Java: String name = "Alex"; int age = 20;
来源：http://hai.nwbrower.top

Go:   name := "Alex"; age := 20
来源：http://xbg.aibaodan.cn

Ruby: name = "Alex"; age = 20
来源：http://qzd.ctjpmb.com

C#:   string name = "Alex"; int age = 20;
来源：http://cid.sweek.top

[A03] 常量定义
来源：http://ylw.gogol.net.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://apo.yangfankeji.com

PHP:  const PI = 3.14159;
来源：http://jgh.nanxuanxn.top

JS:   const PI = 3.14159;
来源：http://wkd.mhx1999.top

TS:   const PI: number = 3.14159;
来源：http://vxo.cashguo.top

Java: static final double PI = 3.14159;
来源：http://ups.ctjpmb.com

Go:   const PI = 3.14159
来源：http://vhw.zhaomingkeji.xyz

Ruby: PI = 3.14159
来源：http://hdn.yj20258888.top

C#:   const double PI = 3.14159;
来源：http://nuh.cashguo.top

[A04] 判断变量类型
来源：http://cqr.yj20258888.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://aod.nwbrower.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hpx.shanyushiyangkeji.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mci.yj20258.top

TS:   typeof x; x instanceof Date
来源：http://fue.zhongyouzk.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lcq.jinyuanbaomall.cn


<!-- 参考信息 -->