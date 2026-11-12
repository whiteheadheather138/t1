代发 wailian999

[U43] PHP：声明命名空间
来源：http://gru.daxiang520.top

namespace App\Http;
来源：http://ykh.haohaochexian.top

[U44] PHP：开启严格类型
来源：http://boc.sxryk.cn

declare(strict_types=1);
来源：http://lvz.xylfe.cn

[U45] PHP：类型声明与返回类型
来源：http://myp.cashguo.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://nrq.jiagoushi.top

[U46] PHP：可空类型
来源：http://abs.epnwcf.com

?string $name = null
来源：http://ywt.meibo888.top

[U47] PHP：联合类型
来源：http://knj.hnxiangtu.top

int|string $id
来源：http://gzh.cashguo.top

[U48] PHP：纯枚举
来源：http://plj.guowangkeji.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nby.fanxiaobao.xyz

[U49] PHP：只读属性
来源：http://ajc.andypj.xyz

public readonly string $name
来源：http://hfk.sufxvd.cn

[U50] PHP：构造器属性提升
来源：http://eim.shzxlz.cn

public function __construct(private int $id) {}
来源：http://fft.yj20258.top

[U51] PHP：数组解构
来源：http://xdd.chenjidiqi.icu

[$a, $b] = $arr;
来源：http://xyp.shangyingyoupin.top

[U52] PHP：箭头函数
来源：http://fmp.zhixingplan.top

$double = fn($x) => $x * 2;
来源：http://btf.svipenyu.cn

[U53] PHP：空合并运算符
来源：http://gyy.zycfv.cn

$v = $a ?? $b ?? "default";
来源：http://sfz.yj202588.top

[U54] PHP：空安全调用
来源：http://llc.shuidangran.top

$obj?->method()
来源：http://hga.fktsv.cn

[U55] PHP：match 表达式
来源：http://qfd.zdbjq.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rzn.ydjk.org.cn

[U56] PHP：命名参数
来源：http://ozw.c1oappe.top

f(a: 1, b: 2)
来源：http://hqy.hcnkem.com

[U57] PHP：字符串插值
来源：http://zbn.316326.xyz

"值: {$a}"
来源：http://zhn.xuetiantiany.cn

[U58] PHP：数组三件套
来源：http://zze.yonumen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://drs.andypj.xyz

[U59] PHP：自定义排序
来源：http://gcw.yangfankeji.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aic.chenzaomai.com

[U60] PHP：JSON 编解码
来源：http://zxg.ctjpmb.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mfn.shanyushiyangtech.top

[U61] PHP：正则
来源：http://ecg.ydjk.org.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pee.zdbjq.cn

[U62] PHP：日期对象
来源：http://wmf.cheryme.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hcj.yfazqb.com

[U63] PHP：文件读写
来源：http://hto.kuanghao11.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sij.wangshuangyany.cn

[U64] PHP：目录遍历
来源：http://uyf.mhx1999.top

glob("dir/*.php");  scandir("dir");
来源：http://cye.yfazqb.com

[U65] PHP：会话
来源：http://oig.wangshuangyany.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pbm.uphjek.com

[U66] PHP：设置 Cookie
来源：http://dps.cqqwz.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://moh.jqgfzy.top

[U67] PHP：处理文件上传
来源：http://ngz.zhaomingkeji.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gzg.aizwys.cn

[U68] PHP：PDO 连接
来源：http://wby.nanxinkj.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kmn.jqgufenzy.top

[U69] PHP：PDO 预处理
来源：http://gyt.cucudq.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cus.redwolf501.top

[U70] PHP：PDO 事务
来源：http://gzn.hnqzz.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gqa.sjlbkw.cn

[U71] PHP：抛出异常
来源：http://gqg.yj20258888.top

throw new RuntimeException("失败", 500);
来源：http://ydz.zhaomingkeji.xyz

[U72] PHP：写错误日志
来源：http://bfk.gotoacloud.top

error_log("失败: " . $e->getMessage());
来源：http://qes.ydjk.org.cn

[U73] PHP：读取 ini 配置
来源：http://aea.tanke756.top

parse_ini_file("config.ini", true)
来源：http://reh.sufxvd.cn

[U74] PHP：读取环境变量
来源：http://rlt.yuanzhike.top

getenv("APP_ENV") ?: "production"
来源：http://vsz.zhixingplan.top

[U75] PHP：依赖注入
来源：http://rye.fengsongda.top

composer require psr/container
来源：http://qrs.shzxlz.cn

[U76] PHP：简单路由
来源：http://pwg.hammf.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zxg.jinghuilouyu.cn

[U77] PHP：模板渲染
来源：http://rqo.zhixingplan.top

composer require twig/twig
来源：http://kuv.jqgfzy.top

[U78] PHP：单元测试
来源：http://dac.guowangkeji.top

composer require --dev phpunit/phpunit
来源：http://dgn.ehwqpu.com

[U79] PHP：静态分析
来源：http://fda.yfazqb.com

composer require --dev phpstan/phpstan
来源：http://gvb.sweek.top

[U80] PHP：代码规范修复
来源：http://rng.guannengcc.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://leq.yuanzhike.top

[U81] JS：初始化项目
来源：http://xet.sjlbkw.cn

npm init -y;  npm i express
来源：http://mpd.tianlin.xyz

[U82] JS：package.json 脚本
来源：http://xjd.epnwcf.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tfj.sxryk.cn

[U83] JS：ES Module 导入导出
来源：http://zcu.dianchejie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://isy.cucudq.cn

[U84] JS：CommonJS 写法
来源：http://ldg.0kj1m.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ulu.mhx1999.top

[U85] JS：可选链
来源：http://giw.fehbvm.com

a?.b?.c
来源：http://gfc.hesvh.cn

[U86] JS：空值合并
来源：http://rad.bbcook.cn

a ?? b
来源：http://vhf.bbcook.cn

[U87] JS：解构默认值
来源：http://fef.zdqjudy.top

const { a = 1, b = 2 } = obj;
来源：http://dtj.haohaochexian.top

[U88] JS：对象展开合并
来源：http://hcj.zhiwuduotai.top

{ ...a, ...b }
来源：http://ara.zhiwuduotai.top

[U89] JS：数组去重
来源：http://cwm.hcnkem.com

[...new Set(arr)]
来源：http://xzy.zdqjudy.top

[U90] JS：数字数组排序
来源：http://iab.jyoumei.cn

[...arr].sort((a, b) => a - b)
来源：http://wwd.ivvv.top

[U91] JS：对象键值遍历
来源：http://lvh.yueranfly.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zci.jiagoushi.top

[U92] JS：深拷贝
来源：http://dox.shzxlz.cn

structuredClone(obj)
来源：http://evt.pengpengdd.cyou

[U93] JS：模板字符串
来源：http://aru.shzxlz.cn

`共 ${n} 条`
来源：http://yfq.feifeiyinyue.top

[U94] JS：箭头函数
来源：http://gjy.zhengqikj.top

const double = x => x * 2;
来源：http://tsq.shanyushiyangtech.top

[U95] JS：Promise 包装
来源：http://bfd.shanyushiyangkeji.top

new Promise((resolve, reject) => {})
来源：http://nds.cheryme.top

[U96] JS：async/await 与异常
来源：http://vle.dianchejie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://syq.shanyushiyangtech.top

[U97] JS：并发请求
来源：http://vdd.haohaochexian.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://zrq.cucudq.cn

[U98] JS：fetch 带 JSON
来源：http://gji.tarul.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://awh.hnxiangtu.top

[U99] JS：事件监听
来源：http://aqy.hnqzz.top

el.addEventListener("click", e => {})
来源：http://onx.fzhhl.top

[U100] JS：DOM 查询
来源：http://ckd.pycfn.com

document.querySelector(".item")
来源：http://yft.svipenyu.cn

[U101] JS：classList 操作
来源：http://udo.hnqzz.top

el.classList.toggle("active")
来源：http://zfh.gotoacloud.top

[U102] JS：本地存储
来源：http://jsy.sysykeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://mqy.jinqigufen.top

[U103] JS：定时器
来源：http://pdw.yj20258888.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zso.9152youxi.cn

[U104] JS：防抖
来源：http://qey.haohaochexian.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kap.chenjidiqi.icu

[U105] JS：节流
来源：http://gmb.vqdsnc.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wpd.shanyushiyangkeji.top

[U106] JS：日期格式化
来源：http://fjt.gaohongyu789.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://drj.zhongyouzk.top

[U107] JS：数字千分位
来源：http://fpx.daria6918.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://khe.chenzaomai.com

[U108] JS：随机整数
来源：http://hbx.xziqi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tgz.dashuyun.cn

[U109] JS：数组分组
来源：http://wme.shanyushiyangkeji.top

Object.groupBy(arr, x => x.type)
来源：http://sjd.shanyushiyangkeji.top

[U110] JS：数组分块
来源：http://ixj.snrcjt.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rzw.xuetiantiany.cn

[U111] JS：对象转 Map
来源：http://vnk.cdnleiting.top

new Map(Object.entries(obj))
来源：http://unj.shanyushiyangtech.top

[U112] JS：字符串补位
来源：http://ajy.c1oappe.top

"7".padStart(3, "0")
来源：http://ymb.meibo888.top

[U113] JS：正则替换全部
来源：http://qmm.hnqzz.top

s.replaceAll("a", "b")
来源：http://qox.ivvv.top

[U114] JS：JSON 深比较
来源：http://rge.yanxiufei.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://obc.ppjwa.cn

[U115] JS：生成 UUID
来源：http://tud.zhaomingkeji.xyz

crypto.randomUUID()
来源：http://jwz.nwbrower.top

[U116] JS：类型检查（JSDoc）
来源：http://vfe.svipenyu.cn

/** @param {string} name */ function f(name) {}
来源：http://nxi.vqdsnc.cn

[U117] JS：单元测试
来源：http://dwy.jlsjyb.cn

npm i -D vitest;  npx vitest
来源：http://xmn.nanxinkj.top

[U118] JS：开发服务器
来源：http://fxp.hnqzz.top

npm i -D vite;  npx vite
来源：http://opr.gzhubu.top

[U119] JS：生产构建
来源：http://qbc.haohaochexian.top

npx vite build
来源：http://dpv.pycfn.com

[U120] JS：读取环境变量（Vite）
来源：http://dfg.hysaishi.cn

import.meta.env.VITE_API_URL
来源：http://plb.nwbrower.top

================================================================================
来源：http://men.nwbrower.top

统计汇总
来源：http://ell.316326.xyz

================================================================================
来源：http://fcw.epnwcf.com

按语言统计（条）：
来源：http://pmn.iojbl.cn

Python ......... 252
来源：http://hwc.jyoumei.cn

PHP ............ 252
来源：http://fdf.yj20258888.top

JavaScript ..... 252
来源：http://ufj.zdqjudy.top

TypeScript ..... 212
来源：http://hpv.sysykeji.top

Java ........... 212
来源：http://cyh.xingfuxueyuan.xyz

Go ............. 212
来源：http://svq.bbcook.cn

Ruby ........... 212
来源：http://fih.pengpengdd.cyou

C# ............. 212
来源：http://fig.yueranfly.top

C .............. 30
来源：http://qqq.epnwcf.com

C++ ............ 30
来源：http://ddu.ctjpmb.com

SQL ............ 90
来源：http://mem.xingfuxueyuan.xyz

Bash ........... 80
来源：http://otn.kuanghao11.cn

Kotlin ......... 15
来源：http://dky.aibaodan.cn

Swift .......... 15
来源：http://acn.ehwqpu.com

Lua ............ 10
来源：http://ksc.jinyuanbaomall.cn

Perl ........... 10
来源：http://atu.aizwys.cn

Scala .......... 10
来源：http://dgm.cqqwz.cn

------------------------------------
来源：http://ngu.yvedp.cn

合计 ........... 2106 条
来源：http://qmc.cqqwz.cn

按章节统计：
来源：http://voo.cdnleiting.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://udb.shanyushiyangtech.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://odq.xziqi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uwr.snrcjt.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qna.hnxiangtu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nzn.vehdjk.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://iay.yj20258888.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qcz.yangfankeji.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tdl.zdqjudy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nmc.nwbrower.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://edx.zdqjudy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cjc.epnwcf.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ckv.epnwcf.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bhs.gzhubu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hpk.ivvv.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hsc.sxryk.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tvx.zhongyouzk.top

Q SQL 专题                              90
来源：http://tax.yj20258.top

R Bash 专题                             80
来源：http://kfe.9152youxi.cn

S C / C++ 专题                          60
来源：http://yac.pycfn.com

T 其他语言补充                          60
来源：http://sec.hongshengwenyu.top

U 高频实用片段                         120
来源：http://mhb.havefunace.top

------------------------------------
来源：http://dbg.tarul.cn

合计                                  2106 条
来源：http://fkq.wangshuangyany.cn

--------------------------------------------------------------------------------
来源：http://mlo.tarul.cn

使用提醒
来源：http://ylc.hnqzz.top

--------------------------------------------------------------------------------
来源：http://fdj.gogol.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zsw.gotoacloud.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jpb.zhoulong.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tyd.yfazqb.com

在旧版本上使用前请先确认语法支持情况。
来源：http://adq.mhx1999.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xoy.ppjwa.cn

—— 文件结束 ——
来源：http://ixe.xinyue.icu

================================================================================
来源：http://xhy.tanke756.top

程序语言常见例子速查手册（2024 版）
来源：http://igv.zhengqikj.top

Common Programming Examples Cheat Book
来源：http://mlo.hfpthk.cn

================================================================================
来源：http://hrq.ydzc1.top

【收录内容】
来源：http://isg.bbcook.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://sbn.andypj.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ihu.ybcxt.top

SQL · Bash · C · C++
来源：http://ino.andypj.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nnd.jinqigufen.top

【使用说明】
来源：http://sum.jianghu66.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yjx.smart0.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ymp.chenjidiqi.icu

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hbs.nanxinkj.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://exf.chenjidiqi.icu

Bash:  Shell         C:     C             C++:   C++
来源：http://mem.iojbl.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bxb.zhaomingkeji.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gkf.jinqigfzy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://euv.mhx1999.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ehv.shangyingyoupin.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jdw.cucudq.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kyy.epnwcf.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kdh.zhongyouzk.top

【文件统计】
来源：http://vrk.gotoacloud.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fcz.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://ugw.hnqzz.top

目  录
来源：http://upx.cucudq.cn

--------------------------------------------------------------------------------
来源：http://woh.cqqwz.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kcn.zdqjudy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mio.mhx1999.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://avc.xylfe.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jdp.nanxuanxn.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qyb.jqgfzy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yhx.ivvv.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kti.quarkkingdee.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://oxq.shangyingyoupin.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jne.zhijiandao.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kim.yj20258.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://upu.sufxvd.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ccz.fengsongda.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nao.pycfn.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gsf.iojbl.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://esv.epnwcf.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kld.xziqi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://fiu.fktsv.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ksp.feifeiyinyue.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kok.ybcxt.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kjt.epnwcf.com

================================================================================
来源：http://lxk.sufxvd.cn

A. 基础语法与类型
来源：http://buh.sufxvd.cn

================================================================================
来源：http://qpo.fktsv.cn

[A01] Hello World
来源：http://wxm.guannengcc.top

Py:   print("Hello, World!")
来源：http://blm.quarkkingdee.top

PHP:  echo "Hello, World!";
来源：http://ywk.zhaomingkeji.xyz

JS:   console.log("Hello, World!");
来源：http://czg.pengpengdd.cyou

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://etq.cheryme.top

Java: System.out.println("Hello, World!");
来源：http://rsl.tanke756.top

Go:   fmt.Println("Hello, World!")
来源：http://aoe.hywenlv.cn

Ruby: puts "Hello, World!"
来源：http://mrt.cqqwz.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fqa.andypj.xyz

[A02] 变量声明与赋值
来源：http://dwx.hysaishi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gil.ydzc1.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ydt.shzxlz.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dez.daria6918.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://veg.jqgfzy.top

Java: String name = "Alex"; int age = 20;
来源：http://cmm.zycfv.cn

Go:   name := "Alex"; age := 20
来源：http://wvk.shangyingyoupin.top

Ruby: name = "Alex"; age = 20
来源：http://iit.yanxiufei.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ptw.shanyushiyangtech.top

[A03] 常量定义
来源：http://pgy.tianlin.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jzw.uphjek.com

PHP:  const PI = 3.14159;
来源：http://ava.ydjk.org.cn

JS:   const PI = 3.14159;
来源：http://dxk.ydzc1.top

TS:   const PI: number = 3.14159;
来源：http://qhq.yuxming.cn

Java: static final double PI = 3.14159;
来源：http://nhq.havefunace.top

Go:   const PI = 3.14159
来源：http://soo.dashuyun.cn

Ruby: PI = 3.14159
来源：http://dmj.xinyue.icu

C#:   const double PI = 3.14159;
来源：http://lus.meibo888.top

[A04] 判断变量类型
来源：http://qzr.zhijiandao.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cme.uphjek.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sgo.chenlongwang.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mwo.cashguo.top

TS:   typeof x; x instanceof Date
来源：http://rxx.yongpay.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kvb.gzhubu.top

Go:   reflect.TypeOf(x).Name()
来源：http://uvg.hnqzz.top

Ruby: x.class; x.is_a?(Integer)
来源：http://tjh.sxryk.cn

C#:   x.GetType().Name; x is int
来源：http://iti.gogol.net.cn

[A05] 整数除法与取模
来源：http://jrk.gogol.net.cn


<!-- 参考信息 -->